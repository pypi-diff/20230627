# Comparing `tmp/robotframework-applicationlibrary-1.2.0.tar.gz` & `tmp/robotframework-applicationlibrary-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-applicationlibrary-1.2.0.tar", last modified: Mon Jun 12 19:44:21 2023, max compression
+gzip compressed data, was "robotframework-applicationlibrary-1.2.1.tar", last modified: Tue Jun 27 13:13:00 2023, max compression
```

## Comparing `robotframework-applicationlibrary-1.2.0.tar` & `robotframework-applicationlibrary-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:21.158273 robotframework-applicationlibrary-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-06-12 19:44:21.158273 robotframework-applicationlibrary-1.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:21.158273 robotframework-applicationlibrary-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 19:44:21.162273 robotframework-applicationlibrary-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:21.158273 robotframework-applicationlibrary-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:21.158273 robotframework-applicationlibrary-1.2.0/src/ApplicationLibrary/
--rw-r--r--   0 runner    (1001) docker     (123)    61922 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/src/ApplicationLibrary/DesktopLibrary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:21.158273 robotframework-applicationlibrary-1.2.0/src/ApplicationLibrary/Helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/src/ApplicationLibrary/Helpers/AppiumCommon.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/src/ApplicationLibrary/Helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/src/ApplicationLibrary/MobileLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/src/ApplicationLibrary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:21.158273 robotframework-applicationlibrary-1.2.0/src/robotframework_applicationlibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-06-12 19:44:21.000000 robotframework-applicationlibrary-1.2.0/src/robotframework_applicationlibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-12 19:44:21.000000 robotframework-applicationlibrary-1.2.0/src/robotframework_applicationlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:44:21.000000 robotframework-applicationlibrary-1.2.0/src/robotframework_applicationlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 19:44:21.000000 robotframework-applicationlibrary-1.2.0/src/robotframework_applicationlibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 19:44:21.000000 robotframework-applicationlibrary-1.2.0/src/robotframework_applicationlibrary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 19:44:10.000000 robotframework-applicationlibrary-1.2.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:13:00.786938 robotframework-applicationlibrary-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-06-27 13:13:00.786938 robotframework-applicationlibrary-1.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:13:00.782938 robotframework-applicationlibrary-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 13:13:00.786938 robotframework-applicationlibrary-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:13:00.782938 robotframework-applicationlibrary-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:13:00.782938 robotframework-applicationlibrary-1.2.1/src/ApplicationLibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)    61922 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/src/ApplicationLibrary/DesktopLibrary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:13:00.782938 robotframework-applicationlibrary-1.2.1/src/ApplicationLibrary/Helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/src/ApplicationLibrary/Helpers/AppiumCommon.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/src/ApplicationLibrary/Helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/src/ApplicationLibrary/MobileLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/src/ApplicationLibrary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:13:00.786938 robotframework-applicationlibrary-1.2.1/src/robotframework_applicationlibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-06-27 13:13:00.000000 robotframework-applicationlibrary-1.2.1/src/robotframework_applicationlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-27 13:13:00.000000 robotframework-applicationlibrary-1.2.1/src/robotframework_applicationlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:13:00.000000 robotframework-applicationlibrary-1.2.1/src/robotframework_applicationlibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-27 13:13:00.000000 robotframework-applicationlibrary-1.2.1/src/robotframework_applicationlibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 13:13:00.000000 robotframework-applicationlibrary-1.2.1/src/robotframework_applicationlibrary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 13:12:51.000000 robotframework-applicationlibrary-1.2.1/version.py
```

### Comparing `robotframework-applicationlibrary-1.2.0/LICENSE` & `robotframework-applicationlibrary-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-applicationlibrary-1.2.0/PKG-INFO` & `robotframework-applicationlibrary-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-applicationlibrary
-Version: 1.2.0
+Version: 1.2.1
 Summary: Robot Framework framework for mobile and desktop testing.
 Home-page: https://github.com/Accruent/robotframework-applicationlibrary
 Maintainer: Brandon Wolfe, Neil Howell, Matt Bozek, Pinky Majhi
 Maintainer-email: robosquad@accruent.com
 License: GPL-3.0
 Keywords: Robot Framework robot-framework selenium appium winappdriver appium robotframeworkdesktop windows zoomba python robotframework-library appium-windows appiumlibraryappium-mobile mobile applicationlibrary application app lib
 Platform: any
```

### Comparing `robotframework-applicationlibrary-1.2.0/docs/README.md` & `robotframework-applicationlibrary-1.2.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-applicationlibrary-1.2.0/setup.py` & `robotframework-applicationlibrary-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-applicationlibrary-1.2.0/src/ApplicationLibrary/DesktopLibrary.py` & `robotframework-applicationlibrary-1.2.1/src/ApplicationLibrary/DesktopLibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-applicationlibrary-1.2.0/src/ApplicationLibrary/Helpers/AppiumCommon.py` & `robotframework-applicationlibrary-1.2.1/src/ApplicationLibrary/Helpers/AppiumCommon.py`

 * *Files identical despite different names*

### Comparing `robotframework-applicationlibrary-1.2.0/src/ApplicationLibrary/MobileLibrary.py` & `robotframework-applicationlibrary-1.2.1/src/ApplicationLibrary/MobileLibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-applicationlibrary-1.2.0/src/robotframework_applicationlibrary.egg-info/PKG-INFO` & `robotframework-applicationlibrary-1.2.1/src/robotframework_applicationlibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-applicationlibrary
-Version: 1.2.0
+Version: 1.2.1
 Summary: Robot Framework framework for mobile and desktop testing.
 Home-page: https://github.com/Accruent/robotframework-applicationlibrary
 Maintainer: Brandon Wolfe, Neil Howell, Matt Bozek, Pinky Majhi
 Maintainer-email: robosquad@accruent.com
 License: GPL-3.0
 Keywords: Robot Framework robot-framework selenium appium winappdriver appium robotframeworkdesktop windows zoomba python robotframework-library appium-windows appiumlibraryappium-mobile mobile applicationlibrary application app lib
 Platform: any
```

### Comparing `robotframework-applicationlibrary-1.2.0/src/robotframework_applicationlibrary.egg-info/SOURCES.txt` & `robotframework-applicationlibrary-1.2.1/src/robotframework_applicationlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

