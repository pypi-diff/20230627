# Comparing `tmp/learn_python_check-1.0.0.tar.gz` & `tmp/learn_python_check-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learn_python_check-1.0.0.tar", last modified: Tue Jun 27 10:52:54 2023, max compression
+gzip compressed data, was "learn_python_check-1.0.1.tar", last modified: Tue Jun 27 11:44:18 2023, max compression
```

## Comparing `learn_python_check-1.0.0.tar` & `learn_python_check-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 10:52:54.714965 learn_python_check-1.0.0/
--rw-rw-rw-   0        0        0    35809 2023-06-11 18:53:14.000000 learn_python_check-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3131 2023-06-27 10:52:54.715967 learn_python_check-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2137 2023-06-27 10:51:46.000000 learn_python_check-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 10:52:54.708964 learn_python_check-1.0.0/learn_python_check/
--rw-rw-rw-   0        0        0      300 2023-06-27 10:46:10.000000 learn_python_check-1.0.0/learn_python_check/__init__.py
--rw-rw-rw-   0        0        0     9191 2023-06-12 08:33:13.000000 learn_python_check-1.0.0/learn_python_check/check_answers.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:52:54.714965 learn_python_check-1.0.0/learn_python_check.egg-info/
--rw-rw-rw-   0        0        0     3131 2023-06-27 10:52:54.000000 learn_python_check-1.0.0/learn_python_check.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-27 10:52:54.000000 learn_python_check-1.0.0/learn_python_check.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 10:52:54.000000 learn_python_check-1.0.0/learn_python_check.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 10:52:54.000000 learn_python_check-1.0.0/learn_python_check.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-27 10:52:54.000000 learn_python_check-1.0.0/learn_python_check.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-27 10:52:54.716967 learn_python_check-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1873 2023-06-27 10:52:27.000000 learn_python_check-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:44:18.864374 learn_python_check-1.0.1/
+-rw-rw-rw-   0        0        0    35809 2023-06-11 18:53:14.000000 learn_python_check-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3123 2023-06-27 11:44:18.865376 learn_python_check-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2129 2023-06-27 11:41:44.000000 learn_python_check-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 11:44:18.852410 learn_python_check-1.0.1/learn_python_check/
+-rw-rw-rw-   0        0        0      300 2023-06-27 10:46:10.000000 learn_python_check-1.0.1/learn_python_check/__init__.py
+-rw-rw-rw-   0        0        0     9191 2023-06-12 08:33:13.000000 learn_python_check-1.0.1/learn_python_check/check_answers.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:44:18.864374 learn_python_check-1.0.1/learn_python_check.egg-info/
+-rw-rw-rw-   0        0        0     3123 2023-06-27 11:44:18.000000 learn_python_check-1.0.1/learn_python_check.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-27 11:44:18.000000 learn_python_check-1.0.1/learn_python_check.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:44:18.000000 learn_python_check-1.0.1/learn_python_check.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 11:44:18.000000 learn_python_check-1.0.1/learn_python_check.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 11:44:18.000000 learn_python_check-1.0.1/learn_python_check.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-27 11:44:18.866372 learn_python_check-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1873 2023-06-27 11:43:39.000000 learn_python_check-1.0.1/setup.py
```

### Comparing `learn_python_check-1.0.0/LICENSE.txt` & `learn_python_check-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `learn_python_check-1.0.0/PKG-INFO` & `learn_python_check-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: learn_python_check
-Version: 1.0.0
+Version: 1.0.1
 Summary: learn python check answers
 Home-page: https://github.com/TUDelft-CITG/learn-python-package
-Download-URL: https://github.com/TUDelft-CITG/learn-python-package/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/TUDelft-CITG/learn-python-package/archive/refs/tags/v1.0.1.tar.gz
 Author: Miguel Angel Mendoza-Lugo, Robert Lanzafame, Ahmed Farahat
 Author-email: m.a.mendozalugo@tudelft.nl
 License: GNU
 Project-URL: Bug Tracker, https://github.com/TUDelft-CITG/learn-python-package/issues
 Keywords: pypi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,24 +26,24 @@
 
 A Python package for validating online course _Learn Python for Civil Engineering and Geosciences_ answers.
 
 ## Installation and updating
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the last stable version of the package. 
 
 ```bash
