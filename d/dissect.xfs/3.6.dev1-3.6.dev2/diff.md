# Comparing `tmp/dissect.xfs-3.6.dev1.tar.gz` & `tmp/dissect.xfs-3.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.xfs-3.6.dev1.tar", last modified: Fri Jun 16 12:51:33 2023, max compression
+gzip compressed data, was "dissect.xfs-3.6.dev2.tar", last modified: Tue Jun 27 07:49:46 2023, max compression
```

## Comparing `dissect.xfs-3.6.dev1.tar` & `dissect.xfs-3.6.dev2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:33.120006 dissect.xfs-3.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-16 12:51:33.120006 dissect.xfs-3.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:33.100006 dissect.xfs-3.6.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:33.112006 dissect.xfs-3.6.dev1/dissect/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/dissect/xfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41820 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/dissect/xfs/c_xfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/dissect/xfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/dissect/xfs/xfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:33.112006 dissect.xfs-3.6.dev1/dissect.xfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-16 12:51:33.000000 dissect.xfs-3.6.dev1/dissect.xfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-16 12:51:33.000000 dissect.xfs-3.6.dev1/dissect.xfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:51:33.000000 dissect.xfs-3.6.dev1/dissect.xfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:51:33.000000 dissect.xfs-3.6.dev1/dissect.xfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:51:33.000000 dissect.xfs-3.6.dev1/dissect.xfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-16 12:51:23.000000 dissect.xfs-3.6.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:51:33.120006 dissect.xfs-3.6.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:33.116006 dissect.xfs-3.6.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:33.116006 dissect.xfs-3.6.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/data/xfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42673 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/data/xfs_bigtime.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    45520 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/data/xfs_sparse.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/data/xfs_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42015 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/data/xfs_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/data/xfs_symlink_test3.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:51:33.120006 dissect.xfs-3.6.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tests/test_xfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:51:19.000000 dissect.xfs-3.6.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:46.085658 dissect.xfs-3.6.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-27 07:49:46.085658 dissect.xfs-3.6.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:46.077657 dissect.xfs-3.6.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:46.081658 dissect.xfs-3.6.dev2/dissect/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/dissect/xfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41820 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/dissect/xfs/c_xfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/dissect/xfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/dissect/xfs/xfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:46.081658 dissect.xfs-3.6.dev2/dissect.xfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-27 07:49:46.000000 dissect.xfs-3.6.dev2/dissect.xfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-27 07:49:46.000000 dissect.xfs-3.6.dev2/dissect.xfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:46.000000 dissect.xfs-3.6.dev2/dissect.xfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 07:49:46.000000 dissect.xfs-3.6.dev2/dissect.xfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:49:46.000000 dissect.xfs-3.6.dev2/dissect.xfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-27 07:49:34.000000 dissect.xfs-3.6.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:46.085658 dissect.xfs-3.6.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:46.081658 dissect.xfs-3.6.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:46.081658 dissect.xfs-3.6.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/data/xfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42673 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/data/xfs_bigtime.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    45520 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/data/xfs_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/data/xfs_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42015 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/data/xfs_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/data/xfs_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:46.085658 dissect.xfs-3.6.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tests/test_xfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 07:49:25.000000 dissect.xfs-3.6.dev2/tox.ini
```

### Comparing `dissect.xfs-3.6.dev1/LICENSE` & `dissect.xfs-3.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/PKG-INFO` & `dissect.xfs-3.6.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.xfs
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
 Project-URL: repository, https://github.com/fox-it/dissect.xfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.xfs-3.6.dev1/README.md` & `dissect.xfs-3.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/dissect/xfs/c_xfs.py` & `dissect.xfs-3.6.dev2/dissect/xfs/c_xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/dissect/xfs/xfs.py` & `dissect.xfs-3.6.dev2/dissect/xfs/xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/dissect.xfs.egg-info/PKG-INFO` & `dissect.xfs-3.6.dev2/dissect.xfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.xfs
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
 Project-URL: repository, https://github.com/fox-it/dissect.xfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.xfs-3.6.dev1/dissect.xfs.egg-info/SOURCES.txt` & `dissect.xfs-3.6.dev2/dissect.xfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/pyproject.toml` & `dissect.xfs-3.6.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/tests/data/xfs.bin.gz` & `dissect.xfs-3.6.dev2/tests/data/xfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/tests/data/xfs_bigtime.bin.gz` & `dissect.xfs-3.6.dev2/tests/data/xfs_bigtime.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/tests/data/xfs_sparse.bin.gz` & `dissect.xfs-3.6.dev2/tests/data/xfs_sparse.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/tests/data/xfs_symlink_test1.bin.gz` & `dissect.xfs-3.6.dev2/tests/data/xfs_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/tests/data/xfs_symlink_test2.bin.gz` & `dissect.xfs-3.6.dev2/tests/data/xfs_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/tests/data/xfs_symlink_test3.bin.gz` & `dissect.xfs-3.6.dev2/tests/data/xfs_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/tests/docs/Makefile` & `dissect.xfs-3.6.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/tests/docs/conf.py` & `dissect.xfs-3.6.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/tests/test_xfs.py` & `dissect.xfs-3.6.dev2/tests/test_xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.6.dev1/tox.ini` & `dissect.xfs-3.6.dev2/tox.ini`

 * *Files identical despite different names*

