# Comparing `tmp/socketapp-0.1.5.tar.gz` & `tmp/socketapp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketapp-0.1.5.tar", max compression
+gzip compressed data, was "socketapp-0.1.6.tar", max compression
```

## Comparing `socketapp-0.1.5.tar` & `socketapp-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1211 2023-06-19 16:18:04.689263 socketapp-0.1.5/LICENSE
--rw-r--r--   0        0        0       79 2023-06-19 16:18:04.689263 socketapp-0.1.5/README.md
--rw-r--r--   0        0        0      681 2023-06-19 16:18:21.037644 socketapp-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      120 2023-06-19 16:18:04.689263 socketapp-0.1.5/socketapp/__init__.py
--rw-r--r--   0        0        0     2871 2023-06-19 16:18:04.689263 socketapp-0.1.5/socketapp/client.py
--rw-r--r--   0        0        0     1141 2023-06-19 16:18:04.689263 socketapp-0.1.5/socketapp/event.py
--rw-r--r--   0        0        0     3705 2023-06-19 16:18:04.689263 socketapp-0.1.5/socketapp/server.py
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 socketapp-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-06-27 19:42:43.098113 socketapp-0.1.6/LICENSE
+-rw-r--r--   0        0        0       79 2023-06-27 19:42:43.098113 socketapp-0.1.6/README.md
+-rw-r--r--   0        0        0      691 2023-06-27 19:42:58.638208 socketapp-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-06-27 19:42:43.098113 socketapp-0.1.6/socketapp/__init__.py
+-rw-r--r--   0        0        0     2871 2023-06-27 19:42:43.098113 socketapp-0.1.6/socketapp/client.py
+-rw-r--r--   0        0        0     1135 2023-06-27 19:42:43.098113 socketapp-0.1.6/socketapp/event.py
+-rw-r--r--   0        0        0     3705 2023-06-27 19:42:43.098113 socketapp-0.1.6/socketapp/server.py
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 socketapp-0.1.6/PKG-INFO
```

### Comparing `socketapp-0.1.5/LICENSE` & `socketapp-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `socketapp-0.1.5/socketapp/client.py` & `socketapp-0.1.6/socketapp/client.py`

 * *Files identical despite different names*

### Comparing `socketapp-0.1.5/socketapp/event.py` & `socketapp-0.1.6/socketapp/event.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,8 +37,8 @@
     def to_json(self) -> str:
         return json.dumps(self.to_dict())
 
     @staticmethod
     def load(data: dict[str, t.Any] | str) -> "Event":
         if isinstance(data, str):
             data = t.cast("dict[str, t.Any]", json.loads(data))
-        return Event.event_map[data.pop("cls_id")](**data)
+        return event_map[data.pop("cls_id")](**data)
```

### Comparing `socketapp-0.1.5/socketapp/server.py` & `socketapp-0.1.6/socketapp/server.py`

 * *Files identical despite different names*

### Comparing `socketapp-0.1.5/PKG-INFO` & `socketapp-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketapp
-Version: 0.1.5
+Version: 0.1.6
 Summary: An opinionated library for creating websocket-based applications.
 License: Unlicense
 Author: CircuitSacul
 Author-email: circuitsacul@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

