# Comparing `tmp/pyodb-0.1.2.tar.gz` & `tmp/pyodb-0.1.3.tar.gz`

## Comparing `pyodb-0.1.2.tar` & `pyodb-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 pyodb-0.1.2/.coveragerc
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pyodb-0.1.2/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 pyodb-0.1.2/CHANGELOG.md
--rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 pyodb-0.1.2/MANIFEST.in
--rwxr-xr-x   0        0        0     2776 2020-02-02 00:00:00.000000 pyodb-0.1.2/environment.yaml
--rwxr-xr-x   0        0        0     7206 2020-02-02 00:00:00.000000 pyodb-0.1.2/performance.ipynb
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 pyodb-0.1.2/requirements.txt
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 pyodb-0.1.2/tox.ini
--rwxr-xr-x   0        0        0     1221 2020-02-02 00:00:00.000000 pyodb-0.1.2/.github/workflows/python-package.yml
--rwxr-xr-x   0        0        0     2882 2020-02-02 00:00:00.000000 pyodb-0.1.2/docs/PyODBCacheExamples.md
--rwxr-xr-x   0        0        0     5905 2020-02-02 00:00:00.000000 pyodb-0.1.2/docs/PyODBExamples.md
--rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 pyodb-0.1.2/docs/conversion_example.puml
--rwxr-xr-x   0        0        0     7088 2020-02-02 00:00:00.000000 pyodb-0.1.2/docs/img/Logo.svg
--rwxr-xr-x   0        0        0    25699 2020-02-02 00:00:00.000000 pyodb-0.1.2/docs/img/conversion_example.svg
--rwxr-xr-x   0        0        0     1962 2020-02-02 00:00:00.000000 pyodb-0.1.2/scripts/activate.sh
--rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 pyodb-0.1.2/scripts/deactivate.sh
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/__init__.py
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/__init__.py
--rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/_util.py
--rwxr-xr-x   0        0        0      855 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/error.py
--rwxr-xr-x   0        0        0    12732 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/pyodb.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/__init__.py
--rwxr-xr-x   0        0        0    12188 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/_base_schema.py
--rwxr-xr-x   0        0        0     1634 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/shard_schema.py
--rwxr-xr-x   0        0        0     1398 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/unified_schema.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/base/__init__.py
--rwxr-xr-x   0        0        0     9414 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/base/_operators.py
--rwxr-xr-x   0        0        0    19128 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/base/_sql_builders.py
--rwxr-xr-x   0        0        0     5006 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/base/_table.py
--rwxr-xr-x   0        0        0      973 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/base/_type_defs.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/__init__.py
--rwxr-xr-x   0        0        0    10884 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/pyodb_test.py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/util_test.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/__init__.py
--rwxr-xr-x   0        0        0     6535 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/base_schema_test.py
--rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/shard_schema_test.py
--rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/unified_schema_test.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/base/__init__.py
--rwxr-xr-x   0        0        0     3388 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/base/operators_test.py
--rwxr-xr-x   0        0        0     7777 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/base/sql_builders_test.py
--rwxr-xr-x   0        0        0     1589 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/base/table_test.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/test_models/__init__.py
--rwxr-xr-x   0        0        0     2635 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/test_models/complex_models.py
--rwxr-xr-x   0        0        0     2135 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/test_models/high_complex_models.py
--rwxr-xr-x   0        0        0     4821 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/test_models/primitive_models.py
--rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 pyodb-0.1.2/.gitignore
--rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 pyodb-0.1.2/LICENSE
--rwxr-xr-x   0        0        0     9337 2020-02-02 00:00:00.000000 pyodb-0.1.2/README.md
--rwxr-xr-x   0        0        0     1889 2020-02-02 00:00:00.000000 pyodb-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    11302 2020-02-02 00:00:00.000000 pyodb-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 pyodb-0.1.3/.coveragerc
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pyodb-0.1.3/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 pyodb-0.1.3/CHANGELOG.md
+-rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 pyodb-0.1.3/MANIFEST.in
+-rwxr-xr-x   0        0        0     3382 2020-02-02 00:00:00.000000 pyodb-0.1.3/environment.yaml
+-rwxr-xr-x   0        0        0    10118 2020-02-02 00:00:00.000000 pyodb-0.1.3/performance.ipynb
+-rwxr-xr-x   0        0        0     1496 2020-02-02 00:00:00.000000 pyodb-0.1.3/requirements.txt
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 pyodb-0.1.3/tox.ini
+-rwxr-xr-x   0        0        0     1221 2020-02-02 00:00:00.000000 pyodb-0.1.3/.github/workflows/python-package.yml
+-rwxr-xr-x   0        0        0     2882 2020-02-02 00:00:00.000000 pyodb-0.1.3/docs/PyODBCacheExamples.md
+-rwxr-xr-x   0        0        0     5905 2020-02-02 00:00:00.000000 pyodb-0.1.3/docs/PyODBExamples.md
+-rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 pyodb-0.1.3/docs/conversion_example.puml
+-rwxr-xr-x   0        0        0     7088 2020-02-02 00:00:00.000000 pyodb-0.1.3/docs/img/Logo.svg
+-rwxr-xr-x   0        0        0    25699 2020-02-02 00:00:00.000000 pyodb-0.1.3/docs/img/conversion_example.svg
+-rwxr-xr-x   0        0        0     1962 2020-02-02 00:00:00.000000 pyodb-0.1.3/scripts/activate.sh
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 pyodb-0.1.3/scripts/deactivate.sh
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/__init__.py
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/__init__.py
+-rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/_util.py
+-rwxr-xr-x   0        0        0      855 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/error.py
+-rwxr-xr-x   0        0        0    12729 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/pyodb.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/schema/__init__.py
+-rwxr-xr-x   0        0        0    12188 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/schema/_base_schema.py
+-rwxr-xr-x   0        0        0     1634 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/schema/shard_schema.py
+-rwxr-xr-x   0        0        0     1398 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/schema/unified_schema.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/schema/base/__init__.py
+-rwxr-xr-x   0        0        0     9424 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/schema/base/_operators.py
+-rwxr-xr-x   0        0        0    19135 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/schema/base/_sql_builders.py
+-rwxr-xr-x   0        0        0     5008 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/schema/base/_table.py
+-rwxr-xr-x   0        0        0      973 2020-02-02 00:00:00.000000 pyodb-0.1.3/src/pyodb/schema/base/_type_defs.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/__init__.py
+-rwxr-xr-x   0        0        0    11350 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/pyodb_test.py
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/util_test.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/schema/__init__.py
+-rwxr-xr-x   0        0        0     6535 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/schema/base_schema_test.py
+-rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/schema/shard_schema_test.py
+-rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/schema/unified_schema_test.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/schema/base/__init__.py
+-rwxr-xr-x   0        0        0     4638 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/schema/base/operators_test.py
+-rwxr-xr-x   0        0        0     7777 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/schema/base/sql_builders_test.py
+-rwxr-xr-x   0        0        0     1589 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/pyodb/schema/base/table_test.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/test_models/__init__.py
+-rwxr-xr-x   0        0        0     2914 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/test_models/complex_models.py
+-rwxr-xr-x   0        0        0     2508 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/test_models/high_complex_models.py
+-rwxr-xr-x   0        0        0     5172 2020-02-02 00:00:00.000000 pyodb-0.1.3/test/test_models/primitive_models.py
+-rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 pyodb-0.1.3/.gitignore
+-rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 pyodb-0.1.3/LICENSE
+-rwxr-xr-x   0        0        0     9336 2020-02-02 00:00:00.000000 pyodb-0.1.3/README.md
+-rwxr-xr-x   0        0        0     1889 2020-02-02 00:00:00.000000 pyodb-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    11301 2020-02-02 00:00:00.000000 pyodb-0.1.3/PKG-INFO
```

### Comparing `pyodb-0.1.2/.pre-commit-config.yaml` & `pyodb-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/environment.yaml` & `pyodb-0.1.3/environment.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -61,39 +61,65 @@
   - wcwidth=0.2.6=pyhd8ed1ab_0
   - wheel=0.38.4=py310h06a4308_0
   - xz=5.2.10=h5eee18b_1
   - zeromq=4.3.4=h9c3ff4c_1
   - zlib=1.2.13=h5eee18b_0
   - pip:
     - attrs==22.2.0
