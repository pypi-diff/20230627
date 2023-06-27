# Comparing `tmp/arthub_login_widgets-0.3.2.tar.gz` & `tmp/arthub_login_widgets-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_login_widgets-0.3.2.tar", last modified: Mon Mar 27 11:24:25 2023, max compression
+gzip compressed data, was "arthub_login_widgets-0.3.3.tar", last modified: Tue Jun 27 13:54:03 2023, max compression
```

## Comparing `arthub_login_widgets-0.3.2.tar` & `arthub_login_widgets-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 11:24:25.947116 arthub_login_widgets-0.3.2/
--rw-rw-rw-   0        0        0      375 2023-03-27 11:24:25.947116 arthub_login_widgets-0.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-27 11:24:25.873274 arthub_login_widgets-0.3.2/arthub_login_widgets/
--rw-rw-rw-   0        0        0      435 2023-03-23 06:34:09.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/__init__.py
--rw-rw-rw-   0        0        0       23 2023-03-27 11:24:19.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/__version__.py
--rw-rw-rw-   0        0        0      502 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/constants.py
--rw-rw-rw-   0        0        0     7756 2023-03-23 06:37:43.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/core.py
--rw-rw-rw-   0        0        0     1182 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/filesystem.py
-drwxrwxrwx   0        0        0        0 2023-03-27 11:24:25.877262 arthub_login_widgets-0.3.2/arthub_login_widgets/resources/
--rw-rw-rw-   0        0        0        0 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/resources/__init__.py
--rw-rw-rw-   0        0        0    12338 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/resources/arthub_white.png
--rw-rw-rw-   0        0        0      721 2023-03-23 03:49:40.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/resources/style.qss
-drwxrwxrwx   0        0        0        0 2023-03-27 11:24:25.883247 arthub_login_widgets-0.3.2/arthub_login_widgets/test/
--rw-rw-rw-   0        0        0      173 2023-01-31 11:18:49.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/test/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/test/test_core.py
--rw-rw-rw-   0        0        0      766 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/test/test_filesystem.py
--rw-rw-rw-   0        0        0      699 2023-02-07 12:54:18.000000 arthub_login_widgets-0.3.2/arthub_login_widgets/test/test_imports.py
-drwxrwxrwx   0        0        0        0 2023-03-27 11:24:25.941135 arthub_login_widgets-0.3.2/arthub_login_widgets.egg-info/
--rw-rw-rw-   0        0        0      375 2023-03-27 11:24:25.000000 arthub_login_widgets-0.3.2/arthub_login_widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1177 2023-03-27 11:24:25.000000 arthub_login_widgets-0.3.2/arthub_login_widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 11:24:25.000000 arthub_login_widgets-0.3.2/arthub_login_widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-03-27 11:24:25.000000 arthub_login_widgets-0.3.2/arthub_login_widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-03-27 11:24:25.000000 arthub_login_widgets-0.3.2/arthub_login_widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 11:24:25.948075 arthub_login_widgets-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1217 2023-03-27 11:20:09.000000 arthub_login_widgets-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:54:03.065169 arthub_login_widgets-0.3.3/
+-rw-rw-rw-   0        0        0      375 2023-06-27 13:54:03.065169 arthub_login_widgets-0.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 13:54:03.023552 arthub_login_widgets-0.3.3/arthub_login_widgets/
+-rw-rw-rw-   0        0        0      435 2023-03-23 06:34:09.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-27 13:45:55.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/__version__.py
+-rw-rw-rw-   0        0        0      502 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/constants.py
+-rw-rw-rw-   0        0        0     7756 2023-03-23 06:37:43.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/core.py
+-rw-rw-rw-   0        0        0     1182 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/filesystem.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:54:03.047218 arthub_login_widgets-0.3.3/arthub_login_widgets/resources/
+-rw-rw-rw-   0        0        0        0 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/resources/__init__.py
+-rw-rw-rw-   0        0        0    12338 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/resources/arthub_white.png
+-rw-rw-rw-   0        0        0      721 2023-03-23 03:49:40.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/resources/style.qss
+drwxrwxrwx   0        0        0        0 2023-06-27 13:54:03.054201 arthub_login_widgets-0.3.3/arthub_login_widgets/test/
+-rw-rw-rw-   0        0        0      173 2023-01-31 11:18:49.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/test/__init__.py
+-rw-rw-rw-   0        0        0     1628 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_core.py
+-rw-rw-rw-   0        0        0      766 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_filesystem.py
+-rw-rw-rw-   0        0        0      699 2023-02-07 12:54:18.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_imports.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:54:03.063176 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/
+-rw-rw-rw-   0        0        0      375 2023-06-27 13:54:02.000000 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-06-27 13:54:02.000000 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:54:02.000000 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-27 13:54:02.000000 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 13:54:02.000000 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 13:54:03.066168 arthub_login_widgets-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-06-27 13:46:39.000000 arthub_login_widgets-0.3.3/setup.py
```

### Comparing `arthub_login_widgets-0.3.2/arthub_login_widgets/core.py` & `arthub_login_widgets-0.3.3/arthub_login_widgets/core.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.2/arthub_login_widgets/filesystem.py` & `arthub_login_widgets-0.3.3/arthub_login_widgets/filesystem.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.2/arthub_login_widgets/resources/arthub_white.png` & `arthub_login_widgets-0.3.3/arthub_login_widgets/resources/arthub_white.png`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.2/arthub_login_widgets/resources/style.qss` & `arthub_login_widgets-0.3.3/arthub_login_widgets/resources/style.qss`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.2/arthub_login_widgets/test/test_core.py` & `arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_core.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.2/arthub_login_widgets/test/test_filesystem.py` & `arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.2/arthub_login_widgets/test/test_imports.py` & `arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.2/arthub_login_widgets.egg-info/SOURCES.txt` & `arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,12 @@
 ./arthub_login_widgets/resources/__init__.py
 ./arthub_login_widgets/resources/arthub_white.png
 ./arthub_login_widgets/resources/style.qss
 ./arthub_login_widgets/test/__init__.py
 ./arthub_login_widgets/test/test_core.py
 ./arthub_login_widgets/test/test_filesystem.py
 ./arthub_login_widgets/test/test_imports.py
-arthub_login_widgets/__init__.py
-arthub_login_widgets/__version__.py
-arthub_login_widgets/constants.py
-arthub_login_widgets/core.py
-arthub_login_widgets/filesystem.py
 arthub_login_widgets.egg-info/PKG-INFO
 arthub_login_widgets.egg-info/SOURCES.txt
 arthub_login_widgets.egg-info/dependency_links.txt
 arthub_login_widgets.egg-info/requires.txt
-arthub_login_widgets.egg-info/top_level.txt
-arthub_login_widgets/resources/__init__.py
-arthub_login_widgets/resources/arthub_white.png
-arthub_login_widgets/resources/style.qss
-arthub_login_widgets/test/__init__.py
-arthub_login_widgets/test/test_core.py
-arthub_login_widgets/test/test_filesystem.py
-arthub_login_widgets/test/test_imports.py
+arthub_login_widgets.egg-info/top_level.txt
```

### Comparing `arthub_login_widgets-0.3.2/setup.py` & `arthub_login_widgets-0.3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,12 +30,12 @@
     package_data={"": ["*.png", "*.qss"]},
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
     install_requires=[
-        "arthub_api>=1.1",
+        "arthub_api==1.4.1",
         "platformdirs==2.0.2",
         "qtpy"
     ]
 )
```

