# Comparing `tmp/hein_robots-0.5.3.tar.gz` & `tmp/hein_robots-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hein_robots-0.5.3.tar", last modified: Wed Aug 17 17:10:02 2022, max compression
+gzip compressed data, was "dist/hein_robots-0.6.0.tar", last modified: Tue Jun 27 18:59:29 2023, max compression
```

## Comparing `hein_robots-0.5.3.tar` & `hein_robots-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 17:10:02.000000 hein_robots-0.5.3/
--rw-r--r--   0 root         (0) root         (0)     1260 2022-08-17 17:10:02.000000 hein_robots-0.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1085 2022-08-17 17:09:54.000000 hein_robots-0.5.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1874 2022-08-17 17:09:54.000000 hein_robots-0.5.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 17:10:01.000000 hein_robots-0.5.3/hein_robots/
--rw-rw-rw-   0 root         (0) root         (0)    23748 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/robotics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 17:10:02.000000 hein_robots-0.5.3/hein_robots/robodk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/robodk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4071 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/robodk/sim_arm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 17:10:02.000000 hein_robots-0.5.3/hein_robots/base/
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/base/grippers.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11595 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/base/robot_arms.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/base/actuators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 17:10:02.000000 hein_robots-0.5.3/hein_robots/robotiq/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/robotiq/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5585 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/robotiq/gripper.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3561 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 17:10:02.000000 hein_robots-0.5.3/hein_robots/kinova/
--rw-rw-rw-   0 root         (0) root         (0)    17469 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/kinova/kinova_gen3.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/kinova/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2472 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/kinova/kinova_gripper.py
--rw-rw-rw-   0 root         (0) root         (0)     6446 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/kinova/kortex.py
--rw-rw-rw-   0 root         (0) root         (0)     5668 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/kinova/kinova_sequence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 17:10:02.000000 hein_robots-0.5.3/hein_robots/universal_robots/
--rw-rw-rw-   0 root         (0) root         (0)     2237 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/universal_robots/urscript_sequence.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/universal_robots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10327 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/universal_robots/ur3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 17:10:02.000000 hein_robots-0.5.3/hein_robots/vention/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/vention/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/vention/gantry.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     5101 2022-08-17 17:09:54.000000 hein_robots-0.5.3/hein_robots/grids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 17:10:02.000000 hein_robots-0.5.3/hein_robots.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1260 2022-08-17 17:10:01.000000 hein_robots-0.5.3/hein_robots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      942 2022-08-17 17:10:01.000000 hein_robots-0.5.3/hein_robots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-17 17:10:01.000000 hein_robots-0.5.3/hein_robots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-08-17 17:10:01.000000 hein_robots-0.5.3/hein_robots.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-08-17 17:10:01.000000 hein_robots-0.5.3/hein_robots.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      873 2022-08-17 17:09:54.000000 hein_robots-0.5.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-17 17:10:02.000000 hein_robots-0.5.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 18:59:29.000000 hein_robots-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-06-27 18:59:29.000000 hein_robots-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-27 18:59:23.000000 hein_robots-0.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-06-27 18:59:23.000000 hein_robots-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots/
+-rw-rw-rw-   0 root         (0) root         (0)    23748 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/robotics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots/robodk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/robodk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4071 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/robodk/sim_arm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots/base/
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/base/grippers.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11595 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/base/robot_arms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/base/actuators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6752 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots/robotiq/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/robotiq/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5585 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/robotiq/gripper.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3561 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots/kinova/
+-rw-rw-rw-   0 root         (0) root         (0)    17469 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/kinova/kinova_gen3.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/kinova/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/kinova/kinova_gripper.py
+-rw-rw-rw-   0 root         (0) root         (0)     6446 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/kinova/kortex.py
+-rw-rw-rw-   0 root         (0) root         (0)     5668 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/kinova/kinova_sequence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots/universal_robots/
+-rw-rw-rw-   0 root         (0) root         (0)     2237 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/universal_robots/urscript_sequence.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/universal_robots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10327 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/universal_robots/ur3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots/vention/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/vention/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/vention/gantry.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5101 2023-06-27 18:59:23.000000 hein_robots-0.6.0/hein_robots/grids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-27 18:59:29.000000 hein_robots-0.6.0/hein_robots.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-27 18:59:23.000000 hein_robots-0.6.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 18:59:29.000000 hein_robots-0.6.0/setup.cfg
```

### Comparing `hein_robots-0.5.3/PKG-INFO` & `hein_robots-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hein_robots
-Version: 0.5.3
+Version: 0.6.0
 Summary: An easy-to-use package that provides a common interface for controlling robots used by the Hein Lab
 Home-page: https://gitlab.com/heingroup/hein_robots
 Author: Sean Clark
 Author-email: sean@v13inc.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
