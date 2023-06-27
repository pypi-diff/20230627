# Comparing `tmp/reliableGPT-0.2.916.tar.gz` & `tmp/reliableGPT-0.2.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.916.tar", last modified: Mon Jun 26 23:29:07 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.918.tar", last modified: Tue Jun 27 00:44:15 2023, max compression
```

## Comparing `reliableGPT-0.2.916.tar` & `reliableGPT-0.2.918.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:29:07.334197 reliableGPT-0.2.916/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.916/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 23:29:07.334087 reliableGPT-0.2.916/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.916/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:29:07.333015 reliableGPT-0.2.916/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 23:29:07.000000 reliableGPT-0.2.916/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      354 2023-06-26 23:29:07.000000 reliableGPT-0.2.916/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 23:29:07.000000 reliableGPT-0.2.916/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 23:29:07.000000 reliableGPT-0.2.916/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 23:29:07.000000 reliableGPT-0.2.916/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:29:07.333847 reliableGPT-0.2.916/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      140 2023-06-26 23:26:24.000000 reliableGPT-0.2.916/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3061 2023-06-26 23:28:53.000000 reliableGPT-0.2.916/reliablegpt/api_handler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 23:28:52.000000 reliableGPT-0.2.916/reliablegpt/custom_queue.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    14404 2023-06-26 23:28:56.000000 reliableGPT-0.2.916/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1427 2023-06-26 23:10:37.000000 reliableGPT-0.2.916/reliablegpt/test_batching.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.916/reliablegpt/tests_main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 23:29:07.334235 reliableGPT-0.2.916/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      380 2023-06-26 23:29:00.000000 reliableGPT-0.2.916/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-27 00:44:15.933988 reliableGPT-0.2.918/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.918/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-27 00:44:15.933884 reliableGPT-0.2.918/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.918/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-27 00:44:15.932527 reliableGPT-0.2.918/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-27 00:44:15.000000 reliableGPT-0.2.918/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      377 2023-06-27 00:44:15.000000 reliableGPT-0.2.918/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-27 00:44:15.000000 reliableGPT-0.2.918/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-27 00:44:15.000000 reliableGPT-0.2.918/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-27 00:44:15.000000 reliableGPT-0.2.918/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-27 00:44:15.933590 reliableGPT-0.2.918/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      140 2023-06-26 23:38:53.000000 reliableGPT-0.2.918/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3356 2023-06-27 00:43:56.000000 reliableGPT-0.2.918/reliablegpt/api_handler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 23:38:53.000000 reliableGPT-0.2.918/reliablegpt/custom_queue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    15336 2023-06-27 00:44:00.000000 reliableGPT-0.2.918/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1449 2023-06-27 00:39:33.000000 reliableGPT-0.2.918/reliablegpt/test_batch.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1548 2023-06-27 00:43:49.000000 reliableGPT-0.2.918/reliablegpt/test_satya.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.918/reliablegpt/tests_main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-27 00:44:15.934042 reliableGPT-0.2.918/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      380 2023-06-27 00:44:10.000000 reliableGPT-0.2.918/setup.py
```

### Comparing `reliableGPT-0.2.916/LICENSE` & `reliableGPT-0.2.918/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.916/README.md` & `reliableGPT-0.2.918/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.916/reliablegpt/custom_queue.py` & `reliableGPT-0.2.918/reliablegpt/custom_queue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.916/reliablegpt/main.py` & `reliableGPT-0.2.918/reliablegpt/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -173,22 +173,20 @@
         return # safe function, should not impact error handling if logging fails
 
 class batchRequests:
     def __init__(self,
                process_func,
                max_token_capacity,
                max_request_capacity,
-               set_timeout=10,
                verbose=False):
         super().__init__()
         self.api_handler = APICallHandler(max_token_capacity,
                                         max_request_capacity,
                                         verbose=verbose)
         self.process_func = process_func
-        self.set_timeout = set_timeout
         self.verbose = verbose
 
     def print_verbose(self, *args):
         if self.verbose:
             print(*args)
 
     def get_result(self, text):
