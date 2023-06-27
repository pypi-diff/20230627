# Comparing `tmp/chatlab-0.14.1.tar.gz` & `tmp/chatlab-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatlab-0.14.1.tar", max compression
+gzip compressed data, was "chatlab-0.15.0.tar", max compression
```

## Comparing `chatlab-0.14.1.tar` & `chatlab-0.15.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1504 2023-06-25 18:11:28.688504 chatlab-0.14.1/LICENSE
--rw-r--r--   0        0        0     7121 2023-06-25 18:11:28.688504 chatlab-0.14.1/README.md
--rw-r--r--   0        0        0     1863 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/__init__.py
--rw-r--r--   0        0        0       23 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/_version.py
--rw-r--r--   0        0        0      897 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/builtins.py
--rw-r--r--   0        0        0     9684 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/conversation.py
--rw-r--r--   0        0        0     2382 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/decorators.py
--rw-r--r--   0        0        0     7698 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/display.py
--rw-r--r--   0        0        0      114 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/errors.py
--rw-r--r--   0        0        0     3304 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/markdown.py
--rw-r--r--   0        0        0     3290 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/messaging.py
--rw-r--r--   0        0        0     1869 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/models.py
--rw-r--r--   0        0        0     7212 2023-06-25 18:11:28.688504 chatlab-0.14.1/chatlab/registry.py
--rw-r--r--   0        0        0     2023 2023-06-25 18:11:28.688504 chatlab-0.14.1/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-25 18:11:28.688504 chatlab-0.14.1/tests/__init__.py
--rw-r--r--   0        0        0      357 2023-06-25 18:11:28.688504 chatlab-0.14.1/tests/test_chatlab.py
--rw-r--r--   0        0        0     1103 2023-06-25 18:11:28.688504 chatlab-0.14.1/tests/test_decorators.py
--rw-r--r--   0        0        0     1066 2023-06-25 18:11:28.688504 chatlab-0.14.1/tests/test_messaging.py
--rw-r--r--   0        0        0     6792 2023-06-25 18:11:28.688504 chatlab-0.14.1/tests/test_registry.py
--rw-r--r--   0        0        0     8121 1970-01-01 00:00:00.000000 chatlab-0.14.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-06-27 20:49:59.855197 chatlab-0.15.0/LICENSE
+-rw-r--r--   0        0        0     7121 2023-06-27 20:49:59.855197 chatlab-0.15.0/README.md
+-rw-r--r--   0        0        0     1863 2023-06-27 20:49:59.855197 chatlab-0.15.0/chatlab/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-27 20:49:59.855197 chatlab-0.15.0/chatlab/_version.py
+-rw-r--r--   0        0        0      588 2023-06-27 20:49:59.855197 chatlab-0.15.0/chatlab/builtins.py
+-rw-r--r--   0        0        0     9684 2023-06-27 20:49:59.855197 chatlab-0.15.0/chatlab/conversation.py
+-rw-r--r--   0        0        0     2382 2023-06-27 20:49:59.859197 chatlab-0.15.0/chatlab/decorators.py
+-rw-r--r--   0        0        0     7995 2023-06-27 20:49:59.859197 chatlab-0.15.0/chatlab/display.py
+-rw-r--r--   0        0        0      114 2023-06-27 20:49:59.859197 chatlab-0.15.0/chatlab/errors.py
+-rw-r--r--   0        0        0     3304 2023-06-27 20:49:59.859197 chatlab-0.15.0/chatlab/markdown.py
+-rw-r--r--   0        0        0     3290 2023-06-27 20:49:59.859197 chatlab-0.15.0/chatlab/messaging.py
+-rw-r--r--   0        0        0     1869 2023-06-27 20:49:59.859197 chatlab-0.15.0/chatlab/models.py
+-rw-r--r--   0        0        0     7343 2023-06-27 20:49:59.859197 chatlab-0.15.0/chatlab/registry.py
+-rw-r--r--   0        0        0     5783 2023-06-27 20:49:59.859197 chatlab-0.15.0/chatlab/shells/python.py
+-rw-r--r--   0        0        0     2119 2023-06-27 20:49:59.859197 chatlab-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-27 20:49:59.859197 chatlab-0.15.0/tests/__init__.py
+-rw-r--r--   0        0        0      357 2023-06-27 20:49:59.859197 chatlab-0.15.0/tests/test_chatlab.py
+-rw-r--r--   0        0        0     1103 2023-06-27 20:49:59.859197 chatlab-0.15.0/tests/test_decorators.py
+-rw-r--r--   0        0        0     1066 2023-06-27 20:49:59.859197 chatlab-0.15.0/tests/test_messaging.py
+-rw-r--r--   0        0        0     5977 2023-06-27 20:49:59.859197 chatlab-0.15.0/tests/test_registry.py
+-rw-r--r--   0        0        0     8284 1970-01-01 00:00:00.000000 chatlab-0.15.0/PKG-INFO
```

### Comparing `chatlab-0.14.1/LICENSE` & `chatlab-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.1/README.md` & `chatlab-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.1/chatlab/__init__.py` & `chatlab-0.15.0/chatlab/__init__.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.1/chatlab/conversation.py` & `chatlab-0.15.0/chatlab/conversation.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.1/chatlab/decorators.py` & `chatlab-0.15.0/chatlab/decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.1/chatlab/display.py` & `chatlab-0.15.0/chatlab/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,18 +168,20 @@
 
         # Execute the function and get the result
         try:
             output = self.function_registry.call(function_name, function_args)
         except FunctionArgumentError as e:
             self.finished = True
             self.set_state("Errored")
