# Comparing `tmp/maci-0.2.0.tar.gz` & `tmp/maci-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maci-0.2.0.tar", last modified: Fri Dec 30 08:04:44 2022, max compression
+gzip compressed data, was "maci-0.3.0.tar", last modified: Tue Jun 27 00:20:49 2023, max compression
```

## Comparing `maci-0.2.0.tar` & `maci-0.3.0.tar`

### file list

```diff
@@ -1,47 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-30 08:04:44.469465 maci-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2022-12-30 08:04:30.000000 maci-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2308 2022-12-30 08:04:44.469465 maci-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2022-12-30 08:04:43.000000 maci-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-30 08:04:44.461465 maci-0.2.0/maci/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-30 08:04:44.465465 maci-0.2.0/maci/__hash/
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__hash/comparefilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__hash/createfilehash.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-30 08:04:44.465465 maci-0.2.0/maci/__ini/
--rw-r--r--   0 runner    (1001) docker     (122)     1608 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__ini/inibuildauto.py
--rw-r--r--   0 runner    (1001) docker     (122)      904 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__ini/inibuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     1633 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__ini/inidump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__ini/iniload.py
--rw-r--r--   0 runner    (1001) docker     (122)     3162 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-30 08:04:44.465465 maci-0.2.0/maci/__json/
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__json/jsondump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__json/jsondumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__json/jsonload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1215 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__json/jsonloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-30 08:04:44.465465 maci-0.2.0/maci/__native/
--rw-r--r--   0 runner    (1001) docker     (122)      779 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__native/builddata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2373 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__native/cleanformat.py
--rw-r--r--   0 runner    (1001) docker     (122)     8698 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__native/dump.py
--rw-r--r--   0 runner    (1001) docker     (122)     3373 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__native/dumpraw.py
--rw-r--r--   0 runner    (1001) docker     (122)    14684 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__native/load.py
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__native/loadattrs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__native/loadraw.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-30 08:04:44.469465 maci-0.2.0/maci/__xml/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__xml/xmlbuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__xml/xmldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__xml/xmldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__xml/xmlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__xml/xmlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-30 08:04:44.469465 maci-0.2.0/maci/__yaml/
--rw-r--r--   0 runner    (1001) docker     (122)     1441 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__yaml/yamldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__yaml/yamldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__yaml/yamlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1621 2022-12-30 08:04:43.000000 maci-0.2.0/maci/__yaml/yamlloadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1716 2022-12-30 08:04:43.000000 maci-0.2.0/maci/error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-30 08:04:44.465465 maci-0.2.0/maci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2308 2022-12-30 08:04:44.000000 maci-0.2.0/maci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      865 2022-12-30 08:04:44.000000 maci-0.2.0/maci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-30 08:04:44.000000 maci-0.2.0/maci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2022-12-30 08:04:44.000000 maci-0.2.0/maci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-12-30 08:04:44.000000 maci-0.2.0/maci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-30 08:04:44.469465 maci-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1750 2022-12-30 08:04:30.000000 maci-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.541262 maci-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-27 00:20:39.000000 maci-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-27 00:20:49.541262 maci-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-06-27 00:20:49.000000 maci-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.533262 maci-0.3.0/maci/
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-27 00:20:49.000000 maci-0.3.0/maci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci/_hash/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_hash/comparefilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_hash/createfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3336 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_hash/createhash.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci/_ini/
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_ini/inibuildauto.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_ini/inibuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_ini/inidump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_ini/iniload.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci/_json/
+-rw-r--r--   0 runner    (1001) docker     (122)     2531 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_json/jsondump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_json/jsondumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_json/jsonload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_json/jsonloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci/_native/
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2316 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/cleanformat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7191 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4417 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/dumpraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6484 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/dumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3633 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/loadattrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4175 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/loaddict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/loadraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/loadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_native/loadstrdict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci/_toml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_toml/tomldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_toml/tomldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_toml/tomlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_toml/tomlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.541262 maci-0.3.0/maci/_xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_xml/xmlbuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_xml/xmldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_xml/xmldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_xml/xmlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_xml/xmlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.541262 maci-0.3.0/maci/_yaml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_yaml/yamldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_yaml/yamldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_yaml/yamlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-06-27 00:20:49.000000 maci-0.3.0/maci/_yaml/yamlloadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71589 2023-06-27 00:20:49.000000 maci-0.3.0/maci/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2981 2023-06-27 00:20:49.000000 maci-0.3.0/maci/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-27 00:20:49.000000 maci-0.3.0/maci/hint.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 00:20:49.537262 maci-0.3.0/maci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-27 00:20:49.000000 maci-0.3.0/maci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-27 00:20:49.000000 maci-0.3.0/maci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 00:20:49.000000 maci-0.3.0/maci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-06-27 00:20:49.000000 maci-0.3.0/maci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-27 00:20:49.000000 maci-0.3.0/maci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-06-27 00:20:49.541262 maci-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-06-27 00:20:39.000000 maci-0.3.0/setup.py
```

### Comparing `maci-0.2.0/PKG-INFO` & `maci-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.2.0
+Version: 0.3.0
 Summary: The easy to use library for your data, configuration, and save files
