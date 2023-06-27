# Comparing `tmp/zein-0.0.1.tar.gz` & `tmp/zein-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zein-0.0.1.tar", last modified: Tue Jun 27 08:01:21 2023, max compression
+gzip compressed data, was "zein-0.0.2.tar", last modified: Tue Jun 27 08:08:42 2023, max compression
```

## Comparing `zein-0.0.1.tar` & `zein-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:01:21.278945 zein-0.0.1/
--rw-rw-rw-   0        0        0     1070 2023-06-27 06:45:13.000000 zein-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      801 2023-06-27 08:01:21.277948 zein-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-06-27 06:53:20.000000 zein-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 08:01:21.278945 zein-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1047 2023-06-27 08:00:37.000000 zein-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:01:21.255521 zein-0.0.1/zein/
--rw-rw-rw-   0        0        0       36 2023-06-27 07:49:23.000000 zein-0.0.1/zein/__init__.py
--rw-rw-rw-   0        0        0     2027 2023-06-27 06:31:56.000000 zein-0.0.1/zein/text.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:01:21.274955 zein-0.0.1/zein.egg-info/
--rw-rw-rw-   0        0        0      801 2023-06-27 08:01:20.000000 zein-0.0.1/zein.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-06-27 08:01:20.000000 zein-0.0.1/zein.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:01:20.000000 zein-0.0.1/zein.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 08:01:20.000000 zein-0.0.1/zein.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-27 08:01:20.000000 zein-0.0.1/zein.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 08:08:42.248063 zein-0.0.2/
+-rw-rw-rw-   0        0        0     1070 2023-06-27 06:45:13.000000 zein-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      801 2023-06-27 08:08:42.247066 zein-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-06-27 06:53:20.000000 zein-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:08:42.248063 zein-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2023-06-27 08:07:20.000000 zein-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:08:42.230647 zein-0.0.2/zein/
+-rw-rw-rw-   0        0        0       36 2023-06-27 07:49:23.000000 zein-0.0.2/zein/__init__.py
+-rw-rw-rw-   0        0        0     2027 2023-06-27 06:31:56.000000 zein-0.0.2/zein/text.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:08:42.245071 zein-0.0.2/zein.egg-info/
+-rw-rw-rw-   0        0        0      801 2023-06-27 08:08:42.000000 zein-0.0.2/zein.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-06-27 08:08:42.000000 zein-0.0.2/zein.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:08:42.000000 zein-0.0.2/zein.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 08:08:42.000000 zein-0.0.2/zein.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-27 08:08:42.000000 zein-0.0.2/zein.egg-info/top_level.txt
```

### Comparing `zein-0.0.1/LICENSE.txt` & `zein-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zein-0.0.1/PKG-INFO` & `zein-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python library for ensuring the safety and security of ML models
 Home-page: UNKNOWN
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
 License: UNKNOWN
 Keywords: python,arabic filtering,text filtering,profanity check
 Platform: UNKNOWN
```

### Comparing `zein-0.0.1/README.md` & `zein-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zein-0.0.1/setup.py` & `zein-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
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
-    install_requires=['re', 'pandas'],
+    install_requires=['pandas'],
     keywords=['python','arabic filtering', 'text filtering', 'profanity check'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `zein-0.0.1/zein/text.py` & `zein-0.0.2/zein/text.py`

 * *Files identical despite different names*

### Comparing `zein-0.0.1/zein.egg-info/PKG-INFO` & `zein-0.0.2/zein.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python library for ensuring the safety and security of ML models
 Home-page: UNKNOWN
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
 License: UNKNOWN
 Keywords: python,arabic filtering,text filtering,profanity check
 Platform: UNKNOWN
```