+            self.function_result = repr(e)
             return system(f"Function arguments for {function_name} were invalid: {e}")
         except UnknownFunctionError as e:
             self.finished = True
             self.set_state("No function named")
+            self.function_result = repr(e)
             return system(f"Function {function_name} not found in function registry: {e}")
         except Exception as e:
             # Check to see if the user has requested that the exception be exposed to LLM.
             # If not, then we just raise it and let the user handle it.
             chatlab_metadata = self.function_registry.get_chatlab_metadata(function_name)
 
             if not chatlab_metadata.expose_exception_to_llm:
@@ -191,15 +193,21 @@
             self.function_result = repr_llm
             self.finished = True
             self.state = "Errored"
             self.update_displays()
 
             return function_result(name=function_name, content=repr_llm)
 
-        repr_llm = repr(output)
+        repr_llm = ""
+        if isinstance(output, str):
+            repr_llm = output
+        elif getattr(output, "_repr_llm_", None) is not None:
+            repr_llm = output._repr_llm_()
+        else:
+            repr_llm = repr(output)
 
         self.function_result = repr_llm
         self.finished = True
         self.state = "Ran"
         self.update_displays()
 
         return function_result(name=function_name, content=repr_llm)
```

### Comparing `chatlab-0.14.1/chatlab/markdown.py` & `chatlab-0.15.0/chatlab/markdown.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.1/chatlab/messaging.py` & `chatlab-0.15.0/chatlab/messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.1/chatlab/models.py` & `chatlab-0.15.0/chatlab/models.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.1/chatlab/registry.py` & `chatlab-0.15.0/chatlab/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -207,15 +207,18 @@
         elif arguments is None or arguments == "":
             parameters = {}
         else:
             try:
                 parameters = json.loads(arguments)
                 # TODO: Validate parameters against schema
             except json.JSONDecodeError:
-                raise FunctionArgumentError(f"Invalid JSON for parameters of function {name}")
+                raise FunctionArgumentError(f"Invalid Function call on {name}. Arguments must be a valid JSON object")
+
+        if function is None:
+            raise UnknownFunctionError(f"Function {name} is not registered")
 
         result = function(**parameters)
         return result
 
     def __contains__(self, name) -> bool:
         """Check if a function is registered by name."""
         return name in self.__functions
```

### Comparing `chatlab-0.14.1/pyproject.toml` & `chatlab-0.15.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatlab"
-version = "0.14.1"
+version = "0.15.0"
 homepage = "https://github.com/rgbkrk/chatlab"
 description = "Markdown for LLMs."
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -25,14 +25,18 @@
 python = ">=3.9.0,<3.12"
 ipython = "^8.12.0"
 openai = "^0.27.4"
 pydantic = "^1.10.9"
 typing-extensions = "^4.6.3"
 vdom = "^1.0.0"
 deprecation = "^2.1.0"