-Home-page: https://github.com/aaronater10/maci
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
+Project-URL: Docs, https://docs.macilib.org
+Project-URL: Code, https://github.com/aaronater10/maci
+Project-URL: Bugs, https://github.com/aaronater10/maci/issues
+Project-URL: CI, https://github.com/aaronater10/maci/actions
 Keywords: maci,aaronater10,python,py,config,file,export,parse,text file,cfg,conf,save file,config file,db,database,simple,configuration,alternative,safe,ini,json,xml,yml,data,import
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.2.0
+##### Latest Version: 0.3.0
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.2.0/README.md` & `maci-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.2.0
+##### Latest Version: 0.3.0
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.2.0/maci/__hash/comparefilehash.py` & `maci-0.3.0/maci/_hash/comparefilehash.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # comparefilehash
 #########################################################################################################
 # Imports
-from .createfilehash import createfilehash
-from ..__native.load import load
-from ..error import CompareFileHash
+from typing import Union as _Union
+from typing import Any as _Any
+from .createfilehash import createfilehash as _createfilehash
+from .._native.load import load as _load
+from ..error import CompareFileHash, CreateFileHash, Load
 
 #########################################################################################################
 # Compare file hashes
-def comparefilehash(file_to_hash: str, stored_hash_file: str, hash_algorithm: str='sha256') -> bool:
+def comparefilehash(file_to_hash: str, stored_hash_file: str, hash_algorithm: str='sha256', *, encoding: _Union[str, None]=None) -> bool:
     """
     Compares hash of any file by importing the previously stored hash file data from using "createfilehash"
 
     Returns a bool if the hash does/doesn't match
 
     Enter file locations as str
 
@@ -22,24 +24,32 @@
     [Example Use]
     
     comparefilehash('path/to/src_filename', 'path/to/src_hash_filename')
 
     This is using the hashlib library shipped with the python standard library. For more
     information on hashlib, visit: https://docs.python.org/3/library/hashlib.html
     """
-    __ALGO_OPTIONS = ('sha256', 'sha512', 'sha384', 'sha1', 'md5')
+    ALGO_OPTIONS = ('sha256', 'sha512', 'sha384', 'sha1', 'md5')
 
     # Error checks
-    __err_msg_str_file_src = f"Only str is allowed for file_to_hash"
-    __err_msg_hash_file = f"Only str is allowed for stored_hash_file"
-    __err_msg_str_hash = f"Only str is allowed for hash_algorithm"
-    __err_msg_hash = f"Invalid or no hash option chosen for hash_algorithm"
-
-    if not isinstance(file_to_hash, str): raise CompareFileHash(__err_msg_str_file_src, f'"{file_to_hash}"')
-    if not isinstance(stored_hash_file, str): raise CompareFileHash(__err_msg_hash_file, f'"{stored_hash_file}"')
-    if not isinstance(hash_algorithm, str): raise CompareFileHash(__err_msg_str_hash, f'"{hash_algorithm}"')
-    if not hash_algorithm in __ALGO_OPTIONS: raise CompareFileHash(__err_msg_hash, f'"{hash_algorithm}"')
-    
+    _err_msg_str_file_src = f"Only str is allowed for file_to_hash"
+    _err_msg_hash_file = f"Only str is allowed for stored_hash_file"
+    _err_msg_str_hash = f"Only str is allowed for hash_algorithm"
+    _err_msg_hash = f"Invalid or no hash option chosen for hash_algorithm"
+    err_msg_str_encoding = f"Only str|None or valid option is allowed for 'encoding'"
+
+    if not isinstance(file_to_hash, str): raise CompareFileHash(_err_msg_str_file_src, f'"{file_to_hash}"')
+    if not isinstance(stored_hash_file, str): raise CompareFileHash(_err_msg_hash_file, f'"{stored_hash_file}"')
+    if not isinstance(hash_algorithm, str): raise CompareFileHash(_err_msg_str_hash, f'"{hash_algorithm}"')
+    if not hash_algorithm in ALGO_OPTIONS: raise CompareFileHash(_err_msg_hash, f'"{hash_algorithm}"')
+    if not isinstance(encoding, (str, type(None))): raise CompareFileHash(err_msg_str_encoding, f'\nGot: {repr(encoding)}')
+
     # Collect hash data, then return result
-    __hash_data = createfilehash(file_to_hash, False, hash_algorithm)
-    __stored_hash_data = load(stored_hash_file)
-    return (__hash_data == __stored_hash_data.hash_data)
+    try: _hash_data = _createfilehash(file_to_hash, None, hash_algorithm, encoding=encoding)
+    except CreateFileHash as err_msg: raise CompareFileHash(err_msg)
+
+    try:
+        _stored_hash_data: _Any  # ignore type checker
+        _stored_hash_data = _load(stored_hash_file, encoding=encoding)
+    except Load as err_msg: raise CompareFileHash(err_msg)
+
+    return (_hash_data == _stored_hash_data.hash_data)
```

### Comparing `maci-0.2.0/maci/__ini/inibuildmanual.py` & `maci-0.3.0/maci/_ini/inibuildmanual.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # inibuildmanual
 #########################################################################################################
 # Imports
-from configparser import ConfigParser as __ConfigParser
-from configparser import ExtendedInterpolation as __ExtendedInterpolation
+from configparser import ConfigParser as _ConfigParser
+from configparser import ExtendedInterpolation as _ExtendedInterpolation
 
 #########################################################################################################
 # Build manual ini data
