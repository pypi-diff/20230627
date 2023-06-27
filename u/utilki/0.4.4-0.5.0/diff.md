# Comparing `tmp/utilki-0.4.4.tar.gz` & `tmp/utilki-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.4.4.tar", max compression
+gzip compressed data, was "utilki-0.5.0.tar", max compression
```

## Comparing `utilki-0.4.4.tar` & `utilki-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-20 13:42:18.372101 utilki-0.4.4/README.md
--rw-r--r--   0        0        0      525 2023-06-20 13:42:18.372101 utilki-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      269 2023-06-20 13:42:18.372101 utilki-0.4.4/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-06-20 13:42:18.372101 utilki-0.4.4/utilki/cli.py
--rw-r--r--   0        0        0     5273 2023-06-20 13:42:18.372101 utilki-0.4.4/utilki/log_utils.py
--rw-r--r--   0        0        0     6698 2023-06-20 13:42:18.372101 utilki-0.4.4/utilki/task_mixin.py
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-27 13:59:08.321137 utilki-0.5.0/README.md
+-rw-r--r--   0        0        0      525 2023-06-27 13:59:08.321137 utilki-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-06-27 13:59:08.321137 utilki-0.5.0/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-06-27 13:59:08.321137 utilki-0.5.0/utilki/cli.py
+-rw-r--r--   0        0        0     5273 2023-06-27 13:59:08.321137 utilki-0.5.0/utilki/log_utils.py
+-rw-r--r--   0        0        0     6939 2023-06-27 13:59:08.321137 utilki-0.5.0/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.5.0/PKG-INFO
```

### Comparing `utilki-0.4.4/README.md` & `utilki-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.4.4/pyproject.toml` & `utilki-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.4.4"
+version = "0.5.0"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.4.4/utilki/cli.py` & `utilki-0.5.0/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.4.4/utilki/log_utils.py` & `utilki-0.5.0/utilki/log_utils.py`

 * *Files identical despite different names*

### Comparing `utilki-0.4.4/utilki/task_mixin.py` & `utilki-0.5.0/utilki/task_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     List[int],
     List[float],
     List[str],
 ]
 
 
 singles = [int, float, str, bool, datetime]
-lists = [List[int], List[float], List[str], List[bool]]
+lists = [List[int], List[float], List[str], List[bool], List[List[str]]]
 options = [
     Union[int, None],
     Union[float, None],
     Union[str, None],
     Union[bool, None],
 ]
 
@@ -165,14 +165,16 @@
         return parse_list(value, int, name_)
     elif type_ == List[str]:
         return parse_list(value, str, name_)
     elif type_ == List[float]:
         return parse_list(value, float, name_)
     elif type_ == List[bool]:
         return parse_list(value, parse_bool, name_)
+    elif type_ == List[List[str]]:
+        return json.loads(value)
     elif type_ == Union[int, None]:
         return parse_options(value, int)
     elif type_ == Union[str, None]:
         return parse_options(value, str)
     elif type_ == Union[float, None]:
         return parse_options(value, float)
     elif type_ == Union[bool, None]:
@@ -213,7 +215,12 @@
             value = value.replace("T", "-")
             value = value.replace(":", "-")
             return get_date(value)
         elif num_parts == 3:
             return get_date(value)
         else:
             raise TypeError("Invalid datetime format")
+    elif type_ in types_we_support:
+        try:
+            return json.loads(value)
+        except Exception:
+            raise TypeError("Invalid type")
```

### Comparing `utilki-0.4.4/PKG-INFO` & `utilki-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.4.4
+Version: 0.5.0
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

