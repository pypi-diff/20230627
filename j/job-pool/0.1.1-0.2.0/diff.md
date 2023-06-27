# Comparing `tmp/job_pool-0.1.1-py3-none-any.whl.zip` & `tmp/job_pool-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 7509 bytes, number of entries: 5
+Zip file size: 8345 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1624 b- defN 80-Jan-01 00:00 job_pool/__init__.py
 -rw-r--r--  2.0 unx     5510 b- defN 80-Jan-01 00:00 job_pool/job_pool.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 job_pool-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1507 b- defN 80-Jan-01 00:00 job_pool-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 job_pool-0.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      376 b- defN 16-Jan-01 00:00 job_pool-0.1.1.dist-info/RECORD
-5 files, 18838 bytes uncompressed, 6815 bytes compressed:  63.8%
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 job_pool-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1527 b- defN 80-Jan-01 00:00 job_pool-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 job_pool-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      453 b- defN 16-Jan-01 00:00 job_pool-0.2.0.dist-info/RECORD
+6 files, 20559 bytes uncompressed, 7535 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
+Filename: job_pool/__init__.py
+Comment: 
+
 Filename: job_pool/job_pool.py
 Comment: 
 
-Filename: job_pool-0.1.1.dist-info/LICENSE
+Filename: job_pool-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: job_pool-0.1.1.dist-info/METADATA
+Filename: job_pool-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: job_pool-0.1.1.dist-info/WHEEL
+Filename: job_pool-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: job_pool-0.1.1.dist-info/RECORD
+Filename: job_pool-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `job_pool-0.1.1.dist-info/LICENSE` & `job_pool-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `job_pool-0.1.1.dist-info/METADATA` & `job_pool-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: job-pool
-Version: 0.1.1
+Version: 0.2.0
 Summary: Enhanced Job Pool for Python Multiprocessing
 License: Apache-2.0
 Author: Matthew The
 Author-email: matthew.the@tum.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
 def add_one(i):
     return i + 1
 
 def multiprocessed_add_one():
     pool = JobPool(4)
     for i in range(20):
         pool.applyAsync(add_one, [i])
-    results = pool.checkPool()
+    results = pool.checkPool(printProgressEvery=5)
     assert results == list(range(1,21))
 ```
 
 ## Installation
 
 job-pool is available on PyPI and can be installed with `pip`:
```