-def inibuildmanual() -> __ConfigParser:
+def inibuildmanual() -> _ConfigParser:
     """    
-    Returns an empty ConfigParser obj to manually build ini data
+    Returns an empty ConfigParser object to manually build ini data
     
     Assign the output to var
 
     This is using the native configparser library shipped with the python standard library. Using ConfigParser method
     with ExtendedInterpolation enabled by default. For more information on the configparser library, 
     visit: https://docs.python.org/3/library/configparser.html
     """
-    return __ConfigParser(interpolation=__ExtendedInterpolation())
+    return _ConfigParser(interpolation=_ExtendedInterpolation())
```

### Comparing `maci-0.2.0/maci/__ini/inidump.py` & `maci-0.3.0/maci/_native/loadraw.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,48 @@
-# inidump
+# loadraw
 #########################################################################################################
 # Imports
-from configparser import ConfigParser as __ConfigParser
-from ..error import IniDump
+from typing import Union as _Union
+from os import path as __path
+from ..error import LoadRaw
 
 #########################################################################################################
-# Export ini file
+# Import raw data from file
+def loadraw(filename: str, *, byte_data: bool=False, encoding: _Union[str, None]=None) -> _Union[str, bytes]:
+    """
+    Imports any raw data from a file.
 
-# Create hollow reference name for "ini_data" to denote ini data needs to be exported for hinting exports
-class __dummy_ini:
-    """Not meant to be used"""
-    class ini_data:
-        """Not meant to be used"""
+    Returns a str. Assign the output to var
 
-def inidump(filename: str, data: __dummy_ini.ini_data) -> None:
-    """
-    Exports a new file from a ini data (ConfigParser) obj
-    
-    Enter new filename as str. Pass ini data for output to file
-    
-    [Example Use]
+    [Options]
+    byte_data: Set to True if importing byte data
 
-    inidump('path/to/filename.ini', data)
+    [Example Use]
 
-    This is using the native configparser library shipped with the python standard library. Using ConfigParser method.
-    For more information on the configparser library, visit: https://docs.python.org/3/library/configparser.html
+    loadraw('path/to/filename')
     """
-    __err_msg_parser = f"Invalid data to export, type, or nothing specified"
-        
-    if not isinstance(data, __ConfigParser):
-        raise IniDump(__err_msg_parser, f'\nFILE: "{filename}" \nDATA: {data}')
-    try:
-        with open(filename, 'w') as f:
-            data.write(f)
-    except TypeError as __err_msg: raise IniDump(__err_msg, f'\nFILE: "{filename}" \nDATA: {data}')
-    except ValueError as __err_msg: raise IniDump(__err_msg, f'\nFILE: "{filename}" \nDATA: {data}')
-    except FileNotFoundError as __err_msg: raise IniDump(__err_msg, f'\nFILE: "{filename}"')
+    # Error Checks
+    err_msg_type_filename = "Only str is allowed for 'filename'"
+    err_msg_type_byte_data = "Only bool is allowed for 'byte_data'"
+    err_msg_type_encoding = "Only str|None or valid option is allowed for 'encoding'"
+
+    if not isinstance(filename, str): raise LoadRaw(err_msg_type_filename, f'\nGot: {repr(filename)}')
+    if not isinstance(byte_data, bool): raise LoadRaw(err_msg_type_byte_data, f'\nGot: {repr(byte_data)}')
+    if not isinstance(encoding, (str, type(None))): raise LoadRaw(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
+
+    # Validate file exists. Import File then return the raw data
+    if not byte_data:
+        try:
+            with open(filename, 'r', encoding=encoding) as f:
+                if __path.getsize(filename) == 0:
+                    return ''
+                return f.read()
+        except (FileNotFoundError, OSError) as __err_msg: raise LoadRaw(__err_msg, f'\nGot: "{filename}"')
+        except LookupError: raise LoadRaw(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
+    
+    if byte_data: # pragma: no branch
+        try:
+            with open(filename, 'rb') as f:
+                if __path.getsize(filename) == 0:
+                    return b''
+                return f.read()
+        except (FileNotFoundError, OSError) as __err_msg: raise LoadRaw(__err_msg, f'\nGot: "{filename}"')
```

### Comparing `maci-0.2.0/maci/__ini/iniload.py` & `maci-0.3.0/maci/_ini/iniload.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # iniload
 #########################################################################################################
 # Imports
-from configparser import ConfigParser as __ConfigParser
-from configparser import ExtendedInterpolation as __ExtendedInterpolation
+from typing import Union as _Union
+from configparser import ConfigParser as _ConfigParser
+from configparser import ExtendedInterpolation as _ExtendedInterpolation
 from ..error import IniLoad
 
 #########################################################################################################
 # Import ini file
-def iniload(filename: str) -> __ConfigParser:
+def iniload(filename: str, *, encoding: _Union[str, None]=None) -> _ConfigParser:
     """
     Imports ini data from a file.
 
     Returns a ConfigParser obj. Assign the output to var
 
     Enter ini file location as str to import.
 
