# Comparing `tmp/alpaca-trade-api-3.0.0.tar.gz` & `tmp/alpaca-trade-api-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca-trade-api-3.0.0.tar", last modified: Sun Mar  5 01:21:50 2023, max compression
+gzip compressed data, was "alpaca-trade-api-3.0.2.tar", last modified: Tue Jun 27 13:28:54 2023, max compression
```

## Comparing `alpaca-trade-api-3.0.0.tar` & `alpaca-trade-api-3.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-05 01:21:50.858131 alpaca-trade-api-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      176 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (116)    28758 2023-03-05 01:21:50.858131 alpaca-trade-api-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    28428 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-05 01:21:50.858131 alpaca-trade-api-3.0.0/alpaca_trade_api/
--rw-r--r--   0 runner    (1001) docker     (116)      157 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/alpaca_trade_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      575 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/alpaca_trade_api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3229 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/alpaca_trade_api/common.py
--rw-r--r--   0 runner    (1001) docker     (116)     6750 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/alpaca_trade_api/entity.py
--rw-r--r--   0 runner    (1001) docker     (116)     6597 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/alpaca_trade_api/entity_v2.py
--rw-r--r--   0 runner    (1001) docker     (116)    43120 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/alpaca_trade_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (116)     6069 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/alpaca_trade_api/rest_async.py
--rw-r--r--   0 runner    (1001) docker     (116)    36449 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/alpaca_trade_api/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-05 01:21:50.858131 alpaca-trade-api-3.0.0/alpaca_trade_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    28758 2023-03-05 01:21:50.000000 alpaca-trade-api-3.0.0/alpaca_trade_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      486 2023-03-05 01:21:50.000000 alpaca-trade-api-3.0.0/alpaca_trade_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-05 01:21:50.000000 alpaca-trade-api-3.0.0/alpaca_trade_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      168 2023-03-05 01:21:50.000000 alpaca-trade-api-3.0.0/alpaca_trade_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2023-03-05 01:21:50.000000 alpaca-trade-api-3.0.0/alpaca_trade_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      198 2023-03-05 01:21:50.862130 alpaca-trade-api-3.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     1110 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-05 01:21:50.858131 alpaca-trade-api-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)    37333 2023-03-05 01:21:38.000000 alpaca-trade-api-3.0.0/tests/test_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:28:54.645141 alpaca-trade-api-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    28758 2023-06-27 13:28:54.645141 alpaca-trade-api-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28428 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:28:54.645141 alpaca-trade-api-3.0.2/alpaca_trade_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/alpaca_trade_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/alpaca_trade_api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/alpaca_trade_api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/alpaca_trade_api/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/alpaca_trade_api/entity_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43120 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/alpaca_trade_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/alpaca_trade_api/rest_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36940 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/alpaca_trade_api/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:28:54.645141 alpaca-trade-api-3.0.2/alpaca_trade_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28758 2023-06-27 13:28:54.000000 alpaca-trade-api-3.0.2/alpaca_trade_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-27 13:28:54.000000 alpaca-trade-api-3.0.2/alpaca_trade_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:28:54.000000 alpaca-trade-api-3.0.2/alpaca_trade_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-27 13:28:54.000000 alpaca-trade-api-3.0.2/alpaca_trade_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 13:28:54.000000 alpaca-trade-api-3.0.2/alpaca_trade_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-27 13:28:54.645141 alpaca-trade-api-3.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1110 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:28:54.645141 alpaca-trade-api-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    37333 2023-06-27 13:28:42.000000 alpaca-trade-api-3.0.2/tests/test_rest.py
```

### Comparing `alpaca-trade-api-3.0.0/LICENSE` & `alpaca-trade-api-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca-trade-api-3.0.0/PKG-INFO` & `alpaca-trade-api-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-trade-api
-Version: 3.0.0
+Version: 3.0.2
 Summary: Alpaca API python client
 Home-page: https://github.com/alpacahq/alpaca-trade-api-python
 Author: Alpaca
 Author-email: oss@alpaca.markets
 Keywords: financial,timeseries,api,trade
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `alpaca-trade-api-3.0.0/README.md` & `alpaca-trade-api-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alpaca-trade-api-3.0.0/alpaca_trade_api/__main__.py` & `alpaca-trade-api-3.0.2/alpaca_trade_api/__main__.py`

 * *Files identical despite different names*

### Comparing `alpaca-trade-api-3.0.0/alpaca_trade_api/common.py` & `alpaca-trade-api-3.0.2/alpaca_trade_api/common.py`

 * *Files identical despite different names*

### Comparing `alpaca-trade-api-3.0.0/alpaca_trade_api/entity.py` & `alpaca-trade-api-3.0.2/alpaca_trade_api/entity.py`

 * *Files identical despite different names*

### Comparing `alpaca-trade-api-3.0.0/alpaca_trade_api/entity_v2.py` & `alpaca-trade-api-3.0.2/alpaca_trade_api/entity_v2.py`

 * *Files identical despite different names*

### Comparing `alpaca-trade-api-3.0.0/alpaca_trade_api/rest.py` & `alpaca-trade-api-3.0.2/alpaca_trade_api/rest.py`

 * *Files identical despite different names*

### Comparing `alpaca-trade-api-3.0.0/alpaca_trade_api/rest_async.py` & `alpaca-trade-api-3.0.2/alpaca_trade_api/rest_async.py`

 * *Files identical despite different names*

### Comparing `alpaca-trade-api-3.0.0/alpaca_trade_api/stream.py` & `alpaca-trade-api-3.0.2/alpaca_trade_api/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,19 +561,30 @@
         if not self._raw_data:
             if msg_type == 'n':
                 result = NewsV2(msg)
         return result
 
     async def _dispatch(self, msg):
         msg_type = msg.get('T')
-        symbol = msg.get('S')
         if msg_type == 'n':
-            handler = self._handlers['news'].get(
-                symbol, self._handlers['news'].get('*', None))
-            if handler:
+            symbols = msg.get('symbols', [])
+            # A news article could be unrelated to any symbols,
+            # resulting in an empty symbols list. Those news articles
+            # should still be dispatched to the wildcard event handler.
+            if not symbols:
+                symbols.append('*')
+
+            handlers = set()
+            for symbol in symbols:
+                handler = self._handlers['news'].get(symbol)
+                if handler is None:
+                    handler = self._handlers['news'].get('*')
+                if handler is not None:
+                    handlers.add(handler)
+            for handler in handlers:
                 await handler(self._cast(msg_type, msg))
         else:
             await super()._dispatch(msg)
 
     async def _unsubscribe(self, news=()):
         if news:
             await self._ws.send(
```

### Comparing `alpaca-trade-api-3.0.0/alpaca_trade_api.egg-info/PKG-INFO` & `alpaca-trade-api-3.0.2/alpaca_trade_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-trade-api
-Version: 3.0.0
+Version: 3.0.2
 Summary: Alpaca API python client
 Home-page: https://github.com/alpacahq/alpaca-trade-api-python
 Author: Alpaca
 Author-email: oss@alpaca.markets
 Keywords: financial,timeseries,api,trade
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `alpaca-trade-api-3.0.0/setup.py` & `alpaca-trade-api-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca-trade-api-3.0.0/tests/test_rest.py` & `alpaca-trade-api-3.0.2/tests/test_rest.py`

 * *Files identical despite different names*

