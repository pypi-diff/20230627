# Comparing `tmp/dissect.extfs-3.6.dev1.tar.gz` & `tmp/dissect.extfs-3.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.extfs-3.6.dev1.tar", last modified: Fri Jun 16 12:49:44 2023, max compression
+gzip compressed data, was "dissect.extfs-3.6.dev2.tar", last modified: Tue Jun 27 07:49:11 2023, max compression
```

## Comparing `dissect.extfs-3.6.dev1.tar` & `dissect.extfs-3.6.dev2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.442848 dissect.extfs-3.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-16 12:49:44.442848 dissect.extfs-3.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.434847 dissect.extfs-3.6.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.438847 dissect.extfs-3.6.dev1/dissect/extfs/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/c_jdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/extfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/dissect/extfs/journal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.438847 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-16 12:49:44.000000 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-16 12:49:44.000000 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:49:44.000000 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:49:44.000000 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:49:44.000000 dissect.extfs-3.6.dev1/dissect.extfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-16 12:49:32.000000 dissect.extfs-3.6.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:49:44.442848 dissect.extfs-3.6.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.438847 dissect.extfs-3.6.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:27.000000 dissect.extfs-3.6.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.442848 dissect.extfs-3.6.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/data/ext4.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/data/ext4_sparse.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test3.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:44.442848 dissect.extfs-3.6.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tests/test_ext4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:49:26.000000 dissect.extfs-3.6.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:11.264058 dissect.extfs-3.6.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-27 07:49:11.264058 dissect.extfs-3.6.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:11.252057 dissect.extfs-3.6.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:11.260058 dissect.extfs-3.6.dev2/dissect/extfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/dissect/extfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/dissect/extfs/c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/dissect/extfs/c_jdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/dissect/extfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/dissect/extfs/extfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/dissect/extfs/journal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:11.256058 dissect.extfs-3.6.dev2/dissect.extfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-27 07:49:11.000000 dissect.extfs-3.6.dev2/dissect.extfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-27 07:49:11.000000 dissect.extfs-3.6.dev2/dissect.extfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:11.000000 dissect.extfs-3.6.dev2/dissect.extfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 07:49:11.000000 dissect.extfs-3.6.dev2/dissect.extfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:49:11.000000 dissect.extfs-3.6.dev2/dissect.extfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-27 07:48:57.000000 dissect.extfs-3.6.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:11.264058 dissect.extfs-3.6.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:11.260058 dissect.extfs-3.6.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:11.260058 dissect.extfs-3.6.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/data/ext4.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/data/ext4_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/data/ext4_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/data/ext4_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/data/ext4_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:11.260058 dissect.extfs-3.6.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tests/test_ext4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 07:48:46.000000 dissect.extfs-3.6.dev2/tox.ini
```

### Comparing `dissect.extfs-3.6.dev1/LICENSE` & `dissect.extfs-3.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/PKG-INFO` & `dissect.extfs-3.6.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.extfs-3.6.dev1/README.md` & `dissect.extfs-3.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/dissect/extfs/c_ext.py` & `dissect.extfs-3.6.dev2/dissect/extfs/c_ext.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/dissect/extfs/c_jdb2.py` & `dissect.extfs-3.6.dev2/dissect/extfs/c_jdb2.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/dissect/extfs/extfs.py` & `dissect.extfs-3.6.dev2/dissect/extfs/extfs.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/dissect/extfs/journal.py` & `dissect.extfs-3.6.dev2/dissect/extfs/journal.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/dissect.extfs.egg-info/PKG-INFO` & `dissect.extfs-3.6.dev2/dissect.extfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.extfs-3.6.dev1/dissect.extfs.egg-info/SOURCES.txt` & `dissect.extfs-3.6.dev2/dissect.extfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/pyproject.toml` & `dissect.extfs-3.6.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/tests/conftest.py` & `dissect.extfs-3.6.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/tests/data/ext4.bin.gz` & `dissect.extfs-3.6.dev2/tests/data/ext4.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/tests/data/ext4_sparse.bin.gz` & `dissect.extfs-3.6.dev2/tests/data/ext4_sparse.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test1.bin.gz` & `dissect.extfs-3.6.dev2/tests/data/ext4_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test2.bin.gz` & `dissect.extfs-3.6.dev2/tests/data/ext4_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/tests/data/ext4_symlink_test3.bin.gz` & `dissect.extfs-3.6.dev2/tests/data/ext4_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/tests/docs/Makefile` & `dissect.extfs-3.6.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/tests/docs/conf.py` & `dissect.extfs-3.6.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/tests/test_ext4.py` & `dissect.extfs-3.6.dev2/tests/test_ext4.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.6.dev1/tox.ini` & `dissect.extfs-3.6.dev2/tox.ini`

 * *Files identical despite different names*

