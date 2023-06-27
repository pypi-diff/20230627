# Comparing `tmp/ipos-0.0.5.tar.gz` & `tmp/ipos-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipos-0.0.5.tar", last modified: Tue Jun 27 16:49:24 2023, max compression
+gzip compressed data, was "ipos-0.0.6.tar", last modified: Tue Jun 27 16:59:16 2023, max compression
```

## Comparing `ipos-0.0.5.tar` & `ipos-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 16:49:24.935083 ipos-0.0.5/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.5/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.5/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 16:49:24.934962 ipos-0.0.5/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.5/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 16:49:24.933278 ipos-0.0.5/ipos/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 16:49:17.000000 ipos-0.0.5/ipos/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     5295 2023-06-27 16:49:17.000000 ipos-0.0.5/ipos/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.5/ipos/core.py
--rw-r--r--   0 solst      (501) staff       (20)    22648 2023-06-27 16:49:17.000000 ipos-0.0.5/ipos/imp.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 16:49:24.934781 ipos-0.0.5/ipos.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 16:49:24.000000 ipos-0.0.5/ipos.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 16:49:24.000000 ipos-0.0.5/ipos.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 16:49:24.000000 ipos-0.0.5/ipos.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 16:49:24.000000 ipos-0.0.5/ipos.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.5/ipos.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 16:49:24.000000 ipos-0.0.5/ipos.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 16:49:24.000000 ipos-0.0.5/ipos.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 14:47:09.000000 ipos-0.0.5/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 16:49:24.935128 ipos-0.0.5/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.5/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 16:59:16.620763 ipos-0.0.6/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.6/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.6/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 16:59:16.620634 ipos-0.0.6/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.6/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 16:59:16.619398 ipos-0.0.6/ipos/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 16:59:07.000000 ipos-0.0.6/ipos/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     5295 2023-06-27 16:59:07.000000 ipos-0.0.6/ipos/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.6/ipos/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    22796 2023-06-27 16:59:07.000000 ipos-0.0.6/ipos/imp.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 16:59:16.620453 ipos-0.0.6/ipos.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.6/ipos.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 16:50:34.000000 ipos-0.0.6/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 16:59:16.620803 ipos-0.0.6/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.6/setup.py
```

### Comparing `ipos-0.0.5/LICENSE` & `ipos-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipos-0.0.5/PKG-INFO` & `ipos-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.5
+Version: 0.0.6
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.5/README.md` & `ipos-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ipos-0.0.5/ipos/_modidx.py` & `ipos-0.0.6/ipos/_modidx.py`

 * *Files identical despite different names*

### Comparing `ipos-0.0.5/ipos/imp.py` & `ipos-0.0.6/ipos/imp.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,16 @@
     
     def update_namespace(
         self, 
         updates: Optional[VariableDict] = None,
         namespace: Optional[VariableDict] = None,
     ) -> VariableDict:        
         updates = getattr(self, '_updates', updates)
-        namespace = getattr(self, 'namespace', (namespace or globals()))
+        namespace = getattr(self, 'namespace', namespace)
+        namespace = namespace or globals()
         namespace.update(updates)
         self.namespace = namespace
         return namespace
 
 # %% ../nbs/00_core.ipynb 20
 @dataclass
 class ImpSubSpec(BaseImp):
@@ -631,14 +632,15 @@
 
         # print('updates', updates, 'fallbacks', self.fallbacks.items())
         updates = self.fallbacks.give(updates)
         # print('updates', updates, 'fallbacks', self.fallbacks.items())
         
         self._updates = updates
         self.update_namespace(updates, self.namespace)
+        return updates
 
 # %% ../nbs/00_core.ipynb 27
 @dataclass
 class Imp(BaseImp):
     """
     Import Module class.
     
@@ -685,16 +687,18 @@
     _ : KW_ONLY
     _module: Module = field(init=False, repr=False, default=None)
     _spec: ImpSpec = field(init=False, repr=False, default=None)
 
     def load(self):
         self._spec = ImpSpec(self.name, self.nick, self.lazy, self.subspecs, self.fallbacks)
         self._spec._imp_main()
-        self._spec._imp_subs()
+        updates = self._spec._imp_subs()
         self._module = sys.modules[self.name]
+        self._updates = updates
+        self.update_namespace(updates, self.namespace)
 
     def __post_init__(self):
         if isinstance(self.fallbacks, dict):
             self.fallbacks = Fallbacks.from_dict(self.fallbacks)
             
         if not self.delay:
             self.load()
```

### Comparing `ipos-0.0.5/ipos.egg-info/PKG-INFO` & `ipos-0.0.6/ipos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.5
+Version: 0.0.6
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.5/settings.ini` & `ipos-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ipos
 lib_name = ipos
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ipos
 nbs_path = nbs
 recursive = True
```

### Comparing `ipos-0.0.5/setup.py` & `ipos-0.0.6/setup.py`

 * *Files identical despite different names*

