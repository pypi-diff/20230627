# Comparing `tmp/ipos-0.0.7.tar.gz` & `tmp/ipos-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipos-0.0.7.tar", last modified: Tue Jun 27 18:22:47 2023, max compression
+gzip compressed data, was "ipos-0.0.8.tar", last modified: Tue Jun 27 18:27:10 2023, max compression
```

## Comparing `ipos-0.0.7.tar` & `ipos-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:22:47.276331 ipos-0.0.7/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.7/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.7/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 18:22:47.276206 ipos-0.0.7/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.7/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:22:47.275058 ipos-0.0.7/ipos/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 18:22:45.000000 ipos-0.0.7/ipos/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     5889 2023-06-27 18:22:45.000000 ipos-0.0.7/ipos/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.7/ipos/core.py
--rw-r--r--   0 solst      (501) staff       (20)    23985 2023-06-27 18:22:45.000000 ipos-0.0.7/ipos/imp.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:22:47.275958 ipos-0.0.7/ipos.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.7/ipos.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 17:00:24.000000 ipos-0.0.7/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 18:22:47.276373 ipos-0.0.7/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.7/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:27:10.057903 ipos-0.0.8/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.8/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.8/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 18:27:10.057791 ipos-0.0.8/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.8/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:27:10.056506 ipos-0.0.8/ipos/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 18:27:07.000000 ipos-0.0.8/ipos/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     5889 2023-06-27 18:27:07.000000 ipos-0.0.8/ipos/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.8/ipos/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    23982 2023-06-27 18:27:07.000000 ipos-0.0.8/ipos/imp.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:27:10.057613 ipos-0.0.8/ipos.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.8/ipos.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 18:27:10.000000 ipos-0.0.8/ipos.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 18:23:59.000000 ipos-0.0.8/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 18:27:10.057941 ipos-0.0.8/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.8/setup.py
```

### Comparing `ipos-0.0.7/LICENSE` & `ipos-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ipos-0.0.7/PKG-INFO` & `ipos-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.7
+Version: 0.0.8
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.7/README.md` & `ipos-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ipos-0.0.7/ipos/_modidx.py` & `ipos-0.0.8/ipos/_modidx.py`

 * *Files identical despite different names*

### Comparing `ipos-0.0.7/ipos/imp.py` & `ipos-0.0.8/ipos/imp.py`

 * *Files 0% similar despite different names*

```diff
@@ -725,16 +725,16 @@
 
     _ : KW_ONLY
     _module: Module = field(init=False, repr=False, default=None)
     _spec: ImpSpec = field(init=False, repr=False, default=None)
 
     def load(self):
         self._spec = ImpSpec(self.name, self.nick, self.lazy, self.subspecs, self.fallbacks)
+        self._updates = self._spec._import()              
         self._module = sys.modules[self.name]
-        self._updates = self._spec._import()                 
         self.update_namespace(self._updates, self.namespace)
 
     def __post_init__(self):
         if isinstance(self.fallbacks, dict):
             self.fallbacks = Fallbacks.from_dict(self.fallbacks)
             
         if not self.delay:
```

### Comparing `ipos-0.0.7/ipos.egg-info/PKG-INFO` & `ipos-0.0.8/ipos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.7
+Version: 0.0.8
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.7/settings.ini` & `ipos-0.0.8/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ipos
 lib_name = ipos
-version = 0.0.7
+version = 0.0.8
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ipos
 nbs_path = nbs
 recursive = True
```

### Comparing `ipos-0.0.7/setup.py` & `ipos-0.0.8/setup.py`

 * *Files identical despite different names*

