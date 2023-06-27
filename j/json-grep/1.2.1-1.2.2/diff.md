# Comparing `tmp/json-grep-1.2.1.tar.gz` & `tmp/json-grep-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-grep-1.2.1.tar", last modified: Tue Jun 27 07:20:26 2023, max compression
+gzip compressed data, was "json-grep-1.2.2.tar", last modified: Tue Jun 27 08:53:04 2023, max compression
```

## Comparing `json-grep-1.2.1.tar` & `json-grep-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 07:20:26.620216 json-grep-1.2.1/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       24 2021-03-10 21:40:32.000000 json-grep-1.2.1/MANIFEST.in
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1793 2023-06-27 07:20:26.620216 json-grep-1.2.1/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1372 2023-05-15 09:17:46.000000 json-grep-1.2.1/README.md
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 07:20:26.620216 json-grep-1.2.1/json_grep.egg-info/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1793 2023-06-27 07:20:26.000000 json-grep-1.2.1/json_grep.egg-info/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      396 2023-06-27 07:20:26.000000 json-grep-1.2.1/json_grep.egg-info/SOURCES.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-06-27 07:20:26.000000 json-grep-1.2.1/json_grep.egg-info/dependency_links.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      106 2023-06-27 07:20:26.000000 json-grep-1.2.1/json_grep.egg-info/entry_points.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-05-15 09:12:34.000000 json-grep-1.2.1/json_grep.egg-info/not-zip-safe
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        9 2023-06-27 07:20:26.000000 json-grep-1.2.1/json_grep.egg-info/top_level.txt
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 07:20:26.620216 json-grep-1.2.1/jsongrep/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        5 2023-06-27 07:20:06.000000 json-grep-1.2.1/jsongrep/VERSION
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 18:47:36.000000 json-grep-1.2.1/jsongrep/__init__.py
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 07:20:26.620216 json-grep-1.2.1/jsongrep/libs/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 21:48:52.000000 json-grep-1.2.1/jsongrep/libs/__init__.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      766 2023-06-27 07:16:08.000000 json-grep-1.2.1/jsongrep/libs/cli_colors.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     3420 2023-06-27 07:12:39.000000 json-grep-1.2.1/jsongrep/libs/json_filter.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      333 2021-08-06 07:59:08.000000 json-grep-1.2.1/jsongrep/libs/setuptools.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     2364 2023-06-27 07:00:36.000000 json-grep-1.2.1/jsongrep/main.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-06-27 07:20:26.620216 json-grep-1.2.1/setup.cfg
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1142 2021-03-10 21:46:39.000000 json-grep-1.2.1/setup.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 08:53:04.698366 json-grep-1.2.2/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       24 2021-03-10 21:40:32.000000 json-grep-1.2.2/MANIFEST.in
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1793 2023-06-27 08:53:04.698366 json-grep-1.2.2/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1372 2023-05-15 09:17:46.000000 json-grep-1.2.2/README.md
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 08:53:04.698366 json-grep-1.2.2/json_grep.egg-info/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1793 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      396 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/SOURCES.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/dependency_links.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      106 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/entry_points.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/not-zip-safe
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        9 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/top_level.txt
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 08:53:04.698366 json-grep-1.2.2/jsongrep/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        5 2023-06-27 08:52:37.000000 json-grep-1.2.2/jsongrep/VERSION
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 18:47:36.000000 json-grep-1.2.2/jsongrep/__init__.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 08:53:04.698366 json-grep-1.2.2/jsongrep/libs/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 21:48:52.000000 json-grep-1.2.2/jsongrep/libs/__init__.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      766 2023-06-27 07:16:08.000000 json-grep-1.2.2/jsongrep/libs/cli_colors.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     3350 2023-06-27 08:49:11.000000 json-grep-1.2.2/jsongrep/libs/json_filter.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      333 2021-08-06 07:59:08.000000 json-grep-1.2.2/jsongrep/libs/setuptools.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     2364 2023-06-27 07:00:36.000000 json-grep-1.2.2/jsongrep/main.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-06-27 08:53:04.698366 json-grep-1.2.2/setup.cfg
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1142 2021-03-10 21:46:39.000000 json-grep-1.2.2/setup.py
```

### Comparing `json-grep-1.2.1/PKG-INFO` & `json-grep-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-grep
-Version: 1.2.1
+Version: 1.2.2
 Summary: Filtering JSON dict keys from STDOUT
 Home-page: https://gitlab.com/alda78/json-grep
 Author: Ales Adamek
 Author-email: alda78@seznam.cz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `json-grep-1.2.1/README.md` & `json-grep-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `json-grep-1.2.1/json_grep.egg-info/PKG-INFO` & `json-grep-1.2.2/json_grep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-grep
-Version: 1.2.1
+Version: 1.2.2
 Summary: Filtering JSON dict keys from STDOUT
 Home-page: https://gitlab.com/alda78/json-grep
 Author: Ales Adamek
 Author-email: alda78@seznam.cz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `json-grep-1.2.1/jsongrep/libs/cli_colors.py` & `json-grep-1.2.2/jsongrep/libs/cli_colors.py`

 * *Files identical despite different names*

### Comparing `json-grep-1.2.1/jsongrep/libs/json_filter.py` & `json-grep-1.2.2/jsongrep/libs/json_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,14 @@
                             ret[key] = json_data_flat[key]
                         elif operator == "=" and str(value) == str(json_data_flat[key]):
                             ret[key] = json_data_flat[key]
                             is_value_matched = True
                         elif operator == "~" and str(value) in str(json_data_flat[key]):
                             ret[key] = json_data_flat[key]
                             is_value_matched = True
-                        else:
-                            return None
         except Exception as ex:
             raise JsonFilterException("Error decoding JSON from line: {} caused by: {}".format(line, ex))
         if is_value_operator_used and not is_value_matched:
             return None
         return ret
 
     @classmethod
```

### Comparing `json-grep-1.2.1/jsongrep/main.py` & `json-grep-1.2.2/jsongrep/main.py`

 * *Files identical despite different names*

### Comparing `json-grep-1.2.1/setup.py` & `json-grep-1.2.2/setup.py`

 * *Files identical despite different names*

