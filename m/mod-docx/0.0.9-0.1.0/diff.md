# Comparing `tmp/mod_docx-0.0.9.tar.gz` & `tmp/mod_docx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mod_docx-0.0.9.tar", last modified: Tue Jun 27 10:20:42 2023, max compression
+gzip compressed data, was "mod_docx-0.1.0.tar", last modified: Tue Jun 27 13:53:44 2023, max compression
```

## Comparing `mod_docx-0.0.9.tar` & `mod_docx-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:20:42.442554 mod_docx-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-27 10:20:27.000000 mod_docx-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-27 10:20:42.442554 mod_docx-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 10:20:27.000000 mod_docx-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-27 10:20:27.000000 mod_docx-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 10:20:42.442554 mod_docx-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:20:42.438554 mod_docx-0.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 10:20:27.000000 mod_docx-0.0.9/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:20:42.442554 mod_docx-0.0.9/src/mod_docx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-27 10:20:42.000000 mod_docx-0.0.9/src/mod_docx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-27 10:20:42.000000 mod_docx-0.0.9/src/mod_docx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:20:42.000000 mod_docx-0.0.9/src/mod_docx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 10:20:42.000000 mod_docx-0.0.9/src/mod_docx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-27 10:20:27.000000 mod_docx-0.0.9/src/mod_docx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:53:44.527804 mod_docx-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-27 13:53:34.000000 mod_docx-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-27 13:53:44.527804 mod_docx-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-27 13:53:34.000000 mod_docx-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-27 13:53:34.000000 mod_docx-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:53:44.527804 mod_docx-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:53:44.523804 mod_docx-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 13:53:34.000000 mod_docx-0.1.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:53:44.527804 mod_docx-0.1.0/src/mod_docx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-27 13:53:44.000000 mod_docx-0.1.0/src/mod_docx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-27 13:53:44.000000 mod_docx-0.1.0/src/mod_docx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:53:44.000000 mod_docx-0.1.0/src/mod_docx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 13:53:44.000000 mod_docx-0.1.0/src/mod_docx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-06-27 13:53:34.000000 mod_docx-0.1.0/src/mod_docx.py
```

### Comparing `mod_docx-0.0.9/LICENSE` & `mod_docx-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mod_docx-0.0.9/pyproject.toml` & `mod_docx-0.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mod_docx"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Jamilah Foucher", email="j622amilah@gmail.com" },
 ]
 description = "The purpose of this library is to serve as a reliable and simple library to reassemble docx documents after they have been treated using AI/machine learning text treatment."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
+#https://pypi.org/classifiers/
 
 [project.urls]
 "Homepage" = "https://github.com/DevopsPractice7/mod_docx"
 "Bug Tracker" = "https://github.com/DevopsPractice7/mod_docx/issues"
+
```

### Comparing `mod_docx-0.0.9/src/mod_docx.py` & `mod_docx-0.1.0/src/mod_docx.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,12 +233,12 @@
         for ind, val in enumerate(tag_cle):
             docxfile.writestr(val, text_value[ind])
         
         # Enregistez le fichier docx à le reporitoire que vous avez specifié     
         docxfile.close()
         
         # -------------------
-
-	# Remove unzip temp folder
-	shutil.rmtree(extract_path)
+        
+        # Remove unzip temp folder
+        shutil.rmtree(extract_path)
 
         return
```

