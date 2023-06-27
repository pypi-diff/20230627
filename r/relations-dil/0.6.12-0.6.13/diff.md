# Comparing `tmp/relations-dil-0.6.12.tar.gz` & `tmp/relations-dil-0.6.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/service/dist/.tmp-tdtn4pmd/relations-dil-0.6.12.tar", last modified: Fri Nov 25 17:27:34 2022, max compression
+gzip compressed data, was "/opt/service/dist/.tmp-hkzvlsil/relations-dil-0.6.13.tar", last modified: Tue Jun 27 17:07:51 2023, max compression
```

## Comparing `relations-dil-0.6.12.tar` & `relations-dil-0.6.13.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 17:27:34.016050 relations-dil-0.6.12/
--rw-r--r--   0 root         (0) root         (0)     1066 2022-08-05 17:35:15.000000 relations-dil-0.6.12/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3315 2022-11-25 17:27:34.015050 relations-dil-0.6.12/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2976 2022-08-05 17:35:15.000000 relations-dil-0.6.12/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 17:27:33.865050 relations-dil-0.6.12/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 17:27:33.930050 relations-dil-0.6.12/lib/relations/
--rw-r--r--   0 root         (0) root         (0)     1175 2022-02-17 16:06:06.000000 relations-dil-0.6.12/lib/relations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17733 2022-11-25 17:26:14.000000 relations-dil-0.6.12/lib/relations/field.py
--rw-r--r--   0 root         (0) root         (0)     8368 2022-03-14 16:04:33.000000 relations-dil-0.6.12/lib/relations/migrations.py
--rw-r--r--   0 root         (0) root         (0)    32824 2022-11-25 17:26:14.000000 relations-dil-0.6.12/lib/relations/model.py
--rw-r--r--   0 root         (0) root         (0)     6847 2022-11-25 17:26:14.000000 relations-dil-0.6.12/lib/relations/record.py
--rw-r--r--   0 root         (0) root         (0)     2601 2021-11-21 01:21:03.000000 relations-dil-0.6.12/lib/relations/relation.py
--rw-r--r--   0 root         (0) root         (0)     6012 2022-02-17 15:58:52.000000 relations-dil-0.6.12/lib/relations/source.py
--rw-r--r--   0 root         (0) root         (0)     2391 2022-11-25 17:26:14.000000 relations-dil-0.6.12/lib/relations/titles.py
--rw-r--r--   0 root         (0) root         (0)    19602 2022-11-25 17:26:14.000000 relations-dil-0.6.12/lib/relations/unittest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 17:27:34.009050 relations-dil-0.6.12/lib/relations_dil.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3315 2022-11-25 17:27:33.000000 relations-dil-0.6.12/lib/relations_dil.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      458 2022-11-25 17:27:33.000000 relations-dil-0.6.12/lib/relations_dil.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-25 17:27:33.000000 relations-dil-0.6.12/lib/relations_dil.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-25 17:27:33.000000 relations-dil-0.6.12/lib/relations_dil.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-11-25 17:27:33.000000 relations-dil-0.6.12/lib/relations_dil.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-25 17:27:34.016050 relations-dil-0.6.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      934 2022-11-25 17:26:14.000000 relations-dil-0.6.12/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 17:07:51.709305 relations-dil-0.6.13/
+-rw-r--r--   0 root         (0) root         (0)     1066 2022-08-05 17:35:15.000000 relations-dil-0.6.13/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-27 17:07:51.709305 relations-dil-0.6.13/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2976 2022-08-05 17:35:15.000000 relations-dil-0.6.13/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 17:07:51.656305 relations-dil-0.6.13/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 17:07:51.691305 relations-dil-0.6.13/lib/relations/
+-rw-r--r--   0 root         (0) root         (0)     1175 2022-02-17 16:06:06.000000 relations-dil-0.6.13/lib/relations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17733 2022-11-25 17:26:14.000000 relations-dil-0.6.13/lib/relations/field.py
+-rw-r--r--   0 root         (0) root         (0)     8368 2022-03-14 16:04:33.000000 relations-dil-0.6.13/lib/relations/migrations.py
+-rw-r--r--   0 root         (0) root         (0)    32824 2022-11-25 17:26:14.000000 relations-dil-0.6.13/lib/relations/model.py
+-rw-r--r--   0 root         (0) root         (0)     6847 2022-11-25 17:26:14.000000 relations-dil-0.6.13/lib/relations/record.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2021-11-21 01:21:03.000000 relations-dil-0.6.13/lib/relations/relation.py
+-rw-r--r--   0 root         (0) root         (0)     6012 2022-02-17 15:58:52.000000 relations-dil-0.6.13/lib/relations/source.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2022-11-25 17:26:14.000000 relations-dil-0.6.13/lib/relations/titles.py
+-rw-r--r--   0 root         (0) root         (0)    21731 2023-06-27 17:06:43.000000 relations-dil-0.6.13/lib/relations/unittest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 17:07:51.706305 relations-dil-0.6.13/lib/relations_dil.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-27 17:07:51.000000 relations-dil-0.6.13/lib/relations_dil.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-27 17:07:51.000000 relations-dil-0.6.13/lib/relations_dil.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 17:07:51.000000 relations-dil-0.6.13/lib/relations_dil.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-27 17:07:51.000000 relations-dil-0.6.13/lib/relations_dil.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-27 17:07:51.000000 relations-dil-0.6.13/lib/relations_dil.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 17:07:51.709305 relations-dil-0.6.13/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      934 2023-06-27 17:06:43.000000 relations-dil-0.6.13/setup.py
```

### Comparing `relations-dil-0.6.12/LICENSE.txt` & `relations-dil-0.6.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `relations-dil-0.6.12/PKG-INFO` & `relations-dil-0.6.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relations-dil
-Version: 0.6.12
+Version: 0.6.13
 Home-page: https://github.com/relations-dil/python-relations
 Author: Gaffer Fitch
 Author-email: relations@gaf3.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `relations-dil-0.6.12/README.md` & `relations-dil-0.6.13/README.md`

 * *Files identical despite different names*

### Comparing `relations-dil-0.6.12/lib/relations/__init__.py` & `relations-dil-0.6.13/lib/relations/__init__.py`

 * *Files identical despite different names*

### Comparing `relations-dil-0.6.12/lib/relations/field.py` & `relations-dil-0.6.13/lib/relations/field.py`

 * *Files identical despite different names*

### Comparing `relations-dil-0.6.12/lib/relations/migrations.py` & `relations-dil-0.6.13/lib/relations/migrations.py`

 * *Files identical despite different names*

### Comparing `relations-dil-0.6.12/lib/relations/model.py` & `relations-dil-0.6.13/lib/relations/model.py`

 * *Files identical despite different names*

### Comparing `relations-dil-0.6.12/lib/relations/record.py` & `relations-dil-0.6.13/lib/relations/record.py`

 * *Files identical despite different names*

### Comparing `relations-dil-0.6.12/lib/relations/relation.py` & `relations-dil-0.6.13/lib/relations/relation.py`

 * *Files identical despite different names*

### Comparing `relations-dil-0.6.12/lib/relations/source.py` & `relations-dil-0.6.13/lib/relations/source.py`

 * *Files identical despite different names*

### Comparing `relations-dil-0.6.12/lib/relations/titles.py` & `relations-dil-0.6.13/lib/relations/titles.py`

 * *Files identical despite different names*

### Comparing `relations-dil-0.6.12/lib/relations/unittest.py` & `relations-dil-0.6.13/lib/relations/unittest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Unittest Tools for Relations
 """
 
-# pylint: disable=unused-argument,arguments-differ,too-many-public-methods,invalid-name
+# pylint: disable=unused-argument,arguments-differ,too-many-public-methods,invalid-name,not-callable
 
 import glob
 import copy
 import json
 import unittest
 import overscore
 import relations
@@ -44,34 +44,42 @@
     SELECT = MockQuery
     INSERT = MockQuery
     UPDATE = MockQuery
     DELETE = MockQuery
 
     ids = None  # ID's keyed by model names
     data = None # Data keyed by model names
+    unique = None # Unqiues keyed by model names
     migrations = None # Migrations applied so far
 
+    transaction = None # Whether there's a current transaction for rollbacks
+
     def __init__(self, name, **kwargs):
 
         self.ids = {}
         self.data = {}
+        self.unique = {}
         self.migrations = None
 
     def init(self, model):
         """
         Init the model
         """
 
         self.record_init(model._fields)
 
         # Even models without ids will have id's internally
         # They just won't be set in the model
 
         self.ids.setdefault(model.NAME, 0)
         self.data.setdefault(model.NAME, {})
+        self.unique.setdefault(model.NAME, {})
+
+        for unique in model._unique:
+            self.unique[model.NAME].setdefault(unique, {})
 
         if model._id is not None and model._fields._names[model._id].auto is None:
             model._fields._names[model._id].auto = True
 
     def field_define(self, field, definitions):
         """
         define the field
