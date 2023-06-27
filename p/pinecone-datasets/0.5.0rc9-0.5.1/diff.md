# Comparing `tmp/pinecone_datasets-0.5.0rc9.tar.gz` & `tmp/pinecone_datasets-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_datasets-0.5.0rc9.tar", max compression
+gzip compressed data, was "pinecone_datasets-0.5.1.tar", max compression
```

## Comparing `pinecone_datasets-0.5.0rc9.tar` & `pinecone_datasets-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0     8945 2023-06-25 09:17:35.695850 pinecone_datasets-0.5.0rc9/README.md
--rw-r--r--   0        0        0      291 2023-06-26 17:28:59.587083 pinecone_datasets-0.5.0rc9/pinecone_datasets/__init__.py
--rw-r--r--   0        0        0     3471 2023-06-25 18:34:09.170949 pinecone_datasets-0.5.0rc9/pinecone_datasets/catalog.py
--rw-r--r--   0        0        0     1185 2023-06-25 09:17:35.697617 pinecone_datasets-0.5.0rc9/pinecone_datasets/cfg.py
--rw-r--r--   0        0        0    22497 2023-06-26 13:24:10.799023 pinecone_datasets-0.5.0rc9/pinecone_datasets/dataset.py
--rw-r--r--   0        0        0     1765 2023-06-25 09:17:35.699080 pinecone_datasets-0.5.0rc9/pinecone_datasets/ds_utils.py
--rw-r--r--   0        0        0      969 2023-06-09 17:14:09.503269 pinecone_datasets-0.5.0rc9/pinecone_datasets/fs.py
--rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.0rc9/pinecone_datasets/public.py
--rw-r--r--   0        0        0      227 2023-06-25 09:17:35.699474 pinecone_datasets-0.5.0rc9/pinecone_datasets/testing.py
--rw-r--r--   0        0        0      907 2023-06-26 17:28:46.149152 pinecone_datasets-0.5.0rc9/pyproject.toml
--rw-r--r--   0        0        0     9956 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc9/PKG-INFO
+-rw-r--r--   0        0        0     9002 2023-06-27 19:27:57.256133 pinecone_datasets-0.5.1/README.md
+-rw-r--r--   0        0        0      221 2023-06-27 19:27:57.256477 pinecone_datasets-0.5.1/pinecone_datasets/__init__.py
+-rw-r--r--   0        0        0     3471 2023-06-27 19:27:57.256891 pinecone_datasets-0.5.1/pinecone_datasets/catalog.py
+-rw-r--r--   0        0        0     1185 2023-06-27 19:27:57.257561 pinecone_datasets-0.5.1/pinecone_datasets/cfg.py
+-rw-r--r--   0        0        0    21934 2023-06-27 19:30:18.407338 pinecone_datasets-0.5.1/pinecone_datasets/dataset.py
+-rw-r--r--   0        0        0      969 2023-06-27 19:27:57.258399 pinecone_datasets-0.5.1/pinecone_datasets/fs.py
+-rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.1/pinecone_datasets/public.py
+-rw-r--r--   0        0        0      881 2023-06-27 19:31:34.790867 pinecone_datasets-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9967 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.1/PKG-INFO
```

### Comparing `pinecone_datasets-0.5.0rc9/README.md` & `pinecone_datasets-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -168,14 +168,16 @@
 ```
 
 
 ### upserting to Index
 
 When upserting a Dataset to an Index, only the document data will be upserted to the index. The queries data will be ignored. 
 
+TODO: add example for API Key adn Environment Variables
+
 ```python
 ds = load_dataset("dataset_name")
 
 # If index exists
 ds.to_index("index_name")
 
 # If index does not exist use create_index=True, this will create the index with the default pinecone settings and dimension from the dataset metadata.
```

### Comparing `pinecone_datasets-0.5.0rc9/pinecone_datasets/catalog.py` & `pinecone_datasets-0.5.1/pinecone_datasets/catalog.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc9/pinecone_datasets/cfg.py` & `pinecone_datasets-0.5.1/pinecone_datasets/cfg.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc9/pinecone_datasets/dataset.py` & `pinecone_datasets-0.5.1/pinecone_datasets/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 if version("pinecone-client").startswith("3"):
     from pinecone import Client as pc, Index
 elif version("pinecone-client").startswith("2"):
     import pinecone as pc
 
     try:
         from pinecone import GRPCIndex as Index
-    except ImportError:
+    except:
         from pinecone import Index
 else:
     warnings.warn(
         message="Pinecone client version not supported or non-existent,"
         + "please use pip ineall pinecone-client to install v2 or "
         + "pip install pinecone-datasets[clientv3] to install v3"
     )
