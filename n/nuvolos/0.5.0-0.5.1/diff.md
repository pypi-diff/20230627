# Comparing `tmp/nuvolos-0.5.0.tar.gz` & `tmp/nuvolos-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvolos-0.5.0.tar", last modified: Fri Jun 23 16:45:04 2023, max compression
+gzip compressed data, was "nuvolos-0.5.1.tar", last modified: Tue Jun 27 05:45:19 2023, max compression
```

## Comparing `nuvolos-0.5.0.tar` & `nuvolos-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-23 16:45:04.449768 nuvolos-0.5.0/
--rw-r--r--   0 salid      (501) staff       (20)       18 2022-07-22 09:01:09.000000 nuvolos-0.5.0/MANIFEST.in
--rw-r--r--   0 salid      (501) staff       (20)      694 2023-06-23 16:45:04.449649 nuvolos-0.5.0/PKG-INFO
--rw-r--r--   0 salid      (501) staff       (20)      461 2022-07-22 09:01:09.000000 nuvolos-0.5.0/README.rst
-drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-23 16:45:04.448506 nuvolos-0.5.0/nuvolos/
--rw-r--r--   0 salid      (501) staff       (20)    11647 2022-07-22 09:14:09.000000 nuvolos-0.5.0/nuvolos/__init__.py
--rw-r--r--   0 salid      (501) staff       (20)    17166 2022-07-22 09:21:50.000000 nuvolos-0.5.0/nuvolos/sql_utils.py
--rw-r--r--   0 salid      (501) staff       (20)       22 2023-06-23 12:49:15.000000 nuvolos-0.5.0/nuvolos/version.py
-drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-23 16:45:04.449224 nuvolos-0.5.0/nuvolos.egg-info/
--rw-r--r--   0 salid      (501) staff       (20)      694 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/PKG-INFO
--rw-r--r--   0 salid      (501) staff       (20)      296 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/SOURCES.txt
--rw-r--r--   0 salid      (501) staff       (20)        1 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/dependency_links.txt
--rw-r--r--   0 salid      (501) staff       (20)        1 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/not-zip-safe
--rw-r--r--   0 salid      (501) staff       (20)       90 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/requires.txt
--rw-r--r--   0 salid      (501) staff       (20)        8 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/top_level.txt
--rw-r--r--   0 salid      (501) staff       (20)       38 2023-06-23 16:45:04.449800 nuvolos-0.5.0/setup.cfg
--rw-r--r--   0 salid      (501) staff       (20)      815 2023-06-23 13:19:10.000000 nuvolos-0.5.0/setup.py
-drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-23 16:45:04.449349 nuvolos-0.5.0/tests/
--rw-r--r--   0 salid      (501) staff       (20)     8813 2023-06-23 14:50:50.000000 nuvolos-0.5.0/tests/test_to_sql.py
+drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-27 05:45:19.918153 nuvolos-0.5.1/
+-rw-r--r--   0 salid      (501) staff       (20)       18 2022-07-22 09:01:09.000000 nuvolos-0.5.1/MANIFEST.in
+-rw-r--r--   0 salid      (501) staff       (20)      694 2023-06-27 05:45:19.918044 nuvolos-0.5.1/PKG-INFO
+-rw-r--r--   0 salid      (501) staff       (20)      461 2022-07-22 09:01:09.000000 nuvolos-0.5.1/README.rst
+drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-27 05:45:19.916834 nuvolos-0.5.1/nuvolos/
+-rw-r--r--   0 salid      (501) staff       (20)    11647 2022-07-22 09:14:09.000000 nuvolos-0.5.1/nuvolos/__init__.py
+-rw-r--r--   0 salid      (501) staff       (20)    17166 2022-07-22 09:21:50.000000 nuvolos-0.5.1/nuvolos/sql_utils.py
+-rw-r--r--   0 salid      (501) staff       (20)       22 2023-06-27 05:39:08.000000 nuvolos-0.5.1/nuvolos/version.py
+drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-27 05:45:19.917642 nuvolos-0.5.1/nuvolos.egg-info/
+-rw-r--r--   0 salid      (501) staff       (20)      694 2023-06-27 05:45:19.000000 nuvolos-0.5.1/nuvolos.egg-info/PKG-INFO
+-rw-r--r--   0 salid      (501) staff       (20)      296 2023-06-27 05:45:19.000000 nuvolos-0.5.1/nuvolos.egg-info/SOURCES.txt
+-rw-r--r--   0 salid      (501) staff       (20)        1 2023-06-27 05:45:19.000000 nuvolos-0.5.1/nuvolos.egg-info/dependency_links.txt
+-rw-r--r--   0 salid      (501) staff       (20)        1 2023-06-23 16:45:04.000000 nuvolos-0.5.1/nuvolos.egg-info/not-zip-safe
+-rw-r--r--   0 salid      (501) staff       (20)      107 2023-06-27 05:45:19.000000 nuvolos-0.5.1/nuvolos.egg-info/requires.txt
+-rw-r--r--   0 salid      (501) staff       (20)        8 2023-06-27 05:45:19.000000 nuvolos-0.5.1/nuvolos.egg-info/top_level.txt
+-rw-r--r--   0 salid      (501) staff       (20)       38 2023-06-27 05:45:19.918187 nuvolos-0.5.1/setup.cfg
+-rw-r--r--   0 salid      (501) staff       (20)      833 2023-06-27 05:44:26.000000 nuvolos-0.5.1/setup.py
+drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-27 05:45:19.917776 nuvolos-0.5.1/tests/
+-rw-r--r--   0 salid      (501) staff       (20)     8972 2023-06-27 05:44:39.000000 nuvolos-0.5.1/tests/test_to_sql.py
```

### Comparing `nuvolos-0.5.0/PKG-INFO` & `nuvolos-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvolos
-Version: 0.5.0
+Version: 0.5.1
 Summary: The Nuvolos python library for database connectivity
 Home-page: https://github.com/nuvolos-cloud/python-connector
 Author: Alphacruncher
 Author-email: support@nuvolos.cloud
 License: MIT
 
 nuvolos - The database connectivity library for Nuvolos
