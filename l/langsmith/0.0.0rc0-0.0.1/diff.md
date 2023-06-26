# Comparing `tmp/langsmith-0.0.0rc0.tar.gz` & `tmp/langsmith-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsmith-0.0.0rc0.tar", max compression
+gzip compressed data, was "langsmith-0.0.1.tar", max compression
```

## Comparing `langsmith-0.0.0rc0.tar` & `langsmith-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     8006 2023-06-26 21:49:14.459291 langsmith-0.0.0rc0/README.md
--rw-r--r--   0        0        0      479 2023-06-26 21:47:00.744671 langsmith-0.0.0rc0/langsmith/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 22:33:42.162840 langsmith-0.0.0rc0/langsmith/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-06-06 22:33:42.162946 langsmith-0.0.0rc0/langsmith/cli/conf/nginx.conf
--rw-r--r--   0        0        0      315 2023-06-06 22:33:42.163009 langsmith-0.0.0rc0/langsmith/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1061 2023-06-14 13:47:41.867397 langsmith-0.0.0rc0/langsmith/cli/docker-compose.yaml
--rw-r--r--   0        0        0    14097 2023-06-26 21:46:06.630189 langsmith-0.0.0rc0/langsmith/cli/main.py
--rw-r--r--   0        0        0    27732 2023-06-26 21:47:00.748635 langsmith-0.0.0rc0/langsmith/client.py
--rw-r--r--   0        0        0      234 2023-06-26 21:42:08.517344 langsmith-0.0.0rc0/langsmith/evaluation/__init__.py
--rw-r--r--   0        0        0     1411 2023-06-26 21:42:08.531755 langsmith-0.0.0rc0/langsmith/evaluation/evaluator.py
--rw-r--r--   0        0        0     1529 2023-06-26 21:42:08.531868 langsmith-0.0.0rc0/langsmith/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     9462 2023-06-26 21:42:08.517144 langsmith-0.0.0rc0/langsmith/run_helpers.py
--rw-r--r--   0        0        0     6120 2023-06-26 21:49:42.954134 langsmith-0.0.0rc0/langsmith/run_trees.py
--rw-r--r--   0        0        0     6575 2023-06-23 09:42:59.404625 langsmith-0.0.0rc0/langsmith/schemas.py
--rw-r--r--   0        0        0     3688 2023-06-26 21:48:34.873509 langsmith-0.0.0rc0/langsmith/utils.py
--rw-r--r--   0        0        0      881 2023-06-26 22:04:27.754542 langsmith-0.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0     8612 1970-01-01 00:00:00.000000 langsmith-0.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     8006 2023-06-26 21:49:14.459291 langsmith-0.0.1/README.md
+-rw-r--r--   0        0        0      479 2023-06-26 21:47:00.744671 langsmith-0.0.1/langsmith/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:33:42.162840 langsmith-0.0.1/langsmith/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-06 22:33:42.162946 langsmith-0.0.1/langsmith/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      315 2023-06-06 22:33:42.163009 langsmith-0.0.1/langsmith/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1061 2023-06-14 13:47:41.867397 langsmith-0.0.1/langsmith/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    14097 2023-06-26 21:46:06.630189 langsmith-0.0.1/langsmith/cli/main.py
+-rw-r--r--   0        0        0    27732 2023-06-26 21:47:00.748635 langsmith-0.0.1/langsmith/client.py
+-rw-r--r--   0        0        0      234 2023-06-26 21:42:08.517344 langsmith-0.0.1/langsmith/evaluation/__init__.py
+-rw-r--r--   0        0        0     1411 2023-06-26 21:42:08.531755 langsmith-0.0.1/langsmith/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1529 2023-06-26 21:42:08.531868 langsmith-0.0.1/langsmith/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     9462 2023-06-26 21:42:08.517144 langsmith-0.0.1/langsmith/run_helpers.py
+-rw-r--r--   0        0        0     6120 2023-06-26 21:49:42.954134 langsmith-0.0.1/langsmith/run_trees.py
+-rw-r--r--   0        0        0     6575 2023-06-23 09:42:59.404625 langsmith-0.0.1/langsmith/schemas.py
+-rw-r--r--   0        0        0     3688 2023-06-26 21:48:34.873509 langsmith-0.0.1/langsmith/utils.py
+-rw-r--r--   0        0        0      878 2023-06-26 22:59:57.421302 langsmith-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8609 1970-01-01 00:00:00.000000 langsmith-0.0.1/PKG-INFO
```

### Comparing `langsmith-0.0.0rc0/README.md` & `langsmith-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.0rc0/langsmith/cli/docker-compose.yaml` & `langsmith-0.0.1/langsmith/cli/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.0rc0/langsmith/cli/main.py` & `langsmith-0.0.1/langsmith/cli/main.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.0rc0/langsmith/client.py` & `langsmith-0.0.1/langsmith/client.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.0rc0/langsmith/evaluation/evaluator.py` & `langsmith-0.0.1/langsmith/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.0rc0/langsmith/evaluation/string_evaluator.py` & `langsmith-0.0.1/langsmith/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.0rc0/langsmith/run_helpers.py` & `langsmith-0.0.1/langsmith/run_helpers.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.0rc0/langsmith/run_trees.py` & `langsmith-0.0.1/langsmith/run_trees.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.0rc0/langsmith/schemas.py` & `langsmith-0.0.1/langsmith/schemas.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.0rc0/langsmith/utils.py` & `langsmith-0.0.1/langsmith/utils.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.0rc0/pyproject.toml` & `langsmith-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langsmith"
-version = "0.0.0rc0"
+version = "0.0.1"
 description = "Client library to connect to the LangSmith LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langsmith"}]
 
 [tool.poetry.scripts]
```

### Comparing `langsmith-0.0.0rc0/PKG-INFO` & `langsmith-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsmith
-Version: 0.0.0rc0
+Version: 0.0.1
 Summary: Client library to connect to the LangSmith LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

