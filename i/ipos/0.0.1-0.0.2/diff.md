# Comparing `tmp/ipos-0.0.1.tar.gz` & `tmp/ipos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipos-0.0.1.tar", last modified: Tue Jun 27 14:24:11 2023, max compression
+gzip compressed data, was "ipos-0.0.2.tar", last modified: Tue Jun 27 14:33:26 2023, max compression
```

## Comparing `ipos-0.0.1.tar` & `ipos-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:24:11.283775 ipos-0.0.1/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.1/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.1/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 14:24:11.283656 ipos-0.0.1/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.1/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:24:11.282568 ipos-0.0.1/ipos/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 14:22:42.000000 ipos-0.0.1/ipos/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     4629 2023-06-27 14:22:51.000000 ipos-0.0.1/ipos/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.1/ipos/core.py
--rw-r--r--   0 solst      (501) staff       (20)    17875 2023-06-27 14:22:42.000000 ipos-0.0.1/ipos/imp.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:24:11.283470 ipos-0.0.1/ipos.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 14:24:11.000000 ipos-0.0.1/ipos.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 14:24:11.000000 ipos-0.0.1/ipos.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.1/ipos.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 14:24:11.000000 ipos-0.0.1/ipos.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.1/ipos.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 14:24:11.000000 ipos-0.0.1/ipos.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 14:24:11.000000 ipos-0.0.1/ipos.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      954 2023-06-27 12:22:58.000000 ipos-0.0.1/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 14:24:11.283835 ipos-0.0.1/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.1/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:33:26.321557 ipos-0.0.2/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.2/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.2/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 14:33:26.321434 ipos-0.0.2/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.2/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:33:26.320361 ipos-0.0.2/ipos/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 14:33:21.000000 ipos-0.0.2/ipos/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     4629 2023-06-27 14:33:21.000000 ipos-0.0.2/ipos/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.2/ipos/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    18036 2023-06-27 14:33:21.000000 ipos-0.0.2/ipos/imp.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 14:33:26.321236 ipos-0.0.2/ipos.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.2/ipos.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 14:33:26.000000 ipos-0.0.2/ipos.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 14:33:21.000000 ipos-0.0.2/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 14:33:26.321598 ipos-0.0.2/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.2/setup.py
```

### Comparing `ipos-0.0.1/LICENSE` & `ipos-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipos-0.0.1/PKG-INFO` & `ipos-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.1
+Version: 0.0.2
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.1/README.md` & `ipos-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ipos-0.0.1/ipos/_modidx.py` & `ipos-0.0.2/ipos/_modidx.py`

 * *Files identical despite different names*

### Comparing `ipos-0.0.1/ipos/imp.py` & `ipos-0.0.2/ipos/imp.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,14 +498,19 @@
             warnings.warn(f'Could not import {self.name}')
             return
         
     def _imp_subs(self):
         updates = dict()
         for subspec in self.subspecs:
             updates.update(subspec.get_updates())
+
+        for name, fallback in self.fallbacks.items():
+            if name not in updates and not is_mod_or_var(name):
+                updates[name] = fallback
+
         globals().update(updates)
 
 # %% ../nbs/00_core.ipynb 14
 @dataclass
 class Imp:
     """
     Import Module class.
```

### Comparing `ipos-0.0.1/ipos.egg-info/PKG-INFO` & `ipos-0.0.2/ipos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.1
+Version: 0.0.2
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.1/setup.py` & `ipos-0.0.2/setup.py`

 * *Files identical despite different names*