+    - bleach==6.0.0
     - build==0.10.0
     - cachetools==5.3.0
+    - cffi==1.15.1
     - cfgv==3.3.1
     - chardet==5.1.0
+    - charset-normalizer==3.1.0
+    - click==8.1.3
     - colorama==0.4.6
     - coverage==7.2.2
+    - cryptography==40.0.1
     - distlib==0.3.6
+    - docutils==0.19
     - exceptiongroup==1.1.1
     - filelock==3.10.0
     - identify==2.5.21
+    - idna==3.4
+    - importlib-metadata==6.3.0
     - iniconfig==2.0.0
+    - jaraco-classes==3.2.3
+    - jeepney==0.8.0
     - jinja2==3.1.2
+    - keyring==23.13.1
     - markdown-it-py==2.2.0
     - markupsafe==2.1.2
     - mdurl==0.1.2
     - memray==1.7.0
+    - more-itertools==9.1.0
     - nodeenv==1.7.0
     - pdoc==13.0.0
+    - pkginfo==1.9.6
     - pluggy==1.0.0
     - pre-commit==3.2.0
+    - pycparser==2.21
+    - pydantic==1.10.9
+    - pyodb==0.1.1
     - pyproject-api==1.5.1
     - pyproject-hooks==1.0.0
     - pytest==7.2.2
     - pytest-cov==4.0.0
     - pyyaml==6.0
