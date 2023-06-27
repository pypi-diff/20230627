# Comparing `tmp/autoclickerPy-0.0.1.tar.gz` & `tmp/autoclickerPy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoclickerPy-0.0.1.tar", last modified: Tue Jun 27 18:19:49 2023, max compression
+gzip compressed data, was "autoclickerPy-0.0.2.tar", last modified: Tue Jun 27 18:26:38 2023, max compression
```

## Comparing `autoclickerPy-0.0.1.tar` & `autoclickerPy-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 18:19:49.484916 autoclickerPy-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-27 16:29:17.000000 autoclickerPy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1128 2023-06-27 18:19:49.484916 autoclickerPy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      563 2023-06-27 17:08:17.000000 autoclickerPy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 18:19:49.480928 autoclickerPy-0.0.1/autoclickerPy/
--rw-rw-rw-   0        0        0       38 2023-06-27 18:19:40.000000 autoclickerPy-0.0.1/autoclickerPy/__init__.py
--rw-rw-rw-   0        0        0     2103 2023-06-27 17:08:17.000000 autoclickerPy-0.0.1/autoclickerPy/autoclicker.py
-drwxrwxrwx   0        0        0        0 2023-06-27 18:19:49.483919 autoclickerPy-0.0.1/autoclickerPy.egg-info/
--rw-rw-rw-   0        0        0     1128 2023-06-27 18:19:49.000000 autoclickerPy-0.0.1/autoclickerPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-06-27 18:19:49.000000 autoclickerPy-0.0.1/autoclickerPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 18:19:49.000000 autoclickerPy-0.0.1/autoclickerPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-27 18:19:49.000000 autoclickerPy-0.0.1/autoclickerPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-27 18:19:49.000000 autoclickerPy-0.0.1/autoclickerPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 18:19:49.484916 autoclickerPy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-06-27 18:13:22.000000 autoclickerPy-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 18:26:38.310161 autoclickerPy-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 16:29:17.000000 autoclickerPy-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1100 2023-06-27 18:26:38.309163 autoclickerPy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-06-27 18:26:23.000000 autoclickerPy-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 18:26:38.306060 autoclickerPy-0.0.2/autoclickerPy/
+-rw-rw-rw-   0        0        0       38 2023-06-27 18:19:40.000000 autoclickerPy-0.0.2/autoclickerPy/__init__.py
+-rw-rw-rw-   0        0        0     2101 2023-06-27 18:21:53.000000 autoclickerPy-0.0.2/autoclickerPy/autoclicker.py
+drwxrwxrwx   0        0        0        0 2023-06-27 18:26:38.308167 autoclickerPy-0.0.2/autoclickerPy.egg-info/
+-rw-rw-rw-   0        0        0     1100 2023-06-27 18:26:38.000000 autoclickerPy-0.0.2/autoclickerPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-27 18:26:38.000000 autoclickerPy-0.0.2/autoclickerPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 18:26:38.000000 autoclickerPy-0.0.2/autoclickerPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-27 18:26:38.000000 autoclickerPy-0.0.2/autoclickerPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-27 18:26:38.000000 autoclickerPy-0.0.2/autoclickerPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 18:26:38.310161 autoclickerPy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-06-27 18:26:28.000000 autoclickerPy-0.0.2/setup.py
```

### Comparing `autoclickerPy-0.0.1/LICENSE` & `autoclickerPy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autoclickerPy-0.0.1/PKG-INFO` & `autoclickerPy-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoclickerPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple autoclicker for python
 Author: Geo
 Author-email: <geocraft31@gamil.com>
 Keywords: python,autoclicker
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -20,27 +20,27 @@
 Simple autoclicker in python.
 
 ## How to use
 
 Running the autoclicker for some time
 
 ```python
-from Autoclicker_geo.autoclicker import Autoclicker
+from autoclickerPy import Autoclicker
 from pynput.mouse import Button
 
 clicker = Autoclicker(delay=0.1, mouseButton=Button.left)
 
 # Runs autoclicker for 1 second
 clicker.run(1)
 ```
 
 Starting and stoping the autoclicker
 
 ```python
-from Autoclicker_geo.autoclicker import Autoclicker
+from autoclickerPy import Autoclicker
 from pynput.mouse import Button
 import time
 
 clicker = Autoclicker(delay=0.1, mouseButton=Button.left)
 
 clicker.start()
  ... some code ...
```

### Comparing `autoclickerPy-0.0.1/README.md` & `autoclickerPy-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 Simple autoclicker in python.
 
 ## How to use
 
 Running the autoclicker for some time
 
 ```python
-from Autoclicker_geo.autoclicker import Autoclicker
+from autoclickerPy import Autoclicker
 from pynput.mouse import Button
 
 clicker = Autoclicker(delay=0.1, mouseButton=Button.left)
 
 # Runs autoclicker for 1 second
 clicker.run(1)
 ```
 
 Starting and stoping the autoclicker
 
 ```python
-from Autoclicker_geo.autoclicker import Autoclicker
+from autoclickerPy import Autoclicker
 from pynput.mouse import Button
 import time
 
 clicker = Autoclicker(delay=0.1, mouseButton=Button.left)
 
 clicker.start()
  ... some code ...
```

### Comparing `autoclickerPy-0.0.1/autoclickerPy/autoclicker.py` & `autoclickerPy-0.0.2/autoclickerPy/autoclicker.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,9 +78,9 @@
         time.sleep(timeSec)
         self.stop()
 
     def _clicker(self):
         # private! Not for public use
         
         while not self._stopEvent.is_set():
-            self._mouse.click(self._mouseButton)
-            time.sleep(self._delay)
+            self._mouse.click(self.mouseButton)
+            time.sleep(self.delay)
```

### Comparing `autoclickerPy-0.0.1/autoclickerPy.egg-info/PKG-INFO` & `autoclickerPy-0.0.2/autoclickerPy.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoclickerPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple autoclicker for python
 Author: Geo
 Author-email: <geocraft31@gamil.com>
 Keywords: python,autoclicker
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -20,27 +20,27 @@
 Simple autoclicker in python.
 
 ## How to use
 
 Running the autoclicker for some time
 
 ```python
-from Autoclicker_geo.autoclicker import Autoclicker
+from autoclickerPy import Autoclicker
 from pynput.mouse import Button
 
 clicker = Autoclicker(delay=0.1, mouseButton=Button.left)
 
 # Runs autoclicker for 1 second
 clicker.run(1)
 ```
 
 Starting and stoping the autoclicker
 
 ```python
-from Autoclicker_geo.autoclicker import Autoclicker
+from autoclickerPy import Autoclicker
 from pynput.mouse import Button
 import time
 
 clicker = Autoclicker(delay=0.1, mouseButton=Button.left)
 
 clicker.start()
  ... some code ...
```

### Comparing `autoclickerPy-0.0.1/setup.py` & `autoclickerPy-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Simple autoclicker for python'
 LONGDESCRIPTION = 'Simple autoclicker for python long description'
 
 # Setting up
 setup(
     name="autoclickerPy",
     version=VERSION,
```

