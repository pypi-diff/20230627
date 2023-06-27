# Comparing `tmp/pytheus_backend_rs-0.0.5.tar.gz` & `tmp/pytheus_backend_rs-0.0.6.tar.gz`

## Comparing `pytheus_backend_rs-0.0.5.tar` & `pytheus_backend_rs-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      319 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.5/Cargo.toml
--rw-r--r--   0     1001      123     2792 2023-06-25 23:51:58.000000 pytheus_backend_rs-0.0.5/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-25 23:51:58.000000 pytheus_backend_rs-0.0.5/.gitignore
--rw-r--r--   0     1001      123      620 2023-06-25 23:51:58.000000 pytheus_backend_rs-0.0.5/pyproject.toml
--rw-r--r--   0     1001      123    13267 2023-06-25 23:51:58.000000 pytheus_backend_rs-0.0.5/src/lib.rs
--rw-r--r--   0     1001      123    12764 2023-06-25 23:52:04.000000 pytheus_backend_rs-0.0.5/Cargo.lock
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.6/Cargo.toml
+-rw-r--r--   0     1001      123     2792 2023-06-27 00:50:17.000000 pytheus_backend_rs-0.0.6/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-27 00:50:17.000000 pytheus_backend_rs-0.0.6/.gitignore
+-rw-r--r--   0     1001      123      620 2023-06-27 00:50:17.000000 pytheus_backend_rs-0.0.6/pyproject.toml
+-rw-r--r--   0     1001      123    13415 2023-06-27 00:50:17.000000 pytheus_backend_rs-0.0.6/src/lib.rs
+-rw-r--r--   0     1001      123    13468 2023-06-27 00:50:17.000000 pytheus_backend_rs-0.0.6/Cargo.lock
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.6/PKG-INFO
```

### Comparing `pytheus_backend_rs-0.0.5/.github/workflows/CI.yml` & `pytheus_backend_rs-0.0.6/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.5/.gitignore` & `pytheus_backend_rs-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.5/pyproject.toml` & `pytheus_backend_rs-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.5/src/lib.rs` & `pytheus_backend_rs-0.0.6/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 use crossbeam::channel;
 use itertools::Itertools;
 use pyo3::exceptions::PyException;
 use pyo3::intern;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyType};
-use redis::Commands;
-use redis::{Connection, RedisResult};
+use redis::ConnectionLike;
 use std::collections::HashMap;
 use std::sync::{mpsc, Mutex, OnceLock};
 use std::thread;
 
 // This could be completely wrong, not sure if it would break the channel, let's try 🤞
 static REDIS_JOB_TX: OnceLock<Mutex<mpsc::Sender<RedisJob>>> = OnceLock::new();
 static REDIS_PIPELINE_JOB_TX: OnceLock<Mutex<channel::Sender<RedisPipelineJob>>> = OnceLock::new();
@@ -106,19 +105,45 @@
         {
             pydict.set_item(collector, samples.into_py(py))?;
         }
         Ok(pydict.into())
     }
 }
 
