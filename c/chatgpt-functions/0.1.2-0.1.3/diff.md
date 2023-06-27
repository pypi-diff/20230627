# Comparing `tmp/chatgpt_functions-0.1.2.tar.gz` & `tmp/chatgpt_functions-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_functions-0.1.2.tar", last modified: Tue Jun 27 15:10:52 2023, max compression
+gzip compressed data, was "chatgpt_functions-0.1.3.tar", last modified: Tue Jun 27 15:33:02 2023, max compression
```

## Comparing `chatgpt_functions-0.1.2.tar` & `chatgpt_functions-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 15:10:52.825977 chatgpt_functions-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-06-26 13:13:15.000000 chatgpt_functions-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1935 2023-06-27 15:10:52.826985 chatgpt_functions-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1374 2023-06-26 12:54:41.000000 chatgpt_functions-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 15:10:52.808933 chatgpt_functions-0.1.2/chatgpt_functions/
--rw-rw-rw-   0        0        0       83 2023-06-26 13:35:12.000000 chatgpt_functions-0.1.2/chatgpt_functions/__init__.py
--rw-rw-rw-   0        0        0     2226 2023-06-27 15:07:15.000000 chatgpt_functions-0.1.2/chatgpt_functions/chatgpt.py
--rw-rw-rw-   0        0        0      722 2023-06-26 11:01:56.000000 chatgpt_functions-0.1.2/chatgpt_functions/chatgpt_function.py
--rw-rw-rw-   0        0        0      476 2023-06-26 15:36:46.000000 chatgpt_functions-0.1.2/chatgpt_functions/chatgpt_types.py
--rw-rw-rw-   0        0        0     1319 2023-06-26 12:53:31.000000 chatgpt_functions-0.1.2/chatgpt_functions/function_parameters.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:10:52.823461 chatgpt_functions-0.1.2/chatgpt_functions.egg-info/
--rw-rw-rw-   0        0        0     1935 2023-06-27 15:10:52.000000 chatgpt_functions-0.1.2/chatgpt_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-06-27 15:10:52.000000 chatgpt_functions-0.1.2/chatgpt_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 15:10:52.000000 chatgpt_functions-0.1.2/chatgpt_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-27 15:10:52.000000 chatgpt_functions-0.1.2/chatgpt_functions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-27 15:10:52.000000 chatgpt_functions-0.1.2/chatgpt_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      682 2023-06-26 14:36:57.000000 chatgpt_functions-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-27 15:10:52.829987 chatgpt_functions-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      875 2023-06-27 15:09:52.000000 chatgpt_functions-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:02.347543 chatgpt_functions-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-26 13:13:15.000000 chatgpt_functions-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1935 2023-06-27 15:33:02.348543 chatgpt_functions-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1374 2023-06-26 12:54:41.000000 chatgpt_functions-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:02.330490 chatgpt_functions-0.1.3/chatgpt_functions/
+-rw-rw-rw-   0        0        0       83 2023-06-26 13:35:12.000000 chatgpt_functions-0.1.3/chatgpt_functions/__init__.py
+-rw-rw-rw-   0        0        0     2858 2023-06-27 15:30:53.000000 chatgpt_functions-0.1.3/chatgpt_functions/chatgpt.py
+-rw-rw-rw-   0        0        0      722 2023-06-26 11:01:56.000000 chatgpt_functions-0.1.3/chatgpt_functions/chatgpt_function.py
+-rw-rw-rw-   0        0        0      476 2023-06-26 15:36:46.000000 chatgpt_functions-0.1.3/chatgpt_functions/chatgpt_types.py
+-rw-rw-rw-   0        0        0     1319 2023-06-26 12:53:31.000000 chatgpt_functions-0.1.3/chatgpt_functions/function_parameters.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:33:02.345537 chatgpt_functions-0.1.3/chatgpt_functions.egg-info/
+-rw-rw-rw-   0        0        0     1935 2023-06-27 15:33:02.000000 chatgpt_functions-0.1.3/chatgpt_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-06-27 15:33:02.000000 chatgpt_functions-0.1.3/chatgpt_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 15:33:02.000000 chatgpt_functions-0.1.3/chatgpt_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-27 15:33:02.000000 chatgpt_functions-0.1.3/chatgpt_functions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-27 15:33:02.000000 chatgpt_functions-0.1.3/chatgpt_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      682 2023-06-26 14:36:57.000000 chatgpt_functions-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 15:33:02.349542 chatgpt_functions-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-06-27 15:32:49.000000 chatgpt_functions-0.1.3/setup.py
```

### Comparing `chatgpt_functions-0.1.2/LICENSE` & `chatgpt_functions-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.1.2/PKG-INFO` & `chatgpt_functions-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt_functions
-Version: 0.1.2
+Version: 0.1.3
 Summary: Wrapper over the gpt3.5 model, capable of calling functions
 Home-page: https://github.com/Wellmare/chatgpt-functions
 Author: Wellmare
 Author-email: ivan.kolipov@gmail.com
 Keywords: chatgpt functions gpt
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatgpt_functions-0.1.2/README.md` & `chatgpt_functions-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.1.2/chatgpt_functions/chatgpt.py` & `chatgpt_functions-0.1.3/chatgpt_functions/chatgpt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import json
 
 import openai
 from .chatgpt_function import ChatGptFunction
 from .chatgpt_types import Message, Roles
 from .function_parameters import Parameters, Property
