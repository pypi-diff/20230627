# Comparing `tmp/maci-0.3.0.tar.gz` & `tmp/maci-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maci-0.3.0.tar", last modified: Tue Jun 27 00:20:49 2023, max compression
+gzip compressed data, was "maci-0.3.1.tar", last modified: Tue Jun 27 01:38:29 2023, max compression
```

## Comparing `maci-0.3.0.tar` & `maci-0.3.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.541262 maci-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-27 00:20:39.000000 maci-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-27 00:20:49.541262 maci-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-06-27 00:20:49.000000 maci-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.533262 maci-0.3.0/maci/
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-27 00:20:49.000000 maci-0.3.0/maci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci/_hash/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_hash/comparefilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_hash/createfilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3336 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_hash/createhash.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci/_ini/
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_ini/inibuildauto.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_ini/inibuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_ini/inidump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_ini/iniload.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci/_json/
--rw-r--r--   0 runner    (1001) docker     (122)     2531 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_json/jsondump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_json/jsondumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_json/jsonload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_json/jsonloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci/_native/
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     2316 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/cleanformat.py
--rw-r--r--   0 runner    (1001) docker     (122)     7191 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/dump.py
--rw-r--r--   0 runner    (1001) docker     (122)     4417 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/dumpraw.py
--rw-r--r--   0 runner    (1001) docker     (122)     6484 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/dumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3633 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/load.py
--rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/loadattrs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4175 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/loaddict.py
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/loadraw.py
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/loadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/loadstrdict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci/_toml/
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_toml/tomldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_toml/tomldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_toml/tomlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_toml/tomlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.541262 maci-0.3.0/maci/_xml/
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_xml/xmlbuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_xml/xmldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_xml/xmldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_xml/xmlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_xml/xmlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.541262 maci-0.3.0/maci/_yaml/
--rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_yaml/yamldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_yaml/yamldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_yaml/yamlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_yaml/yamlloadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)    71589 2023-06-27 00:20:49.000000 maci-0.3.0/maci/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2981 2023-06-27 00:20:49.000000 maci-0.3.0/maci/error.py
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-27 00:20:49.000000 maci-0.3.0/maci/hint.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-27 00:20:49.000000 maci-0.3.0/maci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-27 00:20:49.000000 maci-0.3.0/maci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 00:20:49.000000 maci-0.3.0/maci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-06-27 00:20:49.000000 maci-0.3.0/maci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-27 00:20:49.000000 maci-0.3.0/maci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-06-27 00:20:49.541262 maci-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-06-27 00:20:39.000000 maci-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.544375 maci-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-27 01:38:17.000000 maci-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-27 01:38:29.544375 maci-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-06-27 01:38:29.000000 maci-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.532374 maci-0.3.1/maci/
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-27 01:38:29.000000 maci-0.3.1/maci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.536374 maci-0.3.1/maci/_hash/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_hash/comparefilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_hash/createfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3336 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_hash/createhash.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.536374 maci-0.3.1/maci/_ini/
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_ini/inibuildauto.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_ini/inibuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_ini/inidump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_ini/iniload.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.536374 maci-0.3.1/maci/_json/
+-rw-r--r--   0 runner    (1001) docker     (122)     2531 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_json/jsondump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_json/jsondumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_json/jsonload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_json/jsonloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.540374 maci-0.3.1/maci/_native/
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2316 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/cleanformat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7191 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4417 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/dumpraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6484 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/dumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3633 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/loadattrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4175 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/loaddict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/loadraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/loadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/loadstrdict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.540374 maci-0.3.1/maci/_toml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_toml/tomldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_toml/tomldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_toml/tomlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_toml/tomlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.540374 maci-0.3.1/maci/_xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_xml/xmlbuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_xml/xmldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_xml/xmldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_xml/xmlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_xml/xmlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.544375 maci-0.3.1/maci/_yaml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_yaml/yamldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_yaml/yamldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_yaml/yamlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_yaml/yamlloadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71589 2023-06-27 01:38:29.000000 maci-0.3.1/maci/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2981 2023-06-27 01:38:29.000000 maci-0.3.1/maci/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-27 01:38:29.000000 maci-0.3.1/maci/hint.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.000000 maci-0.3.1/maci/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.536374 maci-0.3.1/maci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-27 01:38:29.000000 maci-0.3.1/maci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1121 2023-06-27 01:38:29.000000 maci-0.3.1/maci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 01:38:29.000000 maci-0.3.1/maci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-06-27 01:38:29.000000 maci-0.3.1/maci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-27 01:38:29.000000 maci-0.3.1/maci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1384 2023-06-27 01:38:29.544375 maci-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-06-27 01:38:17.000000 maci-0.3.1/setup.py
```

### Comparing `maci-0.3.0/PKG-INFO` & `maci-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.3.0
+Version: 0.3.1
 Summary: The easy to use library for your data, configuration, and save files
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
 Project-URL: Docs, https://docs.macilib.org
 Project-URL: Code, https://github.com/aaronater10/maci
 Project-URL: Bugs, https://github.com/aaronater10/maci/issues