-fn create_redis_connection(host: &str, port: u16) -> RedisResult<Connection> {
+fn create_redis_pool(
+    host: &str,
+    port: u16,
+) -> Result<r2d2::Pool<redis::Client>, Box<dyn std::error::Error>> {
     let url = format!("redis://{host}:{port}");
     let client = redis::Client::open(url)?;
-    let con = client.get_connection()?;
-    Ok(con)
+    let pool = r2d2::Pool::builder().build(client)?;
+    Ok(pool)
+}
+
+fn add_job_to_pipeline(received: RedisJob, pipe: &mut redis::Pipeline) {
+    match received.action {
+        BackendAction::Inc | BackendAction::Dec => {
+            match received.labels_hash {
+                Some(labels_hash) => pipe
+                    .hincr(&received.key_name, &labels_hash, received.value)
+                    .ignore(),
+                None => pipe.incr(&received.key_name, received.value).ignore(),
+            };
+            pipe.expire(&received.key_name, EXPIRE_KEY_SECONDS).ignore();
+        }
+        BackendAction::Set => {
+            match received.labels_hash {
+                Some(labels_hash) => pipe
+                    .hset(&received.key_name, &labels_hash, received.value)
+                    .ignore(),
+                None => pipe.set(&received.key_name, received.value).ignore(),
+            };
+            pipe.expire(&received.key_name, EXPIRE_KEY_SECONDS).ignore();
+        }
+    }
 }
 
 #[pymethods]
 impl RedisBackend {
     #[new]
     fn new(config: &PyDict, metric: &PyAny, histogram_bucket: Option<String>) -> PyResult<Self> {
         // producer
@@ -184,75 +209,67 @@
 
     #[classmethod]
     fn _initialize(_cls: &PyType, config: &PyDict) -> PyResult<()> {
         // using the PyAny::get_item so that it will raise a KeyError on missing key
         let host: &str = PyAny::get_item(config, intern!(config.py(), "host"))?.extract()?;
         let port: u16 = PyAny::get_item(config, intern!(config.py(), "port"))?.extract()?;
 
-        let mut connection = match create_redis_connection(host, port) {
-            Ok(connection) => connection,
+        let pool = match create_redis_pool(host, port) {
+            Ok(pool) => pool,
             Err(e) => return Err(PyException::new_err(e.to_string())),
         };
 
         // producer / consumer
         let (tx, rx) = mpsc::channel();
         REDIS_JOB_TX.get_or_init(|| Mutex::new(tx));
 
         let (pipeline_tx, pipeline_rx) = crossbeam::channel::unbounded();
         REDIS_PIPELINE_JOB_TX.get_or_init(|| Mutex::new(pipeline_tx));
 
         for i in 0..4 {
             let cloned_pipeline_rx = pipeline_rx.clone();
-            let mut pipeline_connection = match create_redis_connection(host, port) {
-                Ok(connection) => connection,
-                Err(e) => return Err(PyException::new_err(e.to_string())),
-            };
+            let pool = pool.clone();
             thread::spawn(move || {
                 println!("Starting pipeline thread....{i}");
+                let mut connection = pool.get().unwrap();
                 while let Ok(received) = cloned_pipeline_rx.recv() {
+                    if !connection.is_open() {
+                        connection = pool.get().unwrap();
+                    }
+
                     let pipe = received.pipeline;
-                    let results: Vec<Option<f64>> = pipe.query(&mut pipeline_connection).unwrap();
+                    let results: Vec<Option<f64>> = pipe.query(&mut connection).unwrap();
 
                     let values = results.into_iter().map(|val| val.unwrap_or(0f64)).collect();
 
                     received
                         .result_tx
                         .send(RedisPipelineJobResult { values })
                         .unwrap();
                 }
             });
         }
 
         thread::spawn(move || {
             println!("Starting BackendAction thread....");
+            let mut connection = pool.get().unwrap();
             while let Ok(received) = rx.recv() {
-                match received.action {
-                    BackendAction::Inc | BackendAction::Dec => {
-                        match received.labels_hash {
-                            Some(labels_hash) => connection
-                                .hincr(&received.key_name, &labels_hash, received.value)
-                                .unwrap(),
-                            None => connection.incr(&received.key_name, received.value).unwrap(),
-                        }
-                        let _: () = connection
-                            .expire(&received.key_name, EXPIRE_KEY_SECONDS)
-                            .unwrap();
-                    }
-                    BackendAction::Set => {
-                        match received.labels_hash {
-                            Some(labels_hash) => connection
-                                .hset(&received.key_name, &labels_hash, received.value)
-                                .unwrap(),
-                            None => connection.set(&received.key_name, received.value).unwrap(),
-                        }
-                        let _: () = connection
-                            .expire(&received.key_name, EXPIRE_KEY_SECONDS)
-                            .unwrap();
-                    }
+                if !connection.is_open() {
+                    connection = pool.get().unwrap();
+                }
+
+                let mut pipe = redis::pipe();
+
+                add_job_to_pipeline(received, &mut pipe);
+
+                for received in rx.try_iter() {
+                    add_job_to_pipeline(received, &mut pipe);
                 }
+
+                let _: () = pipe.query(&mut connection).unwrap();
             }
         });
 
         Ok(())
     }
 
     #[classmethod]
@@ -313,15 +330,15 @@
         send_tx
             .send(RedisPipelineJob {
                 result_tx: tx,
                 pipeline: pipe,
             })
             .unwrap();
 
-        let job_result = rx.recv().unwrap();
+        let job_result = py.allow_threads(move || rx.recv().unwrap());
 
         // map back the values from redis into the appropriate Sample
         let mut samples_vec_united = vec![];
         for samples_vec in &mut samples_result_dict.samples_vec {
             samples_vec_united.extend(samples_vec);
         }
```

### Comparing `pytheus_backend_rs-0.0.5/Cargo.lock` & `pytheus_backend_rs-0.0.6/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,20 @@
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "log"
+version = "0.4.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
+
+[[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
@@ -282,40 +288,53 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pytheus-backend-rs"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
  "crossbeam",
  "itertools",
  "pyo3",
+ "r2d2",
  "redis",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "r2d2"
+version = "0.8.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51de85fb3fb6524929c8a2eb85e6b6d363de4e8c48f9e2c2eac4944abc181c93"
+dependencies = [
+ "log",
+ "parking_lot",
+ "scheduled-thread-pool",
+]
+
+[[package]]
 name = "redis"
 version = "0.23.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3ea8c51b5dc1d8e5fd3350ec8167f464ec0995e79f2e90a075b63371500d557f"
 dependencies = [
  "combine",
  "itoa",
  "percent-encoding",
+ "r2d2",
  "ryu",
  "sha1_smol",
  "url",
 ]
 
 [[package]]
 name = "redox_syscall"
@@ -329,14 +348,23 @@
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
+name = "scheduled-thread-pool"
+version = "0.2.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3cbc66816425a074528352f5789333ecff06ca41b36b0b0efdfbb29edc391a19"
+dependencies = [
+ "parking_lot",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "sha1_smol"
```