+tabulate = "^0.9.0"
+ipykernel = "^6.23.3"
+pyte = "^0.8.1"
+repr-llm = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.4.11"
 black = "^23.3.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.7.0"
@@ -44,14 +48,15 @@
 twine = "^4.0.2"
 pre-commit = "^3.2.2"
 toml = "^0.10.2"
 bump2version = "^1.0.1"
 jinja2 = "^3.1.2"
 ipykernel = "^6.23.2"
 types-toml = "^0.10.8.6"
+pandas = "^2.0.2"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "mypy",
```

### Comparing `chatlab-0.14.1/tests/test_decorators.py` & `chatlab-0.15.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.1/tests/test_messaging.py` & `chatlab-0.15.0/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-0.14.1/tests/test_registry.py` & `chatlab-0.15.0/tests/test_registry.py`

 * *Files 15% similar despite different names*

```diff
@@ -88,15 +88,17 @@
     with pytest.raises(UnknownFunctionError, match="Function unknown is not registered"):
         registry.call("unknown")
 
 
 def test_function_registry_function_argument_error():
     registry = FunctionRegistry()
     registry.register(simple_func, SimpleModel)
-    with pytest.raises(FunctionArgumentError, match="Invalid JSON for parameters of function simple_func"):
+    with pytest.raises(
+        FunctionArgumentError, match="Invalid Function call on simple_func. Arguments must be a valid JSON object"
+    ):
         registry.call("simple_func", arguments="not json")
 
 
 def test_function_registry_call():
     registry = FunctionRegistry()
     registry.register(simple_func, SimpleModel)
     result = registry.call("simple_func", arguments='{"x": 1, "y": "str", "z": true}')
@@ -130,35 +132,14 @@
     registry = FunctionRegistry()
     registry.register(simple_func, SimpleModel)
     function_definitions = registry.function_definitions
     assert len(function_definitions) == 1
     assert function_definitions[0]["name"] == "simple_func"
 
 
-# Testing for registry's call method with a valid python hallucination
-# Note that unlike all other functions, we allow the LLM to pass us a string
-# likely containing newlines. No JSON here.
-@patch('chatlab.builtins.get_ipython')
-def test_function_registry_call_python_hallucination_valid(mock_get_ipython):
-    # Set up the mock
-    mock_ipython_instance = MagicMock()
-    mock_run_cell = MagicMock()
-    mock_run_cell.return_value.result = 5
-    mock_ipython_instance.run_cell = mock_run_cell
-    mock_get_ipython.return_value = mock_ipython_instance
-
-    registry = FunctionRegistry(allow_hallucinated_python=True)
-    result = registry.call("python", arguments='2+3')
-
-    # Assert the result and that the mock was called correctly
-    mock_get_ipython.assert_called_once()
-    mock_run_cell.assert_called_once_with("2+3")
-    assert result == 5
-
-
 # Test that we do not allow python hallucination when False
 def test_function_registry_call_python_hallucination_invalid():
     registry = FunctionRegistry(allow_hallucinated_python=False)
     with pytest.raises(Exception, match="Function python is not registered"):
         registry.call("python", arguments='1 + 4')
```

### Comparing `chatlab-0.14.1/PKG-INFO` & `chatlab-0.15.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatlab
-Version: 0.14.1
+Version: 0.15.0
 Summary: Markdown for LLMs.
 Home-page: https://github.com/rgbkrk/chatlab
 License: BSD-3-Clause
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,17 +15,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: dev
 Provides-Extra: test
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
+Requires-Dist: ipykernel (>=6.23.3,<7.0.0)
 Requires-Dist: ipython (>=8.12.0,<9.0.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: pyte (>=0.8.1,<0.9.0)
+Requires-Dist: repr-llm (>=0.1.0,<0.2.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Requires-Dist: vdom (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ChatLab
 
 **Chat Experiments, Simplified**
```

