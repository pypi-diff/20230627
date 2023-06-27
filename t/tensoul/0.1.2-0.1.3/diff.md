# Comparing `tmp/tensoul-0.1.2.tar.gz` & `tmp/tensoul-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensoul-0.1.2.tar", max compression
+gzip compressed data, was "tensoul-0.1.3.tar", max compression
```

## Comparing `tensoul-0.1.2.tar` & `tensoul-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      445 2023-05-29 02:06:44.856253 tensoul-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      944 2023-05-25 04:14:31.440763 tensoul-0.1.2/README.md
--rw-r--r--   0        0        0       48 2023-05-24 15:43:55.027885 tensoul-0.1.2/tensoul/__init__.py
--rw-r--r--   0        0        0   168833 2023-05-25 02:49:24.087394 tensoul-0.1.2/tensoul/cfg.json
--rw-r--r--   0        0        0      163 2023-05-24 15:36:34.423992 tensoul-0.1.2/tensoul/cfg.py
--rw-r--r--   0        0        0     2377 2023-05-29 02:03:29.081206 tensoul-0.1.2/tensoul/constants.py
--rw-r--r--   0        0        0     7056 2023-05-25 08:27:21.930832 tensoul-0.1.2/tensoul/downloader.py
--rw-r--r--   0        0        0    10263 2023-05-29 02:05:05.387320 tensoul-0.1.2/tensoul/model.py
--rw-r--r--   0        0        0    14218 2023-05-29 01:57:19.665195 tensoul-0.1.2/tensoul/parser.py
--rw-r--r--   0        0        0      452 2023-05-25 04:10:00.171590 tensoul-0.1.2/tensoul/utils.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 tensoul-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      445 2023-06-27 02:49:07.715727 tensoul-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      944 2023-05-25 04:14:31.440763 tensoul-0.1.3/README.md
+-rw-r--r--   0        0        0       48 2023-05-24 15:43:55.027885 tensoul-0.1.3/tensoul/__init__.py
+-rw-r--r--   0        0        0   168833 2023-05-25 02:49:24.087394 tensoul-0.1.3/tensoul/cfg.json
+-rw-r--r--   0        0        0      163 2023-05-24 15:36:34.423992 tensoul-0.1.3/tensoul/cfg.py
+-rw-r--r--   0        0        0     2377 2023-05-29 02:03:29.081206 tensoul-0.1.3/tensoul/constants.py
+-rw-r--r--   0        0        0     7056 2023-05-25 08:27:21.930832 tensoul-0.1.3/tensoul/downloader.py
+-rw-r--r--   0        0        0    10263 2023-06-27 02:49:01.395547 tensoul-0.1.3/tensoul/model.py
+-rw-r--r--   0        0        0    14218 2023-05-29 01:57:19.665195 tensoul-0.1.3/tensoul/parser.py
+-rw-r--r--   0        0        0      452 2023-05-25 04:10:00.171590 tensoul-0.1.3/tensoul/utils.py
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 tensoul-0.1.3/PKG-INFO
```

### Comparing `tensoul-0.1.2/README.md` & `tensoul-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.2/tensoul/cfg.json` & `tensoul-0.1.3/tensoul/cfg.json`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.2/tensoul/constants.py` & `tensoul-0.1.3/tensoul/constants.py`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.2/tensoul/downloader.py` & `tensoul-0.1.3/tensoul/downloader.py`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.2/tensoul/model.py` & `tensoul-0.1.3/tensoul/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
 class AnkanSymbol(NamedTuple):
     tile: Tile
 
     def encode_tenhou(self) -> str:
         t = self.tile.encode_tenhou()
         if self.tile.num == 5 and self.tile.type != TileType.Z:
-            return f"{t}{t}{t}a{Tile(5, self.tile.type).encode_tenhou()}"
+            return f"{Tile(0, self.tile.type).encode_tenhou()}{t}{t}a{t}"
         else:
             return f"{t}{t}{t}a{t}"
 
 
 class PeSymbol:
     # NOTE: tenhou doesn't mark its kita based on when they were drawn
     def encode_tenhou(self) -> str:
```

### Comparing `tensoul-0.1.2/tensoul/parser.py` & `tensoul-0.1.3/tensoul/parser.py`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.2/PKG-INFO` & `tensoul-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensoul
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