@@ -147,32 +155,83 @@
 
         for extracting in [field for field in model._fields._order if field.extract]:
             for extract in extracting.extract:
                 values[f"{extracting.store}__{extract}"] = overscore.get(values.get(extracting.store), extract)
 
         return values
 
+    class UniqueError(relations.model.ModelError):
+        """
+        Exception for vilating unique constraints
+        """
+
+    def rollback(func): # pylint: disable=no-self-argument
+        """
+        Decorator for rolling back a bad transaction
+        """
+
+        def wrapper(self, *args, **kwargs):
+            """
+            Wrapper for rolling back a bad transaction
+            """
+
+            if self.transaction is None:
+
+                self.transaction = (self.ids, self.data, self.unique)
+
+                try:
+
+                    result = func(self, *args, **kwargs)
+
+                except self.UniqueError as exception:
+
+                    (self.ids, self.data, self.unique) = self.transaction
+                    self.transaction = None
+                    raise exception
+
+                self.transaction = None
+                return result
+
+            return func(self, *args, **kwargs)
+
+        return wrapper
+
+    def uniques(self, model, values, id):
+        """
+        Checks unique constraints
+        """
+
+        for unique, fields in model._unique.items():
+            value = json.dumps({field: overscore.get(values, field) for field in fields}, sort_keys=True)
+            for key, exists in self.unique[model.NAME][unique].items():
+                if value == exists and id != key:
+                    raise self.UniqueError(model, f"value {value} violates unique {unique}")
+            self.unique[model.NAME][unique][id] = value
+
     def create_query(self, model):
         """
         create query
         """
 
         return self.INSERT("CREATE")
 
