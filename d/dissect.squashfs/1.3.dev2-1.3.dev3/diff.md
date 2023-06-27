# Comparing `tmp/dissect.squashfs-1.3.dev2.tar.gz` & `tmp/dissect.squashfs-1.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.squashfs-1.3.dev2.tar", last modified: Fri Jun 16 15:32:53 2023, max compression
+gzip compressed data, was "dissect.squashfs-1.3.dev3.tar", last modified: Tue Jun 27 07:49:27 2023, max compression
```

## Comparing `dissect.squashfs-1.3.dev2.tar` & `dissect.squashfs-1.3.dev3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.473765 dissect.squashfs-1.3.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-16 15:32:53.473765 dissect.squashfs-1.3.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.457765 dissect.squashfs-1.3.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.465765 dissect.squashfs-1.3.dev2/dissect/squashfs/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/dissect/squashfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/dissect/squashfs/c_squashfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/dissect/squashfs/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/dissect/squashfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/dissect/squashfs/squashfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.465765 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-16 15:32:53.000000 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-16 15:32:53.000000 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:32:53.000000 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-16 15:32:53.000000 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 15:32:53.000000 dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-16 15:32:42.000000 dissect.squashfs-1.3.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:32:53.473765 dissect.squashfs-1.3.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.469765 dissect.squashfs-1.3.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.473765 dissect.squashfs-1.3.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/gzip-opts.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/gzip.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/lz4.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/lzma.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/lzo.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/xz.sqfs
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/data/zstd.sqfs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:32:53.473765 dissect.squashfs-1.3.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tests/test_squashfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-16 15:32:36.000000 dissect.squashfs-1.3.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:27.891682 dissect.squashfs-1.3.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-27 07:49:27.891682 dissect.squashfs-1.3.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:27.875682 dissect.squashfs-1.3.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:27.883682 dissect.squashfs-1.3.dev3/dissect/squashfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/dissect/squashfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/dissect/squashfs/c_squashfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/dissect/squashfs/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/dissect/squashfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/dissect/squashfs/squashfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:27.883682 dissect.squashfs-1.3.dev3/dissect.squashfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-27 07:49:27.000000 dissect.squashfs-1.3.dev3/dissect.squashfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-27 07:49:27.000000 dissect.squashfs-1.3.dev3/dissect.squashfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:27.000000 dissect.squashfs-1.3.dev3/dissect.squashfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 07:49:27.000000 dissect.squashfs-1.3.dev3/dissect.squashfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:49:27.000000 dissect.squashfs-1.3.dev3/dissect.squashfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-27 07:49:16.000000 dissect.squashfs-1.3.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:27.891682 dissect.squashfs-1.3.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:27.887682 dissect.squashfs-1.3.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:27.887682 dissect.squashfs-1.3.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/data/gzip-opts.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/data/gzip.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/data/lz4.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/data/lzma.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/data/lzo.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/data/xz.sqfs
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/data/zstd.sqfs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:27.891682 dissect.squashfs-1.3.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tests/test_squashfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-27 07:49:11.000000 dissect.squashfs-1.3.dev3/tox.ini
```

### Comparing `dissect.squashfs-1.3.dev2/LICENSE` & `dissect.squashfs-1.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/PKG-INFO` & `dissect.squashfs-1.3.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.squashfs
-Version: 1.3.dev2
+Version: 1.3.dev3
 Summary: A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.squashfs
 Project-URL: repository, https://github.com/fox-it/dissect.squashfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.squashfs-1.3.dev2/README.md` & `dissect.squashfs-1.3.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/dissect/squashfs/c_squashfs.py` & `dissect.squashfs-1.3.dev3/dissect/squashfs/c_squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/dissect/squashfs/compression.py` & `dissect.squashfs-1.3.dev3/dissect/squashfs/compression.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/dissect/squashfs/squashfs.py` & `dissect.squashfs-1.3.dev3/dissect/squashfs/squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/PKG-INFO` & `dissect.squashfs-1.3.dev3/dissect.squashfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.squashfs
-Version: 1.3.dev2
+Version: 1.3.dev3
 Summary: A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.squashfs
 Project-URL: repository, https://github.com/fox-it/dissect.squashfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.squashfs-1.3.dev2/dissect.squashfs.egg-info/SOURCES.txt` & `dissect.squashfs-1.3.dev3/dissect.squashfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/pyproject.toml` & `dissect.squashfs-1.3.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/conftest.py` & `dissect.squashfs-1.3.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/data/gzip-opts.sqfs` & `dissect.squashfs-1.3.dev3/tests/data/gzip-opts.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/data/gzip.sqfs` & `dissect.squashfs-1.3.dev3/tests/data/gzip.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/data/lz4.sqfs` & `dissect.squashfs-1.3.dev3/tests/data/lz4.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/data/lzma.sqfs` & `dissect.squashfs-1.3.dev3/tests/data/lzma.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/data/lzo.sqfs` & `dissect.squashfs-1.3.dev3/tests/data/lzo.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/data/xz.sqfs` & `dissect.squashfs-1.3.dev3/tests/data/xz.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/data/zstd.sqfs` & `dissect.squashfs-1.3.dev3/tests/data/zstd.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/docs/Makefile` & `dissect.squashfs-1.3.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/docs/conf.py` & `dissect.squashfs-1.3.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tests/test_squashfs.py` & `dissect.squashfs-1.3.dev3/tests/test_squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.3.dev2/tox.ini` & `dissect.squashfs-1.3.dev3/tox.ini`

 * *Files identical despite different names*

