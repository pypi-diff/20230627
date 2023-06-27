# Comparing `tmp/xiaogpt-1.46.tar.gz` & `tmp/xiaogpt-1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-1.46.tar", last modified: Wed Jun 14 02:11:02 2023, max compression
+gzip compressed data, was "xiaogpt-1.50.tar", last modified: Tue Jun 27 13:12:47 2023, max compression
```

## Comparing `xiaogpt-1.46.tar` & `xiaogpt-1.50.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-06-14 02:10:51.461803 xiaogpt-1.46/LICENSE
--rw-r--r--   0        0        0    11480 2023-06-14 02:10:51.461803 xiaogpt-1.46/README.md
--rw-r--r--   0        0        0      919 2023-06-14 02:11:02.441948 xiaogpt-1.46/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/__main__.py
--rw-r--r--   0        0        0      639 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      554 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3280 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1605 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1996 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3415 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/cli.py
--rw-r--r--   0        0        0     5318 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/config.py
--rw-r--r--   0        0        0     2071 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/utils.py
--rw-r--r--   0        0        0    18548 2023-06-14 02:10:51.461803 xiaogpt-1.46/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    12066 1970-01-01 00:00:00.000000 xiaogpt-1.46/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-27 13:12:34.775396 xiaogpt-1.50/LICENSE
+-rw-r--r--   0        0        0    11480 2023-06-27 13:12:34.775396 xiaogpt-1.50/README.md
+-rw-r--r--   0        0        0      919 2023-06-27 13:12:47.207531 xiaogpt-1.50/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      639 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      554 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3280 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1605 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1996 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3415 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/cli.py
+-rw-r--r--   0        0        0     5318 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/config.py
+-rw-r--r--   0        0        0     2071 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/utils.py
+-rw-r--r--   0        0        0    18548 2023-06-27 13:12:34.779396 xiaogpt-1.50/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    12066 1970-01-01 00:00:00.000000 xiaogpt-1.50/PKG-INFO
```

### Comparing `xiaogpt-1.46/LICENSE` & `xiaogpt-1.50/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/README.md` & `xiaogpt-1.50/README.md`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/xiaogpt/bot/__init__.py` & `xiaogpt-1.50/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/xiaogpt/bot/base_bot.py` & `xiaogpt-1.50/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-1.50/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-1.50/xiaogpt/bot/gpt3_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/xiaogpt/bot/newbing_bot.py` & `xiaogpt-1.50/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/xiaogpt/cli.py` & `xiaogpt-1.50/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/xiaogpt/config.py` & `xiaogpt-1.50/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/xiaogpt/utils.py` & `xiaogpt-1.50/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/xiaogpt/xiaogpt.py` & `xiaogpt-1.50/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.46/PKG-INFO` & `xiaogpt-1.50/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 1.46
+Version: 1.50
 Summary: Play ChatGPT with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
```