-pip install learn-python-ceg-check
+pip install learn-python-check
 ```
 
 ## Usage
 The package allows for evaluating the answers to the exercises in sections 3, 4 and 6. 
 
 #### Demo of some of the features:
 
 ```python
-import learn_python_ceg_check.check_answers as check
+import learn_python_check.check_answers as check
 
 check.notebook_3(question_number=0, arguments=[car_info, message])
 
 ```
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `learn_python_check-1.0.0/README.md` & `learn_python_check-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 A Python package for validating online course _Learn Python for Civil Engineering and Geosciences_ answers.
 
 ## Installation and updating
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the last stable version of the package. 
 
 ```bash
-pip install learn-python-ceg-check
+pip install learn-python-check
 ```
 
 ## Usage
 The package allows for evaluating the answers to the exercises in sections 3, 4 and 6. 
 
 #### Demo of some of the features:
 
 ```python
-import learn_python_ceg_check.check_answers as check
+import learn_python_check.check_answers as check
 
 check.notebook_3(question_number=0, arguments=[car_info, message])
 
 ```
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `learn_python_check-1.0.0/learn_python_check/check_answers.py` & `learn_python_check-1.0.1/learn_python_check/check_answers.py`

 * *Files identical despite different names*

### Comparing `learn_python_check-1.0.0/learn_python_check.egg-info/PKG-INFO` & `learn_python_check-1.0.1/learn_python_check.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: learn-python-check
-Version: 1.0.0
+Version: 1.0.1
 Summary: learn python check answers
 Home-page: https://github.com/TUDelft-CITG/learn-python-package
-Download-URL: https://github.com/TUDelft-CITG/learn-python-package/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/TUDelft-CITG/learn-python-package/archive/refs/tags/v1.0.1.tar.gz
 Author: Miguel Angel Mendoza-Lugo, Robert Lanzafame, Ahmed Farahat
 Author-email: m.a.mendozalugo@tudelft.nl
 License: GNU
 Project-URL: Bug Tracker, https://github.com/TUDelft-CITG/learn-python-package/issues
 Keywords: pypi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,24 +26,24 @@
 
 A Python package for validating online course _Learn Python for Civil Engineering and Geosciences_ answers.
 
 ## Installation and updating
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the last stable version of the package. 
 
 ```bash
-pip install learn-python-ceg-check
+pip install learn-python-check
 ```
 
 ## Usage
 The package allows for evaluating the answers to the exercises in sections 3, 4 and 6. 
 
 #### Demo of some of the features:
 
 ```python
-import learn_python_ceg_check.check_answers as check
+import learn_python_check.check_answers as check
 
 check.notebook_3(question_number=0, arguments=[car_info, message])
 
 ```
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `learn_python_check-1.0.0/setup.py` & `learn_python_check-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='learn_python_check',                           # should match the package folder
     packages=['learn_python_check'],                   # should match the package folder
-    version='1.0.0',                              # important for updates
+    version='1.0.1',                              # important for updates
     license='GNU',                                  # should match your chosen license
     description='learn python check answers',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='Miguel Angel Mendoza-Lugo, Robert Lanzafame, Ahmed Farahat',
     author_email='m.a.mendozalugo@tudelft.nl',
     url='https://github.com/TUDelft-CITG/learn-python-package', 
@@ -27,9 +27,9 @@
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     
-    download_url="https://github.com/TUDelft-CITG/learn-python-package/archive/refs/tags/v1.0.0.tar.gz",
+    download_url="https://github.com/TUDelft-CITG/learn-python-package/archive/refs/tags/v1.0.1.tar.gz",
 )
```

