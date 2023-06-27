# Comparing `tmp/msmanager-0.2.2.dev2.tar.gz` & `tmp/msmanager-0.2.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.2.2.dev2.tar", max compression
+gzip compressed data, was "msmanager-0.2.2.dev3.tar", max compression
```

## Comparing `msmanager-0.2.2.dev2.tar` & `msmanager-0.2.2.dev3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.2.dev2/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.2.dev2/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.2.dev2/msmanager/__main__.py
--rw-r--r--   0        0        0     7494 2023-06-27 12:06:21.095814 msmanager-0.2.2.dev2/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.2.dev2/msmanager/config.py
--rw-r--r--   0        0        0     3231 2023-06-26 19:57:01.709315 msmanager-0.2.2.dev2/msmanager/exceptions.py
--rw-r--r--   0        0        0     4001 2023-06-26 20:02:25.396576 msmanager-0.2.2.dev2/msmanager/functions.py
--rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.2.dev2/msmanager/models.py
--rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.2.dev2/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.2.dev2/msmanager/types.py
--rw-r--r--   0        0        0      591 2023-06-27 12:07:16.435517 msmanager-0.2.2.dev2/msmanager/units.py
--rw-r--r--   0        0        0      552 2023-06-27 12:07:11.616511 msmanager-0.2.2.dev2/pyproject.toml
--rw-r--r--   0        0        0      704 2023-06-21 22:49:16.590585 msmanager-0.2.2.dev2/README.md
--rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 msmanager-0.2.2.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.2.dev3/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.2.dev3/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.2.dev3/msmanager/__main__.py
+-rw-r--r--   0        0        0     7494 2023-06-27 12:06:21.095814 msmanager-0.2.2.dev3/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.2.dev3/msmanager/config.py
+-rw-r--r--   0        0        0     3231 2023-06-26 19:57:01.709315 msmanager-0.2.2.dev3/msmanager/exceptions.py
+-rw-r--r--   0        0        0     3995 2023-06-27 12:16:45.380300 msmanager-0.2.2.dev3/msmanager/functions.py
+-rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.2.dev3/msmanager/models.py
+-rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.2.dev3/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.2.dev3/msmanager/types.py
+-rw-r--r--   0        0        0      591 2023-06-27 12:07:16.435517 msmanager-0.2.2.dev3/msmanager/units.py
+-rw-r--r--   0        0        0      552 2023-06-27 12:18:59.313591 msmanager-0.2.2.dev3/pyproject.toml
+-rw-r--r--   0        0        0      704 2023-06-21 22:49:16.590585 msmanager-0.2.2.dev3/README.md
+-rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 msmanager-0.2.2.dev3/PKG-INFO
```

### Comparing `msmanager-0.2.2.dev2/LICENSE` & `msmanager-0.2.2.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev2/msmanager/cli.py` & `msmanager-0.2.2.dev3/msmanager/cli.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev2/msmanager/config.py` & `msmanager-0.2.2.dev3/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev2/msmanager/exceptions.py` & `msmanager-0.2.2.dev3/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev2/msmanager/functions.py` & `msmanager-0.2.2.dev3/msmanager/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 # ! Subproccess Functions
 def runner(*args: str) -> Tuple[int, str]:
     return getstatusoutput(" ".join([*args]))
 
 def exists_screen() -> bool:
     out = runner("screen", "-v")[0]
-    return (out[0] == 0) or (out[0] == 1)
+    return (out == 0) or (out == 1)
 
 def exists_java() -> bool:
     return runner("java", "--version")[0] == 0
 
 # ! Parse Functions
 def remove_color(text: str) -> str:
     return replaces(text, COLORS_STRINGS_REPLACEBLE)
```

### Comparing `msmanager-0.2.2.dev2/msmanager/msm.py` & `msmanager-0.2.2.dev3/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev2/msmanager/units.py` & `msmanager-0.2.2.dev3/msmanager/units.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev2/pyproject.toml` & `msmanager-0.2.2.dev3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.2.2.dev2"
+version = "0.2.2.dev3"
 description = "Manager for managing Mindustry servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 
 [tool.poetry.dependencies]
```

### Comparing `msmanager-0.2.2.dev2/README.md` & `msmanager-0.2.2.dev3/README.md`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev2/PKG-INFO` & `msmanager-0.2.2.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.2.2.dev2
+Version: 0.2.2.dev3
 Summary: Manager for managing Mindustry servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