+    - readme-renderer==37.3
+    - requests==2.28.2
+    - requests-toolbelt==0.10.1
+    - rfc3986==2.0.0
     - rich==13.3.2
     - ruff==0.0.257
+    - secretstorage==3.3.3
     - snakeviz==2.1.1
-    - tornado==6.3.2
+    - tornado==6.2
     - tox==4.4.8
+    - tqdm==4.65.0
+    - twine==4.0.2
+    - urllib3==1.26.15
     - virtualenv==20.21.0
+    - webencodings==0.5.1
+    - zipp==3.15.0
 prefix: /usr/miniconda3/envs/pyodb
```

### Comparing `pyodb-0.1.2/.github/workflows/python-package.yml` & `pyodb-0.1.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/docs/PyODBCacheExamples.md` & `pyodb-0.1.3/docs/PyODBCacheExamples.md`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/docs/PyODBExamples.md` & `pyodb-0.1.3/docs/PyODBExamples.md`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/docs/conversion_example.puml` & `pyodb-0.1.3/docs/conversion_example.puml`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/docs/img/Logo.svg` & `pyodb-0.1.3/docs/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/docs/img/conversion_example.svg` & `pyodb-0.1.3/docs/img/conversion_example.svg`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/scripts/activate.sh` & `pyodb-0.1.3/scripts/activate.sh`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/scripts/deactivate.sh` & `pyodb-0.1.3/scripts/deactivate.sh`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/src/pyodb/error.py` & `pyodb-0.1.3/src/pyodb/error.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/src/pyodb/pyodb.py` & `pyodb-0.1.3/src/pyodb/pyodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
 
     @property
     def known_types(self) -> list[type]:
         return [type_ for type_ in self._schema._tables.keys() if type_.__name__ != "Table"]
 
 
-    def save_multiple(self, objs: list[object], expires: float | None = None):
+    def save_multiple(self, objs: list[Any], expires: float | None = None):
         """Saves multiple objects to the database. Does not add the type beforehand unlike `save`!
 
         Args:
             obj (list[object]): The objects to save.
             expires (float | None, optional): When the object expires and gets removed from the
                 database. Defaults to None.
         """