@@ -19,16 +20,23 @@
 
     iniload('path/to/filename.ini')
 
     This is using the native configparser library shipped with the python standard library. Using ConfigParser method
     with ExtendedInterpolation enabled by default. For more information on the configparser library, 
     visit: https://docs.python.org/3/library/configparser.html
     """
+    # Error Checks
+    err_msg_file_type = "Only str is allowed for 'filename'"
+    err_msg_type_encoding = "Only str|None or valid option is allowed for 'encoding'"
+
+    if not isinstance(filename, str): raise IniLoad(err_msg_file_type, f'\nGot: {repr(filename)}')
+    if not isinstance(encoding, (str, type(None))): raise IniLoad(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
+
+    # Load file data
     try:
-        with open(filename, 'r') as f: pass
-    except TypeError as __err_msg: raise IniLoad(__err_msg, f'\nFILE: "{filename}"')
-    except ValueError as __err_msg: raise IniLoad(__err_msg, f'\nFILE: "{filename}"')
-    except FileNotFoundError as __err_msg: raise IniLoad(__err_msg, f'\nFILE: "{filename}"')
-
-    __parser = __ConfigParser(interpolation=__ExtendedInterpolation())
-    __parser.read(filename)
-    return __parser
+        with open(filename, 'r', encoding=encoding): pass
+    except (FileNotFoundError, OSError) as _err_msg: raise IniLoad(_err_msg, f'\nFILE: "{filename}"')
+    except LookupError: raise IniLoad(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
+
+    _parser = _ConfigParser(interpolation=_ExtendedInterpolation())
+    _parser.read(filename, encoding=encoding)
+    return _parser
```

### Comparing `maci-0.2.0/maci/__init__.py` & `maci-0.3.0/maci/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,91 @@
 """
 maci - by aaronater10
 
-Version 0.2.0
+Version 0.3.0
 
 The easy to use library for your data, configuration, and save files.
 
 Import or Export custom, or industry-common, data, config, and save files easily for
 your python program or script!
 
 See tutorials and docs here for more info: https://docs.macilib.org
 
 Source Code: https://github.com/aaronater10/maci
 """
+__version__ = '0.3.0'
+
 #########################################################################################################
 # Imports
 
 # Base Exceptions
 from . import error
 
+# Hints
+from . import hint
+
 # Native Lib
-from .__native.load import load
-#from .__native.loadstr import loadstr
-from .__native.loadraw import loadraw
-from .__native.loadattrs import loadattrs
-from .__native.dump import dump
-#from .__native.dumpstr import dumpstr
-from .__native.dumpraw import dumpraw
-from .__native.cleanformat import cleanformat
-from .__native.builddata import builddata
+from ._native.load import load
+from ._native.loaddict import loaddict
+from ._native.loadstr import loadstr
+from ._native.loadstrdict import loadstrdict
+from ._native.loadraw import loadraw
+from ._native.loadattrs import loadattrs
+from ._native.dump import dump
+from ._native.dumpstr import dumpstr
+from ._native.dumpraw import dumpraw
+from ._native.cleanformat import cleanformat
+from ._native.build import build
 
 # Hash Lib
-from .__hash.createfilehash import createfilehash
-from .__hash.comparefilehash import comparefilehash
+from ._hash.createfilehash import createfilehash
+from ._hash.comparefilehash import comparefilehash
+from ._hash.createhash import createhash
 
 # JSON Lib
-from .__json.jsonload import jsonload
-from .__json.jsonloadstr import jsonloadstr
-from .__json.jsondump import jsondump
-from .__json.jsondumpstr import jsondumpstr
+from ._json.jsonload import jsonload
+from ._json.jsonloadstr import jsonloadstr
+from ._json.jsondump import jsondump
+from ._json.jsondumpstr import jsondumpstr
 
 # YAML Lib
-from .__yaml.yamlload import yamlload
-from .__yaml.yamlloadstr import yamlloadstr
-from .__yaml.yamldump import yamldump
-from .__yaml.yamldumpstr import yamldumpstr
+from ._yaml.yamlload import yamlload
+from ._yaml.yamlloadstr import yamlloadstr
+from ._yaml.yamldump import yamldump
+from ._yaml.yamldumpstr import yamldumpstr
+
+# TOML Lib
+from ._toml.tomlload import tomlload
+from ._toml.tomlloadstr import tomlloadstr
+from ._toml.tomldump import tomldump
+from ._toml.tomldumpstr import tomldumpstr
 
 # INI Lib
-from .__ini.iniload import iniload
-from .__ini.inidump import inidump
-from .__ini.inibuildauto import inibuildauto
-from .__ini.inibuildmanual import inibuildmanual
+from ._ini.iniload import iniload
+from ._ini.inidump import inidump
+from ._ini.inibuildauto import inibuildauto
+from ._ini.inibuildmanual import inibuildmanual
 
 # XML Lib
-from .__xml.xmlload import xmlload
-from .__xml.xmlloadstr import xmlloadstr
-from .__xml.xmldump import xmldump
-from .__xml.xmldumpstr import xmldumpstr
-from .__xml.xmlbuildmanual import xmlbuildmanual
+from ._xml.xmlload import xmlload
+from ._xml.xmlloadstr import xmlloadstr
+from ._xml.xmldump import xmldump
+from ._xml.xmldumpstr import xmldumpstr
+from ._xml.xmlbuildmanual import xmlbuildmanual
 
 
 # Name compatibility aliases/deprecation from ported library
 def __getattr__(attr_name: str) -> object:
     # Native
     if attr_name == 'importfile': return load
     if attr_name == 'importfileraw': return loadraw
     if attr_name == 'importattrs': return loadattrs
     if attr_name == 'savefile': return dump
     if attr_name == 'exportfile': return dumpraw
-    if attr_name == 'appendfile': raise error.GeneralError('"appendfile" no longer available. Use "dumpraw" with mode="a" option')
+    if attr_name == 'appendfile': raise error.GeneralError('"appendfile" no longer available. Use "dumpraw" with append=True option')
     # JSON
     if attr_name == 'jsonimportfile': return jsonload
     if attr_name == 'jsonimportstr': return jsonloadstr
     if attr_name == 'jsonexportfile': return jsondump
     if attr_name == 'jsonexportstr': return jsondumpstr
     # YAML
     if attr_name == 'yamlimportfile': return yamlload
```

### Comparing `maci-0.2.0/maci/__json/jsondump.py` & `maci-0.3.0/maci/_json/jsonload.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,39 @@
-# jsondump
+# jsonload
 #########################################################################################################
 # Imports
 import json as __json
-from ..error import JsonDump
+from ..error import JsonLoad
 from typing import Union
 
 #########################################################################################################
-# Export json file
-def jsondump(filename: str, data: Union[str, int, float, bool, list, dict, tuple, None]) -> None:
+# Import json file
+def jsonload(filename: str, *, encoding: Union[str, None]=None) -> Union[list, dict, str, int, float, bool, None]:
     """