@@ -58,19 +58,15 @@
 
 
 def iter_pandas_dataframe_slices(
     df: pd.DataFrame, batch_size, return_indexes
 ) -> Generator[List[Dict[str, Any]], None, None]:
     for i in range(0, len(df), batch_size):
         if return_indexes:
-            yield (
-                i,
-                df.iloc[i : i + batch_size].to_dict(orient="records"),
-                df.iloc[i : i + batch_size].index,
-            )
+            yield (i, df.iloc[i : i + batch_size].to_dict(orient="records"))
         else:
             yield df.iloc[i : i + batch_size].to_dict(orient="records")
 
 
 def iter_pandas_dataframe_single(
     df: pd.DataFrame,
 ) -> Generator[Dict[str, Any], None, None]:
@@ -421,47 +417,50 @@
             self._pinecone_client.get_index(index_name=index_name)
             if version("pinecone-client").startswith("3")
             else Index(index_name=index_name)
         )
 
         sem = asyncio.Semaphore(concurrency)
 
-        pinecone_failed_batches: Dict[Int, Any] = {}
+        pinecone_failed_batches = []
 
-        async def send_batch(i, df, idx):
+        async def send_batch(i, batch):
             async with sem:
                 try:
-                    batch = df.loc[idx]
                     return await pinecone_index.upsert(vectors=batch, async_req=True)
                 except Exception as pe:
                     if i in pinecone_failed_batches:
                         raise pe
                     else:
