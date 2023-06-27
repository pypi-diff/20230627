# Comparing `tmp/dissect.shellitem-3.6.dev1.tar.gz` & `tmp/dissect.shellitem-3.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.shellitem-3.6.dev1.tar", last modified: Fri Jun 16 12:50:37 2023, max compression
+gzip compressed data, was "dissect.shellitem-3.6.dev2.tar", last modified: Tue Jun 27 07:49:19 2023, max compression
```

## Comparing `dissect.shellitem-3.6.dev1.tar` & `dissect.shellitem-3.6.dev2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:37.208426 dissect.shellitem-3.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-16 12:50:37.208426 dissect.shellitem-3.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:37.192426 dissect.shellitem-3.6.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:37.200426 dissect.shellitem-3.6.dev1/dissect/shellitem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/dissect/shellitem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:37.204426 dissect.shellitem-3.6.dev1/dissect/shellitem/lnk/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/dissect/shellitem/lnk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/dissect/shellitem/lnk/c_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17611 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/dissect/shellitem/lnk/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:37.204426 dissect.shellitem-3.6.dev1/dissect/shellitem/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/dissect/shellitem/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/dissect/shellitem/tools/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:37.200426 dissect.shellitem-3.6.dev1/dissect.shellitem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-16 12:50:37.000000 dissect.shellitem-3.6.dev1/dissect.shellitem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-16 12:50:37.000000 dissect.shellitem-3.6.dev1/dissect.shellitem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:50:37.000000 dissect.shellitem-3.6.dev1/dissect.shellitem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-16 12:50:37.000000 dissect.shellitem-3.6.dev1/dissect.shellitem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:50:37.000000 dissect.shellitem-3.6.dev1/dissect.shellitem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:50:37.000000 dissect.shellitem-3.6.dev1/dissect.shellitem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-16 12:50:27.000000 dissect.shellitem-3.6.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:50:37.212426 dissect.shellitem-3.6.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:37.204426 dissect.shellitem-3.6.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:37.208426 dissect.shellitem-3.6.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/data/downloads.win81.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/data/local.directory.seven.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/data/modified_remote.file.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/data/remote.directory.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/data/remote.file.xp.lnk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:37.208426 dissect.shellitem-3.6.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tests/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:50:23.000000 dissect.shellitem-3.6.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:19.625272 dissect.shellitem-3.6.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-27 07:49:19.625272 dissect.shellitem-3.6.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:19.609272 dissect.shellitem-3.6.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:19.617272 dissect.shellitem-3.6.dev2/dissect/shellitem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/dissect/shellitem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:19.621272 dissect.shellitem-3.6.dev2/dissect/shellitem/lnk/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/dissect/shellitem/lnk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/dissect/shellitem/lnk/c_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17611 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/dissect/shellitem/lnk/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:19.621272 dissect.shellitem-3.6.dev2/dissect/shellitem/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/dissect/shellitem/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/dissect/shellitem/tools/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:19.617272 dissect.shellitem-3.6.dev2/dissect.shellitem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-27 07:49:19.000000 dissect.shellitem-3.6.dev2/dissect.shellitem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-27 07:49:19.000000 dissect.shellitem-3.6.dev2/dissect.shellitem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:19.000000 dissect.shellitem-3.6.dev2/dissect.shellitem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 07:49:19.000000 dissect.shellitem-3.6.dev2/dissect.shellitem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 07:49:19.000000 dissect.shellitem-3.6.dev2/dissect.shellitem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:49:19.000000 dissect.shellitem-3.6.dev2/dissect.shellitem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-27 07:49:09.000000 dissect.shellitem-3.6.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:19.625272 dissect.shellitem-3.6.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:19.621272 dissect.shellitem-3.6.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:19.625272 dissect.shellitem-3.6.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/data/downloads.win81.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/data/local.directory.seven.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/data/modified_remote.file.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/data/remote.directory.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/data/remote.file.xp.lnk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:19.625272 dissect.shellitem-3.6.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tests/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 07:49:05.000000 dissect.shellitem-3.6.dev2/tox.ini
```

### Comparing `dissect.shellitem-3.6.dev1/LICENSE` & `dissect.shellitem-3.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/PKG-INFO` & `dissect.shellitem-3.6.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.shellitem-3.6.dev1/README.md` & `dissect.shellitem-3.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/dissect/shellitem/lnk/c_lnk.py` & `dissect.shellitem-3.6.dev2/dissect/shellitem/lnk/c_lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/dissect/shellitem/lnk/lnk.py` & `dissect.shellitem-3.6.dev2/dissect/shellitem/lnk/lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/dissect/shellitem/tools/lnk.py` & `dissect.shellitem-3.6.dev2/dissect/shellitem/tools/lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/dissect.shellitem.egg-info/PKG-INFO` & `dissect.shellitem-3.6.dev2/dissect.shellitem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.shellitem-3.6.dev1/dissect.shellitem.egg-info/SOURCES.txt` & `dissect.shellitem-3.6.dev2/dissect.shellitem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/pyproject.toml` & `dissect.shellitem-3.6.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/tests/conftest.py` & `dissect.shellitem-3.6.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/tests/data/downloads.win81.lnk` & `dissect.shellitem-3.6.dev2/tests/data/downloads.win81.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/tests/data/local.directory.seven.lnk` & `dissect.shellitem-3.6.dev2/tests/data/local.directory.seven.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/tests/data/modified_remote.file.xp.lnk` & `dissect.shellitem-3.6.dev2/tests/data/modified_remote.file.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/tests/data/remote.directory.xp.lnk` & `dissect.shellitem-3.6.dev2/tests/data/remote.directory.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/tests/data/remote.file.xp.lnk` & `dissect.shellitem-3.6.dev2/tests/data/remote.file.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/tests/docs/Makefile` & `dissect.shellitem-3.6.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/tests/docs/conf.py` & `dissect.shellitem-3.6.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/tests/test_lnk.py` & `dissect.shellitem-3.6.dev2/tests/test_lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.6.dev1/tox.ini` & `dissect.shellitem-3.6.dev2/tox.ini`

 * *Files identical despite different names*

