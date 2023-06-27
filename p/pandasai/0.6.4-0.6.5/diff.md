# Comparing `tmp/pandasai-0.6.4.tar.gz` & `tmp/pandasai-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.6.4.tar", max compression
+gzip compressed data, was "pandasai-0.6.5.tar", max compression
```

## Comparing `pandasai-0.6.4.tar` & `pandasai-0.6.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1055 2023-06-25 17:11:19.104006 pandasai-0.6.4/LICENSE
--rw-r--r--   0        0        0     7705 2023-06-25 17:11:19.104006 pandasai-0.6.4/README.md
--rw-r--r--   0        0        0    24578 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/__init__.py
--rw-r--r--   0        0        0     1235 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3252 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4119 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10606 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     1828 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      577 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2932 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      558 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1270 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1076 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1081 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1072 2023-06-25 17:11:19.112007 pandasai-0.6.4/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1712 2023-06-25 17:11:19.116006 pandasai-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 pandasai-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-27 01:10:43.634056 pandasai-0.6.5/LICENSE
+-rw-r--r--   0        0        0     7705 2023-06-27 01:10:43.638056 pandasai-0.6.5/README.md
+-rw-r--r--   0        0        0    24805 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/__init__.py
+-rw-r--r--   0        0        0     1235 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3471 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4091 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11077 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4518 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      577 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2932 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      558 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1270 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1076 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1081 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1072 2023-06-27 01:10:43.642057 pandasai-0.6.5/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1900 2023-06-27 01:10:43.646057 pandasai-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.6.5/PKG-INFO
```

### Comparing `pandasai-0.6.4/LICENSE` & `pandasai-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/README.md` & `pandasai-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/__init__.py` & `pandasai-0.6.5/pandasai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,24 +29,26 @@
     llm = OpenAI(api_token="YOUR_API_TOKEN")
 
     pandas_ai = PandasAI(llm)
     pandas_ai(df, prompt='Which are the 5 happiest countries?')
 
     ```
 """
+
 import ast
 import io
 import logging
 import re
 import sys
 import uuid
 import time
 from contextlib import redirect_stdout
 from typing import List, Optional, Union, Dict, Type
-
+import importlib.metadata
+__version__ = importlib.metadata.version(__package__ or __name__)
 import astor
 import pandas as pd
 from .constants import (
     WHITELISTED_BUILTINS,
     WHITELISTED_LIBRARIES,
 )
 from .exceptions import BadImportError, LLMNotFoundError
@@ -156,14 +158,15 @@
     def __init__(
         self,
         llm=None,
         conversational=False,
         verbose=False,
         enforce_privacy=False,
         save_charts=False,
+        save_charts_path=None,
         enable_cache=True,
         middlewares=None,
         custom_whitelisted_dependencies=None,
         enable_logging=True,
         non_default_prompts: Optional[Dict[str, Type[Prompt]]] = None,
     ):
         """
@@ -213,14 +216,15 @@
                 "An LLM should be provided to instantiate a PandasAI instance"
             )
         self._load_llm(llm)
         self._is_conversational_answer = conversational
         self._verbose = verbose
         self._enforce_privacy = enforce_privacy
         self._save_charts = save_charts
+        self._save_charts_path = save_charts_path
         self._process_id = str(uuid.uuid4())
 
         self._non_default_prompts = (
             {} if non_default_prompts is None else non_default_prompts
         )
 
         self.notebook = Notebook()
@@ -623,15 +627,17 @@
 
         """
 
         multiple: bool = isinstance(data_frame, list)
 
         # Add save chart code
         if self._save_charts:
-            code = add_save_chart(code, self._prompt_id, not self._verbose)
+            code = add_save_chart(
+                code, self._prompt_id, self._save_charts_path, not self._verbose
+            )
 
         # Get the code to run removing unsafe imports and df overwrites
         code_to_run = self._clean_code(code)
         self.last_code_executed = code_to_run
         self.log(
             f"""
 Code running:
```

### Comparing `pandasai-0.6.4/pandasai/constants.py` & `pandasai-0.6.5/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/exceptions.py` & `pandasai-0.6.5/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/helpers/_optional.py` & `pandasai-0.6.5/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/helpers/anonymizer.py` & `pandasai-0.6.5/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/helpers/cache.py` & `pandasai-0.6.5/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/helpers/from_excel.py` & `pandasai-0.6.5/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/helpers/notebook.py` & `pandasai-0.6.5/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/helpers/save_chart.py` & `pandasai-0.6.5/pandasai/helpers/save_chart.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,32 +45,42 @@
         return all(
             compare_ast(n1, n2, ignore_args) for n1, n2 in zip_longest(node1, node2)
         )
 
     return node1 == node2
 
 
-def add_save_chart(code: str, folder_name: str, print_save_dir: bool = True) -> str:
+def add_save_chart(
+    code: str,
+    folder_name: str,
+    save_charts_path: str = None,
+    print_save_dir: bool = True,
+) -> str:
     """
     Add line to code that save charts to a file, if plt.show() is called.
 
     Args:
         code (str): Code to add line to.
         folder_name (str): Name of folder to save charts to.
+        save_charts_path (str): User Defined Path to save Charts
         print_save_dir (bool): Print the save directory to the console.
             Defaults to True.
 
     Returns:
         str: Code with line added.
 
     """
 
-    # define chart save directory
-    project_root = dirname(dirname(dirname(__file__)))
-    chart_save_dir = os.path.join(project_root, "exports", "charts", folder_name)
+    if save_charts_path is not None:
+        charts_root_dir = save_charts_path
+    else:
+        # define chart save directory
+        charts_root_dir = dirname(dirname(dirname(__file__)))
+
+    chart_save_dir = os.path.join(charts_root_dir, "exports", "charts", folder_name)
 
     tree = ast.parse(code)
 
     # count number of plt.show() calls
     show_count = sum(
         compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True)
         for node in ast.walk(tree)
