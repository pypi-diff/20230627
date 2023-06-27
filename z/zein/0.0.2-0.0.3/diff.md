# Comparing `tmp/zein-0.0.2.tar.gz` & `tmp/zein-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zein-0.0.2.tar", last modified: Tue Jun 27 08:08:42 2023, max compression
+gzip compressed data, was "zein-0.0.3.tar", last modified: Tue Jun 27 08:47:20 2023, max compression
```

## Comparing `zein-0.0.2.tar` & `zein-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:08:42.248063 zein-0.0.2/
--rw-rw-rw-   0        0        0     1070 2023-06-27 06:45:13.000000 zein-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      801 2023-06-27 08:08:42.247066 zein-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-06-27 06:53:20.000000 zein-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 08:08:42.248063 zein-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1041 2023-06-27 08:07:20.000000 zein-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:08:42.230647 zein-0.0.2/zein/
--rw-rw-rw-   0        0        0       36 2023-06-27 07:49:23.000000 zein-0.0.2/zein/__init__.py
--rw-rw-rw-   0        0        0     2027 2023-06-27 06:31:56.000000 zein-0.0.2/zein/text.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:08:42.245071 zein-0.0.2/zein.egg-info/
--rw-rw-rw-   0        0        0      801 2023-06-27 08:08:42.000000 zein-0.0.2/zein.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-06-27 08:08:42.000000 zein-0.0.2/zein.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:08:42.000000 zein-0.0.2/zein.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 08:08:42.000000 zein-0.0.2/zein.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-27 08:08:42.000000 zein-0.0.2/zein.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 08:47:20.148561 zein-0.0.3/
+-rw-rw-rw-   0        0        0     1070 2023-06-27 06:45:13.000000 zein-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      742 2023-06-27 08:47:20.147560 zein-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-06-27 06:53:20.000000 zein-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:47:20.148561 zein-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1156 2023-06-27 08:36:11.000000 zein-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:47:20.123623 zein-0.0.3/zein/
+-rw-rw-rw-   0        0        0       36 2023-06-27 07:49:23.000000 zein-0.0.3/zein/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:47:20.144567 zein-0.0.3/zein/data/
+-rw-rw-rw-   0        0        0      630 2023-06-25 15:14:01.000000 zein-0.0.3/zein/data/data.csv
+-rw-rw-rw-   0        0        0       60 2023-06-27 08:21:38.000000 zein-0.0.3/zein/main.py
+-rw-rw-rw-   0        0        0     2037 2023-06-27 08:17:21.000000 zein-0.0.3/zein/text.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:47:20.141575 zein-0.0.3/zein.egg-info/
+-rw-rw-rw-   0        0        0      742 2023-06-27 08:47:20.000000 zein-0.0.3/zein.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-27 08:47:20.000000 zein-0.0.3/zein.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:47:20.000000 zein-0.0.3/zein.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-27 08:47:18.000000 zein-0.0.3/zein.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-27 08:47:20.000000 zein-0.0.3/zein.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-27 08:47:20.000000 zein-0.0.3/zein.egg-info/top_level.txt
```

### Comparing `zein-0.0.2/LICENSE.txt` & `zein-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zein-0.0.2/PKG-INFO` & `zein-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python library for ensuring the safety and security of ML models
-Home-page: UNKNOWN
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
-License: UNKNOWN
 Keywords: python,arabic filtering,text filtering,profanity check
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 A python library for ensuring the safety and security of ML models and their outputs for the Arabic and Islamic community
-
```

### Comparing `zein-0.0.2/README.md` & `zein-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zein-0.0.2/setup.py` & `zein-0.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A python library for ensuring the safety and security of ML models'
 LONG_DESCRIPTION = 'A python library for ensuring the safety and security of ML models and their outputs for the Arabic and Islamic community'
 
 # Setting up
 setup(
     name="zein",
     version=VERSION,
     author="Mohamed Elsayed",
     author_email="<mohamedelsayed3487@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
+    package_data= {
+      'zein': ['data/*.csv'],
+    },
+    include_package_data=True,
+    zip_safe=False,
     install_requires=['pandas'],
     keywords=['python','arabic filtering', 'text filtering', 'profanity check'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

### Comparing `zein-0.0.2/zein/text.py` & `zein-0.0.3/zein/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import re
 
 
 class ArabicFilter():
-    def __init__(self, path='data/data.csv') -> object:  # default argument
+    def __init__(self, path: object = 'data/data.csv') -> object:  # default argument
         # instance variable
         self.insulting_words = pd.read_csv(path)
 
     def censor(self, text: str) -> str:
         # compile a regular expression pattern
         pattern = re.compile('|'.join(self.insulting_words['words']), re.IGNORECASE)
```

### Comparing `zein-0.0.2/zein.egg-info/PKG-INFO` & `zein-0.0.3/zein.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python library for ensuring the safety and security of ML models
-Home-page: UNKNOWN
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
-License: UNKNOWN
 Keywords: python,arabic filtering,text filtering,profanity check
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 A python library for ensuring the safety and security of ML models and their outputs for the Arabic and Islamic community
-
```

