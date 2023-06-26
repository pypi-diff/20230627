# Comparing `tmp/platformer1234-0.0.1.tar.gz` & `tmp/platformer1234-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platformer1234-0.0.1.tar", last modified: Mon Jun 26 23:34:07 2023, max compression
+gzip compressed data, was "platformer1234-0.0.2.tar", last modified: Mon Jun 26 23:50:43 2023, max compression
```

## Comparing `platformer1234-0.0.1.tar` & `platformer1234-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-06-26 23:34:07.284123 platformer1234-0.0.1/
--rw-r--r--   0 andy       (501) staff       (20)       34 2023-06-26 23:28:45.000000 platformer1234-0.0.1/MANIFEST.in
--rw-r--r--   0 andy       (501) staff       (20)      363 2023-06-26 23:34:07.283740 platformer1234-0.0.1/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)        0 2023-06-26 23:25:42.000000 platformer1234-0.0.1/README
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-06-26 23:34:07.265679 platformer1234-0.0.1/platformer1234/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-06-26 23:34:07.282282 platformer1234-0.0.1/platformer1234/images/
--rw-r--r--   0 andy       (501) staff       (20)     6148 2023-06-15 04:41:29.000000 platformer1234-0.0.1/platformer1234/images/.DS_Store
--rw-r--r--   0 andy       (501) staff       (20)        0 2023-06-26 23:24:04.000000 platformer1234-0.0.1/platformer1234/images/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)       63 2023-06-26 23:20:04.000000 platformer1234-0.0.1/platformer1234/images/__main__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-06-26 23:34:07.282612 platformer1234-0.0.1/platformer1234/images/__pycache__/
--rw-r--r--   0 andy       (501) staff       (20)     4905 2023-06-26 23:22:56.000000 platformer1234-0.0.1/platformer1234/images/__pycache__/platformer.cpython-39.pyc
--rw-------   0 andy       (501) staff       (20)     5866 2023-06-15 04:41:18.000000 platformer1234-0.0.1/platformer1234/images/background.jpg
--rw-------   0 andy       (501) staff       (20)     9393 2023-06-15 04:37:31.000000 platformer1234-0.0.1/platformer1234/images/death effect.jpg
--rw-r--r--   0 andy       (501) staff       (20)     7533 2023-06-12 23:54:55.000000 platformer1234-0.0.1/platformer1234/images/enemy.png
--rw-------   0 andy       (501) staff       (20)     6774 2023-06-15 04:38:48.000000 platformer1234-0.0.1/platformer1234/images/enemy1.jpg
--rw-------   0 andy       (501) staff       (20)   399747 2023-06-15 04:42:09.000000 platformer1234-0.0.1/platformer1234/images/ground.png
--rw-------   0 andy       (501) staff       (20)     4528 2023-06-15 04:35:09.000000 platformer1234-0.0.1/platformer1234/images/gunfire.jpg
--rw-------   0 andy       (501) staff       (20)     5774 2023-06-15 04:36:39.000000 platformer1234-0.0.1/platformer1234/images/platform1.jpg
--rw-------   0 andy       (501) staff       (20)     6768 2023-06-15 04:36:18.000000 platformer1234-0.0.1/platformer1234/images/platform2.jpg
--rw-------   0 andy       (501) staff       (20)     6723 2023-06-15 04:36:35.000000 platformer1234-0.0.1/platformer1234/images/platform3.jpg
--rw-r--r--   0 andy       (501) staff       (20)     5523 2023-06-26 23:22:54.000000 platformer1234-0.0.1/platformer1234/images/platformer.py
--rw-------   0 andy       (501) staff       (20)    12613 2023-06-15 04:39:54.000000 platformer1234-0.0.1/platformer1234/images/player.jpg
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-06-26 23:34:07.269050 platformer1234-0.0.1/platformer1234.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)      363 2023-06-26 23:34:07.000000 platformer1234-0.0.1/platformer1234.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      761 2023-06-26 23:34:07.000000 platformer1234-0.0.1/platformer1234.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2023-06-26 23:34:07.000000 platformer1234-0.0.1/platformer1234.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)        7 2023-06-26 23:34:07.000000 platformer1234-0.0.1/platformer1234.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)       15 2023-06-26 23:34:07.000000 platformer1234-0.0.1/platformer1234.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)       38 2023-06-26 23:34:07.284252 platformer1234-0.0.1/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)      936 2023-06-26 23:31:47.000000 platformer1234-0.0.1/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-06-26 23:50:43.637545 platformer1234-0.0.2/
+-rw-r--r--   0 andy       (501) staff       (20)       34 2023-06-26 23:28:45.000000 platformer1234-0.0.2/MANIFEST.in
+-rw-r--r--   0 andy       (501) staff       (20)      363 2023-06-26 23:50:43.636871 platformer1234-0.0.2/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)        0 2023-06-26 23:25:42.000000 platformer1234-0.0.2/README
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-06-26 23:50:43.631410 platformer1234-0.0.2/platformer1234/
+-rw-r--r--   0 andy       (501) staff       (20)     6148 2023-06-26 23:49:11.000000 platformer1234-0.0.2/platformer1234/.DS_Store
+-rw-r--r--   0 andy       (501) staff       (20)        0 2023-06-26 23:24:04.000000 platformer1234-0.0.2/platformer1234/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)       63 2023-06-26 23:20:04.000000 platformer1234-0.0.2/platformer1234/__main__.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-06-26 23:50:43.635745 platformer1234-0.0.2/platformer1234/__pycache__/
+-rw-r--r--   0 andy       (501) staff       (20)     4905 2023-06-26 23:22:56.000000 platformer1234-0.0.2/platformer1234/__pycache__/platformer.cpython-39.pyc
+-rw-------   0 andy       (501) staff       (20)     5866 2023-06-15 04:41:18.000000 platformer1234-0.0.2/platformer1234/background.jpg
+-rw-------   0 andy       (501) staff       (20)     9393 2023-06-15 04:37:31.000000 platformer1234-0.0.2/platformer1234/death effect.jpg
+-rw-r--r--   0 andy       (501) staff       (20)     7533 2023-06-12 23:54:55.000000 platformer1234-0.0.2/platformer1234/enemy.png
+-rw-------   0 andy       (501) staff       (20)     6774 2023-06-15 04:38:48.000000 platformer1234-0.0.2/platformer1234/enemy1.jpg
+-rw-------   0 andy       (501) staff       (20)   399747 2023-06-15 04:42:09.000000 platformer1234-0.0.2/platformer1234/ground.png
+-rw-------   0 andy       (501) staff       (20)     4528 2023-06-15 04:35:09.000000 platformer1234-0.0.2/platformer1234/gunfire.jpg
+-rw-------   0 andy       (501) staff       (20)     5774 2023-06-15 04:36:39.000000 platformer1234-0.0.2/platformer1234/platform1.jpg
+-rw-------   0 andy       (501) staff       (20)     6768 2023-06-15 04:36:18.000000 platformer1234-0.0.2/platformer1234/platform2.jpg
+-rw-------   0 andy       (501) staff       (20)     6723 2023-06-15 04:36:35.000000 platformer1234-0.0.2/platformer1234/platform3.jpg
+-rw-r--r--   0 andy       (501) staff       (20)     5523 2023-06-26 23:22:54.000000 platformer1234-0.0.2/platformer1234/platformer.py
+-rw-------   0 andy       (501) staff       (20)    12613 2023-06-15 04:39:54.000000 platformer1234-0.0.2/platformer1234/player.jpg
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-06-26 23:50:43.635175 platformer1234-0.0.2/platformer1234.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)      363 2023-06-26 23:50:43.000000 platformer1234-0.0.2/platformer1234.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      656 2023-06-26 23:50:43.000000 platformer1234-0.0.2/platformer1234.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2023-06-26 23:50:43.000000 platformer1234-0.0.2/platformer1234.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)        7 2023-06-26 23:50:43.000000 platformer1234-0.0.2/platformer1234.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)       15 2023-06-26 23:50:43.000000 platformer1234-0.0.2/platformer1234.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)       38 2023-06-26 23:50:43.637806 platformer1234-0.0.2/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)      936 2023-06-26 23:50:00.000000 platformer1234-0.0.2/setup.py
```

### Comparing `platformer1234-0.0.1/platformer1234/images/__pycache__/platformer.cpython-39.pyc` & `platformer1234-0.0.2/platformer1234/__pycache__/platformer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/background.jpg` & `platformer1234-0.0.2/platformer1234/background.jpg`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/death effect.jpg` & `platformer1234-0.0.2/platformer1234/death effect.jpg`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/enemy.png` & `platformer1234-0.0.2/platformer1234/enemy.png`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/enemy1.jpg` & `platformer1234-0.0.2/platformer1234/enemy1.jpg`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/ground.png` & `platformer1234-0.0.2/platformer1234/ground.png`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/gunfire.jpg` & `platformer1234-0.0.2/platformer1234/gunfire.jpg`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/platform1.jpg` & `platformer1234-0.0.2/platformer1234/platform1.jpg`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/platform2.jpg` & `platformer1234-0.0.2/platformer1234/platform2.jpg`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/platform3.jpg` & `platformer1234-0.0.2/platformer1234/platform3.jpg`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/platformer.py` & `platformer1234-0.0.2/platformer1234/platformer.py`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/platformer1234/images/player.jpg` & `platformer1234-0.0.2/platformer1234/player.jpg`

 * *Files identical despite different names*

### Comparing `platformer1234-0.0.1/setup.py` & `platformer1234-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "platformer1234",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Andy Z",
     author_email = "andyzhong147@gmail.com",
     description = ("An demonstration of how to upload project to pypi."),
     license = "MIT License",
     keywords = "tutorial",
     url = "",
     include_package_data = True,
```