-    Exports a new file from python data type to json data.
-    
-    Enter new filename as str. Pass data for output to file
-    
+    Imports json data from a file
+
+    Returns data with matching python data type. Assign the output to var
+
+    Enter json file location as str to import.
+
     [Example Use]
 
-    jsondump('path/to/filename.json', data)    
+    jsonload('path/to/filename.json')
 
     This is using the native json library shipped with the python standard library. For more
     information on the json library, visit: https://docs.python.org/3/library/json.html
-    
     """
+    # Error Checks
+    err_msg_file_type = "Only str is allowed for 'filename'"
+    err_msg_type_encoding = "Only str|None or valid option is allowed for 'encoding'"
+
+    if not isinstance(filename, str): raise JsonLoad(err_msg_file_type, f'\nGot: {repr(filename)}')
+    if not isinstance(encoding, (str, type(None))): raise JsonLoad(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
+
+
+    # Import json file
     try:
-        # Export data to json file
-        with open(filename, 'w') as f:
-            __json.dump(data, f)
-    except TypeError as __err_msg: raise JsonDump(__err_msg, f'\nFILE: "{filename}" \nDATA:{data}')
-    except ValueError as __err_msg: raise JsonDump(__err_msg, f'\nFILE: "{filename}" \nDATA:{data}')
-    except FileNotFoundError as __err_msg: raise JsonDump(__err_msg, f'\nFILE: "{filename}"')
+        with open(filename, 'r', encoding=encoding) as f:
+            return __json.load(f)
+    except (FileNotFoundError, OSError) as __err_msg: raise JsonLoad(__err_msg, f'\nFILE: "{filename}"')
+    except __json.decoder.JSONDecodeError as __err_msg: raise JsonLoad(__err_msg, f'\nFILE: "{filename}"')
+    except LookupError: raise JsonLoad(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
```

### Comparing `maci-0.2.0/maci/__native/loadattrs.py` & `maci-0.3.0/maci/_native/loadattrs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 # loadattrs
 #########################################################################################################
 # Imports
+from typing import NewType as __NewType
+from typing import Union as __Union
 from ..error import LoadAttrs, Load
 from .load import load as __load
-from .load import MaciFileData as __MaciFileData
+from ..data import MaciDataObj as __MaciDataObj
 
 #########################################################################################################
 # Import Attributes from File
-class __MaciDummy:
-    class Class: """dummy class for hinting"""
 
-def loadattrs(filename: str, class_object: '__MaciDummy.Class') -> None:
+# Hinting reference name for "CustomClass" to denote a CustomClass can be used to dump data
+CustomClass = __NewType('CustomClass', object)
+
+def loadattrs(filename: str, class_object: CustomClass, *, encoding: __Union[str, None]=None, attr_name_dedup: bool=False, _ignore_maci_attr_check: bool=True) -> None:
     """
     Import saved attributes from file back into a custom class. This is done in-place
 
     Enter filename as str, Pass custom class object.
 
     [Example Use]
 
     loadattrs('path/of/filename', 'class_object')