```

### Comparing `nuvolos-0.5.0/nuvolos/__init__.py` & `nuvolos-0.5.1/nuvolos/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvolos-0.5.0/nuvolos/sql_utils.py` & `nuvolos-0.5.1/nuvolos/sql_utils.py`

 * *Files identical despite different names*

### Comparing `nuvolos-0.5.0/nuvolos.egg-info/PKG-INFO` & `nuvolos-0.5.1/nuvolos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvolos
-Version: 0.5.0
+Version: 0.5.1
 Summary: The Nuvolos python library for database connectivity
 Home-page: https://github.com/nuvolos-cloud/python-connector
 Author: Alphacruncher
 Author-email: support@nuvolos.cloud
 License: MIT
 
 nuvolos - The database connectivity library for Nuvolos
```

### Comparing `nuvolos-0.5.0/setup.py` & `nuvolos-0.5.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     version=__version__,
     description="The Nuvolos python library for database connectivity",
     long_description=readme(),
     url="https://github.com/nuvolos-cloud/python-connector",
     author="Alphacruncher",
     author_email="support@nuvolos.cloud",
     license="MIT",
-    packages=find_packages(exclude=("tests","venv")),
+    packages=find_packages(exclude=("tests", "venv")),
     include_package_data=True,
     install_requires=[
-        "pyarrow"
-        "keyring",
+        "pyarrow>=12.0.1",
+        "keyring>=24.1.0",
         "pandas<2.1.0",
         "snowflake-connector-python==3.0.4",
         "snowflake-sqlalchemy==1.4.7",
     ],
     zip_safe=False,
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
```

### Comparing `nuvolos-0.5.0/tests/test_to_sql.py` & `nuvolos-0.5.1/tests/test_to_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,23 @@
 @pytest.fixture
 def df_without_ns():
     df = pd.DataFrame(
         {
             "col_without_ns": [
                 pd.Timestamp(year=2022, month=9, day=1, hour=2, minute=34, second=56),
                 pd.NaT,
-                pd.Timestamp(year=2022, month=9, day=1, hour=2, minute=34, second=56, microsecond=123456),
+                pd.Timestamp(
+                    year=2022,
+                    month=9,
+                    day=1,
+                    hour=2,
+                    minute=34,
+                    second=56,
+                    microsecond=123456,
+                ),
             ],
         }
     )
     df["seq_num"] = df.index
     df.set_index("seq_num", inplace=True)
     return df
```

