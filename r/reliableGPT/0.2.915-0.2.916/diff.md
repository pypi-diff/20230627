# Comparing `tmp/reliableGPT-0.2.915.tar.gz` & `tmp/reliableGPT-0.2.916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.915.tar", last modified: Mon Jun 26 23:28:09 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.916.tar", last modified: Mon Jun 26 23:29:07 2023, max compression
```

## Comparing `reliableGPT-0.2.915.tar` & `reliableGPT-0.2.916.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:28:09.613451 reliableGPT-0.2.915/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.915/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 23:28:09.613350 reliableGPT-0.2.915/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.915/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:28:09.611944 reliableGPT-0.2.915/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 23:28:09.000000 reliableGPT-0.2.915/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      354 2023-06-26 23:28:09.000000 reliableGPT-0.2.915/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 23:28:09.000000 reliableGPT-0.2.915/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 23:28:09.000000 reliableGPT-0.2.915/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 23:28:09.000000 reliableGPT-0.2.915/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:28:09.613113 reliableGPT-0.2.915/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      140 2023-06-26 23:26:24.000000 reliableGPT-0.2.915/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3049 2023-06-26 23:10:13.000000 reliableGPT-0.2.915/reliablegpt/api_handler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 23:14:04.000000 reliableGPT-0.2.915/reliablegpt/custom_queue.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    14404 2023-06-26 23:27:48.000000 reliableGPT-0.2.915/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1427 2023-06-26 23:10:37.000000 reliableGPT-0.2.915/reliablegpt/test_batching.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.915/reliablegpt/tests_main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 23:28:09.613492 reliableGPT-0.2.915/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      380 2023-06-26 23:28:03.000000 reliableGPT-0.2.915/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:29:07.334197 reliableGPT-0.2.916/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.916/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 23:29:07.334087 reliableGPT-0.2.916/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.916/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:29:07.333015 reliableGPT-0.2.916/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 23:29:07.000000 reliableGPT-0.2.916/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      354 2023-06-26 23:29:07.000000 reliableGPT-0.2.916/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 23:29:07.000000 reliableGPT-0.2.916/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 23:29:07.000000 reliableGPT-0.2.916/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 23:29:07.000000 reliableGPT-0.2.916/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:29:07.333847 reliableGPT-0.2.916/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      140 2023-06-26 23:26:24.000000 reliableGPT-0.2.916/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3061 2023-06-26 23:28:53.000000 reliableGPT-0.2.916/reliablegpt/api_handler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 23:28:52.000000 reliableGPT-0.2.916/reliablegpt/custom_queue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    14404 2023-06-26 23:28:56.000000 reliableGPT-0.2.916/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1427 2023-06-26 23:10:37.000000 reliableGPT-0.2.916/reliablegpt/test_batching.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.916/reliablegpt/tests_main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 23:29:07.334235 reliableGPT-0.2.916/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      380 2023-06-26 23:29:00.000000 reliableGPT-0.2.916/setup.py
```

### Comparing `reliableGPT-0.2.915/LICENSE` & `reliableGPT-0.2.916/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.915/README.md` & `reliableGPT-0.2.916/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.915/reliablegpt/api_handler.py` & `reliableGPT-0.2.916/reliablegpt/api_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import queue
 from concurrent.futures import ThreadPoolExecutor
 import threading
-from custom_queue import CustomQueue
+from reliablegpt.custom_queue import CustomQueue
 
 class APICallHandler():
 
   def __init__(self, max_token_capacity, max_request_capacity, verbose):
     super().__init__()
     self.verbose = verbose
     self.upperbound = 1000000
```

### Comparing `reliableGPT-0.2.915/reliablegpt/custom_queue.py` & `reliableGPT-0.2.916/reliablegpt/custom_queue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.915/reliablegpt/main.py` & `reliableGPT-0.2.916/reliablegpt/main.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.915/reliablegpt/test_batching.py` & `reliableGPT-0.2.916/reliablegpt/test_batching.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.915/reliablegpt/tests_main.py` & `reliableGPT-0.2.916/reliablegpt/tests_main.py`

 * *Files identical despite different names*

