# Comparing `tmp/qqwry-linux-python3-0.0.4.tar.gz` & `tmp/qqwry-linux-python3-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qqwry-linux-python3-0.0.4.tar", last modified: Tue Jun 27 07:01:39 2023, max compression
+gzip compressed data, was "dist/qqwry-linux-python3-0.0.5.tar", last modified: Tue Jun 27 07:54:52 2023, max compression
```

## Comparing `qqwry-linux-python3-0.0.4.tar` & `qqwry-linux-python3-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/
--rw-r--r--   0 root         (0) root         (0)    11558 2023-03-22 07:03:34.000000 qqwry-linux-python3-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      561 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-27 04:20:12.000000 qqwry-linux-python3-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/qqwry/
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-27 07:01:37.000000 qqwry-linux-python3-0.0.4/qqwry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/qqwry/shell/
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.4/qqwry/shell/__init__.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.4/qqwry/shell/usage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/qqwry/src/
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-27 07:01:25.000000 qqwry-linux-python3-0.0.4/qqwry/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-06-27 06:07:50.000000 qqwry-linux-python3-0.0.4/qqwry/src/qqwry.py
--rw-r--r--   0 root         (0) root         (0)     7516 2023-06-27 06:19:48.000000 qqwry-linux-python3-0.0.4/qqwry/src/update_qqwry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/qqwry_linux_python3.egg-info/
--rw-r--r--   0 root         (0) root         (0)      561 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/qqwry_linux_python3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/qqwry_linux_python3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/qqwry_linux_python3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/qqwry_linux_python3.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/qqwry_linux_python3.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 06:55:29.000000 qqwry-linux-python3-0.0.4/qqwry_linux_python3.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 06:54:25.000000 qqwry-linux-python3-0.0.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 07:01:39.000000 qqwry-linux-python3-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1958 2023-06-27 06:48:57.000000 qqwry-linux-python3-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11558 2023-03-22 07:03:34.000000 qqwry-linux-python3-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      561 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-27 04:20:12.000000 qqwry-linux-python3-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-27 07:54:28.000000 qqwry-linux-python3-0.0.5/qqwry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry/shell/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.5/qqwry/shell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-27 06:32:42.000000 qqwry-linux-python3-0.0.5/qqwry/shell/usage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry/src/
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-27 07:01:25.000000 qqwry-linux-python3-0.0.5/qqwry/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-27 06:07:50.000000 qqwry-linux-python3-0.0.5/qqwry/src/qqwry.py
+-rw-r--r--   0 root         (0) root         (0)     7643 2023-06-27 07:54:13.000000 qqwry-linux-python3-0.0.5/qqwry/src/update_qqwry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      561 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 06:54:25.000000 qqwry-linux-python3-0.0.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 07:54:52.000000 qqwry-linux-python3-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-27 06:48:57.000000 qqwry-linux-python3-0.0.5/setup.py
```

### Comparing `qqwry-linux-python3-0.0.4/LICENSE` & `qqwry-linux-python3-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qqwry-linux-python3-0.0.4/PKG-INFO` & `qqwry-linux-python3-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qqwry-linux-python3
-Version: 0.0.4
+Version: 0.0.5
 Summary: Using and downloading qqwry.dat, for Python 3.6+
 Home-page: https://github.com/lqshome/qqwry-linux-python3
 Author: unclear
 Author-email: qsykgg@gmail.com
 License: MIT License
 Description: # qqwry-linux-python3
         Linux下自动更新qqwry的工具
```

### Comparing `qqwry-linux-python3-0.0.4/qqwry/src/qqwry.py` & `qqwry-linux-python3-0.0.5/qqwry/src/qqwry.py`

 * *Files identical despite different names*

### Comparing `qqwry-linux-python3-0.0.4/qqwry/src/update_qqwry.py` & `qqwry-linux-python3-0.0.5/qqwry/src/update_qqwry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         self.date = None
 
     def handle_starttag(self, tag, attrs):
         # If the tag is li and the class attribute value is album__list-item js_album_item js_wx_tap_highlight wx_tap_cell
         if tag == "li" and ("class", "album__list-item js_album_item js_wx_tap_highlight wx_tap_cell") in attrs:
             # Traverse all attributes, find the data-link attribute, and save its value
             for attr, value in attrs:
-                if attr == "data-link":
+                # If the data-link attribute is found and the download_link has not been found yet
+                if attr == "data-link" and not self.download_link:
                     self.download_link = value
                     break
 
     def handle_data(self, data):
         # If the download_link has been found and the date has not been found yet
         if self.download_link and not self.date:
             # Use regular expressions to match the date format and save the first matching result
```

### Comparing `qqwry-linux-python3-0.0.4/qqwry_linux_python3.egg-info/PKG-INFO` & `qqwry-linux-python3-0.0.5/qqwry_linux_python3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qqwry-linux-python3
-Version: 0.0.4
+Version: 0.0.5
 Summary: Using and downloading qqwry.dat, for Python 3.6+
 Home-page: https://github.com/lqshome/qqwry-linux-python3
 Author: unclear
 Author-email: qsykgg@gmail.com
 License: MIT License
 Description: # qqwry-linux-python3
         Linux下自动更新qqwry的工具
```

### Comparing `qqwry-linux-python3-0.0.4/setup.py` & `qqwry-linux-python3-0.0.5/setup.py`

 * *Files identical despite different names*

