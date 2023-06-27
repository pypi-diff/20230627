# Comparing `tmp/importils-0.1.tar.gz` & `tmp/importils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importils-0.1.tar", last modified: Tue Jun 27 17:00:36 2023, max compression
+gzip compressed data, was "importils-0.2.tar", last modified: Tue Jun 27 17:15:24 2023, max compression
```

## Comparing `importils-0.1.tar` & `importils-0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 17:00:36.350724 importils-0.1/
--rw-rw-rw-   0        0        0      790 2023-06-27 17:00:36.350724 importils-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 17:00:36.350724 importils-0.1/importils/
--rw-rw-rw-   0        0        0       26 2023-06-27 17:00:34.722461 importils-0.1/importils/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-27 16:58:49.200672 importils-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1651 2023-06-27 16:58:49.202615 importils-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:15:24.700618 importils-0.2/
+-rw-rw-rw-   0        0        0      790 2023-06-27 17:15:24.700618 importils-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 17:15:24.700618 importils-0.2/importils/
+-rw-rw-rw-   0        0        0       74 2023-06-27 17:14:40.707207 importils-0.2/importils/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 16:58:49.200672 importils-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1659 2023-06-27 17:15:03.540283 importils-0.2/setup.py
```

### Comparing `importils-0.1/PKG-INFO` & `importils-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: importils
-Version: 0.1
+Version: 0.2
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/TogiFerretFerret/importils
 Author: YOUR NAME
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/TogiFerretFerret/importils/archive/refs/tags/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `importils-0.1/setup.py` & `importils-0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from distutils.core import setup
 setup(
   name = 'importils',         # How you named your package folder (MyLib)
   packages = ['importils'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'YOUR NAME',                   # Type in your name
   author_email = 'your.email@domain.com',      # Type in your E-Mail
   url = 'https://github.com/TogiFerretFerret/importils',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/TogiFerretFerret/importils/archive/refs/tags/v_01.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
-  install_requires=[            # I get to this in a second
+  install_requires=[
+    'numpy',
+    'pandas',
+    'matplotlib'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

