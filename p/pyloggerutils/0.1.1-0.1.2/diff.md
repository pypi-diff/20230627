# Comparing `tmp/pyloggerutils-0.1.1.tar.gz` & `tmp/pyloggerutils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloggerutils-0.1.1.tar", last modified: Tue Jun 27 13:43:57 2023, max compression
+gzip compressed data, was "pyloggerutils-0.1.2.tar", last modified: Tue Jun 27 14:02:09 2023, max compression
```

## Comparing `pyloggerutils-0.1.1.tar` & `pyloggerutils-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 13:43:57.175093 pyloggerutils-0.1.1/
--rw-rw-rw-   0        0        0     1063 2023-06-27 12:21:53.000000 pyloggerutils-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      757 2023-06-27 13:43:57.175093 pyloggerutils-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-27 13:04:54.000000 pyloggerutils-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 13:43:57.166093 pyloggerutils-0.1.1/pyloggerutils/
--rw-rw-rw-   0        0        0     1082 2023-06-27 13:39:27.000000 pyloggerutils-0.1.1/pyloggerutils/__init__.py
--rw-rw-rw-   0        0        0      849 2023-06-27 12:05:34.000000 pyloggerutils-0.1.1/pyloggerutils/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:43:57.174093 pyloggerutils-0.1.1/pyloggerutils.egg-info/
--rw-rw-rw-   0        0        0      757 2023-06-27 13:43:57.000000 pyloggerutils-0.1.1/pyloggerutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-27 13:43:57.000000 pyloggerutils-0.1.1/pyloggerutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 13:43:57.000000 pyloggerutils-0.1.1/pyloggerutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-27 13:43:57.000000 pyloggerutils-0.1.1/pyloggerutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-27 13:43:57.176092 pyloggerutils-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1597 2023-06-27 13:43:54.000000 pyloggerutils-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:02:09.948789 pyloggerutils-0.1.2/
+-rw-rw-rw-   0        0        0     1063 2023-06-27 12:21:53.000000 pyloggerutils-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1029 2023-06-27 14:02:09.948789 pyloggerutils-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-27 13:04:54.000000 pyloggerutils-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 14:02:09.920474 pyloggerutils-0.1.2/pyloggerutils/
+-rw-rw-rw-   0        0        0     1082 2023-06-27 13:39:27.000000 pyloggerutils-0.1.2/pyloggerutils/__init__.py
+-rw-rw-rw-   0        0        0      849 2023-06-27 12:05:34.000000 pyloggerutils-0.1.2/pyloggerutils/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:02:09.947791 pyloggerutils-0.1.2/pyloggerutils.egg-info/
+-rw-rw-rw-   0        0        0     1029 2023-06-27 14:02:09.000000 pyloggerutils-0.1.2/pyloggerutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-27 14:02:09.000000 pyloggerutils-0.1.2/pyloggerutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 14:02:09.000000 pyloggerutils-0.1.2/pyloggerutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-27 14:02:09.000000 pyloggerutils-0.1.2/pyloggerutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-27 14:02:09.949791 pyloggerutils-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1850 2023-06-27 13:59:03.000000 pyloggerutils-0.1.2/setup.py
```

### Comparing `pyloggerutils-0.1.1/LICENSE` & `pyloggerutils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloggerutils-0.1.1/pyloggerutils/__init__.py` & `pyloggerutils-0.1.2/pyloggerutils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyloggerutils-0.1.1/pyloggerutils/logger.py` & `pyloggerutils-0.1.2/pyloggerutils/logger.py`

 * *Files identical despite different names*

### Comparing `pyloggerutils-0.1.1/setup.py` & `pyloggerutils-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from distutils.core import setup
+from setuptools import setup
+# read the contents of your README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 setup(
   name = 'pyloggerutils',         # How you named your package folder (MyLib)
   packages = ['pyloggerutils'],   # Chose the same as "name"
-  version = '0.1.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = """This is Python Logger""",   # Give a short description about your library
   author = 'Sabari Rajan',                   # Type in your name
   author_email = 'mailme@isbarirajan.com',      # Type in your E-Mail
   url = 'https://github.com/ISabariRajan',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.1.tar.gz',    # I explain this later on
   keywords = ['Logger', 'Easy', 'PySy'],   # Keywords that define your package best
@@ -17,8 +21,10 @@
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
   ],
+  long_description=long_description,
+  long_description_content_type='text/markdown'
 )
```

