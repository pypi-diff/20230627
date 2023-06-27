# Comparing `tmp/nonebot_adapter_villa-0.3.0.tar.gz` & `tmp/nonebot_adapter_villa-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.3.0.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.4.0.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.3.0.tar` & `nonebot_adapter_villa-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1062 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/LICENSE
--rw-r--r--   0        0        0     5070 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/README.md
--rw-r--r--   0        0        0      235 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0     4633 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     2905 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     3714 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    12434 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     8899 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    12220 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      263 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    11641 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     6704 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0       76 2023-06-26 13:03:15.075871 nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-06-26 13:03:15.079872 nonebot_adapter_villa-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-27 13:36:27.694732 nonebot_adapter_villa-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5070 2023-06-27 13:36:27.694732 nonebot_adapter_villa-0.4.0/README.md
+-rw-r--r--   0        0        0      235 2023-06-27 13:36:27.694732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    10684 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0     2905 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/cilent.pyi
+-rw-r--r--   0        0        0     3714 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0    12434 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     8899 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    12220 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      359 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    11641 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     6704 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0       76 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-06-27 13:36:27.698732 nonebot_adapter_villa-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.4.0/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.3.0/LICENSE` & `nonebot_adapter_villa-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/README.md` & `nonebot_adapter_villa-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/cilent.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/client.py` & `nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.4.0/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.3.0/pyproject.toml` & `nonebot_adapter_villa-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.3.0"
+version = "0.4.0"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.3.0/PKG-INFO` & `nonebot_adapter_villa-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.3.0
+Version: 0.4.0
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.4.0 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

