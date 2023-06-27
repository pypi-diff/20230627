# Comparing `tmp/dissect.ntfs-3.6.dev2.tar.gz` & `tmp/dissect.ntfs-3.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ntfs-3.6.dev2.tar", last modified: Fri Jun 23 15:01:23 2023, max compression
+gzip compressed data, was "dissect.ntfs-3.6.dev4.tar", last modified: Tue Jun 27 07:49:07 2023, max compression
```

## Comparing `dissect.ntfs-3.6.dev2.tar` & `dissect.ntfs-3.6.dev4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.508539 dissect.ntfs-3.6.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-23 15:01:23.508539 dissect.ntfs-3.6.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.496539 dissect.ntfs-3.6.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.500539 dissect.ntfs-3.6.dev2/dissect/ntfs/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/c_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/mft.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/secure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.496539 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-23 15:01:23.000000 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-23 15:01:23.000000 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:01:23.000000 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 15:01:23.000000 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 15:01:23.000000 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-23 15:01:13.000000 dissect.ntfs-3.6.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:01:23.508539 dissect.ntfs-3.6.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.504539 dissect.ntfs-3.6.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.508539 dissect.ntfs-3.6.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/data/boot_2m.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/data/mft.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)   908628 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/data/ntfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/data/ntfs_fragmented_mft.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/data/sds.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.508539 dissect.ntfs-3.6.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_mft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_secure.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.263544 dissect.ntfs-3.6.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-27 07:49:07.263544 dissect.ntfs-3.6.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.243543 dissect.ntfs-3.6.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.251544 dissect.ntfs-3.6.dev4/dissect/ntfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/c_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/mft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.247543 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-27 07:49:07.000000 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-27 07:49:07.000000 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:07.000000 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 07:49:07.000000 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:49:07.000000 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-27 07:48:57.000000 dissect.ntfs-3.6.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:07.263544 dissect.ntfs-3.6.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.259544 dissect.ntfs-3.6.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:54.000000 dissect.ntfs-3.6.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.259544 dissect.ntfs-3.6.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/data/boot_2m.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/data/mft.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   908628 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/data/ntfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/data/ntfs_fragmented_mft.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/data/sds.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.263544 dissect.ntfs-3.6.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_mft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tox.ini
```

### Comparing `dissect.ntfs-3.6.dev2/LICENSE` & `dissect.ntfs-3.6.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/PKG-INFO` & `dissect.ntfs-3.6.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.6.dev2
+Version: 3.6.dev4
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ntfs-3.6.dev2/README.md` & `dissect.ntfs-3.6.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/dissect/ntfs/__init__.py` & `dissect.ntfs-3.6.dev4/dissect/ntfs/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/dissect/ntfs/attr.py` & `dissect.ntfs-3.6.dev4/dissect/ntfs/attr.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/dissect/ntfs/c_ntfs.py` & `dissect.ntfs-3.6.dev4/dissect/ntfs/c_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/dissect/ntfs/index.py` & `dissect.ntfs-3.6.dev4/dissect/ntfs/index.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/dissect/ntfs/mft.py` & `dissect.ntfs-3.6.dev4/dissect/ntfs/mft.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/dissect/ntfs/ntfs.py` & `dissect.ntfs-3.6.dev4/dissect/ntfs/ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/dissect/ntfs/secure.py` & `dissect.ntfs-3.6.dev4/dissect/ntfs/secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/dissect/ntfs/stream.py` & `dissect.ntfs-3.6.dev4/dissect/ntfs/stream.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/dissect/ntfs/usnjrnl.py` & `dissect.ntfs-3.6.dev4/dissect/ntfs/usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/dissect/ntfs/util.py` & `dissect.ntfs-3.6.dev4/dissect/ntfs/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     :class:`~dissect.ntfs.util.AttributeCollection`, either empty or containing one or more attributes.
     """
 
     def __getattr__(self, attr: str) -> AttributeCollection:
         if attr in ATTRIBUTE_TYPE_CODE:
             return self[ATTRIBUTE_TYPE_CODE[attr]]
 
-        return super().__getattribute__(self, attr)
+        return super().__getattribute__(attr)
 
     def __getitem__(self, item: Union[ATTRIBUTE_TYPE_CODE, int]) -> AttributeCollection:
         if isinstance(item, EnumInstance):
             item = item.value
         return self.data.get(item, AttributeCollection())
 
     def __contains__(self, key: Union[ATTRIBUTE_TYPE_CODE, int]) -> bool:
@@ -95,15 +95,15 @@
     def __getattr__(self, attr: str) -> Any:
         if len(self) == 0:
             raise AttributeError("Attribute not found")
 
         if hasattr(self[0], attr):
             return getattr(self[0], attr)
 
-        return super().__getattribute__(self, attr)
+        return super().__getattribute__(attr)
 
     def open(self, allocated: bool = False) -> BinaryIO:
         """Open the data streams on a list of attributes, resident or non-resident.
 
         Args:
             allocated: Use the actual stream size or the allocated stream size (i.e. include slack space or not).
```

### Comparing `dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/PKG-INFO` & `dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.6.dev2
+Version: 3.6.dev4
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/SOURCES.txt` & `dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/pyproject.toml` & `dissect.ntfs-3.6.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/conftest.py` & `dissect.ntfs-3.6.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/data/boot_2m.bin.gz` & `dissect.ntfs-3.6.dev4/tests/data/boot_2m.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/data/mft.bin.gz` & `dissect.ntfs-3.6.dev4/tests/data/mft.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/data/ntfs.bin.gz` & `dissect.ntfs-3.6.dev4/tests/data/ntfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/data/ntfs_fragmented_mft.csv.gz` & `dissect.ntfs-3.6.dev4/tests/data/ntfs_fragmented_mft.csv.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/data/sds.bin.gz` & `dissect.ntfs-3.6.dev4/tests/data/sds.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/docs/Makefile` & `dissect.ntfs-3.6.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/docs/conf.py` & `dissect.ntfs-3.6.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/test_attr.py` & `dissect.ntfs-3.6.dev4/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/test_index.py` & `dissect.ntfs-3.6.dev4/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/test_mft.py` & `dissect.ntfs-3.6.dev4/tests/test_mft.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/test_ntfs.py` & `dissect.ntfs-3.6.dev4/tests/test_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/test_secure.py` & `dissect.ntfs-3.6.dev4/tests/test_secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/test_usnjrnl.py` & `dissect.ntfs-3.6.dev4/tests/test_usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tests/test_util.py` & `dissect.ntfs-3.6.dev4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev2/tox.ini` & `dissect.ntfs-3.6.dev4/tox.ini`

 * *Files identical despite different names*

