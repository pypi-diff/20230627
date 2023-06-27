# Comparing `tmp/vizmath-0.0.2.tar.gz` & `tmp/vizmath-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vizmath-0.0.2.tar", last modified: Wed Jun 14 06:11:01 2023, max compression
+gzip compressed data, was "dist\vizmath-0.0.3.tar", last modified: Tue Jun 27 01:12:29 2023, max compression
```

## Comparing `vizmath-0.0.2.tar` & `vizmath-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:11:01.000000 vizmath-0.0.2/
--rw-rw-rw-   0        0        0      517 2023-06-14 06:11:01.000000 vizmath-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-14 05:31:09.000000 vizmath-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 06:11:01.000000 vizmath-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-06-14 06:08:20.000000 vizmath-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:11:01.000000 vizmath-0.0.2/vizmath/
--rw-rw-rw-   0        0        0       67 2023-06-14 06:08:07.000000 vizmath-0.0.2/vizmath/__init__.py
--rw-rw-rw-   0        0        0     2332 2023-06-14 04:47:44.000000 vizmath-0.0.2/vizmath/vizmath.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:11:01.000000 vizmath-0.0.2/vizmath.egg-info/
--rw-rw-rw-   0        0        0      517 2023-06-14 06:11:01.000000 vizmath-0.0.2/vizmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-14 06:11:01.000000 vizmath-0.0.2/vizmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:11:01.000000 vizmath-0.0.2/vizmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-14 06:11:01.000000 vizmath-0.0.2/vizmath.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 06:11:01.000000 vizmath-0.0.2/vizmath.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 01:12:29.000000 vizmath-0.0.3/
+-rw-rw-rw-   0        0        0      517 2023-06-27 01:12:29.000000 vizmath-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-27 01:09:47.000000 vizmath-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 01:12:29.000000 vizmath-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-27 01:09:40.000000 vizmath-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath/
+-rw-rw-rw-   0        0        0       67 2023-06-27 01:06:02.000000 vizmath-0.0.3/vizmath/__init__.py
+-rw-rw-rw-   0        0        0    21082 2023-06-27 01:05:42.000000 vizmath-0.0.3/vizmath/vizmath.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/top_level.txt
```

### Comparing `vizmath-0.0.2/PKG-INFO` & `vizmath-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: vizmath
-Version: 0.0.2
+Version: 0.0.3
 Summary: Visualization math toolkit.
 Home-page: https://github.com/nickgerend/vizmath
 Author: Nick Gerend
 Author-email: nickgerend@gmail.com
 License: MIT
 Description: # Welcome to vizmath
         
         ## Setup
         pip install vizmath
         
         ## Usage
         coming soon
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `vizmath-0.0.2/setup.py` & `vizmath-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import setuptools as st
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 setup(
     name="vizmath",
-    version="0.0.2",
+    version="0.0.3",
     description="Visualization math toolkit.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/nickgerend/vizmath",
     author="Nick Gerend",
     author_email="nickgerend@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
     ],
     packages=st.find_namespace_packages(),
-    install_requires=["pandas", "numpy", "matplotlib"],
+    install_requires=["numpy", "scipy"],
     include_package_data=True,
     package_data={'': ['data/*.csv']},
 )
```

### Comparing `vizmath-0.0.2/vizmath.egg-info/PKG-INFO` & `vizmath-0.0.3/vizmath.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: vizmath
-Version: 0.0.2
+Version: 0.0.3
 Summary: Visualization math toolkit.
 Home-page: https://github.com/nickgerend/vizmath
 Author: Nick Gerend
 Author-email: nickgerend@gmail.com
 License: MIT
 Description: # Welcome to vizmath
         
         ## Setup
         pip install vizmath
         
         ## Usage
         coming soon
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

