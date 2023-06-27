# Comparing `tmp/zein-0.0.3.tar.gz` & `tmp/zein-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zein-0.0.3.tar", last modified: Tue Jun 27 08:47:20 2023, max compression
+gzip compressed data, was "zein-0.0.4.tar", last modified: Tue Jun 27 09:14:50 2023, max compression
```

## Comparing `zein-0.0.3.tar` & `zein-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:47:20.148561 zein-0.0.3/
--rw-rw-rw-   0        0        0     1070 2023-06-27 06:45:13.000000 zein-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      742 2023-06-27 08:47:20.147560 zein-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-06-27 06:53:20.000000 zein-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 08:47:20.148561 zein-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1156 2023-06-27 08:36:11.000000 zein-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:47:20.123623 zein-0.0.3/zein/
--rw-rw-rw-   0        0        0       36 2023-06-27 07:49:23.000000 zein-0.0.3/zein/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:47:20.144567 zein-0.0.3/zein/data/
--rw-rw-rw-   0        0        0      630 2023-06-25 15:14:01.000000 zein-0.0.3/zein/data/data.csv
--rw-rw-rw-   0        0        0       60 2023-06-27 08:21:38.000000 zein-0.0.3/zein/main.py
--rw-rw-rw-   0        0        0     2037 2023-06-27 08:17:21.000000 zein-0.0.3/zein/text.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:47:20.141575 zein-0.0.3/zein.egg-info/
--rw-rw-rw-   0        0        0      742 2023-06-27 08:47:20.000000 zein-0.0.3/zein.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-27 08:47:20.000000 zein-0.0.3/zein.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:47:20.000000 zein-0.0.3/zein.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-27 08:47:18.000000 zein-0.0.3/zein.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-27 08:47:20.000000 zein-0.0.3/zein.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-27 08:47:20.000000 zein-0.0.3/zein.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 09:14:50.329738 zein-0.0.4/
+-rw-rw-rw-   0        0        0     1070 2023-06-27 06:45:13.000000 zein-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      742 2023-06-27 09:14:50.328740 zein-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-06-27 06:53:20.000000 zein-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:14:50.329738 zein-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1156 2023-06-27 09:14:14.000000 zein-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:14:50.306771 zein-0.0.4/zein/
+-rw-rw-rw-   0        0        0       36 2023-06-27 07:49:23.000000 zein-0.0.4/zein/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:14:50.325749 zein-0.0.4/zein/data/
+-rw-rw-rw-   0        0        0      630 2023-06-25 15:14:01.000000 zein-0.0.4/zein/data/data.csv
+-rw-rw-rw-   0        0        0       61 2023-06-27 09:13:02.000000 zein-0.0.4/zein/main.py
+-rw-rw-rw-   0        0        0     2100 2023-06-27 09:12:37.000000 zein-0.0.4/zein/text.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:14:50.322759 zein-0.0.4/zein.egg-info/
+-rw-rw-rw-   0        0        0      742 2023-06-27 09:14:50.000000 zein-0.0.4/zein.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-27 09:14:50.000000 zein-0.0.4/zein.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:14:50.000000 zein-0.0.4/zein.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-27 09:14:49.000000 zein-0.0.4/zein.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-27 09:14:50.000000 zein-0.0.4/zein.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-27 09:14:50.000000 zein-0.0.4/zein.egg-info/top_level.txt
```

### Comparing `zein-0.0.3/LICENSE.txt` & `zein-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zein-0.0.3/PKG-INFO` & `zein-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library for ensuring the safety and security of ML models
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
 Keywords: python,arabic filtering,text filtering,profanity check
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zein-0.0.3/README.md` & `zein-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zein-0.0.3/setup.py` & `zein-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A python library for ensuring the safety and security of ML models'
 LONG_DESCRIPTION = 'A python library for ensuring the safety and security of ML models and their outputs for the Arabic and Islamic community'
 
 # Setting up
 setup(
     name="zein",
     version=VERSION,
```

### Comparing `zein-0.0.3/zein/data/data.csv` & `zein-0.0.4/zein/data/data.csv`

 * *Files identical despite different names*

### Comparing `zein-0.0.3/zein/text.py` & `zein-0.0.4/zein/text.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd
 import re
+import pkg_resources
 
 
 class ArabicFilter():
-    def __init__(self, path: object = 'data/data.csv') -> object:  # default argument
+    def __init__(self, path: object = pkg_resources.resource_filename('zein', 'data/data.csv')) -> object:  # default argument
         # instance variable
         self.insulting_words = pd.read_csv(path)
 
     def censor(self, text: str) -> str:
         # compile a regular expression pattern
         pattern = re.compile('|'.join(self.insulting_words['words']), re.IGNORECASE)
```

### Comparing `zein-0.0.3/zein.egg-info/PKG-INFO` & `zein-0.0.4/zein.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library for ensuring the safety and security of ML models
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
 Keywords: python,arabic filtering,text filtering,profanity check
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

