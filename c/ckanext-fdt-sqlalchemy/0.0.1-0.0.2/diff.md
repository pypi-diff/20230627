# Comparing `tmp/ckanext-fdt-sqlalchemy-0.0.1.tar.gz` & `tmp/ckanext-fdt-sqlalchemy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-fdt-sqlalchemy-0.0.1.tar", last modified: Tue Jun 27 11:21:32 2023, max compression
+gzip compressed data, was "ckanext-fdt-sqlalchemy-0.0.2.tar", last modified: Tue Jun 27 11:27:09 2023, max compression
```

## Comparing `ckanext-fdt-sqlalchemy-0.0.1.tar` & `ckanext-fdt-sqlalchemy-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-27 11:21:32.722809 ckanext-fdt-sqlalchemy-0.0.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2023-06-27 08:59:24.000000 ckanext-fdt-sqlalchemy-0.0.1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      213 2023-06-27 08:59:24.000000 ckanext-fdt-sqlalchemy-0.0.1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1972 2023-06-27 11:21:32.722809 ckanext-fdt-sqlalchemy-0.0.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1307 2023-06-27 11:16:38.000000 ckanext-fdt-sqlalchemy-0.0.1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-27 11:21:32.722809 ckanext-fdt-sqlalchemy-0.0.1/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2023-06-27 11:17:51.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-27 11:21:32.722809 ckanext-fdt-sqlalchemy-0.0.1/ckanext/fdt_sqlalchemy/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-27 08:59:24.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext/fdt_sqlalchemy/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3559 2023-06-27 11:17:53.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext/fdt_sqlalchemy/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-27 11:21:32.722809 ckanext-fdt-sqlalchemy-0.0.1/ckanext/fdt_sqlalchemy/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-27 08:59:24.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext/fdt_sqlalchemy/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1352 2023-06-27 11:17:21.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext/fdt_sqlalchemy/tests/test_plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-27 11:21:32.722809 ckanext-fdt-sqlalchemy-0.0.1/ckanext_fdt_sqlalchemy.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1972 2023-06-27 11:21:32.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext_fdt_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      586 2023-06-27 11:21:32.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext_fdt_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-27 11:21:32.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext_fdt_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-06-27 11:21:32.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext_fdt_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-27 11:21:32.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext_fdt_sqlalchemy.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       47 2023-06-27 11:21:32.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext_fdt_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-27 11:21:32.000000 ckanext-fdt-sqlalchemy-0.0.1/ckanext_fdt_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4174 2023-06-27 11:17:29.000000 ckanext-fdt-sqlalchemy-0.0.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-27 08:59:24.000000 ckanext-fdt-sqlalchemy-0.0.1/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1769 2023-06-27 11:21:32.722809 ckanext-fdt-sqlalchemy-0.0.1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2023-06-27 11:17:21.000000 ckanext-fdt-sqlalchemy-0.0.1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-27 11:27:09.653836 ckanext-fdt-sqlalchemy-0.0.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2023-06-27 08:59:24.000000 ckanext-fdt-sqlalchemy-0.0.2/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      213 2023-06-27 08:59:24.000000 ckanext-fdt-sqlalchemy-0.0.2/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1972 2023-06-27 11:27:09.653836 ckanext-fdt-sqlalchemy-0.0.2/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1307 2023-06-27 11:16:38.000000 ckanext-fdt-sqlalchemy-0.0.2/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-27 11:27:09.653836 ckanext-fdt-sqlalchemy-0.0.2/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2023-06-27 11:17:51.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-27 11:27:09.653836 ckanext-fdt-sqlalchemy-0.0.2/ckanext/fdt_sqlalchemy/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-27 08:59:24.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext/fdt_sqlalchemy/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3559 2023-06-27 11:17:53.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext/fdt_sqlalchemy/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-27 11:27:09.653836 ckanext-fdt-sqlalchemy-0.0.2/ckanext/fdt_sqlalchemy/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-27 08:59:24.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext/fdt_sqlalchemy/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1352 2023-06-27 11:17:21.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext/fdt_sqlalchemy/tests/test_plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-27 11:27:09.653836 ckanext-fdt-sqlalchemy-0.0.2/ckanext_fdt_sqlalchemy.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1972 2023-06-27 11:27:09.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext_fdt_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      586 2023-06-27 11:27:09.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext_fdt_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-27 11:27:09.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext_fdt_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-06-27 11:27:09.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext_fdt_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-27 11:27:09.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext_fdt_sqlalchemy.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       30 2023-06-27 11:27:09.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext_fdt_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-27 11:27:09.000000 ckanext-fdt-sqlalchemy-0.0.2/ckanext_fdt_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4174 2023-06-27 11:17:29.000000 ckanext-fdt-sqlalchemy-0.0.2/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-27 08:59:24.000000 ckanext-fdt-sqlalchemy-0.0.2/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1753 2023-06-27 11:27:09.653836 ckanext-fdt-sqlalchemy-0.0.2/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2023-06-27 11:17:21.000000 ckanext-fdt-sqlalchemy-0.0.2/setup.py
```

### Comparing `ckanext-fdt-sqlalchemy-0.0.1/LICENSE` & `ckanext-fdt-sqlalchemy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-fdt-sqlalchemy-0.0.1/PKG-INFO` & `ckanext-fdt-sqlalchemy-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-fdt-sqlalchemy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Enable SQLAlchemy pane of Flask-DebugToolbar
 Home-page: https://github.com/ckan/ckanext-fdt-sqlalchemy
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN SQL debug
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-fdt-sqlalchemy-0.0.1/README.md` & `ckanext-fdt-sqlalchemy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-fdt-sqlalchemy-0.0.1/ckanext/fdt_sqlalchemy/plugin.py` & `ckanext-fdt-sqlalchemy-0.0.2/ckanext/fdt_sqlalchemy/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-fdt-sqlalchemy-0.0.1/ckanext/fdt_sqlalchemy/tests/test_plugin.py` & `ckanext-fdt-sqlalchemy-0.0.2/ckanext/fdt_sqlalchemy/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-fdt-sqlalchemy-0.0.1/ckanext_fdt_sqlalchemy.egg-info/PKG-INFO` & `ckanext-fdt-sqlalchemy-0.0.2/ckanext_fdt_sqlalchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-fdt-sqlalchemy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Enable SQLAlchemy pane of Flask-DebugToolbar
 Home-page: https://github.com/ckan/ckanext-fdt-sqlalchemy
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN SQL debug
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-fdt-sqlalchemy-0.0.1/ckanext_fdt_sqlalchemy.egg-info/SOURCES.txt` & `ckanext-fdt-sqlalchemy-0.0.2/ckanext_fdt_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-fdt-sqlalchemy-0.0.1/pyproject.toml` & `ckanext-fdt-sqlalchemy-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-fdt-sqlalchemy-0.0.1/setup.cfg` & `ckanext-fdt-sqlalchemy-0.0.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-fdt-sqlalchemy
-version = 0.0.1
+version = 0.0.2
 description = Enable SQLAlchemy pane of Flask-DebugToolbar
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ckan/ckanext-fdt-sqlalchemy
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 keywords = CKAN SQL debug
 
 [options]
 packages = find:
 namespace_packages = ckanext
-install_requires = flask-sqlalchemy
+install_requires = 
 include_package_data = True
 
 [options.entry_points]
 ckan.plugins = 
 	fdt_sqlalchemy = ckanext.fdt_sqlalchemy.plugin:FdtSqlalchemyPlugin
 babel.extractors = 
 	ckan = ckan.lib.extract:extract_ckan
```