+
+    [Warning]
+    Turning OFF 'attr_name_dedup' is not recommended as you gain the ability to overwrite
+    your attribute names that already preexist. This also may affect MaciDataObj behavior
+    including the ability to overwrite internal dunder names. This feature is meant to protect you from accidentally
+    duplicating an attribute name in a file that has already been created.
     """
     # Error Checks
-    __err_msg_type_str_filename = "Only str is allowed for filename"
-    __err_msg_type_class_obj = "Only a custom class object is allowed for class_object"
-    __err_msg_type_maci_obj = "Please use 'load' function to properly import a MaciFileData object"
+    err_msg_type_filename = "Only str is allowed for 'filename'"
+    __err_msg_type_class_obj = "Only a custom class object is allowed for 'class_object'"
+    __err_msg_type_maci_obj = "Please use 'load' function to properly import a 'MaciDataObj' object"
+
+    if not isinstance(filename, str): raise LoadAttrs(err_msg_type_filename, f'\nGot: {repr(filename)}')
 
-    if not isinstance(filename, str): raise LoadAttrs(__err_msg_type_str_filename, f'\nFILE: "{filename}"')
-    
     # Verify if Custom Class Obj
     _filter_objects = (str, int, float, bool, list, dict, tuple, set, type(None), bytes, complex, range, frozenset, bytearray, memoryview)
     if isinstance(class_object, _filter_objects):
-        raise LoadAttrs(__err_msg_type_class_obj, f'\nFILE: "{filename}" \nDATA: {class_object}')
+        raise LoadAttrs(__err_msg_type_class_obj, f'\nGot: {repr(class_object)}')
+
+    if isinstance(class_object, __MaciDataObj):
+        raise LoadAttrs(__err_msg_type_maci_obj, f'\nGot: {repr(class_object)}')
 
-    if isinstance(class_object, __MaciFileData):
-        raise LoadAttrs(__err_msg_type_maci_obj, f'\nFILE: "{filename}" \nDATA: {class_object}')
+    if isinstance(class_object, type(__MaciDataObj)):
+        raise LoadAttrs(__err_msg_type_maci_obj, f'\nGot: {repr(class_object)}')
 
     # Import Attrs from File and Inject into Given Class Object
 
     # Skip Key
-    __skip_object_key = ('_MaciFileData', '__maci_file_format_id')
+    __skip_object_key = ('_MaciDataObjConstructor', '__maci_obj_format_id')
 
     # Import Attrs
     try:
-        __imported_data = __load(filename)
+        __imported_data = __load(filename, attr_name_dedup=attr_name_dedup, encoding=encoding, _ignore_maci_attr_check=_ignore_maci_attr_check)
         for key,value in __imported_data.__dict__.items():
             if key.startswith(__skip_object_key): continue
             setattr(class_object, key, value)
     except Load as __err_msg:
         raise LoadAttrs(__err_msg, '')
 
     return None
```

### Comparing `maci-0.2.0/maci/__xml/xmldump.py` & `maci-0.3.0/maci/_xml/xmlloadstr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,29 @@
-# xmldump
+# xmlloadstr
 #########################################################################################################
 # Imports
-from ..__native.dumpraw import dumpraw
-from .xmldumpstr import xmldumpstr
-import xml.etree.ElementTree as __xml_etree
-from ..error import XmlDump
+import xml.etree.ElementTree as _xml_etree
+from ..error import XmlLoadStr
 
 #########################################################################################################
-# Export xml file
-def xmldump(filename: str, data: __xml_etree.Element) -> None:
+# Import xml str
+def xmlloadstr(xml_str_data: str) -> _xml_etree.Element:
     """
-    Exports a new file from xml Element obj as xml data
-    
-    Enter new filename as str. Pass ElementTree data for output to file
-    
+    Imports xml data from a string
+
+    Returns a xml Element. Assign the output to var
+
     [Example Use]
 
-    xmldump('path/to/filename.xml', Element_data)
+    xmlloadstr('<tag>data</tag>')
 
     This is using the native xml library via etree shipped with the python standard library.
     For more information on the xml.etree api, visit: https://docs.python.org/3/library/xml.etree.elementtree.html#module-xml.etree.ElementTree
     """
-    # Check for Error
-    __err_msg_str = f"Only str is allowed for filename"
-    __err_msg_etree = f"Only Element is allowed for data"
-
-    if not isinstance(filename, str): raise XmlDump(__err_msg_str, f'\nFILE: "{filename}"')
-    if not isinstance(data, __xml_etree.Element): raise XmlDump(__err_msg_etree, f"\nDATA: {data}")
-
-    # Export Data
-    try:
-        data = xmldumpstr(data)
-        dumpraw(filename, data)
-    except FileNotFoundError as __err_msg: raise XmlDump(__err_msg, f'\nFILE: "{filename}"')
+    # Error Checks
+    err_msg_str = f"Only str is allowed for 'xml_str_data'"
+
+    if not isinstance(xml_str_data, str): raise XmlLoadStr(err_msg_str, f'\nGot: {repr(xml_str_data)}')
+
+    # Load Str Data
+    try: return _xml_etree.fromstring(str(xml_str_data))
+    except _xml_etree.ParseError as __err_msg: raise XmlLoadStr(__err_msg, f'\nGot: {repr(xml_str_data)}')
```

### Comparing `maci-0.2.0/maci/__xml/xmldumpstr.py` & `maci-0.3.0/maci/_xml/xmldumpstr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # xmldumpstr
 #########################################################################################################
 # Imports
-import xml.etree.ElementTree as __xml_etree
+import xml.etree.ElementTree as _xml_etree
 from ..error import XmlDumpStr
 
 #########################################################################################################
 # Export xml str
-def xmldumpstr(data: __xml_etree.Element) -> str:
+def xmldumpstr(data: _xml_etree.Element, *, encoding: str='utf-8') -> str:
     """
