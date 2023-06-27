# Comparing `tmp/delphai_fastapi-0.1.4.tar.gz` & `tmp/delphai_fastapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_fastapi-0.1.4.tar", max compression
+gzip compressed data, was "delphai_fastapi-0.1.5.tar", max compression
```

## Comparing `delphai_fastapi-0.1.4.tar` & `delphai_fastapi-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-06-27 15:12:39.672267 delphai_fastapi-0.1.4/delphai_fastapi/__init__.py
--rw-r--r--   0        0        0     2521 2023-06-27 15:12:39.672267 delphai_fastapi-0.1.4/delphai_fastapi/app.py
--rw-r--r--   0        0        0     3173 2023-06-27 15:12:39.672267 delphai_fastapi-0.1.4/delphai_fastapi/auth.py
--rw-r--r--   0        0        0        0 2023-06-27 15:12:39.672267 delphai_fastapi-0.1.4/delphai_fastapi/companies/__init__.py
--rw-r--r--   0        0        0     3266 2023-06-27 15:12:39.672267 delphai_fastapi-0.1.4/delphai_fastapi/companies/models.py
--rw-r--r--   0        0        0      375 2023-06-27 15:12:39.672267 delphai_fastapi-0.1.4/delphai_fastapi/decorators.py
--rw-r--r--   0        0        0     1619 2023-06-27 15:12:39.672267 delphai_fastapi-0.1.4/delphai_fastapi/models.py
--rw-r--r--   0        0        0     1342 2023-06-27 15:12:39.672267 delphai_fastapi-0.1.4/delphai_fastapi/types.py
--rw-r--r--   0        0        0      472 2023-06-27 15:13:29.240509 delphai_fastapi-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.4/setup.py
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/__init__.py
+-rw-r--r--   0        0        0     2521 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/app.py
+-rw-r--r--   0        0        0     3173 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/auth.py
+-rw-r--r--   0        0        0        0 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/companies/__init__.py
+-rw-r--r--   0        0        0     3266 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/companies/models.py
+-rw-r--r--   0        0        0      375 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/decorators.py
+-rw-r--r--   0        0        0     1582 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/models.py
+-rw-r--r--   0        0        0     1342 2023-06-27 15:58:32.302265 delphai_fastapi-0.1.5/delphai_fastapi/types.py
+-rw-r--r--   0        0        0      472 2023-06-27 15:59:27.450844 delphai_fastapi-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.5/setup.py
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.5/PKG-INFO
```

### Comparing `delphai_fastapi-0.1.4/delphai_fastapi/app.py` & `delphai_fastapi-0.1.5/delphai_fastapi/app.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.4/delphai_fastapi/auth.py` & `delphai_fastapi-0.1.5/delphai_fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.4/delphai_fastapi/companies/models.py` & `delphai_fastapi-0.1.5/delphai_fastapi/companies/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.4/delphai_fastapi/models.py` & `delphai_fastapi-0.1.5/delphai_fastapi/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import Optional, List
 
 from fastapi_camelcase import CamelModel
 from pydantic import Field
 from datetime import datetime
 
-from companies.models import Company
-
 
 class HTTPExceptionModel(CamelModel):
     detail: str
 
 
 class Location(CamelModel):
     country: Optional[str] = Field(
@@ -34,8 +32,8 @@
     created: datetime = Field(..., description="When the project was created")
     last_modified: datetime = Field(..., description="When the project was last edited or updated")
     available: int = Field(..., description="Number of companies in this project that are accessible in the dashboard", example=29)
 
 
 class Source(CamelModel): 
     name: str = Field(description="Name of the source")
-    credibility_score: float = Field(description="Credibility score of source in percentage", example=0.60)
+    credibility_score: float = Field(description="Credibility score of source in percentage", example=0.60)
```

### Comparing `delphai_fastapi-0.1.4/delphai_fastapi/types.py` & `delphai_fastapi-0.1.5/delphai_fastapi/types.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.4/setup.py` & `delphai_fastapi-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['delphai-utils[config]>=3,<4',
  'fastapi-camelcase>=1.0.5,<2.0.0',
  'fastapi>=0.95,<0.96',
  'pymongo']
 
 setup_kwargs = {
     'name': 'delphai-fastapi',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Package for fastAPI models',
     'long_description': 'None',
     'author': 'Berinike Tech',
     'author_email': 'berinike@delphai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `delphai_fastapi-0.1.4/PKG-INFO` & `delphai_fastapi-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphai-fastapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package for fastAPI models
 Author: Berinike Tech
 Author-email: berinike@delphai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

