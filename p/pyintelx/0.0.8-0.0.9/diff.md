# Comparing `tmp/pyintelx-0.0.8.tar.gz` & `tmp/pyintelx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintelx-0.0.8.tar", last modified: Mon Jun 26 19:32:48 2023, max compression
+gzip compressed data, was "pyintelx-0.0.9.tar", last modified: Tue Jun 27 21:49:23 2023, max compression
```

## Comparing `pyintelx-0.0.8.tar` & `pyintelx-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:48.082282 pyintelx-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-26 19:32:48.078282 pyintelx-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-26 19:32:38.000000 pyintelx-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:48.078282 pyintelx-0.0.8/pyintelx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:38.000000 pyintelx-0.0.8/pyintelx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:48.078282 pyintelx-0.0.8/pyintelx/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-26 19:32:38.000000 pyintelx-0.0.8/pyintelx/cli/pyintelx
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-26 19:32:38.000000 pyintelx-0.0.8/pyintelx/intelx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:48.078282 pyintelx-0.0.8/pyintelx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-26 19:32:48.000000 pyintelx-0.0.8/pyintelx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-26 19:32:48.000000 pyintelx-0.0.8/pyintelx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:32:48.000000 pyintelx-0.0.8/pyintelx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:32:48.000000 pyintelx-0.0.8/pyintelx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:32:48.000000 pyintelx-0.0.8/pyintelx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:32:48.082282 pyintelx-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-26 19:32:38.000000 pyintelx-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:49:23.213893 pyintelx-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 21:49:11.000000 pyintelx-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-27 21:49:23.213893 pyintelx-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-27 21:49:11.000000 pyintelx-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:49:23.213893 pyintelx-0.0.9/pyintelx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:49:11.000000 pyintelx-0.0.9/pyintelx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:49:23.213893 pyintelx-0.0.9/pyintelx/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-27 21:49:11.000000 pyintelx-0.0.9/pyintelx/cli/pyintelx
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-27 21:49:11.000000 pyintelx-0.0.9/pyintelx/intelx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:49:23.213893 pyintelx-0.0.9/pyintelx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-27 21:49:23.000000 pyintelx-0.0.9/pyintelx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-27 21:49:23.000000 pyintelx-0.0.9/pyintelx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:49:23.000000 pyintelx-0.0.9/pyintelx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 21:49:23.000000 pyintelx-0.0.9/pyintelx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:49:23.213893 pyintelx-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-27 21:49:11.000000 pyintelx-0.0.9/setup.py
```

### Comparing `pyintelx-0.0.8/PKG-INFO` & `pyintelx-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.0.8
+Version: 0.0.9
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
-Author: Fermin Baudino, Einar Lanfranco
+Author: Fermin Baudino, Einar Lanfranco, Federico Carrilao
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-PUBLICWWW Python Library   
+INTELX Python Library   
 ========================
 
 This python library is developed based on the original intelx library, but adding the functionality to use Intelx.io Identity API.
 
 Original source could be find here: *https://github.com/IntelligenceX/SDK/tree/master/Python*
 
 Installation
 ------------
 
+You need to install this package and de the original package from IntelX.io
+
 ```bash
-pip3 install pyintelx
+pip install pyintelx
+pip install "intelx @ git+https://github.com/IntelligenceX/SDK#subdirectory=Python"
 ```
 
 Usage as command
 ================
 
 ```bash
```

### Comparing `pyintelx-0.0.8/README.md` & `pyintelx-0.0.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-PUBLICWWW Python Library   
+INTELX Python Library   
 ========================
 
 This python library is developed based on the original intelx library, but adding the functionality to use Intelx.io Identity API.
 
 Original source could be find here: *https://github.com/IntelligenceX/SDK/tree/master/Python*
 
 Installation
 ------------
 
+You need to install this package and de the original package from IntelX.io
+
 ```bash
-pip3 install pyintelx
+pip install pyintelx
+pip install "intelx @ git+https://github.com/IntelligenceX/SDK#subdirectory=Python"
 ```
 
 Usage as command
 ================
 
 ```bash
```

### Comparing `pyintelx-0.0.8/pyintelx/cli/pyintelx` & `pyintelx-0.0.9/pyintelx/cli/pyintelx`

 * *Files identical despite different names*

### Comparing `pyintelx-0.0.8/pyintelx/intelx.py` & `pyintelx-0.0.9/pyintelx/intelx.py`

 * *Files identical despite different names*

### Comparing `pyintelx-0.0.8/pyintelx.egg-info/PKG-INFO` & `pyintelx-0.0.9/pyintelx.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.0.8
+Version: 0.0.9
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
-Author: Fermin Baudino, Einar Lanfranco
+Author: Fermin Baudino, Einar Lanfranco, Federico Carrilao
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-PUBLICWWW Python Library   
+INTELX Python Library   
 ========================
 
 This python library is developed based on the original intelx library, but adding the functionality to use Intelx.io Identity API.
 
 Original source could be find here: *https://github.com/IntelligenceX/SDK/tree/master/Python*
 
 Installation
 ------------
 
+You need to install this package and de the original package from IntelX.io
+
 ```bash
-pip3 install pyintelx
+pip install pyintelx
+pip install "intelx @ git+https://github.com/IntelligenceX/SDK#subdirectory=Python"
 ```
 
 Usage as command
 ================
 
 ```bash
```

### Comparing `pyintelx-0.0.8/setup.py` & `pyintelx-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
+    
 
 setup(
     name='pyintelx',
-    version='0.0.8',
+    version='0.0.9',
     description='This lib add support to use the Identity API from Intelx.io',
-    install_requires=['requests'],
     license='MIT',
     keywords=['python, package, distribution'],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author='Fermin Baudino, Einar Lanfranco',
+    author='Fermin Baudino, Einar Lanfranco, Federico Carrilao',
     url='https://github.com/csirtamericas/pyintelxio',
     packages=['pyintelx'],
     scripts=['pyintelx/cli/pyintelx'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
```

