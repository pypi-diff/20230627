# Comparing `tmp/twilio_python_async-0.2.1.tar.gz` & `tmp/twilio_python_async-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilio_python_async-0.2.1.tar", max compression
+gzip compressed data, was "twilio_python_async-0.2.2.tar", max compression
```

## Comparing `twilio_python_async-0.2.1.tar` & `twilio_python_async-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-05 17:00:25.217553 twilio_python_async-0.2.1/LICENSE
--rw-r--r--   0        0        0     2182 2023-04-05 17:00:25.217553 twilio_python_async-0.2.1/README.md
--rw-r--r--   0        0        0     1889 2023-04-05 17:00:25.221553 twilio_python_async-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       71 2023-04-05 17:00:25.221553 twilio_python_async-0.2.1/twilio_async/__init__.py
--rw-r--r--   0        0        0     5485 2023-04-05 17:00:25.221553 twilio_python_async-0.2.1/twilio_async/client.py
--rw-r--r--   0        0        0        0 2023-04-05 17:00:25.221553 twilio_python_async-0.2.1/twilio_async/models/__init__.py
--rw-r--r--   0        0        0     1719 2023-04-05 17:00:25.221553 twilio_python_async-0.2.1/twilio_async/models/message.py
--rw-r--r--   0        0        0        0 2023-04-05 17:00:25.221553 twilio_python_async-0.2.1/twilio_async/py.typed
--rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 twilio_python_async-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-27 15:15:41.015844 twilio_python_async-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2182 2023-06-27 15:15:41.015844 twilio_python_async-0.2.2/README.md
+-rw-r--r--   0        0        0     1876 2023-06-27 15:15:41.019844 twilio_python_async-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-27 15:15:41.019844 twilio_python_async-0.2.2/twilio_async/__init__.py
+-rw-r--r--   0        0        0     5461 2023-06-27 15:15:41.019844 twilio_python_async-0.2.2/twilio_async/client.py
+-rw-r--r--   0        0        0        0 2023-06-27 15:15:41.019844 twilio_python_async-0.2.2/twilio_async/models/__init__.py
+-rw-r--r--   0        0        0     1719 2023-06-27 15:15:41.019844 twilio_python_async-0.2.2/twilio_async/models/message.py
+-rw-r--r--   0        0        0        0 2023-06-27 15:15:41.019844 twilio_python_async-0.2.2/twilio_async/py.typed
+-rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 twilio_python_async-0.2.2/PKG-INFO
```

### Comparing `twilio_python_async-0.2.1/LICENSE` & `twilio_python_async-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twilio_python_async-0.2.1/README.md` & `twilio_python_async-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `twilio_python_async-0.2.1/pyproject.toml` & `twilio_python_async-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [tool.poetry]
 name = "twilio-python-async"
-version = "0.2.1"
+version = "0.2.2"
 description = "An asynchronous Twilio client"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/twilio-python-async"
 homepage = "https://github.com/sanders41/twilio-python-async"
 documentation = "https://github.com/sanders41/twilio-python-async"
 keywords = ["twilio", "async", "python", "sms", "messaging"]
 classifiers=[
   "Intended Audience :: Developers",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Typing :: Typed",
 ]
 packages = [
   { include = "twilio_async" },
 ]
 include = ["twilio_async/py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 httpx = ">=0.23.3"
 pydantic = ">=1.10.4"
 
 [tool.poetry.group.dev.dependencies]
 mypy = ">=1.1.1"
 pre-commit = ">=2.20.0"
 pytest = ">=7.2.0"
@@ -75,11 +74,12 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov=twilio_async --cov-report term-missing"
 asyncio_mode = "auto"
 
 [tool.ruff]
-select = ["E", "F", "T201", "T203", "I001"]
+select = ["E", "F", "UP", "I001", "T201", "T203"]
 ignore = ["E501"]
 line-length = 100
+target-version = "py38"
 fix = true
```

### Comparing `twilio_python_async-0.2.1/twilio_async/client.py` & `twilio_python_async-0.2.2/twilio_async/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import os
 from types import TracebackType
-from typing import Type
 
 from httpx import AsyncClient as HttpxAsyncClient
 
 from twilio_async.models.message import MessageLogs, MessageResponse, MessageSend
 
 
 class AsyncClient:
@@ -47,16 +46,16 @@
         )
 
     async def __aenter__(self) -> AsyncClient:
         return self
 
     async def __aexit__(
         self,
-        et: Type[BaseException] | None,
-        ev: Type[BaseException] | None,
+        et: type[BaseException] | None,
+        ev: type[BaseException] | None,
         traceback: TracebackType | None,
     ) -> None:
         await self.aclose()
 
     async def aclose(self) -> None:
         """Closes the client.
```

### Comparing `twilio_python_async-0.2.1/twilio_async/models/message.py` & `twilio_python_async-0.2.2/twilio_async/models/message.py`

 * *Files identical despite different names*

### Comparing `twilio_python_async-0.2.1/PKG-INFO` & `twilio_python_async-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 Metadata-Version: 2.1
 Name: twilio-python-async
-Version: 0.2.1
+Version: 0.2.2
 Summary: An asynchronous Twilio client
 Home-page: https://github.com/sanders41/twilio-python-async
 License: MIT
 Keywords: twilio,async,python,sms,messaging
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: httpx (>=0.23.3)
 Requires-Dist: pydantic (>=1.10.4)
 Project-URL: Documentation, https://github.com/sanders41/twilio-python-async
 Project-URL: Repository, https://github.com/sanders41/twilio-python-async
 Description-Content-Type: text/markdown
```

