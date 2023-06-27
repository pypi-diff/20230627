# Comparing `tmp/delphai_fastapi-0.1.2.tar.gz` & `tmp/delphai_fastapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_fastapi-0.1.2.tar", max compression
+gzip compressed data, was "delphai_fastapi-0.1.3.tar", max compression
```

## Comparing `delphai_fastapi-0.1.2.tar` & `delphai_fastapi-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/__init__.py
--rw-r--r--   0        0        0     2521 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/app.py
--rw-r--r--   0        0        0     3173 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/auth.py
--rw-r--r--   0        0        0        0 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/companies/__init__.py
--rw-r--r--   0        0        0     3266 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/companies/models.py
--rw-r--r--   0        0        0      375 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/decorators.py
--rw-r--r--   0        0        0     1619 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/models.py
--rw-r--r--   0        0        0     1342 2023-06-26 08:29:07.579788 delphai_fastapi-0.1.2/delphai_fastapi/types.py
--rw-r--r--   0        0        0      476 2023-06-26 08:29:49.876780 delphai_fastapi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.2/setup.py
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-27 12:48:11.860489 delphai_fastapi-0.1.3/delphai_fastapi/__init__.py
+-rw-r--r--   0        0        0     2521 2023-06-27 12:48:11.860489 delphai_fastapi-0.1.3/delphai_fastapi/app.py
+-rw-r--r--   0        0        0     3173 2023-06-27 12:48:11.860489 delphai_fastapi-0.1.3/delphai_fastapi/auth.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:48:11.860489 delphai_fastapi-0.1.3/delphai_fastapi/companies/__init__.py
+-rw-r--r--   0        0        0     3266 2023-06-27 12:48:11.860489 delphai_fastapi-0.1.3/delphai_fastapi/companies/models.py
+-rw-r--r--   0        0        0      375 2023-06-27 12:48:11.860489 delphai_fastapi-0.1.3/delphai_fastapi/decorators.py
+-rw-r--r--   0        0        0     1619 2023-06-27 12:48:11.864489 delphai_fastapi-0.1.3/delphai_fastapi/models.py
+-rw-r--r--   0        0        0     1342 2023-06-27 12:48:11.864489 delphai_fastapi-0.1.3/delphai_fastapi/types.py
+-rw-r--r--   0        0        0      470 2023-06-27 12:48:50.144449 delphai_fastapi-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.3/setup.py
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.3/PKG-INFO
```

### Comparing `delphai_fastapi-0.1.2/delphai_fastapi/app.py` & `delphai_fastapi-0.1.3/delphai_fastapi/app.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.2/delphai_fastapi/auth.py` & `delphai_fastapi-0.1.3/delphai_fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.2/delphai_fastapi/companies/models.py` & `delphai_fastapi-0.1.3/delphai_fastapi/companies/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.2/delphai_fastapi/models.py` & `delphai_fastapi-0.1.3/delphai_fastapi/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.2/delphai_fastapi/types.py` & `delphai_fastapi-0.1.3/delphai_fastapi/types.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.2/setup.py` & `delphai_fastapi-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['delphai_fastapi', 'delphai_fastapi.companies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bson>=0.5.10,<0.6.0',
+['bson',
  'delphai-utils[config]>=3,<4',
  'fastapi-camelcase>=1.0.5,<2.0.0',
  'fastapi>=0.95,<0.96']
 
 setup_kwargs = {
     'name': 'delphai-fastapi',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Package for fastAPI models',
     'long_description': 'None',
     'author': 'Berinike Tech',
     'author_email': 'berinike@delphai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `delphai_fastapi-0.1.2/PKG-INFO` & `delphai_fastapi-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: delphai-fastapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package for fastAPI models
 Author: Berinike Tech
 Author-email: berinike@delphai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bson (>=0.5.10,<0.6.0)
+Requires-Dist: bson
 Requires-Dist: delphai-utils[config] (>=3,<4)
 Requires-Dist: fastapi (>=0.95,<0.96)
 Requires-Dist: fastapi-camelcase (>=1.0.5,<2.0.0)
```

