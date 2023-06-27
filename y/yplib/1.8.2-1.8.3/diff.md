# Comparing `tmp/yplib-1.8.2.tar.gz` & `tmp/yplib-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.8.2.tar", last modified: Mon Jun 26 01:33:37 2023, max compression
+gzip compressed data, was "dist\yplib-1.8.3.tar", last modified: Tue Jun 27 01:46:02 2023, max compression
```

## Comparing `yplib-1.8.2.tar` & `yplib-1.8.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 01:33:37.337210 yplib-1.8.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.8.2/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-26 01:33:37.336762 yplib-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.8.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 01:33:37.337546 yplib-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-26 01:33:20.000000 yplib-1.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:33:37.333373 yplib-1.8.2/yplib/
--rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.8.2/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-1.8.2/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.8.2/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-1.8.2/yplib/db.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.8.2/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.8.2/yplib/http_util.py
--rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.8.2/yplib/index.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.8.2/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:33:37.336283 yplib-1.8.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-26 01:33:37.000000 yplib-1.8.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-26 01:33:37.000000 yplib-1.8.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 01:33:37.000000 yplib-1.8.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-26 01:33:37.000000 yplib-1.8.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 01:46:02.520671 yplib-1.8.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.8.3/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-27 01:46:02.520671 yplib-1.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.8.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 01:46:02.520671 yplib-1.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-27 01:45:24.000000 yplib-1.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:46:02.516619 yplib-1.8.3/yplib/
+-rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.8.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-1.8.3/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.8.3/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-1.8.3/yplib/db.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.8.3/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.8.3/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26791 2023-06-27 01:45:16.000000 yplib-1.8.3/yplib/index.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.8.3/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:46:02.520114 yplib-1.8.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-27 01:46:02.000000 yplib-1.8.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-27 01:46:02.000000 yplib-1.8.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 01:46:02.000000 yplib-1.8.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-27 01:46:02.000000 yplib-1.8.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.8.2/LICENSE` & `yplib-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.8.2/setup.py` & `yplib-1.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.8.2",
+  version="1.8.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.8.2/yplib/chart.py` & `yplib-1.8.3/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.2/yplib/chart_html.py` & `yplib-1.8.3/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.2/yplib/db.py` & `yplib-1.8.3/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.2/yplib/file.py` & `yplib-1.8.3/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.2/yplib/http_util.py` & `yplib-1.8.3/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.2/yplib/index.py` & `yplib-1.8.3/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,22 +500,22 @@
         # 判断结束位置
         if end_index is not None and i + 1 >= to_int(end_index):
             continue
         # 判断数量
         if count is not None and c >= to_int(count):
             continue
         # 开始标记位
-        if not start_flag and line.find(start_line) > -1:
+        if start_flag is not None and not start_flag and line.find(start_line) > -1:
             start_flag = True
         # 开始标记位
-        if not end_flag and line.find(end_line) > -1:
+        if end_flag is not None and not end_flag and line.find(end_line) > -1:
             end_flag = True
-        if not start_flag:
+        if start_flag is not None and not start_flag:
             continue
-        elif end_flag:
+        elif end_flag is not None and end_flag:
             continue
         c += 1
         if separator is not None:
             data_list.append(line.split(str(separator)))
         else:
             data_list.append(line)
     if separator_all is not None:
```