+    @rollback
     def create(self, model):
         """
         Executes the create
         """
 
         for creating in model._each("create"):
 
             values = creating._record.create({})
 
             self.ids[model.NAME] += 1
 
+            self.uniques(model, values, self.ids[model.NAME])
+
             if model._id is not None and values.get(model._id) is None:
                 values[model._fields._names[model._id].store] = self.ids[model.NAME]
                 creating[model._id] = self.ids[model.NAME]
 
             self.data[model.NAME][self.ids[model.NAME]] = self.extract(creating, values)
 
             if not model._bulk:
@@ -338,37 +397,40 @@
     def update_query(self, model):
         """
         update query
         """
 
         return self.UPDATE("UPDATE")
 
+    @rollback
     def update(self, model):
         """
         Executes the update
         """
 
         updated = 0
 
         # If the overall model is retrieving and the record has values set
 
         if model._action == "retrieve" and model._record._action == "update":
 
             values = model._record.mass({})
 
-            for data in self.data[model.NAME].values():
+            for id, data in self.data[model.NAME].items():
                 if model._record.retrieve(data):
                     updated += 1
+                    self.uniques(model, {**data, **values}, id)
                     data.update(self.extract(model, copy.deepcopy(values)))
 
         elif model._id:
 
             for updating in model._each("update"):
-
-                self.data[model.NAME][updating[model._id]].update(self.extract(updating, updating._record.update({})))
+                data = self.extract(updating, updating._record.update({}))
+                self.uniques(model, data, updating[model._id])
+                self.data[model.NAME][updating[model._id]].update(data)
 
                 updated += 1
 
                 for parent_child in updating.CHILDREN:
                     if updating._children.get(parent_child):
                         updating._children[parent_child].create().update()
 
@@ -407,16 +469,20 @@
             model._action = "create"
 
         else:
 
             raise relations.model.ModelError(model, "nothing to delete from")
 
         for id in ids:
+
             del self.data[model.NAME][id]
 
+            for unique in model._unique:
+                del self.unique[model.NAME][unique][id]
+
         return len(ids)
 
     def definition(self, file_path, source_path):
         """"
         Converts a definition file to a source definition file
         """
```

### Comparing `relations-dil-0.6.12/lib/relations_dil.egg-info/PKG-INFO` & `relations-dil-0.6.13/lib/relations_dil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relations-dil
-Version: 0.6.12
+Version: 0.6.13
 Home-page: https://github.com/relations-dil/python-relations
 Author: Gaffer Fitch
 Author-email: relations@gaf3.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `relations-dil-0.6.12/setup.py` & `relations-dil-0.6.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="relations-dil",
-    version="0.6.12",
+    version="0.6.13",
     package_dir = {'': 'lib'},
     py_modules = [
         'relations',
         'relations.source',
         'relations.unittest',
         'relations.field',
         'relations.titles',
```

