# Comparing `tmp/parsagon-0.7.1.tar.gz` & `tmp/parsagon-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.7.1.tar", last modified: Fri Jun 23 09:51:50 2023, max compression
+gzip compressed data, was "parsagon-0.7.2.tar", last modified: Tue Jun 27 10:13:26 2023, max compression
```

## Comparing `parsagon-0.7.1.tar` & `parsagon-0.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-23 09:51:50.884628 parsagon-0.7.1/
--rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-23 09:51:50.884159 parsagon-0.7.1/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 20:10:33.000000 parsagon-0.7.1/README.md
--rw-r--r--   0 amsuh    (10002)    18010      935 2023-06-23 09:51:06.000000 parsagon-0.7.1/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-23 09:51:50.884807 parsagon-0.7.1/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-23 09:51:50.872076 parsagon-0.7.1/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.1/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-23 09:51:50.877690 parsagon-0.7.1/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       46 2023-06-19 21:24:16.000000 parsagon-0.7.1/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3634 2023-06-20 03:09:34.000000 parsagon-0.7.1/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.1/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010    10224 2023-06-23 09:50:27.000000 parsagon-0.7.1/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     6683 2023-06-21 21:23:22.000000 parsagon-0.7.1/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     1085 2023-06-18 04:18:36.000000 parsagon-0.7.1/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-23 09:51:50.883661 parsagon-0.7.1/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.1/src/parsagon/tests/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-23 09:51:50.882817 parsagon-0.7.1/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      437 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      209 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-23 09:51:50.000000 parsagon-0.7.1/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-27 10:13:26.074568 parsagon-0.7.2/
+-rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-27 10:13:26.074024 parsagon-0.7.2/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 20:10:33.000000 parsagon-0.7.2/README.md
+-rw-r--r--   0 amsuh    (10002)    18010      935 2023-06-27 10:04:55.000000 parsagon-0.7.2/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-27 10:13:26.074711 parsagon-0.7.2/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-27 10:13:26.063509 parsagon-0.7.2/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.2/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-27 10:13:26.068215 parsagon-0.7.2/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       46 2023-06-26 21:26:23.000000 parsagon-0.7.2/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3678 2023-06-27 10:04:55.000000 parsagon-0.7.2/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.2/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010    10517 2023-06-27 10:04:55.000000 parsagon-0.7.2/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     7100 2023-06-27 10:04:55.000000 parsagon-0.7.2/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     1085 2023-06-18 04:18:36.000000 parsagon-0.7.2/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-27 10:13:26.073542 parsagon-0.7.2/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.2/src/parsagon/tests/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-27 10:13:26.072877 parsagon-0.7.2/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      437 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      209 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.7.1/PKG-INFO` & `parsagon-0.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.1
+Version: 0.7.2
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.7.1/README.md` & `parsagon-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.1/pyproject.toml` & `parsagon-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.7.1"
+version = "0.7.2"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
```

### Comparing `parsagon-0.7.1/src/parsagon/api.py` & `parsagon-0.7.2/src/parsagon/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,17 @@
     )
 
 
 def get_pipelines():
     return _api_call(httpx.get, f"/pipelines/")
 
 
-def get_pipeline_code(pipeline_name, variables, environment):
+def get_pipeline_code(pipeline_name, variables, environment, headless):
     return _api_call(
         httpx.post,
         f"/pipelines/name/{pipeline_name}/code/",
         json={
             "variables": variables,
             "environment": environment,
+            "headless": headless,
         },
     )
```

### Comparing `parsagon-0.7.1/src/parsagon/custom_function.py` & `parsagon-0.7.2/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.1/src/parsagon/executor.py` & `parsagon-0.7.2/src/parsagon/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 import time
 
 import lxml.html
+from pyvirtualdisplay import Display
 from selenium import webdriver
 import seleniumwire.undetected_chromedriver as uc
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.select import Select
 
@@ -27,15 +28,18 @@
 
 
 class Executor:
     """
     Executes code produced by GPT with the proper context.  Records custom_function usage along the way.
     """
 