@@ -23,15 +23,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.3.0
+##### Latest Version: 0.3.1
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.3.0/README.md` & `maci-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.3.0
+##### Latest Version: 0.3.1
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.3.0/maci/__init__.py` & `maci-0.3.1/maci/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 maci - by aaronater10
 
-Version 0.3.0
+Version 0.3.1
 
 The easy to use library for your data, configuration, and save files.
 
 Import or Export custom, or industry-common, data, config, and save files easily for
 your python program or script!
 
 See tutorials and docs here for more info: https://docs.macilib.org
 
 Source Code: https://github.com/aaronater10/maci
 """
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 #########################################################################################################
 # Imports
 
 # Base Exceptions
 from . import error
```

### Comparing `maci-0.3.0/maci/_hash/comparefilehash.py` & `maci-0.3.1/maci/_hash/comparefilehash.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_hash/createfilehash.py` & `maci-0.3.1/maci/_hash/createfilehash.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_hash/createhash.py` & `maci-0.3.1/maci/_hash/createhash.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_ini/inibuildauto.py` & `maci-0.3.1/maci/_ini/inibuildauto.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_ini/inibuildmanual.py` & `maci-0.3.1/maci/_ini/inibuildmanual.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_ini/inidump.py` & `maci-0.3.1/maci/_ini/inidump.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_ini/iniload.py` & `maci-0.3.1/maci/_ini/iniload.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_json/jsondump.py` & `maci-0.3.1/maci/_json/jsondump.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_json/jsondumpstr.py` & `maci-0.3.1/maci/_json/jsondumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_json/jsonload.py` & `maci-0.3.1/maci/_json/jsonload.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_json/jsonloadstr.py` & `maci-0.3.1/maci/_json/jsonloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/build.py` & `maci-0.3.1/maci/_native/build.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/cleanformat.py` & `maci-0.3.1/maci/_native/cleanformat.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/dump.py` & `maci-0.3.1/maci/_native/dump.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/dumpraw.py` & `maci-0.3.1/maci/_native/dumpraw.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/dumpstr.py` & `maci-0.3.1/maci/_native/dumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/load.py` & `maci-0.3.1/maci/_native/load.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/loadattrs.py` & `maci-0.3.1/maci/_native/loadattrs.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/loaddict.py` & `maci-0.3.1/maci/_native/loaddict.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/loadraw.py` & `maci-0.3.1/maci/_native/loadraw.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/loadstr.py` & `maci-0.3.1/maci/_native/loadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_native/loadstrdict.py` & `maci-0.3.1/maci/_native/loadstrdict.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_toml/tomldump.py` & `maci-0.3.1/maci/_toml/tomldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_toml/tomldumpstr.py` & `maci-0.3.1/maci/_toml/tomldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_toml/tomlload.py` & `maci-0.3.1/maci/_toml/tomlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_toml/tomlloadstr.py` & `maci-0.3.1/maci/_toml/tomlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_xml/xmlbuildmanual.py` & `maci-0.3.1/maci/_xml/xmlbuildmanual.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_xml/xmldump.py` & `maci-0.3.1/maci/_xml/xmldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_xml/xmldumpstr.py` & `maci-0.3.1/maci/_xml/xmldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_xml/xmlload.py` & `maci-0.3.1/maci/_xml/xmlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_xml/xmlloadstr.py` & `maci-0.3.1/maci/_xml/xmlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_yaml/yamldump.py` & `maci-0.3.1/maci/_yaml/yamldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_yaml/yamldumpstr.py` & `maci-0.3.1/maci/_yaml/yamldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_yaml/yamlload.py` & `maci-0.3.1/maci/_yaml/yamlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/_yaml/yamlloadstr.py` & `maci-0.3.1/maci/_yaml/yamlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/data.py` & `maci-0.3.1/maci/data.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci/error.py` & `maci-0.3.1/maci/error.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.0/maci.egg-info/PKG-INFO` & `maci-0.3.1/maci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.3.0
+Version: 0.3.1
 Summary: The easy to use library for your data, configuration, and save files
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
 Project-URL: Docs, https://docs.macilib.org
 Project-URL: Code, https://github.com/aaronater10/maci
 Project-URL: Bugs, https://github.com/aaronater10/maci/issues
@@ -23,15 +23,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.3.0
+##### Latest Version: 0.3.1
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.3.0/maci.egg-info/SOURCES.txt` & `maci-0.3.1/maci.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+./README.md
 maci/__init__.py
 maci/data.py
 maci/error.py
 maci/hint.py
+maci/py.typed
 maci.egg-info/PKG-INFO
 maci.egg-info/SOURCES.txt
 maci.egg-info/dependency_links.txt
 maci.egg-info/requires.txt
 maci.egg-info/top_level.txt
 maci/_hash/comparefilehash.py
 maci/_hash/createfilehash.py
```

### Comparing `maci-0.3.0/setup.cfg` & `maci-0.3.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -58,11 +58,14 @@
 install_requires = 
 	pyyaml >= 5.4
 	types-pyyaml >= 5.4
 	tomli >= 2.0.1
 	tomli-w >= 1.0.0
 python_requires = >= 3.7
 
+[options.package_data]
+maci = py.typed
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

