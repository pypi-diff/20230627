# Comparing `tmp/beancount-sog-0.1.0.tar.gz` & `tmp/beancount_sog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount-sog-0.1.0.tar", max compression
+gzip compressed data, was "beancount_sog-0.1.1.tar", max compression
```

## Comparing `beancount-sog-0.1.0.tar` & `beancount_sog-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4400 2022-10-30 13:51:33.804250 beancount-sog-0.1.0/beancount_sog/__init__.py
--rw-r--r--   0        0        0     1034 2022-10-30 13:47:15.578733 beancount-sog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      790 2022-10-30 13:56:55.668317 beancount-sog-0.1.0/setup.py
--rw-r--r--   0        0        0     1103 2022-10-30 13:56:55.668578 beancount-sog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4487 2023-06-27 20:04:04.076644 beancount_sog-0.1.1/beancount_sog/__init__.py
+-rw-r--r--   0        0        0     1034 2023-06-27 20:05:22.876070 beancount_sog-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 beancount_sog-0.1.1/setup.py
+-rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 beancount_sog-0.1.1/PKG-INFO
```

### Comparing `beancount-sog-0.1.0/beancount_sog/__init__.py` & `beancount_sog-0.1.1/beancount_sog/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,31 @@
 
 from beancount.core import data
 from beancount.core.amount import Amount
 from beancount.core.number import Decimal
 from beancount.ingest import importer
 
 actions = [
+    "CARTE",
     "PRLV EUROP PONCTUEL",
     "PRELEVEMENT EUROPEEN",
     "VIR RECU",
+    "VIR INST RE",
     "VIR INST REC",
     "VIR PERM",
     "VIR INSTANTANE EMIS",
     "VIR EUROPEEN EMIS",
     "PRELEVEMENT EUROPEEN",
     "VIREMENT RECU",
     "VIREMENT EMIS",
     "FRAIS VIR INSTANTANE",
     "CHEQUE",
     "REMISE CHEQUE",
+    "FRAIS PAIEMENT HORS ZONE EURO",
+    "COTISATION",
 ]
 
 
 class SoGImporter(importer.ImporterProtocol):
     def __init__(
         self,
         account: str,
```

### Comparing `beancount-sog-0.1.0/pyproject.toml` & `beancount_sog-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beancount-sog"
-version = "0.1.0"
+version = "0.1.1"
 description = "Beancount Importer for Société Générale CSV files"
 authors = ["Paul Khuat-Duy <paul@khuat-duy.org>"]
 license = "MIT"
 classifiers = [
     "Environment :: Plugins",
     "Intended Audience :: Financial and Insurance Industry",
     "License :: OSI Approved :: MIT License",
```

### Comparing `beancount-sog-0.1.0/setup.py` & `beancount_sog-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,21 @@
  'black>=22.1.0,<23.0.0',
  'flake8>=4.0.1,<5.0.0',
  'ipython>=8.1.1,<9.0.0',
  'isort>=5.10.1,<6.0.0']
 
 setup_kwargs = {
     'name': 'beancount-sog',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Beancount Importer for Société Générale CSV files',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Paul Khuat-Duy',
     'author_email': 'paul@khuat-duy.org',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/Eazhi/beancount-sog',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `beancount-sog-0.1.0/PKG-INFO` & `beancount_sog-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: beancount-sog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Beancount Importer for Société Générale CSV files
 Home-page: https://github.com/Eazhi/beancount-sog
 License: MIT
 Keywords: banking,beancount,cli-accounting,finance
 Author: Paul Khuat-Duy
 Author-email: paul@khuat-duy.org
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Dist: beancount (>=2.3.5,<3.0.0)
```

