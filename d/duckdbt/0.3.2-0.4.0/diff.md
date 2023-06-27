# Comparing `tmp/duckdbt-0.3.2.tar.gz` & `tmp/duckdbt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdbt-0.3.2.tar", last modified: Tue May 16 19:45:14 2023, max compression
+gzip compressed data, was "duckdbt-0.4.0.tar", last modified: Tue Jun 27 04:58:54 2023, max compression
```

## Comparing `duckdbt-0.3.2.tar` & `duckdbt-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:45:14.435883 duckdbt-0.3.2/
--rw-r--r--   0 jwills     (501) staff       (20)       53 2023-01-14 04:58:00.000000 duckdbt-0.3.2/MANIFEST.in
--rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-16 19:45:14.435758 duckdbt-0.3.2/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)       53 2023-05-08 20:57:22.000000 duckdbt-0.3.2/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:45:14.434517 duckdbt-0.3.2/duckdbt/
--rw-r--r--   0 jwills     (501) staff       (20)     1248 2023-05-08 20:17:37.000000 duckdbt-0.3.2/duckdbt/api.py
--rw-r--r--   0 jwills     (501) staff       (20)      938 2023-05-16 19:23:48.000000 duckdbt-0.3.2/duckdbt/common.py
--rw-r--r--   0 jwills     (501) staff       (20)     1736 2023-05-08 20:17:37.000000 duckdbt-0.3.2/duckdbt/extensions.py
--rw-r--r--   0 jwills     (501) staff       (20)      536 2023-05-16 19:23:48.000000 duckdbt-0.3.2/duckdbt/ipython.py
--rw-r--r--   0 jwills     (501) staff       (20)     1786 2023-05-09 00:15:58.000000 duckdbt-0.3.2/duckdbt/load_db_profile.py
--rw-r--r--   0 jwills     (501) staff       (20)     1165 2023-05-16 19:23:48.000000 duckdbt-0.3.2/duckdbt/server.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:45:14.435373 duckdbt-0.3.2/duckdbt/static/
--rw-r--r--   0 jwills     (501) staff       (20)     1489 2023-05-16 19:23:48.000000 duckdbt-0.3.2/duckdbt/static/dashboard.css
--rw-r--r--   0 jwills     (501) staff       (20)     1406 2023-05-08 20:17:37.000000 duckdbt-0.3.2/duckdbt/static/favicon.ico
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:45:14.435580 duckdbt-0.3.2/duckdbt/templates/
--rw-r--r--   0 jwills     (501) staff       (20)     4910 2023-05-16 19:23:48.000000 duckdbt-0.3.2/duckdbt/templates/index.html
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-16 19:45:14.435072 duckdbt-0.3.2/duckdbt.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)      302 2023-05-16 19:45:14.000000 duckdbt-0.3.2/duckdbt.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)      388 2023-05-16 19:45:14.000000 duckdbt-0.3.2/duckdbt.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-16 19:45:14.000000 duckdbt-0.3.2/duckdbt.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       87 2023-05-16 19:45:14.000000 duckdbt-0.3.2/duckdbt.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)        8 2023-05-16 19:45:14.000000 duckdbt-0.3.2/duckdbt.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-16 19:45:14.435914 duckdbt-0.3.2/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)      951 2023-05-16 19:44:44.000000 duckdbt-0.3.2/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-27 04:58:54.520819 duckdbt-0.4.0/
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2023-01-14 04:58:00.000000 duckdbt-0.4.0/MANIFEST.in
+-rw-r--r--   0 jwills     (501) staff       (20)      302 2023-06-27 04:58:54.520714 duckdbt-0.4.0/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2023-05-08 20:57:22.000000 duckdbt-0.4.0/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-27 04:58:54.519360 duckdbt-0.4.0/duckdbt/
+-rw-r--r--   0 jwills     (501) staff       (20)     1248 2023-05-08 20:17:37.000000 duckdbt-0.4.0/duckdbt/api.py
+-rw-r--r--   0 jwills     (501) staff       (20)      938 2023-05-16 19:23:48.000000 duckdbt-0.4.0/duckdbt/common.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1736 2023-05-08 20:17:37.000000 duckdbt-0.4.0/duckdbt/extensions.py
+-rw-r--r--   0 jwills     (501) staff       (20)      536 2023-05-16 19:23:48.000000 duckdbt-0.4.0/duckdbt/ipython.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1786 2023-05-09 00:15:58.000000 duckdbt-0.4.0/duckdbt/load_db_profile.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1165 2023-05-16 19:23:48.000000 duckdbt-0.4.0/duckdbt/server.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-27 04:58:54.520203 duckdbt-0.4.0/duckdbt/static/
+-rw-r--r--   0 jwills     (501) staff       (20)     1489 2023-05-16 19:23:48.000000 duckdbt-0.4.0/duckdbt/static/dashboard.css
+-rw-r--r--   0 jwills     (501) staff       (20)     1406 2023-05-08 20:17:37.000000 duckdbt-0.4.0/duckdbt/static/favicon.ico
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-27 04:58:54.520555 duckdbt-0.4.0/duckdbt/templates/
+-rw-r--r--   0 jwills     (501) staff       (20)     4910 2023-05-16 19:23:48.000000 duckdbt-0.4.0/duckdbt/templates/index.html
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-06-27 04:58:54.519896 duckdbt-0.4.0/duckdbt.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)      302 2023-06-27 04:58:54.000000 duckdbt-0.4.0/duckdbt.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)      388 2023-06-27 04:58:54.000000 duckdbt-0.4.0/duckdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-06-27 04:58:54.000000 duckdbt-0.4.0/duckdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       87 2023-06-27 04:58:54.000000 duckdbt-0.4.0/duckdbt.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        8 2023-06-27 04:58:54.000000 duckdbt-0.4.0/duckdbt.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-06-27 04:58:54.520849 duckdbt-0.4.0/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)      951 2023-06-27 04:58:37.000000 duckdbt-0.4.0/setup.py
```

### Comparing `duckdbt-0.3.2/duckdbt/api.py` & `duckdbt-0.4.0/duckdbt/api.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.2/duckdbt/common.py` & `duckdbt-0.4.0/duckdbt/common.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.2/duckdbt/extensions.py` & `duckdbt-0.4.0/duckdbt/extensions.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.2/duckdbt/ipython.py` & `duckdbt-0.4.0/duckdbt/ipython.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.2/duckdbt/load_db_profile.py` & `duckdbt-0.4.0/duckdbt/load_db_profile.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.2/duckdbt/server.py` & `duckdbt-0.4.0/duckdbt/server.py`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.2/duckdbt/static/dashboard.css` & `duckdbt-0.4.0/duckdbt/static/dashboard.css`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.2/duckdbt/static/favicon.ico` & `duckdbt-0.4.0/duckdbt/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.2/duckdbt/templates/index.html` & `duckdbt-0.4.0/duckdbt/templates/index.html`

 * *Files identical despite different names*

### Comparing `duckdbt-0.3.2/setup.py` & `duckdbt-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 package_name = "duckdbt"
 
 
-package_version = "0.3.2"
+package_version = "0.4.0"
 description = """The Modern Data Stack in a Python Package"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
@@ -24,12 +24,12 @@
     author_email="joshwills+duckdbt@gmail.com",
     url="https://github.com/jwills/duckdbt",
     packages=find_namespace_packages(include=["duckdbt", "duckdbt.*"]),
     include_package_data=True,
     install_requires=[
         "buenavista[duckdb]~=0.3.0",
         "dbt-duckdb~=1.5.0",
-        "duckdb~=0.7.0",
+        "duckdb~=0.8.0",
         "fastapi[all]",
         "psycopg2-binary",
     ],
 )
```

