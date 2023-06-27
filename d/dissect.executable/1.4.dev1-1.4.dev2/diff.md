# Comparing `tmp/dissect.executable-1.4.dev1.tar.gz` & `tmp/dissect.executable-1.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.executable-1.4.dev1.tar", last modified: Fri Jun 16 12:49:38 2023, max compression
+gzip compressed data, was "dissect.executable-1.4.dev2.tar", last modified: Tue Jun 27 07:48:53 2023, max compression
```

## Comparing `dissect.executable-1.4.dev1.tar` & `dissect.executable-1.4.dev2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:38.492971 dissect.executable-1.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-16 12:49:38.492971 dissect.executable-1.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:38.472970 dissect.executable-1.4.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:38.480970 dissect.executable-1.4.dev1/dissect/executable/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/dissect/executable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:38.484970 dissect.executable-1.4.dev1/dissect/executable/elf/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/dissect/executable/elf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/dissect/executable/elf/c_elf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/dissect/executable/elf/elf.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/dissect/executable/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:38.484970 dissect.executable-1.4.dev1/dissect/executable/macho/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/dissect/executable/macho/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:38.484970 dissect.executable-1.4.dev1/dissect/executable/pe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/dissect/executable/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:38.480970 dissect.executable-1.4.dev1/dissect.executable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-16 12:49:38.000000 dissect.executable-1.4.dev1/dissect.executable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-16 12:49:38.000000 dissect.executable-1.4.dev1/dissect.executable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:49:38.000000 dissect.executable-1.4.dev1/dissect.executable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:49:38.000000 dissect.executable-1.4.dev1/dissect.executable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:49:38.000000 dissect.executable-1.4.dev1/dissect.executable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-16 12:49:26.000000 dissect.executable-1.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:49:38.492971 dissect.executable-1.4.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:38.488970 dissect.executable-1.4.dev1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:38.488970 dissect.executable-1.4.dev1/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16608 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/data/hello_world.out
--rwxr-xr-x   0 runner    (1001) docker     (123)    14416 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/data/hello_world.stripped.out
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:49:38.488970 dissect.executable-1.4.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/test_elf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/test_section.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/test_segment_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:49:19.000000 dissect.executable-1.4.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:53.278407 dissect.executable-1.4.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-27 07:48:53.278407 dissect.executable-1.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:53.274407 dissect.executable-1.4.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:53.274407 dissect.executable-1.4.dev2/dissect/executable/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/dissect/executable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:53.274407 dissect.executable-1.4.dev2/dissect/executable/elf/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/dissect/executable/elf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/dissect/executable/elf/c_elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/dissect/executable/elf/elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/dissect/executable/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:53.278407 dissect.executable-1.4.dev2/dissect/executable/macho/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:39.000000 dissect.executable-1.4.dev2/dissect/executable/macho/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:53.278407 dissect.executable-1.4.dev2/dissect/executable/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:39.000000 dissect.executable-1.4.dev2/dissect/executable/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:53.274407 dissect.executable-1.4.dev2/dissect.executable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-27 07:48:53.000000 dissect.executable-1.4.dev2/dissect.executable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-27 07:48:53.000000 dissect.executable-1.4.dev2/dissect.executable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:48:53.000000 dissect.executable-1.4.dev2/dissect.executable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 07:48:53.000000 dissect.executable-1.4.dev2/dissect.executable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:48:53.000000 dissect.executable-1.4.dev2/dissect.executable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-27 07:48:43.000000 dissect.executable-1.4.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:48:53.278407 dissect.executable-1.4.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:53.278407 dissect.executable-1.4.dev2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:53.278407 dissect.executable-1.4.dev2/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16608 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/data/hello_world.out
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14416 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/data/hello_world.stripped.out
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:53.278407 dissect.executable-1.4.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/test_elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/test_segment_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 07:48:38.000000 dissect.executable-1.4.dev2/tox.ini
```

### Comparing `dissect.executable-1.4.dev1/LICENSE` & `dissect.executable-1.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/PKG-INFO` & `dissect.executable-1.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.executable
-Version: 1.4.dev1
+Version: 1.4.dev2
 Summary: A Dissect module implementing a parsers for various executable formats such as PE, ELF and Macho-O
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.executable
 Project-URL: repository, https://github.com/fox-it/dissect.executable
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.executable-1.4.dev1/README.md` & `dissect.executable-1.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/dissect/executable/elf/c_elf.py` & `dissect.executable-1.4.dev2/dissect/executable/elf/c_elf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/dissect/executable/elf/elf.py` & `dissect.executable-1.4.dev2/dissect/executable/elf/elf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/dissect.executable.egg-info/PKG-INFO` & `dissect.executable-1.4.dev2/dissect.executable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.executable
-Version: 1.4.dev1
+Version: 1.4.dev2
 Summary: A Dissect module implementing a parsers for various executable formats such as PE, ELF and Macho-O
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.executable
 Project-URL: repository, https://github.com/fox-it/dissect.executable
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.executable-1.4.dev1/dissect.executable.egg-info/SOURCES.txt` & `dissect.executable-1.4.dev2/dissect.executable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/pyproject.toml` & `dissect.executable-1.4.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/tests/data/hello_world.out` & `dissect.executable-1.4.dev2/tests/data/hello_world.out`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/tests/data/hello_world.stripped.out` & `dissect.executable-1.4.dev2/tests/data/hello_world.stripped.out`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/tests/docs/Makefile` & `dissect.executable-1.4.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/tests/docs/conf.py` & `dissect.executable-1.4.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/tests/test_dump.py` & `dissect.executable-1.4.dev2/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/tests/test_section.py` & `dissect.executable-1.4.dev2/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/tests/test_segment.py` & `dissect.executable-1.4.dev2/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/tests/test_segment_table.py` & `dissect.executable-1.4.dev2/tests/test_segment_table.py`

 * *Files identical despite different names*

### Comparing `dissect.executable-1.4.dev1/tox.ini` & `dissect.executable-1.4.dev2/tox.ini`

 * *Files identical despite different names*

