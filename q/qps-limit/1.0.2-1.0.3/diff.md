# Comparing `tmp/qps_limit-1.0.2-py3-none-any.whl.zip` & `tmp/qps_limit-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4969 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      165 b- defN 23-Jun-23 02:46 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     4665 b- defN 23-Jun-23 02:19 qps_limit/limiter.py
--rw-rw-r--  2.0 unx     4335 b- defN 23-Jun-23 02:19 qps_limit/run.py
--rw-rw-r--  2.0 unx     2509 b- defN 23-Jun-23 02:46 qps_limit-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 02:46 qps_limit-1.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-23 02:46 qps_limit-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-23 02:46 qps_limit-1.0.2.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jun-23 02:46 qps_limit-1.0.2.dist-info/RECORD
-8 files, 12398 bytes uncompressed, 3885 bytes compressed:  68.7%
+Zip file size: 4975 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      165 b- defN 23-Jun-27 11:02 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     4655 b- defN 23-Jun-27 11:02 qps_limit/limiter.py
+-rw-rw-r--  2.0 unx     4335 b- defN 23-Jun-27 10:58 qps_limit/run.py
+-rw-rw-r--  2.0 unx     2509 b- defN 23-Jun-27 11:03 qps_limit-1.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 11:03 qps_limit-1.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-27 11:03 qps_limit-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-27 11:03 qps_limit-1.0.3.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      621 b- defN 23-Jun-27 11:03 qps_limit-1.0.3.dist-info/RECORD
+8 files, 12388 bytes uncompressed, 3891 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: qps_limit/limiter.py
 Comment: 
 
 Filename: qps_limit/run.py
 Comment: 
 
-Filename: qps_limit-1.0.2.dist-info/METADATA
+Filename: qps_limit-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-1.0.2.dist-info/WHEEL
+Filename: qps_limit-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-1.0.2.dist-info/top_level.txt
+Filename: qps_limit-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-1.0.2.dist-info/zip-safe
+Filename: qps_limit-1.0.3.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-1.0.2.dist-info/RECORD
+Filename: qps_limit-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 
 from .run import batch_run, async_batch_run
 from .limiter import Limiter
 
 __all__ = [
     'batch_run',
     'async_batch_run',
```

## qps_limit/limiter.py

```diff
@@ -22,34 +22,36 @@
         callback: Optional[Callable] = None,
         progress: bool = True,
         ordered: bool = True,
         verbose: bool = False,
         max_workers: int = 128,
         warmup_steps: int = 1
     ) -> Callable:
+        multiprocessing.set_start_method('fork')
+
         self.func = func
         self.params = params
         self.num_workers = num_workers
         self.worker_max_qps = worker_max_qps
         self.streaming = streaming
         self.callback = callback
         self.progress = progress
         self.ordered = ordered
         self.verbose = verbose
 
         self.count_iterator, self.param_iterator = itertools.tee(self.params(), 2)
         counter = itertools.count()
         collections.deque(zip(self.count_iterator, counter), maxlen=0)
         self.count = next(counter)
+        if self.verbose:
+            print("find {} data, warmup workers with {} data".format(self.count, warmup_steps))
 
         self.param_iterator, warmup_param_iterator = itertools.tee(self.param_iterator, 2)
         warmup_param_iterator = itertools.islice(warmup_param_iterator, warmup_steps)
         warmup_start_time = time.time()
-        if self.verbose:
-            print("warm up workers with {} data".format(warmup_steps))
         batch_run(
             func=self.func,
             params=warmup_param_iterator,
             max_qps=None,
             max_workers=1
         )
         warmup_end_time = time.time()
@@ -65,29 +67,28 @@
             self.dict = multiprocessing.Manager().dict()
         else:
             self.queue = multiprocessing.Queue()
 
         self.workers = []
         if self.progress:
             self.progress_queue = multiprocessing.Queue()