```

### Comparing `pandasai-0.6.4/pandasai/helpers/shortcuts.py` & `pandasai-0.6.5/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/llm/azure_openai.py` & `pandasai-0.6.5/pandasai/llm/azure_openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,21 +30,21 @@
 
     api_base: str
     api_type: str = "azure"
     api_version: str
     engine: str
 
     def __init__(
-            self,
-            api_token: Optional[str] = None,
-            api_base: Optional[str] = None,
-            api_version: Optional[str] = None,
-            deployment_name: str = None,
-            is_chat_model: Optional[bool] = False,
-            **kwargs,
+        self,
+        api_token: Optional[str] = None,
+        api_base: Optional[str] = None,
+        api_version: Optional[str] = None,
+        deployment_name: str = None,
+        is_chat_model: Optional[bool] = False,
+        **kwargs,
     ):
         """
         __init__ method of AzureOpenAI Class
 
         Args:
             api_token (str): Azure OpenAI API token.
             api_base (str): Base url of the Azure endpoint.
```

### Comparing `pandasai-0.6.4/pandasai/llm/base.py` & `pandasai-0.6.5/pandasai/llm/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -309,17 +309,17 @@
     """Base class to implement a new Google LLM
 
     LLM base class is extended to be used with Google Palm API.
     """
 
     genai: Any
     temperature: Optional[float] = 0
-    top_p: Optional[float] = None
-    top_k: Optional[float] = None
-    max_output_tokens: Optional[int] = None
+    top_p: Optional[float] = 0.8
+    top_k: Optional[float] = 0.3
+    max_output_tokens: Optional[int] = 1000
 
     def _configure(self, api_key: str):
         """
         Configure Google Palm API Key
         Args:
             api_key (str): A string of API keys generated from Google Cloud
 
@@ -332,14 +332,30 @@
 
         err_msg = "Install google-generativeai >= 0.1 for Google Palm API"
         genai = import_dependency("google.generativeai", extra=err_msg)
 
         genai.configure(api_key=api_key)
         self.genai = genai
 
+    def _configurevertexai(self, project_id: str, location: str):
+        """
+        Configure Google VertexAi
+        Args:
+            project_id: GCP Project
+            location: Location of Project
+
+        Returns: Vertexai Object
+
+        """
+
+        err_msg = "Install google-cloud-aiplatform for Google Vertexai"
+        vertexai = import_dependency("vertexai", extra=err_msg)
+        vertexai.init(project=project_id, location=location)
+        self.vertexai = vertexai
+
     def _valid_params(self):
         return ["temperature", "top_p", "top_k", "max_output_tokens"]
 
     def _set_params(self, **kwargs):
         """
         Set Parameters
         Args:
@@ -390,10 +406,10 @@
             instruction (object): Instruction to pass
             value (str): Value to pass
             suffix (str): Suffix to pass
 
         Returns:
             str: Response
         """
-        self.last_prompt = str(instruction) + str(value)
-        prompt = str(instruction) + str(value) + suffix
+        self.last_prompt = str(instruction) + value
+        prompt = str(instruction) + value + suffix
         return self._generate_text(prompt)
```

### Comparing `pandasai-0.6.4/pandasai/llm/fake.py` & `pandasai-0.6.5/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/llm/falcon.py` & `pandasai-0.6.5/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/llm/langchain.py` & `pandasai-0.6.5/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/llm/open_assistant.py` & `pandasai-0.6.5/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/llm/openai.py` & `pandasai-0.6.5/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/llm/starcoder.py` & `pandasai-0.6.5/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/middlewares/base.py` & `pandasai-0.6.5/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/middlewares/charts.py` & `pandasai-0.6.5/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/middlewares/streamlit.py` & `pandasai-0.6.5/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/prompts/base.py` & `pandasai-0.6.5/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.6.5/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.6.5/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/prompts/generate_python_code.py` & `pandasai-0.6.5/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.6.5/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.4/pyproject.toml` & `pandasai-0.6.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.6.4"
+version = "0.6.5"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
@@ -12,29 +12,35 @@
 python-dotenv = "^1.0.0"
 pandas = "1.5.3"
 astor = "^0.8.1"
 openai = "^0.27.5"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
 google-generativeai = { version = "^0.1.0rc2", optional = true }
+google-cloud-aiplatform = { version = "^1.26.1", optional = true }
 langchain = { version = "^0.0.199", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 ruff = "^0.0.220"
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 pytest-env = "^0.8.1"
 click = "^8.1.3"
 
+
+[tool.poetry.group.extras.dependencies]
+google-cloud-aiplatform = "^1.26.1"
+
 [tool.poetry.extras]
 google = ["google-generativeai"]
 tests = ["numpy", "seaborn"]
 langchain = ["langchain"]
+google-cloud = ["google-cloud-aiplatform"]
 
 [tool.poetry.group.whitelist.dependencies]
 statsmodels = {version = "^0.14.0", optional = true}
 scikit-learn = {version = "^1.2.2", optional = true}
 seaborn = {version = "^0.12.2", optional = true}
 plotly = {version = "^5.14.1", optional = true}
 ggplot = {version = "^0.11.5", optional = true}
```

### Comparing `pandasai-0.6.4/PKG-INFO` & `pandasai-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.6.4
+Version: 0.6.5
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: google
+Provides-Extra: google-cloud
 Provides-Extra: langchain
 Provides-Extra: tests
 Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: google-cloud-aiplatform (>=1.26.1,<2.0.0) ; extra == "google-cloud"
 Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
 Requires-Dist: langchain (>=0.0.199,<0.0.200) ; extra == "langchain"
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
```