```

### Comparing `pyodb-0.1.2/src/pyodb/schema/_base_schema.py` & `pyodb-0.1.3/src/pyodb/schema/_base_schema.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/src/pyodb/schema/shard_schema.py` & `pyodb-0.1.3/src/pyodb/schema/shard_schema.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/src/pyodb/schema/unified_schema.py` & `pyodb-0.1.3/src/pyodb/schema/unified_schema.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/src/pyodb/schema/base/_operators.py` & `pyodb-0.1.3/src/pyodb/schema/base/_operators.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,36 +83,36 @@
         table = tables[base_type]
         objs = []
         subrows: dict[type, dict[str, object]] = {}
         for row in rows:
             obj = object.__new__(base_type)
             for name, type_ in table.members.items():
                 if row[name] is None:
-                    setattr(obj, name, None)
+                    obj.__dict__[name] = None
                     continue
 
                 if isinstance(type_, (GenericAlias, UnionType)):
                     type_ = cls.get_base_type(type_)
 
                 if type_ in PRIMITIVES:
-                    setattr(obj, name, type_(row[name]))
+                    obj.__dict__[name] = type_(row[name])
 
                 elif type_ in CONTAINERS:
-                    setattr(obj, name, pickle.loads(row[name]))
+                    obj.__dict__[name] = pickle.loads(row[name])
 
                 elif isinstance(type_, type):
                     if str(row[name])[:2] == "b'" or str(row[name])[:2] == "b\"":
-                        setattr(obj, name, pickle.loads(row[name]))
+                        obj.__dict__[name] = pickle.loads(row[name])
                         continue
 
                     ttype: type = locate(row[name]) # type: ignore
 
                     if ttype not in subrows:
                         subrows[ttype] = cls._get_sub_rows(tables[ttype], tables, table.fqcn)
-                    setattr(obj, name, subrows[ttype][row["_uid_"]])
+                    obj.__dict__[name] = subrows[ttype][row["_uid_"]]
             if "__odb_reassemble__" in base_type.__dict__:
                 obj.__odb_reassemble__()
             objs += [obj]
         return objs
 
 
     @classmethod
@@ -131,37 +131,37 @@
         Raises:
             DBConnError: In case a sub-table does not have a valid database connection.
         """
         table = tables[base_type]
         obj = object.__new__(base_type)
         for name, type_ in table.members.items():
             if row[name] is None:
-                setattr(obj, name, None)
+                obj.__dict__[name] = None
                 continue
 
             if isinstance(type_, (GenericAlias, UnionType)):
                 type_ = cls.get_base_type(type_)
 
             if type_ in PRIMITIVES:
-                setattr(obj, name, type_(row[name]))
+                obj.__dict__[name] = type_(row[name])
 
             elif type_ in CONTAINERS:
-                setattr(obj, name, pickle.loads(row[name]))
+                obj.__dict__[name] = pickle.loads(row[name])
 
             elif isinstance(type_, type):
                 if str(row[name])[:2] == "b'" or str(row[name])[:2] == "b\"":
-                    setattr(obj, name, pickle.loads(row[name]))
+                    obj.__dict__[name] = pickle.loads(row[name])
                     continue
 
                 ttype: type = locate(row[name]) # type: ignore
                 subtable = tables[ttype]
                 subrow: sql.Row = subtable.dbconn.execute(
                     f"SELECT * FROM \"{subtable.fqcn}\" WHERE _parent_ = '{row['_uid_']}'"
                 ).fetchone()
-                setattr(obj, name, cls.assemble_type(ttype, tables, subrow))
+                obj.__dict__[name] = cls.assemble_type(ttype, tables, subrow)
         if "__odb_reassemble__" in base_type.__dict__:
             obj.__odb_reassemble__()
         return obj
 
 
 class Disassembler:
     sharded = False
```

### Comparing `pyodb-0.1.2/src/pyodb/schema/base/_sql_builders.py` & `pyodb-0.1.3/src/pyodb/schema/base/_sql_builders.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,16 @@
 
         Args:
             dbconn (sql.Connection): A connection to the SQL database.
         """
         insert = f"INSERT INTO \"{self._table_name}\" VALUES("
         insert += "?,"*len(self._vals[0])
         insert = insert[:-1] + ");"