@@ -203,37 +201,66 @@
 
         while time.time() - start_time < self.set_timeout:
             result = self.api_handler.get_result(task_id)
         if result:
             return result
 
         return None
+    
+    def get_result(self, text, set_timeout):
+        task_id = uuid.uuid4().int
+        self.print_verbose("task_id: ", task_id)
+        self.api_handler.add_task(process_func=self.process_func,
+                                input=text,
+                                task_id=task_id)
+
+        start_time = time.time()
+
+        while time.time() - start_time < set_timeout:
+            result = self.api_handler.get_result(task_id)
+            if result:
+                return result
+
+        return None
+
+    
+    def get_request(self, question, set_timeout=1200):
+        task_id = uuid.uuid4().int
+        self.print_verbose("task_id: ", task_id)
+        self.api_handler.add_task(process_func=self.process_func,
+                                    input=question, task_id=task_id)
+
+        start_time = time.time() 
+        while time.time() - start_time < set_timeout:
+            results = self.api_handler.get_result(task_id=task_id)
+            if results:
+                return results
+        return None
 
     def get_results(self):
         return self.api_handler.get_results()
 
-    def get_result_threaded(self, test_question, results):
+    def get_result_threaded(self, test_question, results, set_timeout):
         self.print_verbose(f"Enters reliableGPT with question: {test_question}")
         start_time = time.time()
-        result = self.get_result(test_question)
+        result = self.get_result(test_question, set_timeout)
         results.append(result)
         end_time = time.time()
         self.print_verbose(f"Gets result from reliableGPT: {result}",
                         end_time - start_time)
 
 
-    def execute(self, questions=[]):
+    def execute(self, questions=[], set_timeout=1200):
         for question in questions: 
             task_id = uuid.uuid4().int
             self.print_verbose("task_id: ", task_id)
             self.api_handler.add_task(process_func=self.process_func,
                                         input=question, task_id=task_id)
-            self.api_handler.set_upperbound(len(questions))
         start_time = time.time() 
-        while time.time() - start_time < self.set_timeout:
+        while time.time() - start_time < set_timeout:
             results = self.api_handler.get_results()
             if len(results) >= len(questions):
                 return results
         return self.api_handler.get_results()
 
 
 
@@ -320,16 +347,14 @@
             result = self.openai_create_function(*args, **kwargs)
             save_request(self, args, kwargs, "", result=result)
             return result
         except Exception as e:
             return self.handle_exception(args, kwargs, e)
 
 
-
-
 ### OpenAI Key Management - Optional code if you want to use reliableGPT for Key Mgmt ###
 def add_keys(user_email="", keys=[]):
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/add_keys"
     if user_email == "":
         return "reliableGPT: Please add an Email to add your keys"
     if len(keys) == 0:
         return "reliableGPT: Please add keys to add"
```

### Comparing `reliableGPT-0.2.916/reliablegpt/test_batching.py` & `reliableGPT-0.2.918/reliablegpt/test_batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import main
 from main import batchRequests
 import openai
 
 
+openai.api_key = "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"
 
 def simple_openai_call(prompt):
   print(f"in simple openai call with question:  {prompt}")
   model = "gpt-4"
   messages = [
     {
       "role": "system",
@@ -20,16 +21,15 @@
   result = openai.ChatCompletion.create(model=model, messages=messages)
   print(f"Result: from open ai for {prompt}, result {result}")
   return result
 
 
 batch_requests = batchRequests(process_func=simple_openai_call,
                               max_token_capacity=40000,
-                              max_request_capacity=200,
-                              set_timeout=12000)
+                              max_request_capacity=200)
 
 list_questions = [
   "What is the difference between a list and a tuple in Python?",
   "How do you iterate over a dictionary in Python?",
   "What is the purpose of the 'self' parameter in a class method?",
   "What are lambda functions in Python?",
   "How do you remove duplicates from a list in Python?",
```

### Comparing `reliableGPT-0.2.916/reliablegpt/tests_main.py` & `reliableGPT-0.2.918/reliablegpt/tests_main.py`

 * *Files identical despite different names*

