# Comparing `tmp/chatgpt_functions-0.1.0.tar.gz` & `tmp/chatgpt_functions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_functions-0.1.0.tar", last modified: Mon Jun 26 15:38:18 2023, max compression
+gzip compressed data, was "chatgpt_functions-0.1.1.tar", last modified: Tue Jun 27 14:38:43 2023, max compression
```

## Comparing `chatgpt_functions-0.1.0.tar` & `chatgpt_functions-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 15:38:18.196909 chatgpt_functions-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-06-26 13:13:15.000000 chatgpt_functions-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1935 2023-06-26 15:38:18.199911 chatgpt_functions-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1374 2023-06-26 12:54:41.000000 chatgpt_functions-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 15:38:18.127758 chatgpt_functions-0.1.0/chatgpt_functions/
--rw-rw-rw-   0        0        0       83 2023-06-26 13:35:12.000000 chatgpt_functions-0.1.0/chatgpt_functions/__init__.py
--rw-rw-rw-   0        0        0     2060 2023-06-26 12:52:30.000000 chatgpt_functions-0.1.0/chatgpt_functions/chatgpt.py
--rw-rw-rw-   0        0        0      722 2023-06-26 11:01:56.000000 chatgpt_functions-0.1.0/chatgpt_functions/chatgpt_function.py
--rw-rw-rw-   0        0        0      476 2023-06-26 15:36:46.000000 chatgpt_functions-0.1.0/chatgpt_functions/chatgpt_types.py
--rw-rw-rw-   0        0        0     1319 2023-06-26 12:53:31.000000 chatgpt_functions-0.1.0/chatgpt_functions/function_parameters.py
-drwxrwxrwx   0        0        0        0 2023-06-26 15:38:18.192389 chatgpt_functions-0.1.0/chatgpt_functions.egg-info/
--rw-rw-rw-   0        0        0     1935 2023-06-26 15:38:17.000000 chatgpt_functions-0.1.0/chatgpt_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-06-26 15:38:17.000000 chatgpt_functions-0.1.0/chatgpt_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 15:38:17.000000 chatgpt_functions-0.1.0/chatgpt_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-26 15:38:17.000000 chatgpt_functions-0.1.0/chatgpt_functions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-26 15:38:17.000000 chatgpt_functions-0.1.0/chatgpt_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      682 2023-06-26 14:36:57.000000 chatgpt_functions-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 15:38:18.205426 chatgpt_functions-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      875 2023-06-26 15:37:58.000000 chatgpt_functions-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:38:43.840599 chatgpt_functions-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-26 13:13:15.000000 chatgpt_functions-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1935 2023-06-27 14:38:43.840599 chatgpt_functions-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1374 2023-06-26 12:54:41.000000 chatgpt_functions-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 14:38:43.824799 chatgpt_functions-0.1.1/chatgpt_functions/
+-rw-rw-rw-   0        0        0       83 2023-06-26 13:35:12.000000 chatgpt_functions-0.1.1/chatgpt_functions/__init__.py
+-rw-rw-rw-   0        0        0     2222 2023-06-27 12:49:29.000000 chatgpt_functions-0.1.1/chatgpt_functions/chatgpt.py
+-rw-rw-rw-   0        0        0      722 2023-06-26 11:01:56.000000 chatgpt_functions-0.1.1/chatgpt_functions/chatgpt_function.py
+-rw-rw-rw-   0        0        0      476 2023-06-26 15:36:46.000000 chatgpt_functions-0.1.1/chatgpt_functions/chatgpt_types.py
+-rw-rw-rw-   0        0        0     1319 2023-06-26 12:53:31.000000 chatgpt_functions-0.1.1/chatgpt_functions/function_parameters.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:38:43.838573 chatgpt_functions-0.1.1/chatgpt_functions.egg-info/
+-rw-rw-rw-   0        0        0     1935 2023-06-27 14:38:43.000000 chatgpt_functions-0.1.1/chatgpt_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-06-27 14:38:43.000000 chatgpt_functions-0.1.1/chatgpt_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 14:38:43.000000 chatgpt_functions-0.1.1/chatgpt_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-27 14:38:43.000000 chatgpt_functions-0.1.1/chatgpt_functions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-27 14:38:43.000000 chatgpt_functions-0.1.1/chatgpt_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      682 2023-06-26 14:36:57.000000 chatgpt_functions-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 14:38:43.843575 chatgpt_functions-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-06-27 12:46:31.000000 chatgpt_functions-0.1.1/setup.py
```

### Comparing `chatgpt_functions-0.1.0/LICENSE` & `chatgpt_functions-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.1.0/PKG-INFO` & `chatgpt_functions-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt_functions
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper over the gpt3.5 model, capable of calling functions
 Home-page: https://github.com/Wellmare/chatgpt-functions
 Author: Wellmare
 Author-email: ivan.kolipov@gmail.com
 Keywords: chatgpt functions gpt
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatgpt_functions-0.1.0/README.md` & `chatgpt_functions-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.1.0/chatgpt_functions/chatgpt.py` & `chatgpt_functions-0.1.1/chatgpt_functions/chatgpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,35 @@
         model: str = "gpt-3.5-turbo-0613",
     ):
         openai.api_key = openai_api_key
         self.model = model
         self.messages: list[Message] = []
 
     async def get_chatgpt_response_with_functions(
-        self, functions: list[ChatGptFunction], messages: list[Message] | None = None
+        self,
+        functions: list[ChatGptFunction],
+        messages: list[Message] | None = None,
+        temperature: float = 0.5,
+        max_tokens: int = 1024,
     ) -> None | str:
         if messages is not None:
             self.messages = messages
         functions_to_chatgpt = [
             function.append_avaliable_functions(self.AVAILABLE_FUNCTIONS)
             or function.__dict__()
             for function in functions
         ]
 
         response = await openai.ChatCompletion.acreate(
             model="gpt-3.5-turbo-0613",
             messages=[message.__dict__() for message in self.messages],
             functions=functions_to_chatgpt,
-            function_call="auto",  # auto is default, but we'll be explicit
+            function_call="auto",  # auto is default, but we'll be explicit,
+            temperature=temperature,
+            max_tokens=max_tokens,
         )
         response_message = response["choices"][0]["message"]
         print(response_message)
 
         if response_message.get("function_call"):
             # Step 3: call the function
             # Note: the JSON response may not always be valid; be sure to handle errors
```

### Comparing `chatgpt_functions-0.1.0/chatgpt_functions/chatgpt_function.py` & `chatgpt_functions-0.1.1/chatgpt_functions/chatgpt_function.py`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.1.0/chatgpt_functions/function_parameters.py` & `chatgpt_functions-0.1.1/chatgpt_functions/function_parameters.py`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.1.0/chatgpt_functions.egg-info/PKG-INFO` & `chatgpt_functions-0.1.1/chatgpt_functions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-functions
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper over the gpt3.5 model, capable of calling functions
 Home-page: https://github.com/Wellmare/chatgpt-functions
 Author: Wellmare
 Author-email: ivan.kolipov@gmail.com
 Keywords: chatgpt functions gpt
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatgpt_functions-0.1.0/pyproject.toml` & `chatgpt_functions-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.1.0/setup.py` & `chatgpt_functions-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(
     name="chatgpt_functions",
-    version="0.1.0",
+    version="0.1.1",
     author="Wellmare",
     author_email="ivan.kolipov@gmail.com",
     description="Wrapper over the gpt3.5 model, capable of calling functions",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/Wellmare/chatgpt-functions",
     packages=find_packages(),
```