+import typing
+from dataclasses import dataclass
+
+
+@dataclass
+class ChatGPTMethodReponse:
+    is_function_called: bool
+    function_response: None | typing.Any
+    chatgpt_response_message: Message
 
 
 class ChatGPT:
     AVAILABLE_FUNCTIONS = {}
 
     def __init__(
         self,
@@ -21,15 +30,15 @@
 
     async def get_chatgpt_response_with_functions(
         self,
         functions: list[ChatGptFunction],
         messages: list[Message] | None = None,
         temperature: float = 0.5,
         max_tokens: int = 1024,
-    ) -> None | Message:
+    ) -> ChatGPTMethodReponse:
         if messages is not None:
             self.messages = messages
         functions_to_chatgpt = [
             function.append_avaliable_functions(self.AVAILABLE_FUNCTIONS)
             or function.__dict__()
             for function in functions
         ]
@@ -49,11 +58,21 @@
             # Step 3: call the function
             # Note: the JSON response may not always be valid; be sure to handle errors
             # only one function in this example, but you can have multiple
             function_name = response_message["function_call"]["name"]
             function_to_call = self.AVAILABLE_FUNCTIONS[function_name]
             function_args = json.loads(response_message["function_call"]["arguments"])
             function_response = function_to_call(function_args)
+            return ChatGPTMethodReponse(
+                is_function_called=True,
+                function_response=function_response,
+                chatgpt_response_message=response_message,
+            )
         else:
-            print("Функция не вызвана")
-            print(response["choices"][0]["message"])
-            return response["choices"][0]["message"]
+            # print("Функция не вызвана")
+            # print(response["choices"][0]["message"])
+            # return response["choices"][0]["message"]
+            return ChatGPTMethodReponse(
+                is_function_called=False,
+                function_response=None,
+                chatgpt_response_message=response_message,
+            )
```

### Comparing `chatgpt_functions-0.1.2/chatgpt_functions/chatgpt_function.py` & `chatgpt_functions-0.1.3/chatgpt_functions/chatgpt_function.py`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.1.2/chatgpt_functions/function_parameters.py` & `chatgpt_functions-0.1.3/chatgpt_functions/function_parameters.py`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.1.2/chatgpt_functions.egg-info/PKG-INFO` & `chatgpt_functions-0.1.3/chatgpt_functions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-functions
-Version: 0.1.2
+Version: 0.1.3
 Summary: Wrapper over the gpt3.5 model, capable of calling functions
 Home-page: https://github.com/Wellmare/chatgpt-functions
 Author: Wellmare
 Author-email: ivan.kolipov@gmail.com
 Keywords: chatgpt functions gpt
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatgpt_functions-0.1.2/pyproject.toml` & `chatgpt_functions-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.1.2/setup.py` & `chatgpt_functions-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(
     name="chatgpt_functions",
-    version="0.1.2",
+    version="0.1.3",
     author="Wellmare",
     author_email="ivan.kolipov@gmail.com",
     description="Wrapper over the gpt3.5 model, capable of calling functions",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/Wellmare/chatgpt-functions",
     packages=find_packages(),
```

