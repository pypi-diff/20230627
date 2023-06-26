# Comparing `tmp/reliableGPT-0.2.905.tar.gz` & `tmp/reliableGPT-0.2.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.905.tar", last modified: Mon Jun 26 21:47:21 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.906.tar", last modified: Mon Jun 26 22:46:56 2023, max compression
```

## Comparing `reliableGPT-0.2.905.tar` & `reliableGPT-0.2.906.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 21:47:21.602080 reliableGPT-0.2.905/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.905/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 21:47:21.601967 reliableGPT-0.2.905/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.905/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 21:47:21.601045 reliableGPT-0.2.905/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 21:47:21.000000 reliableGPT-0.2.905/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      356 2023-06-26 21:47:21.000000 reliableGPT-0.2.905/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 21:47:21.000000 reliableGPT-0.2.905/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 21:47:21.000000 reliableGPT-0.2.905/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 21:47:21.000000 reliableGPT-0.2.905/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 21:47:21.601800 reliableGPT-0.2.905/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3048 2023-06-26 21:41:37.000000 reliableGPT-0.2.905/reliablegpt/APICallHandler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 19:46:40.000000 reliableGPT-0.2.905/reliablegpt/CustomQueue.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.905/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    15049 2023-06-26 20:55:31.000000 reliableGPT-0.2.905/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1434 2023-06-26 21:45:37.000000 reliableGPT-0.2.905/reliablegpt/test_batching.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.905/reliablegpt/tests_main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 21:47:21.602127 reliableGPT-0.2.905/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      351 2023-06-26 21:46:11.000000 reliableGPT-0.2.905/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:46:56.630522 reliableGPT-0.2.906/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.906/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 22:46:56.630421 reliableGPT-0.2.906/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.906/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:46:56.629104 reliableGPT-0.2.906/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 22:46:56.000000 reliableGPT-0.2.906/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      354 2023-06-26 22:46:56.000000 reliableGPT-0.2.906/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 22:46:56.000000 reliableGPT-0.2.906/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 22:46:56.000000 reliableGPT-0.2.906/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 22:46:56.000000 reliableGPT-0.2.906/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:46:56.630150 reliableGPT-0.2.906/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.906/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3049 2023-06-26 22:46:08.000000 reliableGPT-0.2.906/reliablegpt/api_handler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 22:46:07.000000 reliableGPT-0.2.906/reliablegpt/custom_queue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    14392 2023-06-26 22:45:07.000000 reliableGPT-0.2.906/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1427 2023-06-26 22:46:47.000000 reliableGPT-0.2.906/reliablegpt/test_batching.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.906/reliablegpt/tests_main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 22:46:56.630562 reliableGPT-0.2.906/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      351 2023-06-26 22:46:23.000000 reliableGPT-0.2.906/setup.py
```

### Comparing `reliableGPT-0.2.905/LICENSE` & `reliableGPT-0.2.906/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.905/README.md` & `reliableGPT-0.2.906/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.905/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.906/reliablegpt/api_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import queue
 from concurrent.futures import ThreadPoolExecutor
 import threading
-from CustomQueue import CustomQueue
+from custom_queue import CustomQueue
 
 class APICallHandler():
 
   def __init__(self, max_token_capacity, max_request_capacity, verbose):
     super().__init__()
     self.verbose = verbose
     self.upperbound = 1000000
```

### Comparing `reliableGPT-0.2.905/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.906/reliablegpt/custom_queue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.905/reliablegpt/main.py` & `reliableGPT-0.2.906/reliablegpt/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import requests
 from posthog import Posthog
 from klotty import Klotty
 from tqdm import tqdm
 
 ## Import for Batch requests
 import uuid
-from APICallHandler import APICallHandler
+from api_handler import APICallHandler
 import time
 import threading
 
 client = Klotty(api_key="re_X1PBTBvD_5mJfFM98AuF2278fNAGfXVNV") # email client
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
@@ -216,33 +216,14 @@
         start_time = time.time()
         result = self.get_result(test_question)
         results.append(result)
         end_time = time.time()
         self.print_verbose(f"Gets result from reliableGPT: {result}",
                         end_time - start_time)
 
-    # def execute(self, questions=[]):
-    #     thread_list = []
-    #     results = []
-    #     print(f"ReliableGPT: Processing {len(questions)} Requests")
-
-    #     for idx, q in enumerate(questions):
-    #         self.api_handler.add_task()
-    #         thread = threading.Thread(target=self.get_result_threaded,
-    #                                 args=(q, results))
-    #     thread.start()
-    #     thread_list.append(thread)
-
-    #     # Join all threads
-    #     for thread in thread_list:
-    #         thread.join()
-
-    #     self.print_verbose("All threads completed.")
-    #     self.print_verbose(results)
-    #     return results
 
     def execute(self, questions=[]):
         for question in questions: 
             task_id = uuid.uuid4().int
             self.print_verbose("task_id: ", task_id)
             self.api_handler.add_task(process_func=self.process_func,
                                         input=question, task_id=task_id)
```

### Comparing `reliableGPT-0.2.905/reliablegpt/test_batching.py` & `reliableGPT-0.2.906/reliablegpt/test_batching.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import main
 from main import batchRequests
 import openai
 
-openai.api_key = ""
+
 
 def simple_openai_call(prompt):
   print(f"in simple openai call with question:  {prompt}")
   model = "gpt-4"
   messages = [
     {
       "role": "system",
```

### Comparing `reliableGPT-0.2.905/reliablegpt/tests_main.py` & `reliableGPT-0.2.906/reliablegpt/tests_main.py`

 * *Files identical despite different names*

