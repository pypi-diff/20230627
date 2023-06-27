# Comparing `tmp/ipos-0.0.6.tar.gz` & `tmp/ipos-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipos-0.0.6.tar", last modified: Tue Jun 27 16:59:16 2023, max compression
+gzip compressed data, was "ipos-0.0.7.tar", last modified: Tue Jun 27 18:22:47 2023, max compression
```

## Comparing `ipos-0.0.6.tar` & `ipos-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 16:59:16.620763 ipos-0.0.6/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.6/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.6/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 16:59:16.620634 ipos-0.0.6/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.6/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 16:59:16.619398 ipos-0.0.6/ipos/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 16:59:07.000000 ipos-0.0.6/ipos/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     5295 2023-06-27 16:59:07.000000 ipos-0.0.6/ipos/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.6/ipos/core.py
--rw-r--r--   0 solst      (501) staff       (20)    22796 2023-06-27 16:59:07.000000 ipos-0.0.6/ipos/imp.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 16:59:16.620453 ipos-0.0.6/ipos.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.6/ipos.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 16:59:16.000000 ipos-0.0.6/ipos.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 16:50:34.000000 ipos-0.0.6/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 16:59:16.620803 ipos-0.0.6/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.6/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:22:47.276331 ipos-0.0.7/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ipos-0.0.7/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 ipos-0.0.7/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 18:22:47.276206 ipos-0.0.7/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1364 2023-06-27 14:22:35.000000 ipos-0.0.7/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:22:47.275058 ipos-0.0.7/ipos/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 18:22:45.000000 ipos-0.0.7/ipos/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     5889 2023-06-27 18:22:45.000000 ipos-0.0.7/ipos/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-27 12:22:22.000000 ipos-0.0.7/ipos/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    23985 2023-06-27 18:22:45.000000 ipos-0.0.7/ipos/imp.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 18:22:47.275958 ipos-0.0.7/ipos.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2117 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      306 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 14:24:11.000000 ipos-0.0.7/ipos.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-27 18:22:47.000000 ipos-0.0.7/ipos.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      764 2023-06-27 17:00:24.000000 ipos-0.0.7/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 18:22:47.276373 ipos-0.0.7/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ipos-0.0.7/setup.py
```

### Comparing `ipos-0.0.6/LICENSE` & `ipos-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ipos-0.0.6/PKG-INFO` & `ipos-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.6
+Version: 0.0.7
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.6/README.md` & `ipos-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ipos-0.0.6/ipos/_modidx.py` & `ipos-0.0.7/ipos/_modidx.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/ipos',
                 'doc_host': 'https://dsm-72.github.io',
                 'git_url': 'https://github.com/dsm-72/ipos',
                 'lib_path': 'ipos'},
   'syms': { 'ipos.core': {'ipos.core.foo': ('core.html#foo', 'ipos/core.py')},
             'ipos.imp': { 'ipos.imp.BaseImp': ('core.html#baseimp', 'ipos/imp.py'),
-                          'ipos.imp.BaseImp.make_updates_failsafe': ('core.html#baseimp.make_updates_failsafe', 'ipos/imp.py'),
+                          'ipos.imp.BaseImp.give_updates_fallbacks': ('core.html#baseimp.give_updates_fallbacks', 'ipos/imp.py'),
+                          'ipos.imp.BaseImp.squash_name_error': ('core.html#baseimp.squash_name_error', 'ipos/imp.py'),
                           'ipos.imp.BaseImp.update_fallbacks': ('core.html#baseimp.update_fallbacks', 'ipos/imp.py'),
                           'ipos.imp.BaseImp.update_namespace': ('core.html#baseimp.update_namespace', 'ipos/imp.py'),
                           'ipos.imp.Fallbacks': ('core.html#fallbacks', 'ipos/imp.py'),
                           'ipos.imp.Fallbacks.from_dict': ('core.html#fallbacks.from_dict', 'ipos/imp.py'),
                           'ipos.imp.Fallbacks.from_imp': ('core.html#fallbacks.from_imp', 'ipos/imp.py'),
                           'ipos.imp.Fallbacks.from_items': ('core.html#fallbacks.from_items', 'ipos/imp.py'),
                           'ipos.imp.Fallbacks.give': ('core.html#fallbacks.give', 'ipos/imp.py'),
@@ -33,16 +34,20 @@
                           'ipos.imp.ImpItem.has_alias': ('core.html#impitem.has_alias', 'ipos/imp.py'),
                           'ipos.imp.ImpItem.varname': ('core.html#impitem.varname', 'ipos/imp.py'),
                           'ipos.imp.ImpSpec': ('core.html#impspec', 'ipos/imp.py'),
                           'ipos.imp.ImpSpec.__post_init__': ('core.html#impspec.__post_init__', 'ipos/imp.py'),
                           'ipos.imp.ImpSpec._get_loader': ('core.html#impspec._get_loader', 'ipos/imp.py'),
                           'ipos.imp.ImpSpec._imp_main': ('core.html#impspec._imp_main', 'ipos/imp.py'),
                           'ipos.imp.ImpSpec._imp_subs': ('core.html#impspec._imp_subs', 'ipos/imp.py'),
+                          'ipos.imp.ImpSpec._import': ('core.html#impspec._import', 'ipos/imp.py'),
+                          'ipos.imp.ImpSpec.all_expected_items': ('core.html#impspec.all_expected_items', 'ipos/imp.py'),
+                          'ipos.imp.ImpSpec.squash_all_name_errors': ('core.html#impspec.squash_all_name_errors', 'ipos/imp.py'),
                           'ipos.imp.ImpSubSpec': ('core.html#impsubspec', 'ipos/imp.py'),
                           'ipos.imp.ImpSubSpec.__post_init__': ('core.html#impsubspec.__post_init__', 'ipos/imp.py'),
+                          'ipos.imp.ImpSubSpec.expected_items': ('core.html#impsubspec.expected_items', 'ipos/imp.py'),
                           'ipos.imp.ImpSubSpec.fetch': ('core.html#impsubspec.fetch', 'ipos/imp.py'),
                           'ipos.imp.ImpSubSpec.from_str': ('core.html#impsubspec.from_str', 'ipos/imp.py'),
                           'ipos.imp.ImpSubSpec.get_updates': ('core.html#impsubspec.get_updates', 'ipos/imp.py'),
                           'ipos.imp.ImpSubSpec.getitem': ('core.html#impsubspec.getitem', 'ipos/imp.py'),
                           'ipos.imp.ImpSubSpec.items_from_str': ('core.html#impsubspec.items_from_str', 'ipos/imp.py'),
                           'ipos.imp.ImpSubSpec.path': ('core.html#impsubspec.path', 'ipos/imp.py'),
                           'ipos.imp.ImpSubSpec.update_globals': ('core.html#impsubspec.update_globals', 'ipos/imp.py'),
```

### Comparing `ipos-0.0.6/ipos/imp.py` & `ipos-0.0.7/ipos/imp.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # %% auto 0
 __all__ = ['Module', 'Loader', 'ModuleSpec', 'VariableDict', 'FallbackType', 'ImpItemsType', 'ImpSubSpecType', 'GlobalImport',
            'modjoin', 'is_mod', 'is_mod_imp', 'is_var_imp', 'is_mod_or_var', 'is_mod_avail', 'loader_from_spec',
            'module_from_str', 'getmodule', 'ImpItem', 'Fallbacks', 'BaseImp', 'ImpSubSpec', 'ImpSpec', 'Imp']
 
 # %% ../nbs/00_core.ipynb 3
-import sys, types, inspect, importlib, warnings
+import sys, types, inspect, importlib, warnings, itertools
 from importlib.util import (LazyLoader, find_spec, module_from_spec)
 from importlib.abc import Loader
 from importlib.machinery import ModuleSpec
 
 from dataclasses import dataclass, field, KW_ONLY
 from typing import Optional, Dict, Any, TypeAlias, Union, ClassVar, List, Tuple
 
@@ -399,23 +399,23 @@
         Whether or not to use lazy import.
 
     namespace: Optional[VariableDict], default=globals
         The namespace in which to import the module.
         
     """    
     _ : KW_ONLY
-    namespace: Dict[str, Any] = field(default_factory=globals, repr=False)
+    namespace: VariableDict = field(default_factory=globals, repr=False)
     _updates: VariableDict = field(default_factory=dict, repr=False, init=False)
 
     def update_fallbacks(self, other: FallbackType = None, items: ImpItemsType = None) -> 'BaseImp':
         fbnew = Fallbacks.from_imp(other, items)
         self.fallbacks.update(fbnew)
         return self
     
-    def make_updates_failsafe(self, updates: Optional[VariableDict] = dict()) -> VariableDict:
+    def give_updates_fallbacks(self, updates: Optional[VariableDict] = dict()) -> VariableDict:
         oldvals = getattr(self, '_updates', (updates or dict()))
         oldvals.update(updates)
         updates = self.fallbacks.give(oldvals)                
         return updates
     
     def update_namespace(
         self, 
@@ -424,14 +424,25 @@
     ) -> VariableDict:        
         updates = getattr(self, '_updates', updates)
         namespace = getattr(self, 'namespace', namespace)
         namespace = namespace or globals()
         namespace.update(updates)
         self.namespace = namespace
         return namespace
+    
+    def squash_name_error(self, name:str, default: Optional[Any] = None) -> 'BaseImp':
+        namespace = getattr(self, 'namespace', None)
+        namespace = namespace or globals()
+        
+        update = dict()
+        update[name] = namespace.get(name, default)
+
+        namespace.update(update)
+        self.namespace = namespace
+        return self
 
 # %% ../nbs/00_core.ipynb 20
 @dataclass
 class ImpSubSpec(BaseImp):
     """
     A class to represent a sub-specification of the import.
 
@@ -544,15 +555,15 @@
         -------
         VariableDict
             A dictionary mapping the names of the items to their updated values.
         """
         # print('get_updates')
         updates = self.fetch()
         # print('get_updates', updates)
-        updates = self.make_updates_failsafe(updates)
+        updates = self.give_updates_fallbacks(updates)
         # print('get_updates > failsafed', updates)
         self._updates = updates
         return updates
     
     def update_globals(self):
         """
         Updates the global namespace with the fetched updates.
@@ -561,14 +572,25 @@
         -------
         self : 'ImpSubSpec'
             The current instance of the ImpSubSpec.
         """
         updates = self.get_updates()
         self.update_namespace(updates, self.namespace)     
         return self
+    
+    def expected_items(self) -> List[str]:
+        """
+        Returns a list of expected names for the import.
+
+        Returns
+        -------
+        List[str]
+            A list of expected names for the import.
+        """
+        return [imp_item.varname for imp_item in self.items]    
 
 # %% ../nbs/00_core.ipynb 25
 @dataclass
 class ImpSpec(ModuleSpec, BaseImp):
     """
     A class to represent an import specification.
 
@@ -633,14 +655,31 @@
         # print('updates', updates, 'fallbacks', self.fallbacks.items())
         updates = self.fallbacks.give(updates)
         # print('updates', updates, 'fallbacks', self.fallbacks.items())
         
         self._updates = updates
         self.update_namespace(updates, self.namespace)
         return updates
+    
+    def _import(self) -> VariableDict:
+        self._imp_main()
+        updates = self._imp_subs()
+        self._updates = updates
+        self.update_namespace(updates, self.namespace)
+        return updates
+    
+    def all_expected_items(self):
+        expected_items = []
+        for subspec in self.subspecs:
+            expected_items.extend(subspec.expected_items())
+        return expected_items
+    
+    def squash_all_name_errors(self):
+        for name in self.all_expected_items():
+            self.squash_name_error(name)        
 
 # %% ../nbs/00_core.ipynb 27
 @dataclass
 class Imp(BaseImp):
     """
     Import Module class.
     
@@ -686,19 +725,17 @@
 
     _ : KW_ONLY
     _module: Module = field(init=False, repr=False, default=None)
     _spec: ImpSpec = field(init=False, repr=False, default=None)
 
     def load(self):
         self._spec = ImpSpec(self.name, self.nick, self.lazy, self.subspecs, self.fallbacks)
-        self._spec._imp_main()
-        updates = self._spec._imp_subs()
         self._module = sys.modules[self.name]
-        self._updates = updates
-        self.update_namespace(updates, self.namespace)
+        self._updates = self._spec._import()                 
+        self.update_namespace(self._updates, self.namespace)
 
     def __post_init__(self):
         if isinstance(self.fallbacks, dict):
             self.fallbacks = Fallbacks.from_dict(self.fallbacks)
             
         if not self.delay:
             self.load()
@@ -744,7 +781,9 @@
         Returns
         -------
         Any
             The attribute from the imported module.
         """
         return getattr(self._module, key, None)
 
+
+
```

### Comparing `ipos-0.0.6/ipos.egg-info/PKG-INFO` & `ipos-0.0.7/ipos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipos
-Version: 0.0.6
+Version: 0.0.7
 Summary: a devilish import package
 Home-page: https://github.com/dsm-72/ipos
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipos-0.0.6/settings.ini` & `ipos-0.0.7/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = ipos
 lib_name = ipos
-version = 0.0.6
+version = 0.0.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = ipos
 nbs_path = nbs
 recursive = True
```

### Comparing `ipos-0.0.6/setup.py` & `ipos-0.0.7/setup.py`

 * *Files identical despite different names*