-                        pinecone_failed_batches[i] = idx
-                        print(f"failed batches: {pinecone_failed_batches.keys()}")
+                        pinecone_failed_batches.append(i)
                         return UpsertResponse(upserted_count=0)
 
         tasks = [
-            send_batch(i, self.documents, idx)
-            for i, chunk, idx in self.iter_documents(
+            send_batch(i, chunk)
+            for i, chunk in self.iter_documents(
                 batch_size=batch_size, return_indexes=True
             )
         ]
-        failed_tasks_pinecone = []
 
         pbar = tqdm(total=len(self.documents), desc="Upserting Vectors")
         total_upserted_count = 0
         for task in asyncio.as_completed(tasks):
             res = await task
             total_upserted_count += res.upserted_count
             pbar.update(res.upserted_count)
 
         failed_tasks = [
-            send_batch(i, self.documents, index)
-            for i, index in pinecone_failed_batches.items()
+            send_batch(
+                i,
+                self.documents[self._config.Schema.documents_select_columns]
+                .dropna(axis=1, how="all")
+                .loc[i : i + batch_size]
+                .to_dict(orient="records"),
+            )
+            for i in pinecone_failed_batches
         ]
 
         for task in asyncio.as_completed(failed_tasks):
             res = await task
             total_upserted_count += res.upserted_count
             pbar.update(res.upserted_count)
 
@@ -470,31 +469,18 @@
     def _create_index(
         self,
         index_name: str,
         api_key: Optional[str] = None,
         environment: Optional[str] = None,
         **kwargs,
     ) -> Index:
-        dimension = self.metadata.dense_model.dimension
-        api_key = api_key if api_key else os.environ.get("PINECONE_API_KEY", None)
-        environment = (
-            environment if environment else os.environ.get("PINECONE_ENVIRONMENT", None)
-        )
-
-        if not (api_key and environment):
-            raise ValueError(
-                "Please set PINECONE_API_KEY and PINECONE_ENVIRONMENT environment variables, \
-                or pass them as arguments to the function"
-            )
-        # create client
-
         if version("pinecone-client").startswith("3"):
-            self._pinecone_client = pc(api_key=api_key, region=environment)
+            self._pinecone_client = pc(api_key=api_key, region=environment, **kwargs)
         elif version("pinecone-client").startswith("2"):
-            pc.init(api_key=api_key, environment=environment)
+            pc.init(api_key=api_key, environment=environment, **kwargs)
             self._pinecone_client = pc
 
         pinecone_index_list = self._pinecone_client.list_indexes()
 
         if index_name in pinecone_index_list:
             raise ValueError(
                 f"index {index_name} already exists, Pinecone Datasets can only be upserted to a new indexe"
@@ -536,14 +522,15 @@
         Args:
             index_name (str): the name of the index to upsert to
             batch_size (int, optional): the batch size to use for the upsert. Defaults to 100.
             concurrency (int, optional): the concurrency to use for the upsert. Defaults to 10.
 
         Keyword Args:
             kwargs (Dict): additional arguments to pass to the Pinecone Client constructor when creating the index.
+            see available parameters here: https://docs.pinecone.io/reference/create_index
 
 
         Returns:
             UpsertResponse: an object containing the upserted_count
 
         Examples:
             ```python
@@ -555,17 +542,21 @@
         if loop.is_running():
             raise RuntimeError(
                 "You are running inside a Jupyter Notebook or another Asyncio context. "
                 + "Plesae use the function to_pinecone_index_async instead. "
                 + "example: `await dataset.to_pinecone_index_async(index_name)`"
             )
 
-        if not self._create_index(index_name, **kwargs):
+        if not self._create_index(
+            index_name, api_key=api_key, environment=environment, **kwargs
+        ):
             raise RuntimeError("index creation failed")
 
+        # TODO: add concurrency = 0 as sync loop (def _upsert...) and add sync loop
+
         cor = self._async_upsert(
             index_name=index_name,
             batch_size=batch_size,
             concurrency=concurrency,
         )
         return asyncio.run(cor)
 
@@ -591,32 +582,28 @@
         Args:
             index_name (str): the name of the index to upsert to
             batch_size (int, optional): the batch size to use for the upsert. Defaults to 100.
             concurrency (int, optional): the concurrency to use for the upsert. Defaults to 10.
 
         Keyword Args:
             kwargs (Dict): additional arguments to pass to the Pinecone Client constructor when creating the index.
+            see available parameters here: https://docs.pinecone.io/reference/create_index
+
 
         Returns:
             UpsertResponse: an object containing the upserted_count
 
         Examples:
             ```python
             result = await dataset.to_pinecone_index_async(index_name="my_index")
             ```
         """
-        loop = asyncio.get_event_loop()
-        if not loop.is_running():
-            raise RuntimeError(
-                "You are running inside a Jupyter Notebook or another Asyncio context. \
-                Plesae use the function to_pinecone_index instead. \
-                example: `dataset.to_pinecone_index(index_name)`"
-            )
-
-        if not self._create_index(index_name, **kwargs):
+        if not self._create_index(
+            index_name, api_key=api_key, environment=environment, **kwargs
+        ):
             raise RuntimeError("index creation failed")
 
         res = await self._async_upsert(
             index_name=index_name,
             batch_size=batch_size,
             concurrency=concurrency,
         )
```

### Comparing `pinecone_datasets-0.5.0rc9/pinecone_datasets/fs.py` & `pinecone_datasets-0.5.1/pinecone_datasets/fs.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc9/pinecone_datasets/public.py` & `pinecone_datasets-0.5.1/pinecone_datasets/public.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc9/pyproject.toml` & `pinecone_datasets-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "pinecone-datasets"
-version = "0.5.0-rc.9"
+version = "0.5.1"
 description = "Pinecone Datasets lets you easily load datasets into your Pinecone index."
 authors = ["Pinecone"]
 maintainers = [
     "Roy Miara <miararoy@gmail.com>",
 ]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 polars = "^0.16.4"
-pyarrow = "^12.0.0"
+pyarrow = "^11.0.0"
 fsspec = "^2023.1.0"
 gcsfs = "^2023.1.0"
 s3fs = "^2023.1.0"
 pydantic = "^1.10.5"
-protobuf = "~=3.20.0"
 pandas = "^2.0.0"
 tqdm = "^4.65.0"
 pinecone-client = { version = "3.0.0rc2", optional = true }
 
+
 [tool.poetry.extras]
 clientv3 = ["pinecone-client"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `pinecone_datasets-0.5.0rc9/PKG-INFO` & `pinecone_datasets-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-datasets
-Version: 0.5.0rc9
+Version: 0.5.1
 Summary: Pinecone Datasets lets you easily load datasets into your Pinecone index.
 Author: Pinecone
 Maintainer: Roy Miara
 Maintainer-email: miararoy@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -13,16 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: clientv3
 Requires-Dist: fsspec (>=2023.1.0,<2024.0.0)
 Requires-Dist: gcsfs (>=2023.1.0,<2024.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pinecone-client (==3.0.0rc2) ; extra == "clientv3"
 Requires-Dist: polars (>=0.16.4,<0.17.0)
-Requires-Dist: protobuf (>=3.20.0,<3.21.0)
-Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
+Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: s3fs (>=2023.1.0,<2024.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Pinecone Datasets
 
@@ -194,14 +193,16 @@
 ```
 
 
 ### upserting to Index
 
 When upserting a Dataset to an Index, only the document data will be upserted to the index. The queries data will be ignored. 
 
+TODO: add example for API Key adn Environment Variables
+
 ```python
 ds = load_dataset("dataset_name")
 
 # If index exists
 ds.to_index("index_name")
 
 # If index does not exist use create_index=True, this will create the index with the default pinecone settings and dimension from the dataset metadata.
```