-        dbconn.executemany(insert, self._vals)
-        dbconn.commit()
+        with dbconn as conn:
+            conn.executemany(insert, self._vals)
 
 
     @property
     def vals(self) -> list[tuple]:
         return self._vals
```

### Comparing `pyodb-0.1.2/src/pyodb/schema/base/_table.py` & `pyodb-0.1.3/src/pyodb/schema/base/_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,17 @@
             self.base_path / (self.base_type.__name__ + ".db")
                 if self._sharded
                 else self.base_path / "pyodb.db",
             check_same_thread=True,
             isolation_level="IMMEDIATE"
         )
         try:
-            conn.execute("pragma journal_mode = WAL;")
+            # conn.execute("pragma journal_mode = WAL;")
             conn.execute("pragma synchronous = normal;")
-            conn.execute("pragma page_size = 2048;")
+            conn.execute("pragma page_size = 4096;")
             conn.commit()
         except sql.OperationalError:
             # These pragmas are only for performance
             # They may fail because the database is locked or because they are not supported
             # it is not critical in any case
             print("PyODB WARNING: Could not set database performance pragmas.")
```

### Comparing `pyodb-0.1.2/src/pyodb/schema/base/_type_defs.py` & `pyodb-0.1.3/src/pyodb/schema/base/_type_defs.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/test/pyodb/pyodb_test.py` & `pyodb-0.1.3/test/pyodb/pyodb_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import multiprocessing
 import random
 import threading
 from logging import Logger
 from multiprocessing import Process
-from test.test_models.complex_models import ComplexBasic, ComplexMulti
+from test.test_models.complex_models import ComplexBasic, ComplexMulti, ComplexPydantic
 from test.test_models.high_complex_models import HighComplexL3
-from test.test_models.primitive_models import PrimitiveBasic, PrimitiveContainer
+from test.test_models.primitive_models import PrimitiveBasic, PrimitiveContainer, PrimitivePydantic
 from time import sleep, time
 from unittest import TestCase
 
 from pyodb.error import BadTypeError, CacheError, PyODBError
 from pyodb.pyodb import PyODB, PyODBCache
 
 
@@ -76,33 +76,39 @@
 
 
     def test_persistency(self):
         # Test Shard Schema
         del self.pyodb
         self.pyodb = PyODB(sharding=True)
         self.pyodb.add_type(ComplexBasic)
+        self.pyodb.add_type(ComplexPydantic)
         self.pyodb.persistent = True
         del self.pyodb
 
         self.pyodb = PyODB(sharding=True)
         self.assertIn(ComplexBasic, self.pyodb._schema._tables)
         self.assertIn(PrimitiveBasic, self.pyodb._schema._tables)
         self.assertIn(PrimitiveContainer, self.pyodb._schema._tables)
+        self.assertIn(ComplexPydantic, self.pyodb._schema._tables)
+        self.assertIn(PrimitivePydantic, self.pyodb._schema._tables)
         del self.pyodb
 
         # Test Unified Schema
         self.pyodb = PyODB()
         self.pyodb.persistent = True
         self.pyodb.add_type(ComplexBasic)
+        self.pyodb.add_type(ComplexPydantic)
         del self.pyodb
 
         self.pyodb = PyODB()
         self.assertIn(ComplexBasic, self.pyodb._schema._tables)
         self.assertIn(PrimitiveBasic, self.pyodb._schema._tables)
         self.assertIn(PrimitiveContainer, self.pyodb._schema._tables)
+        self.assertIn(ComplexPydantic, self.pyodb._schema._tables)
+        self.assertIn(PrimitivePydantic, self.pyodb._schema._tables)
         del self.pyodb
 
         self.pyodb = PyODB()
         self.assertEqual(1, len(self.pyodb._schema._tables))
 
 
     def test_expires(self):
@@ -111,21 +117,22 @@
         self.pyodb.save_multiple([PrimitiveBasic() for _ in range(3)], time()+5)
         sleep(2)
 
         self.assertEqual(len(self.pyodb.select(PrimitiveBasic).all()), 3)
 
 
     def test_highly_complex_object(self):
