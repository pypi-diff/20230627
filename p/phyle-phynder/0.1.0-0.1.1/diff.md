# Comparing `tmp/phyle_phynder-0.1.0.tar.gz` & `tmp/phyle_phynder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phyle_phynder-0.1.0.tar", max compression
+gzip compressed data, was "phyle_phynder-0.1.1.tar", max compression
```

## Comparing `phyle_phynder-0.1.0.tar` & `phyle_phynder-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      250 2023-06-27 02:34:51.553409 phyle_phynder-0.1.0/file_finder/cli.py
--rw-r--r--   0        0        0      306 2023-06-27 02:44:16.945752 phyle_phynder-0.1.0/file_finder/constants.py
--rw-r--r--   0        0        0      387 2023-06-27 01:50:40.341841 phyle_phynder-0.1.0/file_finder/exceptions.py
--rw-r--r--   0        0        0     5096 2023-06-27 02:42:36.049148 phyle_phynder-0.1.0/file_finder/finder.py
--rw-r--r--   0        0        0     3789 2023-06-27 02:30:47.044650 phyle_phynder-0.1.0/file_finder/utils.py
--rw-r--r--   0        0        0      415 2023-06-27 03:01:29.559126 phyle_phynder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 02:28:51.459120 phyle_phynder-0.1.0/README.md
--rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 phyle_phynder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      250 2023-06-27 02:34:51.553409 phyle_phynder-0.1.1/file_finder/cli.py
+-rw-r--r--   0        0        0      306 2023-06-27 02:44:16.945752 phyle_phynder-0.1.1/file_finder/constants.py
+-rw-r--r--   0        0        0      387 2023-06-27 01:50:40.341841 phyle_phynder-0.1.1/file_finder/exceptions.py
+-rw-r--r--   0        0        0     5096 2023-06-27 02:42:36.049148 phyle_phynder-0.1.1/file_finder/finder.py
+-rw-r--r--   0        0        0     3955 2023-06-27 03:20:27.118737 phyle_phynder-0.1.1/file_finder/utils.py
+-rw-r--r--   0        0        0      415 2023-06-27 03:20:47.933913 phyle_phynder-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-06-27 03:22:33.013330 phyle_phynder-0.1.1/README.md
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 phyle_phynder-0.1.1/PKG-INFO
```

### Comparing `phyle_phynder-0.1.0/file_finder/finder.py` & `phyle_phynder-0.1.1/file_finder/finder.py`

 * *Files identical despite different names*

### Comparing `phyle_phynder-0.1.0/file_finder/utils.py` & `phyle_phynder-0.1.1/file_finder/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime
 from file_finder.exceptions import InvalidInputError
+import platform
 
 
 def get_folders(path):
     """
     Obtém todos os subdiretorios no diretório pesquisado.
     :param path: um objeto Path() que representa o diretório
     :return: uma lista de objetos Path() em que cada elemento
@@ -81,15 +82,21 @@
     """
     files_details = []
 
     for file in files:
         stat = file.stat()
         details = [
             file.name,
-            timestamp_to_string(stat.st_ctime),
+            timestamp_to_string(get_created_timestamp(stat)),
             timestamp_to_string(stat.st_mtime),
             file.absolute()
         ]
 
         files_details.append(details)
 
     return files_details
+
+def get_created_timestamp(stat):
+    if platform.system() == "Darwin":
+        return stat.st_birthtime
+
+    return stat.st_ctime
```