-    Exports xml Element obj to a string
+    Exports xml Element object to a string
 
     Returns a str. Assign the output to var
 
     [Example Use]
 
     xmldumpstr(Element)
 
     This is using the native xml library via etree shipped with the python standard library.
     For more information on the xml.etree api, visit: https://docs.python.org/3/library/xml.etree.elementtree.html#module-xml.etree.ElementTree
     """
-    # Check for Error
-    __err_msg_etree = f"Only Element is allowed for data"
+    # Error Checks
+    err_msg_type_etree = "Only Element is allowed for 'data'"
+    err_msg_type_encoding = "Only str|None or valid option is allowed for 'encoding'"
 
-    if not isinstance(data, __xml_etree.Element): raise XmlDumpStr(__err_msg_etree, f'\nDATA: {data}')
+    if not isinstance(data, _xml_etree.Element): raise XmlDumpStr(err_msg_type_etree, f'\nGot: {repr(data)}')
+    if not isinstance(encoding, (str, type(None))): raise XmlDumpStr(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
     # Export Data
-    return __xml_etree.tostring(data).decode()
+    try: return _xml_etree.tostring(data).decode(encoding=encoding)
+    except LookupError: raise XmlDumpStr(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
```

### Comparing `maci-0.2.0/maci/__xml/xmlload.py` & `maci-0.3.0/maci/_xml/xmlload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 # xmlload
 #########################################################################################################
 # Imports
-import xml.etree.ElementTree as __xml_etree
+from typing import Union as _Union
+import xml.etree.ElementTree as _xml_etree
 from ..error import XmlLoad
 
 #########################################################################################################
 # Import xml file
-def xmlload(filename: str) -> __xml_etree.Element:
+def xmlload(filename: str, *, auto_get_root: bool=True) -> _Union[_xml_etree.Element, _xml_etree.ElementTree]:
     """
     Imports xml data from a file.
 
-    Returns a xml Parsed Element obj with the root. Assign the output to var
+    Returns the root Element object of the ElementTree parsed from a xml file by default. Assign the output to var
 
     Enter xml file location as str to import.
 
     [Example Use]
 
     xmlload('path/to/filename.xml')
 
     This is using the native xml library via etree shipped with the python standard library.
     For more information on the xml.etree api, visit: https://docs.python.org/3/library/xml.etree.elementtree.html#module-xml.etree.ElementTree
     """
-    __err_msg_str = f"Only str is allowed for filename"
-
-    if not isinstance(filename, str): raise XmlLoad(__err_msg_str, f'\nFILE: "{filename}"')
-
-    try: return __xml_etree.parse(filename).getroot()
-    except FileNotFoundError as __err_msg: raise XmlLoad(__err_msg, f'\nFILE: "{filename}"')
-    except __xml_etree.ParseError as __err_msg: raise XmlLoad(__err_msg, f'\nFILE: "{filename}"')
+    # Error Checks
+    err_msg_type_filename = "Only str is allowed for 'filename'"
+    err_msg_type_auto_get_root = "Only bool is allowed for 'auto_get_root'"
+
+    if not isinstance(filename, str): raise XmlLoad(err_msg_type_filename, f'\nGot: {repr(filename)}')
+    if not isinstance(auto_get_root, bool): raise XmlLoad(err_msg_type_auto_get_root, f'\nGot: {repr(auto_get_root)}')
+
+    # Load File Data
+    try:
+        if auto_get_root:
+            return _xml_etree.parse(filename).getroot()
+        return _xml_etree.parse(filename)
+    except (FileNotFoundError, OSError) as __err_msg: raise XmlLoad(__err_msg, f'\nGot: {repr(filename)}')
+    except _xml_etree.ParseError as __err_msg: raise XmlLoad(__err_msg, f'\nGot: {repr(filename)}')
```

### Comparing `maci-0.2.0/maci/__yaml/yamldumpstr.py` & `maci-0.3.0/maci/_yaml/yamldumpstr.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,12 +19,9 @@
 
     This is using the PyYAML framework installed as a dependency from pypi. It is only using the
     "safe_dump" method, which only supports standard YAML tags and cannot represent an arbitrary Python object.
     For more information on PyYAML, visit: https://pypi.org/project/PyYAML/
     
     """
     # Export data to yaml str
-    try:
-        return __yaml.safe_dump(data, stream=None).rstrip() # Strip trailing \n, yaml parser adds this oddly
-    except __yaml.representer.RepresenterError as __err_msg: raise YamlDumpStr(__err_msg, f'\nDATA: {data}')
-    except TypeError as __err_msg: raise YamlDumpStr(__err_msg, f'\nDATA: {data}')
-    except ValueError as __err_msg: raise YamlDumpStr(__err_msg, f'\nDATA: {data}')
+    try: return __yaml.safe_dump(data, stream=None).rstrip() # Strip trailing \n, yaml parser adds this automatically
+    except __yaml.error.YAMLError as __err_msg: raise YamlDumpStr(__err_msg, f'\nGot: {repr(data)}')
```

### Comparing `maci-0.2.0/maci/__yaml/yamlload.py` & `maci-0.3.0/maci/_toml/tomlload.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-# yamlload
+# tomlload
 #########################################################################################################
 # Imports
-from typing import Any as __Any
-import yaml as __yaml
-from ..error import YamlLoad
+import tomli as _tomli
+from ..error import TomlLoad
+from typing import Dict as _Dict
+from typing import Any as _Any
 
 #########################################################################################################
-# Import yaml file
-def yamlload(filename: str) -> __Any:
+# Load toml file
+def tomlload(filename: str) -> _Dict[str, _Any]:
     """
-    Imports yaml data from a file.
+    Loads toml data from a file
 
-    Returns data with matching python data type. Assign the output to var
+    Returns dict data with matching python data type. Assign the output to var
 
-    Enter yaml file location as str to import.
+    Enter toml file location as str to load
 
     [Example Use]
 
-    yamlload('path/to/filename.yml')
+    tomlload('path/to/filename.toml')
 
-    This is using the PyYAML framework installed as a dependency from pypi. It is only using the
-    "safe_load" method to protect from untrusted input.
-    For more information on PyYAML, visit: https://pypi.org/project/PyYAML/
+    This is using the tomli library installed as a dependency from pypi.
+    For more information on tomli, visit: https://pypi.org/project/tomli/
     """