-
-            def _progress_worker():
-                progress_bar = tqdm(total=self.count, desc=self.func.__name__)
-                progress_cnt = 0
-                while progress_cnt < self.count:
-                    progress_bar.update(self.progress_queue.get())
-                    progress_cnt += 1
-                progress_bar.close()
-            self.workers.append(multiprocessing.Process(target=_progress_worker, args=()))
+            self.workers.append(multiprocessing.Process(target=self._progress_worker))
         else:
             self.progress_queue = None
 
         for mod in range(self.num_workers):
             self.workers.append(multiprocessing.Process(target=self._worker, args=(mod,)))
 
+    def _progress_worker(self):
+        progress_bar = tqdm(total=self.count, desc=self.func.__name__)
+        progress_cnt = 0
+        while progress_cnt < self.count:
+            progress_bar.update(self.progress_queue.get())
+            progress_cnt += 1
+
     def _worker(self, mod: int):
         def make_worker_iterator():
             for idx, (args, kwargs) in enumerate(self.param_iterator):
                 if idx % self.num_workers == mod:
                     yield args, kwargs
 
         batch_run_func = batch_run if not self.streaming else streaming_batch_run
```

## qps_limit/run.py

```diff
@@ -63,15 +63,15 @@
     params: Iterable[Tuple[Tuple, Dict]],
     *,
     max_qps: Optional[float] = None,
     max_workers: int = 128,
     callback: Optional[Callable] = None,
     progress_queue: Optional[multiprocessing.Queue] = None
 ):
-    return asyncio.get_event_loop().run_until_complete(async_batch_run(**locals()))
+    return asyncio.new_event_loop().run_until_complete(async_batch_run(**locals()))
 
 
 async def async_streaming_batch_run(
     func: Callable[..., Coroutine[Any, Any, Any]],
     params: Iterable[Tuple[Tuple, Dict]],
     *,
     max_qps: Optional[float] = None,
@@ -139,10 +139,10 @@
                 return True, None
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
-    loop = asyncio.get_event_loop()
+    loop = asyncio.new_event_loop()
     sync_generator = iter_over_async(async_generator, loop)
     return sync_generator
```

## Comparing `qps_limit-1.0.2.dist-info/METADATA` & `qps_limit-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 1.0.2
+Version: 1.0.3
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/qps-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

## Comparing `qps_limit-1.0.2.dist-info/RECORD` & `qps_limit-1.0.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-qps_limit/__init__.py,sha256=TxgSqfPfDDFECLzgdUiE2F2CBDqR4ay9uyfdJbbSkaI,165
-qps_limit/limiter.py,sha256=fDvhBmLwwwIYNdIl6Alco0mkEwiOnV2h4ZnePTADpWg,4665
-qps_limit/run.py,sha256=7osK_VGsB0IVEP6J_pHeBhmAxuH9RZTMCnsmFHgyjdE,4335
-qps_limit-1.0.2.dist-info/METADATA,sha256=-Cye1b-w0o-jGB0SlD2AzW1nPA_1wCEiaZ4d9VCWchM,2509
-qps_limit-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-qps_limit-1.0.2.dist-info/top_level.txt,sha256=vH2iImlC_yaDXYqPQn3x6ZXcQ5Ec2yAe-l0lLJqu0RY,10
-qps_limit-1.0.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-qps_limit-1.0.2.dist-info/RECORD,,
+qps_limit/__init__.py,sha256=THtebmTBMraN5ej92dD5SGMl7lbMfQPfKnI_BzGbxYg,165
+qps_limit/limiter.py,sha256=S8Kx9qoNeOtsQixKmZaRevNRATqSfHaT7FSET7-oJtY,4655
+qps_limit/run.py,sha256=xH63BG0Sp5HAX_KBY3XsK2lUD3tGCn0Ww2S9IFxg_rI,4335
+qps_limit-1.0.3.dist-info/METADATA,sha256=qkTwsQel3TvoSMh6XsIgq-Fes8SM8PEHwqaW3rfyDvY,2509
+qps_limit-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+qps_limit-1.0.3.dist-info/top_level.txt,sha256=vH2iImlC_yaDXYqPQn3x6ZXcQ5Ec2yAe-l0lLJqu0RY,10
+qps_limit-1.0.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+qps_limit-1.0.3.dist-info/RECORD,,
```