-    def __init__(self):
+    def __init__(self, headless=False):
+        self.headless = headless
+        if self.headless:
+            self.display = Display(visible=False, size=(1280, 1050)).start()
         chrome_options = uc.ChromeOptions()
         chrome_options.add_argument("--start-maximized")
         seleniumwire_options = {"disable_capture": True}
         self.driver = uc.Chrome(options=chrome_options, seleniumwire_options=seleniumwire_options)
         self.max_elem_id = 0
         self.execution_context = {
             "goto": self.goto,
@@ -290,9 +294,13 @@
                 }
             ],
         )
         self.add_custom_function(call_id, custom_function)
         return result["data"]
 
     def execute(self, code):
-        exec(code, self.execution_context)
-        self.driver.quit()
+        try:
+            exec(code, self.execution_context)
+        finally:
+            self.driver.quit()
+            if self.headless:
+                self.display.stop()
```

### Comparing `parsagon-0.7.1/src/parsagon/main.py` & `parsagon-0.7.2/src/parsagon/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,19 @@
     parser_create.add_argument(
         "-p",
         "--program",
         dest="program_name",
         type=str,
         help="the name of the program to create (otherwise user input is required)",
     )
+    parser_create.add_argument(
+        "--headless",
+        action="store_true",
+        help="run the browser in headless mode",
+    )
     parser_create.set_defaults(func=create)
 
     # Detail
     parser_detail = subparsers.add_parser(
         "detail",
         description="Outputs details of a created program.",
     )
@@ -73,14 +78,19 @@
     )
     parser_run.add_argument(
         "--variables",
         type=json.loads,
         default="{}",
         help="a JSON object mapping variables to values",
     )
+    parser_run.add_argument(
+        "--headless",
+        action="store_true",
+        help="run the browser in headless mode",
+    )
     parser_run.set_defaults(func=run)
 
     # Delete
     parser_delete = subparsers.add_parser(
         "delete",
         description="Deletes a program.",
     )
@@ -99,27 +109,27 @@
 
     if func:
         return func(**kwargs)
     else:
         parser.print_help()
 
 
-def create(task, program_name=None, verbose=False):
+def create(task, program_name=None, headless=False, verbose=False):
     logger.info("Launched with task description:\n%s", task)
 
     logger.info("Analyzing task description...")
     program_sketches = get_program_sketches(task)
 
     full_program = program_sketches["full"]
     abridged_program = program_sketches["abridged"]
     logger.debug("Program:\n%s", abridged_program)
     abridged_program += "\n\noutput = func()\nprint(f'Program finished and returned a value of:\\n{output}')\n"  # Make the program runnable
 
     # Execute the abridged program to gather examples
-    executor = Executor()
+    executor = Executor(headless=headless)
     executor.execute(abridged_program)
 
     # The user must select a name
     while True:
         if not program_name:
             program_name = input("Name this program, or press enter without typing a name to DISCARD: ")
         if program_name:
@@ -163,35 +173,37 @@
         data = get_pipelines()
     for pipeline in data:
         print(
             f"Program: {pipeline['name']}\nDescription: {pipeline['description']}\nVariables: {pipeline['variables']}\n"
         )
 
 
-def run(program_name, variables={}, environment="LOCAL", verbose=False):
+def run(program_name, variables={}, environment="LOCAL", headless=False, verbose=False):
     """
     Executes pipeline code
     """
     logger.info("Preparing to run program %s", program_name)
     try:
-        code = get_pipeline_code(program_name, variables, environment)["code"]
+        code = get_pipeline_code(program_name, variables, environment, headless)["code"]
     except APIException as e:
         if isinstance(e.value, dict) and e.value.get("detail") == "Not found.":
             logger.error("Error: A program with this name does not exist.")
             return
         else:
             raise e
 
     logger.info("Running program...")
     globals_locals = {"PARSAGON_API_KEY": settings.API_KEY}
     try:
         exec(code, globals_locals, globals_locals)
     finally:
         if "driver" in globals_locals:
             globals_locals["driver"].quit()
+        if "display" in globals_locals:
+            globals_locals["display"].stop()
     logger.info("Done.")
     return globals_locals["output"]
 
 
 def delete(program_name, verbose=False):
     logger.info("Preparing to delete program %s", program_name)
     try:
```

### Comparing `parsagon-0.7.1/src/parsagon/settings.py` & `parsagon-0.7.2/src/parsagon/settings.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.1/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.7.2/src/parsagon.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.1
+Version: 0.7.2
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

