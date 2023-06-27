# Comparing `tmp/pdf_oralia-0.2.5.tar.gz` & `tmp/pdf_oralia-0.2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_oralia-0.2.5.tar", max compression
+gzip compressed data, was "pdf_oralia-0.2.6.5.tar", max compression
```

## Comparing `pdf_oralia-0.2.5.tar` & `pdf_oralia-0.2.6.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2022-09-27 12:44:08.486982 pdf_oralia-0.2.5/README.md
--rw-r--r--   0        0        0        0 2022-09-25 16:31:06.006810 pdf_oralia-0.2.5/pdf_oralia/__init__.py
--rw-r--r--   0        0        0     2571 2022-12-18 10:39:01.920355 pdf_oralia-0.2.5/pdf_oralia/extract.py
--rw-r--r--   0        0        0     1862 2022-10-10 20:08:09.246847 pdf_oralia-0.2.5/pdf_oralia/extract_charge.py
--rw-r--r--   0        0        0     1997 2022-12-18 10:39:01.920355 pdf_oralia-0.2.5/pdf_oralia/extract_locataire.py
--rw-r--r--   0        0        0     2057 2022-12-18 09:11:12.023447 pdf_oralia-0.2.5/pdf_oralia/scripts.py
--rw-r--r--   0        0        0      542 2022-12-18 10:40:18.113692 pdf_oralia-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 pdf_oralia-0.2.5/setup.py
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 pdf_oralia-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-27 09:58:40.860885 pdf_oralia-0.2.6.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 09:58:40.860885 pdf_oralia-0.2.6.5/pdf_oralia/__init__.py
+-rw-r--r--   0        0        0     2571 2023-06-27 09:58:40.860885 pdf_oralia-0.2.6.5/pdf_oralia/extract.py
+-rw-r--r--   0        0        0     1862 2023-06-27 09:58:40.860885 pdf_oralia-0.2.6.5/pdf_oralia/extract_charge.py
+-rw-r--r--   0        0        0     1997 2023-06-27 09:58:40.860885 pdf_oralia-0.2.6.5/pdf_oralia/extract_locataire.py
+-rw-r--r--   0        0        0      902 2023-06-27 09:58:40.860885 pdf_oralia-0.2.6.5/pdf_oralia/join.py
+-rw-r--r--   0        0        0     1591 2023-06-27 09:58:40.860885 pdf_oralia-0.2.6.5/pdf_oralia/scripts.py
+-rw-r--r--   0        0        0      545 2023-06-27 09:58:44.480686 pdf_oralia-0.2.6.5/pyproject.toml
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 pdf_oralia-0.2.6.5/PKG-INFO
```

### Comparing `pdf_oralia-0.2.5/pdf_oralia/extract.py` & `pdf_oralia-0.2.6.5/pdf_oralia/extract.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.2.5/pdf_oralia/extract_charge.py` & `pdf_oralia-0.2.6.5/pdf_oralia/extract_charge.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.2.5/pdf_oralia/extract_locataire.py` & `pdf_oralia-0.2.6.5/pdf_oralia/extract_locataire.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.2.5/pyproject.toml` & `pdf_oralia-0.2.6.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf-oralia"
-version = "0.2.5"
+version = "v0.2.6.5"
 description = ""
 authors = ["Bertrand Benjamin <benjamin.bertrand@opytex.org>"]
 readme = "README.md"
 packages = [{include = "pdf_oralia"}]
 
 [tool.poetry.scripts]
 pdf-oralia = "pdf_oralia.scripts:main"
```

### Comparing `pdf_oralia-0.2.5/PKG-INFO` & `pdf_oralia-0.2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-oralia
-Version: 0.2.5
+Version: 0.2.6.5
 Summary: 
 Author: Bertrand Benjamin
 Author-email: benjamin.bertrand@opytex.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