-        self.pyodb.max_depth=2
+        self.pyodb.max_depth=5
         self.pyodb.add_type(HighComplexL3)
         hc = HighComplexL3()
         self.pyodb.save(hc)
         self.pyodb.save_multiple([HighComplexL3() for _ in range(9)])
         res = self.pyodb.select(HighComplexL3).first()
         self.assertEqual(hc, res)
+        self.assertEqual(hc.high1.pyd.child.test_str, "Test Child")
 
 
 class ThreadingTest(TestCase):
     def job(self, sharding: bool, pyodb: PyODB | None = None):
         random.seed = time() - int(time()-0.5)
         if pyodb is None:
             pyodb = PyODB(max_depth=3, persistent=True, sharding=sharding)
```

### Comparing `pyodb-0.1.2/test/pyodb/schema/base_schema_test.py` & `pyodb-0.1.3/test/pyodb/schema/base_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/test/pyodb/schema/shard_schema_test.py` & `pyodb-0.1.3/test/pyodb/schema/shard_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/test/pyodb/schema/unified_schema_test.py` & `pyodb-0.1.3/test/pyodb/schema/unified_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/test/pyodb/schema/base/sql_builders_test.py` & `pyodb-0.1.3/test/pyodb/schema/base/sql_builders_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/test/pyodb/schema/base/table_test.py` & `pyodb-0.1.3/test/pyodb/schema/base/table_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/test/test_models/complex_models.py` & `pyodb-0.1.3/test/test_models/complex_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from random import randint
+
+from pydantic import BaseModel
 from test.test_models.primitive_models import (PrimitiveBasic, PrimitiveContainer,
-                                               PrimitiveIllegal1, get_random_text)
+                                               PrimitiveIllegal1, PrimitivePydantic, get_random_text)
 from typing import Any
 
 
 class ComplexBasic:
     random_number: int
     basic: PrimitiveBasic
     container: PrimitiveContainer
@@ -83,14 +85,26 @@
         return {
             "complex_list":  list | None,
             "complex_dict": dict,
             "multicomplex_dict": dict
         }
 
 
+class ComplexPydantic(BaseModel):
+    child: PrimitivePydantic
+    test_str: str
+
+    @staticmethod
+    def get_members() -> dict:
+        return {
+            "child": PrimitivePydantic,
+            "test_str": str
+        }
+
+
 class ComplexIllegal1:
     illegal: PrimitiveBasic | str
 
 class ComplexIllegal2:
     illegal: PrimitiveIllegal1
 
 class ComplexIllegal3:
```

### Comparing `pyodb-0.1.2/test/test_models/high_complex_models.py` & `pyodb-0.1.3/test/test_models/high_complex_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 from random import randint
-from test.test_models.primitive_models import PrimitiveBasic, get_random_text
+from test.test_models.complex_models import ComplexPydantic
+from test.test_models.primitive_models import PrimitiveBasic, PrimitivePydantic, get_random_text
 
 
 class HighComplexL1:
     random_number: int
     basic: PrimitiveBasic
     basiclist: list[PrimitiveBasic]
     reassembled = False
+    pyd: ComplexPydantic
 
 
     def __odb_reassemble__(self):
         self.reassembled = True
 
 
     def __init__(self) -> None:
         self.random_number = randint(-1000000, 1000000)
         self.basiclist = [PrimitiveBasic() for _ in range(randint(3, 10))]
         self.basic = PrimitiveBasic()
         self.reassembled = False
