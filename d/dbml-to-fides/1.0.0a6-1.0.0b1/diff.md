# Comparing `tmp/dbml-to-fides-1.0.0a6.tar.gz` & `tmp/dbml-to-fides-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbml-to-fides-1.0.0a6.tar", last modified: Tue May 23 13:09:51 2023, max compression
+gzip compressed data, was "dbml-to-fides-1.0.0b1.tar", last modified: Tue Jun 27 13:11:20 2023, max compression
```

## Comparing `dbml-to-fides-1.0.0a6.tar` & `dbml-to-fides-1.0.0b1.tar`

### file list

```diff
@@ -1,19 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:51.272218 dbml-to-fides-1.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-23 13:09:42.000000 dbml-to-fides-1.0.0a6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-05-23 13:09:51.272218 dbml-to-fides-1.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-23 13:09:42.000000 dbml-to-fides-1.0.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:51.272218 dbml-to-fides-1.0.0a6/dbml_to_fides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:42.000000 dbml-to-fides-1.0.0a6/dbml_to_fides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-23 13:09:42.000000 dbml-to-fides-1.0.0a6/dbml_to_fides/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-23 13:09:42.000000 dbml-to-fides-1.0.0a6/dbml_to_fides/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:51.272218 dbml-to-fides-1.0.0a6/dbml_to_fides.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-05-23 13:09:51.000000 dbml-to-fides-1.0.0a6/dbml_to_fides.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 13:09:51.000000 dbml-to-fides-1.0.0a6/dbml_to_fides.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:09:51.000000 dbml-to-fides-1.0.0a6/dbml_to_fides.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 13:09:51.000000 dbml-to-fides-1.0.0a6/dbml_to_fides.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 13:09:51.000000 dbml-to-fides-1.0.0a6/dbml_to_fides.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 13:09:51.000000 dbml-to-fides-1.0.0a6/dbml_to_fides.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-23 13:09:42.000000 dbml-to-fides-1.0.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:09:51.272218 dbml-to-fides-1.0.0a6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:51.272218 dbml-to-fides-1.0.0a6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-23 13:09:42.000000 dbml-to-fides-1.0.0a6/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:20.686594 dbml-to-fides-1.0.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:20.682593 dbml-to-fides-1.0.0b1/.fides/
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/.fides/sample_dataset.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:20.682593 dbml-to-fides-1.0.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:20.682593 dbml-to-fides-1.0.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-06-27 13:11:20.686594 dbml-to-fides-1.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:20.686594 dbml-to-fides-1.0.0b1/dbml_to_fides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/dbml_to_fides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/dbml_to_fides/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/dbml_to_fides/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:20.686594 dbml-to-fides-1.0.0b1/dbml_to_fides.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-06-27 13:11:20.000000 dbml-to-fides-1.0.0b1/dbml_to_fides.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-27 13:11:20.000000 dbml-to-fides-1.0.0b1/dbml_to_fides.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:11:20.000000 dbml-to-fides-1.0.0b1/dbml_to_fides.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-27 13:11:20.000000 dbml-to-fides-1.0.0b1/dbml_to_fides.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 13:11:20.000000 dbml-to-fides-1.0.0b1/dbml_to_fides.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 13:11:20.000000 dbml-to-fides-1.0.0b1/dbml_to_fides.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/sample.dbml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:11:20.686594 dbml-to-fides-1.0.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:20.686594 dbml-to-fides-1.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:11:20.686594 dbml-to-fides-1.0.0b1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/tests/data/demo_dataset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    96617 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/tests/data/fides_db_dataset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/tests/data/fides_redis_dataset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/tests/data/sample.dbml
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/tests/data/sample_dataset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/tests/data/schema_def.dbml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/tests/data/schema_def_dataset_min.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 13:11:10.000000 dbml-to-fides-1.0.0b1/tox.ini
```

### Comparing `dbml-to-fides-1.0.0a6/LICENSE.txt` & `dbml-to-fides-1.0.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbml-to-fides-1.0.0a6/PKG-INFO` & `dbml-to-fides-1.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbml-to-fides
-Version: 1.0.0a6
+Version: 1.0.0b1
 Summary: Interoperatbility for DBML and Fides dataset manifests
 Author-email: Ee Durbin <ee.opensource@pyfound.org>
 License: Copyright 2023 Ee Durbin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `dbml-to-fides-1.0.0a6/README.md` & `dbml-to-fides-1.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `dbml-to-fides-1.0.0a6/dbml_to_fides/cli.py` & `dbml-to-fides-1.0.0b1/dbml_to_fides/cli.py`

 * *Files identical despite different names*

### Comparing `dbml-to-fides-1.0.0a6/dbml_to_fides/transform.py` & `dbml-to-fides-1.0.0b1/dbml_to_fides/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,17 @@
     _new = unlistify(new)
 
     updated = always_merger.merge(_existing, _new)
 
     return relistify(updated)
 
 
-def dbml_to_fides_dataset_dict(dbml: Database, include_fides_keys: bool = False) -> Dict:
+def dbml_to_fides_dataset_dict(
+    dbml: Database, include_fides_keys: bool = False
+) -> Dict:
     collections = defaultdict(list)
     for table in dbml.tables:
         collection = {**(deepcopy(collection_keys) if include_fides_keys else {})}
 
         collection["name"] = table.name
         if table.note:
             collection["description"] = str(table.note)
```

### Comparing `dbml-to-fides-1.0.0a6/dbml_to_fides.egg-info/PKG-INFO` & `dbml-to-fides-1.0.0b1/dbml_to_fides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbml-to-fides
-Version: 1.0.0a6
+Version: 1.0.0b1
 Summary: Interoperatbility for DBML and Fides dataset manifests
 Author-email: Ee Durbin <ee.opensource@pyfound.org>
 License: Copyright 2023 Ee Durbin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `dbml-to-fides-1.0.0a6/pyproject.toml` & `dbml-to-fides-1.0.0b1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbml-to-fides"
-version = "1.0.0a6"
+dynamic = ["version"]
 description = "Interoperatbility for DBML and Fides dataset manifests"
 
 readme = "README.md"
 requires-python = ">=3.8, <4"
 license = {file = "LICENSE.txt"}
 
 keywords = ["fides", "dbml"]
@@ -28,22 +28,23 @@
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [ # Optional
   "click",
   "deepmerge",
   "fideslang",
-  "pydbml",
+  "pydbml>=1.0.9,<2.0",
   "pyaml",
-  "typing_extensions<4.6.0",
 ]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/ewdurbin/dbml-to-fides"
 "Source" = "https://github.com/ewdurbin/dbml-to-fides"
 
 [project.scripts]  # Optional
 dbml-to-fides = "dbml_to_fides.cli:transform_and_merge"
 
 [build-system]
-requires = ["setuptools>=43.0.0", "wheel"]
+requires = ["setuptools>=43.0.0", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools_scm]
```

### Comparing `dbml-to-fides-1.0.0a6/tests/test_transforms.py` & `dbml-to-fides-1.0.0b1/tests/test_transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     assert manifest == relistify(unlistify(manifest))
 
 
 @pytest.mark.parametrize(
     ("dataset_file", "dbml_file"),
     [
         ("tests/data/sample_dataset.yml", "tests/data/sample.dbml"),
+        ("tests/data/schema_def_dataset_min.yml", "tests/data/schema_def.dbml"),
     ],
 )
 def test_merge(dataset_file, dbml_file):
     manifest = ingest_manifests(dataset_file)
     dbml = PyDBML(open(dbml_file, "r").read())
 
     assert manifest == merge_fides_dataset_dicts(
```

