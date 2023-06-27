# Comparing `tmp/speech_bot_helpers-0.2.3.tar.gz` & `tmp/speech_bot_helpers-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_bot_helpers-0.2.3.tar", max compression
+gzip compressed data, was "speech_bot_helpers-0.2.4.tar", max compression
```

## Comparing `speech_bot_helpers-0.2.3.tar` & `speech_bot_helpers-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956111 speech_bot_helpers-0.2.3/README.md
--rw-r--r--   0        0        0      421 2023-06-25 20:51:49.460386 speech_bot_helpers-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956069 speech_bot_helpers-0.2.3/speech_bot_helpers/__init__.py
--rw-r--r--   0        0        0     2660 2023-06-25 12:12:43.449535 speech_bot_helpers-0.2.3/speech_bot_helpers/clients.py
--rw-r--r--   0        0        0       45 2023-06-25 11:57:14.602410 speech_bot_helpers-0.2.3/speech_bot_helpers/exceptions.py
--rw-r--r--   0        0        0      490 2023-06-25 20:51:11.349830 speech_bot_helpers-0.2.3/speech_bot_helpers/wrappers.py
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 speech_bot_helpers-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956111 speech_bot_helpers-0.2.4/README.md
+-rw-r--r--   0        0        0      421 2023-06-27 15:17:25.532703 speech_bot_helpers-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 11:25:44.956069 speech_bot_helpers-0.2.4/speech_bot_helpers/__init__.py
+-rw-r--r--   0        0        0     2698 2023-06-27 15:11:32.494604 speech_bot_helpers-0.2.4/speech_bot_helpers/clients.py
+-rw-r--r--   0        0        0       45 2023-06-25 11:57:14.602410 speech_bot_helpers-0.2.4/speech_bot_helpers/exceptions.py
+-rw-r--r--   0        0        0      509 2023-06-27 15:11:32.488186 speech_bot_helpers-0.2.4/speech_bot_helpers/wrappers.py
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 speech_bot_helpers-0.2.4/PKG-INFO
```

### Comparing `speech_bot_helpers-0.2.3/speech_bot_helpers/clients.py` & `speech_bot_helpers-0.2.4/speech_bot_helpers/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from contextlib import asynccontextmanager
 from io import BytesIO
 from typing import AsyncGenerator
 
 from aiobotocore.session import AioSession, get_session
-from exceptions import S3ClientException
-from wrappers import catch
+from speech_bot_helpers.exceptions import S3ClientException
+from speech_bot_helpers.wrappers import catch
 
 
 class S3File:
     def __init__(self, file: BytesIO, key: str) -> None:
         self.file = file
         self.key = key
```

