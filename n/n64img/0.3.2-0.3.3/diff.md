# Comparing `tmp/n64img-0.3.2.tar.gz` & `tmp/n64img-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n64img-0.3.2.tar", last modified: Tue Jun 27 04:29:15 2023, max compression
+gzip compressed data, was "n64img-0.3.3.tar", last modified: Tue Jun 27 06:28:48 2023, max compression
```

## Comparing `n64img-0.3.2.tar` & `n64img-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:15.200862 n64img-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-27 04:29:07.000000 n64img-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 04:29:15.200862 n64img-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 04:29:07.000000 n64img-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:15.200862 n64img-0.3.2/n64img/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:07.000000 n64img-0.3.2/n64img/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-27 04:29:07.000000 n64img-0.3.2/n64img/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-27 04:29:07.000000 n64img-0.3.2/n64img/iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:15.200862 n64img-0.3.2/n64img.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 04:29:15.000000 n64img-0.3.2/n64img.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-27 04:29:15.000000 n64img-0.3.2/n64img.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 04:29:15.000000 n64img-0.3.2/n64img.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 04:29:15.000000 n64img-0.3.2/n64img.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 04:29:15.000000 n64img-0.3.2/n64img.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 04:29:07.000000 n64img-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-27 04:29:15.200862 n64img-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:15.200862 n64img-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 04:29:07.000000 n64img-0.3.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-27 04:29:07.000000 n64img-0.3.2/test/test_endian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-27 04:29:07.000000 n64img-0.3.2/test/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:28:48.726430 n64img-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-27 06:28:41.000000 n64img-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 06:28:48.726430 n64img-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 06:28:41.000000 n64img-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:28:48.726430 n64img-0.3.3/n64img/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:28:41.000000 n64img-0.3.3/n64img/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-27 06:28:41.000000 n64img-0.3.3/n64img/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-27 06:28:41.000000 n64img-0.3.3/n64img/iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:28:48.726430 n64img-0.3.3/n64img.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 06:28:48.000000 n64img-0.3.3/n64img.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-27 06:28:48.000000 n64img-0.3.3/n64img.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:28:48.000000 n64img-0.3.3/n64img.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 06:28:48.000000 n64img-0.3.3/n64img.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 06:28:48.000000 n64img-0.3.3/n64img.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 06:28:41.000000 n64img-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-27 06:28:48.730430 n64img-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:28:48.726430 n64img-0.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:28:41.000000 n64img-0.3.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-27 06:28:41.000000 n64img-0.3.3/test/test_endian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-27 06:28:41.000000 n64img-0.3.3/test/test_image.py
```

### Comparing `n64img-0.3.2/LICENSE` & `n64img-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `n64img-0.3.2/n64img/image.py` & `n64img-0.3.3/n64img/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
             return self.data
 
         img = bytearray()
 
         for x, y, i in iter.iter_image_indexes(
             self.width, self.height, self.depth, self.flip_h, self.flip_v
         ):
-            img += bytes((self.data[i + 1], self.data[i]))
+            img += bytes((self.data[i], self.data[i + 1]))
 
         return bytes(img)
 
 
 class RGBA16(Image):
     def __init__(self, data: bytes, width: int, height: int) -> None:
         super().__init__(data, width, height)
```

### Comparing `n64img-0.3.2/n64img/iter.py` & `n64img-0.3.3/n64img/iter.py`

 * *Files identical despite different names*

### Comparing `n64img-0.3.2/test/test_endian.py` & `n64img-0.3.3/test/test_endian.py`

 * *Files identical despite different names*

### Comparing `n64img-0.3.2/test/test_image.py` & `n64img-0.3.3/test/test_image.py`

 * *Files identical despite different names*