```

### Comparing `hein_robots-0.5.3/LICENSE` & `hein_robots-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/setup.py` & `hein_robots-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 REQUIRES_PYTHON = '>=3.6.0'
 VERSION = None
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy',
     'scipy',
+    'pupil-apriltags',
+    'opencv-python'
 ]
 
 REQUIRED_REPOS = [
 ]
 
 # What packages are optional?
 EXTRAS = {
```

### Comparing `hein_robots-0.5.3/hein_robots/robotics.py` & `hein_robots-0.6.0/hein_robots/robotics.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/robodk/sim_arm.py` & `hein_robots-0.6.0/hein_robots/robodk/sim_arm.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/base/grippers.py` & `hein_robots-0.6.0/hein_robots/base/grippers.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/base/robot_arms.py` & `hein_robots-0.6.0/hein_robots/base/robot_arms.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/base/actuators.py` & `hein_robots-0.6.0/hein_robots/base/actuators.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/robotiq/gripper.py` & `hein_robots-0.6.0/hein_robots/robotiq/gripper.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/utils.py` & `hein_robots-0.6.0/hein_robots/utils.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/managers.py` & `hein_robots-0.6.0/hein_robots/managers.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/kinova/kinova_gen3.py` & `hein_robots-0.6.0/hein_robots/kinova/kinova_gen3.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/kinova/kinova_gripper.py` & `hein_robots-0.6.0/hein_robots/kinova/kinova_gripper.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/kinova/kortex.py` & `hein_robots-0.6.0/hein_robots/kinova/kortex.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/kinova/kinova_sequence.py` & `hein_robots-0.6.0/hein_robots/kinova/kinova_sequence.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/universal_robots/urscript_sequence.py` & `hein_robots-0.6.0/hein_robots/universal_robots/urscript_sequence.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/universal_robots/ur3.py` & `hein_robots-0.6.0/hein_robots/universal_robots/ur3.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/vention/gantry.py` & `hein_robots-0.6.0/hein_robots/vention/gantry.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots/grids.py` & `hein_robots-0.6.0/hein_robots/grids.py`

 * *Files identical despite different names*

### Comparing `hein_robots-0.5.3/hein_robots.egg-info/PKG-INFO` & `hein_robots-0.6.0/hein_robots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hein-robots
-Version: 0.5.3
+Version: 0.6.0
 Summary: An easy-to-use package that provides a common interface for controlling robots used by the Hein Lab
 Home-page: https://gitlab.com/heingroup/hein_robots
 Author: Sean Clark
 Author-email: sean@v13inc.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
```

### Comparing `hein_robots-0.5.3/hein_robots.egg-info/SOURCES.txt` & `hein_robots-0.6.0/hein_robots.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 hein_robots/__init__.py
 hein_robots/__version__.py
 hein_robots/grids.py
 hein_robots/managers.py
 hein_robots/robotics.py
 hein_robots/utils.py
+hein_robots/vision.py
 hein_robots.egg-info/PKG-INFO
 hein_robots.egg-info/SOURCES.txt
 hein_robots.egg-info/dependency_links.txt
 hein_robots.egg-info/requires.txt
 hein_robots.egg-info/top_level.txt
 hein_robots/base/__init__.py
 hein_robots/base/actuators.py
```

### Comparing `hein_robots-0.5.3/README.md` & `hein_robots-0.6.0/README.md`

 * *Files identical despite different names*