+        self.pyd = ComplexPydantic(
+            child=PrimitivePydantic(
+                test_bool=False,
+                test_float=9.25,
+                test_str="Test Child",
+                test_number=50
+            ),
+            test_str="Test Parent"
+        )
 
 
     def __eq__(self, __o: object) -> bool:
         if isinstance(__o, HighComplexL1):
             return (
                 self.random_number ==  __o.random_number
                 and self.basic == __o.basic
```

### Comparing `pyodb-0.1.2/test/test_models/primitive_models.py` & `pyodb-0.1.3/test/test_models/primitive_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pydantic import BaseModel
 from random import choice, randint, random
 
 
 def get_random_text(limit: int = 100) -> str:
     allowed_chars = " abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789=!\"§$&/()\\`´\
 #'+*~-_.:,;<>|[]}{^°"
     return "".join(choice(allowed_chars) for _ in range(randint(1, limit)))
@@ -130,14 +131,30 @@
 
     def __eq__(self, __o: object) -> bool:
         if isinstance(__o, PrimitiveContainer):
             return self.listing == __o.listing
         return False
 
 
+class PrimitivePydantic(BaseModel):
+    test_str: str
+    test_float: float
+    test_number: int
+    test_bool: bool
+
+    @staticmethod
+    def get_members() -> dict:
+        return {
+            "test_str": str,
+            "test_float": float,
+            "test_number": int,
+            "test_bool": bool
+        }
+
+
 class ReassemblyTester:
     txt: str
     reassembled: bool
 
     def __init__(self) -> None:
         self.txt = get_random_text(30)
         self.reassembled = False
```

### Comparing `pyodb-0.1.2/.gitignore` & `pyodb-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/LICENSE` & `pyodb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.2/README.md` & `pyodb-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/NeoSecundus/PyODB/python-package.yml)
 [![codecov](https://codecov.io/gh/NeoSecundus/PyODB/branch/main/graph/badge.svg?token=AEXOJTNDWZ)](https://codecov.io/gh/NeoSecundus/PyODB)
 ![Open Issues](https://img.shields.io/github/issues-raw/NeoSecundus/PyODB)
 ![Closed Issues](https://img.shields.io/github/issues-closed-raw/NeoSecundus/PyODB)
 ![PyPI Version](https://img.shields.io/pypi/v/pyodb?color=%23a08)
 ![Supported Python Versions](https://img.shields.io/badge/Python%20Versions-3.10+-48f)
 
-
 <img src="docs/img/Logo.svg" style="margin: auto; width: 20vh" />
 
 Python Object DataBase (PyODB) is a SQLite3 ORM library aiming to be as simple to use as possible.
 This library is supposed to be used for testing, in small projects, when wanting to export complex
 python data in a well structured format or for local inter-process data caching.
 
 **Basics:**
```

### Comparing `pyodb-0.1.2/pyproject.toml` & `pyodb-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyodb"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Nikolas Teuschl", email="nikolas.teuschl@alpha-origin.biz" },
 ]
 description = "Python Object DataBase (PyODB) is an ORM library aiming to be as simple to use as possible."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pyodb-0.1.2/PKG-INFO` & `pyodb-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodb
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Object DataBase (PyODB) is an ORM library aiming to be as simple to use as possible.
 Project-URL: Homepage, https://github.com/NeoSecundus/PyODB
 Project-URL: Bug Tracker, https://github.com/NeoSecundus/PyODB/issues
 Project-URL: Changelog, https://github.com/NeoSecundus/PyODB/blob/main/CHANGELOG.md
 Author-email: Nikolas Teuschl <nikolas.teuschl@alpha-origin.biz>
 License: MIT License
         
@@ -40,15 +40,14 @@
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/NeoSecundus/PyODB/python-package.yml)
 [![codecov](https://codecov.io/gh/NeoSecundus/PyODB/branch/main/graph/badge.svg?token=AEXOJTNDWZ)](https://codecov.io/gh/NeoSecundus/PyODB)
 ![Open Issues](https://img.shields.io/github/issues-raw/NeoSecundus/PyODB)
 ![Closed Issues](https://img.shields.io/github/issues-closed-raw/NeoSecundus/PyODB)
 ![PyPI Version](https://img.shields.io/pypi/v/pyodb?color=%23a08)
 ![Supported Python Versions](https://img.shields.io/badge/Python%20Versions-3.10+-48f)
 
-
 <img src="docs/img/Logo.svg" style="margin: auto; width: 20vh" />
 
 Python Object DataBase (PyODB) is a SQLite3 ORM library aiming to be as simple to use as possible.
 This library is supposed to be used for testing, in small projects, when wanting to export complex
 python data in a well structured format or for local inter-process data caching.
 
 **Basics:**
```