-    # Import yaml file
+    # Error Checks
+    err_msg_type_file = "Only str is allowed for 'filename'"
+
+    if not isinstance(filename, str): raise TomlLoad(err_msg_type_file, f'\nGot: {repr(filename)}')
+
+    # Load toml file
     try:
-        with open(filename, 'r') as f:
-            return __yaml.safe_load(f)
-    except FileNotFoundError as __err_msg: raise YamlLoad(__err_msg, f'\nFILE: "{filename}"')
-    except OSError as __err_msg: raise YamlLoad(__err_msg, f'\nFILE: "{filename}"')
-    except __yaml.scanner.ScannerError as __err_msg: raise YamlLoad(__err_msg, f'\nFILE: "{filename}"')
-    except __yaml.parser.ParserError as __err_msg: raise YamlLoad(__err_msg, f'\nFILE: "{filename}"')
-    except ValueError as __err_msg: raise YamlLoad(__err_msg, f'\nFILE: "{filename}"')
-    except TypeError as __err_msg: raise YamlLoad(__err_msg, f'\nFILE: "{filename}"')
+        with open(filename, 'rb') as f:
+            return _tomli.load(f)
+    except (FileNotFoundError, OSError) as _err_msg: raise TomlLoad(_err_msg, f'\nFILE: "{filename}"')
+    except _tomli.TOMLDecodeError as _err_msg: raise TomlLoad(_err_msg, f'\nFILE: "{filename}"')
```

### Comparing `maci-0.2.0/maci.egg-info/PKG-INFO` & `maci-0.3.0/maci.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.2.0
+Version: 0.3.0
 Summary: The easy to use library for your data, configuration, and save files
-Home-page: https://github.com/aaronater10/maci
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
+Project-URL: Docs, https://docs.macilib.org
+Project-URL: Code, https://github.com/aaronater10/maci
+Project-URL: Bugs, https://github.com/aaronater10/maci/issues
+Project-URL: CI, https://github.com/aaronater10/maci/actions
 Keywords: maci,aaronater10,python,py,config,file,export,parse,text file,cfg,conf,save file,config file,db,database,simple,configuration,alternative,safe,ini,json,xml,yml,data,import
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.2.0
+##### Latest Version: 0.3.0
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.2.0/maci.egg-info/SOURCES.txt` & `maci-0.3.0/maci.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
 maci/__init__.py
+maci/data.py
 maci/error.py
+maci/hint.py
 maci.egg-info/PKG-INFO
 maci.egg-info/SOURCES.txt
 maci.egg-info/dependency_links.txt
 maci.egg-info/requires.txt
 maci.egg-info/top_level.txt
-maci/__hash/comparefilehash.py
-maci/__hash/createfilehash.py
-maci/__ini/inibuildauto.py
-maci/__ini/inibuildmanual.py
-maci/__ini/inidump.py
-maci/__ini/iniload.py
-maci/__json/jsondump.py
-maci/__json/jsondumpstr.py
-maci/__json/jsonload.py
-maci/__json/jsonloadstr.py
-maci/__native/builddata.py
-maci/__native/cleanformat.py
-maci/__native/dump.py
-maci/__native/dumpraw.py
-maci/__native/load.py
-maci/__native/loadattrs.py
-maci/__native/loadraw.py
-maci/__xml/xmlbuildmanual.py
-maci/__xml/xmldump.py
-maci/__xml/xmldumpstr.py
-maci/__xml/xmlload.py
-maci/__xml/xmlloadstr.py
-maci/__yaml/yamldump.py
-maci/__yaml/yamldumpstr.py
-maci/__yaml/yamlload.py
-maci/__yaml/yamlloadstr.py
+maci/_hash/comparefilehash.py
+maci/_hash/createfilehash.py
+maci/_hash/createhash.py
+maci/_ini/inibuildauto.py
+maci/_ini/inibuildmanual.py
+maci/_ini/inidump.py
+maci/_ini/iniload.py
+maci/_json/jsondump.py
+maci/_json/jsondumpstr.py
+maci/_json/jsonload.py
+maci/_json/jsonloadstr.py
+maci/_native/build.py
+maci/_native/cleanformat.py
+maci/_native/dump.py
+maci/_native/dumpraw.py
+maci/_native/dumpstr.py
+maci/_native/load.py
+maci/_native/loadattrs.py
+maci/_native/loaddict.py
+maci/_native/loadraw.py
+maci/_native/loadstr.py
+maci/_native/loadstrdict.py
+maci/_toml/tomldump.py
+maci/_toml/tomldumpstr.py
+maci/_toml/tomlload.py
+maci/_toml/tomlloadstr.py
+maci/_xml/xmlbuildmanual.py
+maci/_xml/xmldump.py
+maci/_xml/xmldumpstr.py
+maci/_xml/xmlload.py
+maci/_xml/xmlloadstr.py
+maci/_yaml/yamldump.py
+maci/_yaml/yamldumpstr.py
+maci/_yaml/yamlload.py
+maci/_yaml/yamlloadstr.py
```

