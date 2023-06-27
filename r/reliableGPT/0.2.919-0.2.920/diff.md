# Comparing `tmp/reliableGPT-0.2.919.tar.gz` & `tmp/reliableGPT-0.2.920.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.919.tar", last modified: Tue Jun 27 00:58:21 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.920.tar", last modified: Tue Jun 27 01:28:03 2023, max compression
```

## Comparing `reliableGPT-0.2.919.tar` & `reliableGPT-0.2.920.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-27 00:58:21.251277 reliableGPT-0.2.919/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.919/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-27 00:58:21.251177 reliableGPT-0.2.919/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.919/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-27 00:58:21.250046 reliableGPT-0.2.919/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-27 00:58:21.000000 reliableGPT-0.2.919/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      377 2023-06-27 00:58:21.000000 reliableGPT-0.2.919/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-27 00:58:21.000000 reliableGPT-0.2.919/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-27 00:58:21.000000 reliableGPT-0.2.919/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-27 00:58:21.000000 reliableGPT-0.2.919/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-27 00:58:21.250942 reliableGPT-0.2.919/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      140 2023-06-26 23:38:53.000000 reliableGPT-0.2.919/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3356 2023-06-27 00:43:56.000000 reliableGPT-0.2.919/reliablegpt/api_handler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 23:38:53.000000 reliableGPT-0.2.919/reliablegpt/custom_queue.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    15382 2023-06-27 00:58:06.000000 reliableGPT-0.2.919/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1389 2023-06-27 00:54:41.000000 reliableGPT-0.2.919/reliablegpt/test_batch.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1620 2023-06-27 00:56:36.000000 reliableGPT-0.2.919/reliablegpt/test_satya.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.919/reliablegpt/tests_main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-27 00:58:21.251315 reliableGPT-0.2.919/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      380 2023-06-27 00:58:09.000000 reliableGPT-0.2.919/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-27 01:28:03.412867 reliableGPT-0.2.920/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.920/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-27 01:28:03.412768 reliableGPT-0.2.920/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.920/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-27 01:28:03.411188 reliableGPT-0.2.920/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-27 01:28:03.000000 reliableGPT-0.2.920/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      377 2023-06-27 01:28:03.000000 reliableGPT-0.2.920/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-27 01:28:03.000000 reliableGPT-0.2.920/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-27 01:28:03.000000 reliableGPT-0.2.920/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-27 01:28:03.000000 reliableGPT-0.2.920/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-27 01:28:03.412418 reliableGPT-0.2.920/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      140 2023-06-26 23:38:53.000000 reliableGPT-0.2.920/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3356 2023-06-27 00:43:56.000000 reliableGPT-0.2.920/reliablegpt/api_handler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 23:38:53.000000 reliableGPT-0.2.920/reliablegpt/custom_queue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    15744 2023-06-27 01:27:44.000000 reliableGPT-0.2.920/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1389 2023-06-27 00:54:41.000000 reliableGPT-0.2.920/reliablegpt/test_batch.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1620 2023-06-27 00:56:36.000000 reliableGPT-0.2.920/reliablegpt/test_satya.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.920/reliablegpt/tests_main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-27 01:28:03.412909 reliableGPT-0.2.920/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      380 2023-06-27 01:27:57.000000 reliableGPT-0.2.920/setup.py
```

### Comparing `reliableGPT-0.2.919/LICENSE` & `reliableGPT-0.2.920/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.919/README.md` & `reliableGPT-0.2.920/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.919/reliablegpt/api_handler.py` & `reliableGPT-0.2.920/reliablegpt/api_handler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.919/reliablegpt/custom_queue.py` & `reliableGPT-0.2.920/reliablegpt/custom_queue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.919/reliablegpt/main.py` & `reliableGPT-0.2.920/reliablegpt/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,21 +175,25 @@
         return # safe function, should not impact error handling if logging fails
 
 class RequestHandler:
     def __init__(self,
                process_func,
                max_token_capacity,
                max_request_capacity,
+               user_email,
                verbose=False):
         super().__init__()
         self.api_handler = APICallHandler(max_token_capacity,
                                         max_request_capacity,
                                         verbose=verbose)
         self.process_func = process_func
         self.verbose = verbose
+        self.user_email = user_email
+        if user_email == "":
+            raise ValueError("Please enter a valid email")
 
     def print_verbose(self, *args):
         if self.verbose:
             print(*args)
 
     def get_result(self, text):
         task_id = uuid.uuid4().int
@@ -207,14 +211,15 @@
             return result
 
         return None
 
     def execute(self, text, set_timeout=1200):
         task_id = uuid.uuid4().int
         self.print_verbose("task_id: ", task_id)
+        posthog.capture(self.user_email, "reliableGPT.RequestHandler.execute", {'question': text})
         self.api_handler.add_task(process_func=self.process_func,
                                 input=text,
                                 task_id=task_id)
 
         start_time = time.time()
 
         while time.time() - start_time < set_timeout:
@@ -248,14 +253,15 @@
         results.append(result)
         end_time = time.time()
         self.print_verbose(f"Gets result from reliableGPT: {result}",
                         end_time - start_time)
 
 
     def batch_process(self, questions=[], set_timeout=1200):
+        posthog.capture(self.user_email, "reliableGPT.RequestHandler.batch_process", {'questions': questions})
         for question in questions: 
             task_id = uuid.uuid4().int
             self.print_verbose("task_id: ", task_id)
             self.api_handler.add_task(process_func=self.process_func,
                                         input=question, task_id=task_id)
         start_time = time.time() 
         while time.time() - start_time < set_timeout:
```

### Comparing `reliableGPT-0.2.919/reliablegpt/test_batch.py` & `reliableGPT-0.2.920/reliablegpt/test_batch.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.919/reliablegpt/test_satya.py` & `reliableGPT-0.2.920/reliablegpt/test_satya.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.919/reliablegpt/tests_main.py` & `reliableGPT-0.2.920/reliablegpt/tests_main.py`

 * *Files identical despite different names*

