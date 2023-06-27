# Comparing `tmp/ga4_data_import-0.1.6.tar.gz` & `tmp/ga4_data_import-0.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga4_data_import-0.1.6.tar", last modified: Tue Jun 27 16:45:15 2023, max compression
+gzip compressed data, was "ga4_data_import-0.1.60.tar", last modified: Tue Jun 27 17:07:53 2023, max compression
```

## Comparing `ga4_data_import-0.1.6.tar` & `ga4_data_import-0.1.60.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:45:15.196881 ga4_data_import-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-27 16:44:49.000000 ga4_data_import-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42690 2023-06-27 16:45:15.196881 ga4_data_import-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-27 16:44:49.000000 ga4_data_import-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:45:15.196881 ga4_data_import-0.1.6/ga4_data_import/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 16:44:49.000000 ga4_data_import-0.1.6/ga4_data_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-27 16:44:49.000000 ga4_data_import-0.1.6/ga4_data_import/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-27 16:44:49.000000 ga4_data_import-0.1.6/ga4_data_import/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-27 16:44:49.000000 ga4_data_import-0.1.6/ga4_data_import/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-27 16:44:49.000000 ga4_data_import-0.1.6/ga4_data_import/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:45:15.196881 ga4_data_import-0.1.6/ga4_data_import.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42690 2023-06-27 16:45:15.000000 ga4_data_import-0.1.6/ga4_data_import.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 16:45:15.000000 ga4_data_import-0.1.6/ga4_data_import.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:45:15.000000 ga4_data_import-0.1.6/ga4_data_import.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-27 16:45:15.000000 ga4_data_import-0.1.6/ga4_data_import.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 16:45:15.000000 ga4_data_import-0.1.6/ga4_data_import.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-27 16:44:49.000000 ga4_data_import-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 16:45:15.196881 ga4_data_import-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:07:53.676383 ga4_data_import-0.1.60/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-27 17:07:22.000000 ga4_data_import-0.1.60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42591 2023-06-27 17:07:53.676383 ga4_data_import-0.1.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-27 17:07:22.000000 ga4_data_import-0.1.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:07:53.672383 ga4_data_import-0.1.60/ga4_data_import/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 17:07:22.000000 ga4_data_import-0.1.60/ga4_data_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-27 17:07:22.000000 ga4_data_import-0.1.60/ga4_data_import/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-27 17:07:22.000000 ga4_data_import-0.1.60/ga4_data_import/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-27 17:07:22.000000 ga4_data_import-0.1.60/ga4_data_import/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-27 17:07:22.000000 ga4_data_import-0.1.60/ga4_data_import/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:07:53.676383 ga4_data_import-0.1.60/ga4_data_import.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42591 2023-06-27 17:07:53.000000 ga4_data_import-0.1.60/ga4_data_import.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 17:07:53.000000 ga4_data_import-0.1.60/ga4_data_import.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:07:53.000000 ga4_data_import-0.1.60/ga4_data_import.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-27 17:07:53.000000 ga4_data_import-0.1.60/ga4_data_import.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 17:07:53.000000 ga4_data_import-0.1.60/ga4_data_import.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-27 17:07:22.000000 ga4_data_import-0.1.60/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:07:53.676383 ga4_data_import-0.1.60/setup.cfg
```

### Comparing `ga4_data_import-0.1.6/LICENSE` & `ga4_data_import-0.1.60/LICENSE`

 * *Files identical despite different names*

### Comparing `ga4_data_import-0.1.6/PKG-INFO` & `ga4_data_import-0.1.60/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4_data_import
-Version: 0.1.6
+Version: 0.1.60
 Summary: Google Analytics 4 Data Import pipeline
 Author-email: Max Ostapenko <ga4_data_import@maxostapenko.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,16 +683,14 @@
 Project-URL: Bug Reports, https://github.com/max-ostapenko/ga4_data_import/issues
 Project-URL: Blog Article, https://www.maxostapenko.com/projects/ga4_data_import
 Project-URL: Funding, https://maxostapenko.com/sponsor
 Keywords: Google Analytics 4,Data Import,SFTP,Google Cloud Storage
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ga4_data_import-0.1.6/README.md` & `ga4_data_import-0.1.60/README.md`

 * *Files identical despite different names*

### Comparing `ga4_data_import-0.1.6/ga4_data_import/common.py` & `ga4_data_import-0.1.60/ga4_data_import/common.py`

 * *Files identical despite different names*

### Comparing `ga4_data_import-0.1.6/ga4_data_import/compute.py` & `ga4_data_import-0.1.60/ga4_data_import/compute.py`

 * *Files identical despite different names*

### Comparing `ga4_data_import-0.1.6/ga4_data_import/storage.py` & `ga4_data_import-0.1.60/ga4_data_import/storage.py`

 * *Files identical despite different names*

### Comparing `ga4_data_import-0.1.6/ga4_data_import/workflow.py` & `ga4_data_import-0.1.60/ga4_data_import/workflow.py`

 * *Files identical despite different names*

### Comparing `ga4_data_import-0.1.6/ga4_data_import.egg-info/PKG-INFO` & `ga4_data_import-0.1.60/ga4_data_import.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4-data-import
-Version: 0.1.6
+Version: 0.1.60
 Summary: Google Analytics 4 Data Import pipeline
 Author-email: Max Ostapenko <ga4_data_import@maxostapenko.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,16 +683,14 @@
 Project-URL: Bug Reports, https://github.com/max-ostapenko/ga4_data_import/issues
 Project-URL: Blog Article, https://www.maxostapenko.com/projects/ga4_data_import
 Project-URL: Funding, https://maxostapenko.com/sponsor
 Keywords: Google Analytics 4,Data Import,SFTP,Google Cloud Storage
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ga4_data_import-0.1.6/pyproject.toml` & `ga4_data_import-0.1.60/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ga4_data_import"
-version = "0.1.6"
+version = "0.1.60"
 description = "Google Analytics 4 Data Import pipeline"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = [
     "Google Analytics 4",
     "Data Import",
@@ -18,16 +18,14 @@
 
 classifiers = [
     "Development Status :: 3 - Alpha",
 
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 
     "Topic :: Internet :: File Transfer Protocol (FTP)",
     "Topic :: Utilities"
 ]
@@ -70,12 +68,12 @@
 type = "python"
 search_path = [ "./" ]
 [tool.pydoc-markdown.renderer]
 type = "markdown"
 filename = "./docs/index.md"
 render_toc = true
 [tool.pydoc-markdown.renderer.source_linker]
-type = "github"
-repo = "max-ostapenko/ga4_data_import"
+type = "git"
+url_template = "https://github.com/max-ostapenko/ga4_data_import/blob/main/{path}#L{lineno}"
 
 [tool.pylint.main]
 disable = ["too-many-arguments"]
```

