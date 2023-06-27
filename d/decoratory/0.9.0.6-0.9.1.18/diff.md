# Comparing `tmp/decoratory-0.9.0.6.tar.gz` & `tmp/decoratory-0.9.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.9.0.6.tar", last modified: Fri Jun 23 07:10:45 2023, max compression
+gzip compressed data, was "decoratory-0.9.1.18.tar", last modified: Tue Jun 27 12:14:32 2023, max compression
```

## Comparing `decoratory-0.9.0.6.tar` & `decoratory-0.9.1.18.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 07:10:45.369796 decoratory-0.9.0.6/
--rw-rw-rw-   0        0        0     2588 2023-06-22 16:28:01.000000 decoratory-0.9.0.6/License.txt
--rw-rw-rw-   0        0        0    48944 2023-06-23 07:10:45.369796 decoratory-0.9.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    47319 2023-06-23 07:04:18.000000 decoratory-0.9.0.6/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-21 06:11:12.000000 decoratory-0.9.0.6/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-23 07:10:45.285134 decoratory-0.9.0.6/Sources/
-drwxrwxrwx   0        0        0        0 2023-06-23 07:10:45.322920 decoratory-0.9.0.6/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.9.0.6/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     7626 2023-06-23 07:10:15.000000 decoratory-0.9.0.6/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5888 2023-06-23 06:53:08.000000 decoratory-0.9.0.6/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14152 2023-06-22 10:12:45.000000 decoratory-0.9.0.6/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    12412 2023-06-21 10:46:45.000000 decoratory-0.9.0.6/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    36898 2023-06-21 17:34:08.000000 decoratory-0.9.0.6/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     7993 2023-06-21 10:46:45.000000 decoratory-0.9.0.6/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    10853 2023-06-21 10:48:51.000000 decoratory-0.9.0.6/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-23 07:10:45.338549 decoratory-0.9.0.6/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    48944 2023-06-23 07:10:45.000000 decoratory-0.9.0.6/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-06-23 07:10:45.000000 decoratory-0.9.0.6/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 07:10:45.000000 decoratory-0.9.0.6/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-23 07:10:45.000000 decoratory-0.9.0.6/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-23 07:10:45.354195 decoratory-0.9.0.6/Unittest/
--rw-rw-rw-   0        0        0    24037 2023-06-21 16:42:40.000000 decoratory-0.9.0.6/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    23858 2023-06-21 11:37:48.000000 decoratory-0.9.0.6/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    40107 2023-06-23 06:53:08.000000 decoratory-0.9.0.6/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10729 2023-06-21 11:37:48.000000 decoratory-0.9.0.6/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0    10193 2023-06-21 11:37:48.000000 decoratory-0.9.0.6/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-06-23 07:10:45.369796 decoratory-0.9.0.6/setup.cfg
--rw-rw-rw-   0        0        0     4515 2023-06-23 07:10:15.000000 decoratory-0.9.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:14:32.190822 decoratory-0.9.1.18/
+-rw-rw-rw-   0        0        0     1252 2023-06-27 11:25:14.000000 decoratory-0.9.1.18/License.txt
+-rw-rw-rw-   0        0        0    49014 2023-06-27 12:14:32.190822 decoratory-0.9.1.18/PKG-INFO
+-rw-rw-rw-   0        0        0    47411 2023-06-27 12:10:25.000000 decoratory-0.9.1.18/Readme.rst
+-rw-rw-rw-   0        0        0     1823 2023-06-27 11:36:48.000000 decoratory-0.9.1.18/ReleaseNotes.txt
+-rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.1.18/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 12:14:32.120852 decoratory-0.9.1.18/Sources/
+drwxrwxrwx   0        0        0        0 2023-06-27 12:14:32.159662 decoratory-0.9.1.18/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.9.1.18/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     7614 2023-06-27 12:13:55.000000 decoratory-0.9.1.18/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5880 2023-06-27 11:42:36.000000 decoratory-0.9.1.18/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14152 2023-06-27 11:42:36.000000 decoratory-0.9.1.18/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    12414 2023-06-27 11:42:36.000000 decoratory-0.9.1.18/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    36902 2023-06-27 11:42:36.000000 decoratory-0.9.1.18/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     7995 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    10855 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:14:32.172235 decoratory-0.9.1.18/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    49014 2023-06-27 12:14:32.000000 decoratory-0.9.1.18/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-06-27 12:14:32.000000 decoratory-0.9.1.18/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:14:32.000000 decoratory-0.9.1.18/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-27 12:14:32.000000 decoratory-0.9.1.18/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 12:14:32.188622 decoratory-0.9.1.18/Unittest/
+-rw-rw-rw-   0        0        0    24037 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    23858 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40107 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10729 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0    10193 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 12:14:32.190822 decoratory-0.9.1.18/setup.cfg
+-rw-rw-rw-   0        0        0     4537 2023-06-27 12:13:55.000000 decoratory-0.9.1.18/setup.py
```

### Comparing `decoratory-0.9.0.6/PKG-INFO` & `decoratory-0.9.1.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.0.6
+Version: 0.9.1.18
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
-License: PSF
+License: MIT
 Project-URL: Projekt, http://evation.eu
 Project-URL: Release Notes, http://evation.eu
 Project-URL: Download, http://evation.eu
 Keywords: decorator singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation
-Classifier: License :: OSI Approved :: Python Software Foundation License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -49,30 +49,30 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu"
     __copyright__ = f"(c) copyright 2020-2023, {__company__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.0.7"
-    __date__ = "2023-06-23"
-    __time__ = "09:04:18"
+    __version__ = "0.9.1.13"
+    __date__ = "2023-06-27"
+    __time__ = "14:10:25"
     __state__ = "Beta"
-    __license__ = "PSF"
+    __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
 ==============================================================================
 
 
 **Introduction**
 
-The *decoratory package* is based on the `Decorator Arguments Pattern`_, an
+The *decoratory package* is based on the `Decorator Arguments Template`_, an
 integrated concept for Python decorators with and without parameters. In
 addition, all decorators created with it support complex arguments, e.g.
 lists of values and functions, without unnecessarily complicating the
 decoration of simple cases by these extensions. All implementation details
 are described on the `project homepage`_.
 
 
@@ -121,15 +121,15 @@
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of
 a class to a single (unique) instance. This is useful when exactly one unique
 object is needed i.e. to manage an expensive resource or coordinate actions
 across module boundaries.
 
 As a simple example serves the decoration of the class  ``Animal`` as a
-singleton. In the context of the `Decorator Arguments Pattern`_, this can be
+singleton. In the context of the `Decorator Arguments Template`_, this can be
 done both without brackets (decorator class) and with brackets (decorator
 instance), meaning both notations describe the same functional situation.
 
 .. code-block:: python
 
     # *** example_singleton.py - class Animal with Singleton decoration
 
@@ -175,15 +175,15 @@
     # Case 2: Dynamic decoration providing extra initial default values
     Animal = Singleton(Animal, 'Teddy')
     Animal()                        # Using the decorator's default 'Teddy'
     a = Animal(name='Roxie')        # Returns Teddy
     print(a)                        # Animal('Teddy')
 
 Quite generally, for all the following decorators based on this
-`Decorator Arguments Pattern`_, these two properties are always fulfilled:
+`Decorator Arguments Template`_, these two properties are always fulfilled:
 
 #. Decoration as a class (without parentheses) and Decoration as an instance
    (with empty parentheses) are equivalent
 #. For dynamic decoration, extra parameters can be passed, e.g. for the
    class constructor
 
 So far, this singleton implementation follows the concept of *once
@@ -1148,14 +1148,18 @@
 However, it bears the risk of losing track of all dependencies.
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.9.1.*, Build: 2023-06-27**
+
+- Switch from PSF License to MIT License
+
 **Version: 0.9.0.*, Build: 2023-06-23**
 
 - Unit test integration for Windows, Linux (and probably MacOS - feedback?)
 - Pre production state, version 0.9.* for module
     - observer [ ``python -m decoratory.observer --version`` ]
 - Pre production state, version 0.9.* for package
     - decoratory [ ``python -m decoratory --version`` ]
@@ -1206,9 +1210,9 @@
 
 
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Pattern: http://evation.eu
+.. _Decorator Arguments Template: http://evation.eu
```

### Comparing `decoratory-0.9.0.6/Readme.rst` & `decoratory-0.9.1.18/Readme.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu"
     __copyright__ = f"(c) copyright 2020-2023, {__company__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.0.7"
-    __date__ = "2023-06-23"
-    __time__ = "09:04:18"
+    __version__ = "0.9.1.13"
+    __date__ = "2023-06-27"
+    __time__ = "14:10:25"
     __state__ = "Beta"
-    __license__ = "PSF"
+    __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
 ==============================================================================
 
 
 **Introduction**
 
-The *decoratory package* is based on the `Decorator Arguments Pattern`_, an
+The *decoratory package* is based on the `Decorator Arguments Template`_, an
 integrated concept for Python decorators with and without parameters. In
 addition, all decorators created with it support complex arguments, e.g.
 lists of values and functions, without unnecessarily complicating the
 decoration of simple cases by these extensions. All implementation details
 are described on the `project homepage`_.
 
 
@@ -82,15 +82,15 @@
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of
 a class to a single (unique) instance. This is useful when exactly one unique
 object is needed i.e. to manage an expensive resource or coordinate actions
 across module boundaries.
 
 As a simple example serves the decoration of the class  ``Animal`` as a
-singleton. In the context of the `Decorator Arguments Pattern`_, this can be
+singleton. In the context of the `Decorator Arguments Template`_, this can be
 done both without brackets (decorator class) and with brackets (decorator
 instance), meaning both notations describe the same functional situation.
 
 .. code-block:: python
 
     # *** example_singleton.py - class Animal with Singleton decoration
 
@@ -136,15 +136,15 @@
     # Case 2: Dynamic decoration providing extra initial default values
     Animal = Singleton(Animal, 'Teddy')
     Animal()                        # Using the decorator's default 'Teddy'
     a = Animal(name='Roxie')        # Returns Teddy
     print(a)                        # Animal('Teddy')
 
 Quite generally, for all the following decorators based on this
-`Decorator Arguments Pattern`_, these two properties are always fulfilled:
+`Decorator Arguments Template`_, these two properties are always fulfilled:
 
 #. Decoration as a class (without parentheses) and Decoration as an instance
    (with empty parentheses) are equivalent
 #. For dynamic decoration, extra parameters can be passed, e.g. for the
    class constructor
 
 So far, this singleton implementation follows the concept of *once
@@ -1109,14 +1109,18 @@
 However, it bears the risk of losing track of all dependencies.
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.9.1.*, Build: 2023-06-27**
+
+- Switch from PSF License to MIT License
+
 **Version: 0.9.0.*, Build: 2023-06-23**
 
 - Unit test integration for Windows, Linux (and probably MacOS - feedback?)
 - Pre production state, version 0.9.* for module
     - observer [ ``python -m decoratory.observer --version`` ]
 - Pre production state, version 0.9.* for package
     - decoratory [ ``python -m decoratory --version`` ]
@@ -1167,9 +1171,9 @@
 
 
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Pattern: http://evation.eu
+.. _Decorator Arguments Template: http://evation.eu
```

### Comparing `decoratory-0.9.0.6/Sources/decoratory/__main__.py` & `decoratory-0.9.1.18/Sources/decoratory/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.6"
-__date__ = "2023-06-23"
-__time__ = "09:10:15"
+__version__ = "0.9.1.18"
+__date__ = "2023-06-27"
+__time__ = "14:13:55"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 __all__ = ["get_file_location"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 import sys
@@ -140,18 +140,18 @@
 
 {module} is a Python package you cannot execute directly from command line.
 
 The package provides a framework for Python decorators as well as concrete 
 implementations of useful decorators, e.g. Singleton, Multiton, Observable 
 and a configurable Wrapper.
 
-{module} is provided by {__company__} under the {__license__} license \
-included with 
-this package. It comes without any warranty, but with the intention of saving 
-working time and improving code quality and productivity.
+{module} is provided under the {__license__} License included with this \
+module. It 
+comes without any warranty, but with the intention of saving work, time and 
+improving code quality as well as productivity.
 
 All kinds of bugs, questions, improvement suggestions, change requests etc. 
 are welcome to be directed to the product maintainers email {__email__}.
 
 The current version of the installed package is:
 {module}: Version {__version__}, Build {__date__} {__time__}, \
 State '{__state__}'
```

### Comparing `decoratory-0.9.0.6/Sources/decoratory/banner.py` & `decoratory-0.9.1.18/Sources/decoratory/banner.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.12"
-__date__ = "2023-06-23"
-__time__ = "08:53:07"
+__version__ = "0.9.1.15"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 import sys
@@ -110,17 +110,17 @@
 -------------------------------------------------------------------------------
 {title.upper(): ^79}
 -------------------------------------------------------------------------------
 
 {module} is a Python module you cannot execute directly from command line.
 This module provides a {name} decorator.
 
-{module} is provided by {company} under the {license} license included with 
-this module. It comes without any warranty, but with the intention of saving 
-working time and improving code quality and productivity.
+{module} is provided under the {license} License included with this module. It 
+comes without any warranty, but with the intention of saving work, time and 
+improving code quality as well as productivity.
 
 All kinds of bugs, questions, improvement suggestions, change requests etc. 
 are welcome to be directed to the product maintainers email {email}.
 
 The current version of the installed package is:
 {module}: Version {version}, Build {date} {time}, State '{state}'
```

### Comparing `decoratory-0.9.0.6/Sources/decoratory/basic.py` & `decoratory-0.9.1.18/Sources/decoratory/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.4"
-__date__ = "2023-06-22"
-__time__ = "12:12:42"
+__version__ = "0.9.1.6"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 __all__ = ["Activation", "Parser", "F", "X"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 from enum import IntFlag
 from typing import Union
```

### Comparing `decoratory-0.9.0.6/Sources/decoratory/multiton.py` & `decoratory-0.9.1.18/Sources/decoratory/multiton.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,19 +125,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.2"
-__date__ = "2023-06-21"
-__time__ = "12:46:42"
+__version__ = "0.9.1.5"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 from functools import update_wrapper
 from typing import Union
@@ -213,24 +213,24 @@
             def reset(s: object = self) -> None:
                 """Define reset method"""
                 s.set_instances(None)
 
             # Add the reset method
             setattr(self, 'reset', reset)
 
-        # --- Decorator Arguments Pattern (1/2)
+        # --- Decorator Arguments Template (1/2)
         if self.__get__substitute() is not None:
             # Decoration without parameter(s)
             self.__set__substitute(
                 F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
     def __call__(self, *args, **kwargs):
         """Apply the decorator"""
-        # --- Decorator Arguments Pattern (2/2)
+        # --- Decorator Arguments Template (2/2)
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
         else:  # *** Wrapper ***
             # If no current values, take defaults
```

### Comparing `decoratory-0.9.0.6/Sources/decoratory/observer.py` & `decoratory-0.9.1.18/Sources/decoratory/observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,19 +407,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.2"
-__date__ = "2023-06-21"
-__time__ = "19:34:05"
+__version__ = "0.9.1.5"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 from functools import update_wrapper
 from typing import Union
@@ -623,28 +623,28 @@
             None.
         """
         self.__set__substitute(substitute)
         self.__set__observers(observers)
         self.__set__methods(methods)
         self.__set__activate(activate)
 
-        # --- Decorator Arguments Pattern (1/2)
+        # --- Decorator Arguments Template (1/2)
         if self.__get__substitute() is not None:
             # Decoration without parameter(s)
             self.__set__substitute(
                 F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
             self.__set__observable(Observable.BaseClass())
         else:
             # Decoration with parameter(s)
             self.__set__observable(Observable.BaseClass(*args, **kwargs))
 
     def __call__(self, *args, **kwargs):
-        # --- Decorator Arguments Pattern (2/2)
+        # --- Decorator Arguments Template (2/2)
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
 
             # Decoration of a type means decoration of *all* submitted methods
             if self.__get__methods():
                 # Resolve list of methods:
@@ -802,28 +802,28 @@
         Returns:
             None.
         """
         self.__set__substitute(substitute)
         self.__set__observables(observables)
         self.__set__methods(methods)
 
-        # --- Decorator Arguments Pattern (1/2)
+        # --- Decorator Arguments Template (1/2)
         if self.__get__substitute() is not None:
             # Decoration without parameter(s)
             self.__set__substitute(
                 F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
             self.__set__observer(Observer.BaseClass())
         else:
             # Decoration with parameter(s)
             self.__set__observer(Observer.BaseClass(*args, **kwargs))
 
     def __call__(self, *args, **kwargs):
-        # --- Decorator Arguments Pattern (2/2)
+        # --- Decorator Arguments Template (2/2)
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
 
             # Decoration of a type means decoration of *all* submitted methods
             if self.__get__methods():
                 # Resolve list of methods:
```

### Comparing `decoratory-0.9.0.6/Sources/decoratory/singleton.py` & `decoratory-0.9.1.18/Sources/decoratory/singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,19 +84,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.2"
-__date__ = "2023-06-21"
-__time__ = "12:46:42"
+__version__ = "0.9.1.5"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 __all__ = ["Singleton", "SemiSingleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 from functools import update_wrapper
 from typing import Union
@@ -151,25 +151,25 @@
             def reset(s: object = self) -> None:
                 """Define reset method"""
                 s.__instance = None
 
             # Add the reset method
             setattr(self, 'reset', reset)
 
-        # --- Decorator Arguments Pattern (1/2)
+        # --- Decorator Arguments Template (1/2)
         if self.__get__substitute() is not None:
             # Decoration without parameter(s)
             self.__set__substitute(
                 F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
     def __call__(self, *args, **kwargs):
         """Apply the decorator."""
 
-        # --- Decorator Arguments Pattern (2/2)
+        # --- Decorator Arguments Template (2/2)
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
         else:  # *** Wrapper ***
             # Create and store new or return existing instance
```

### Comparing `decoratory-0.9.0.6/Sources/decoratory/wrapper.py` & `decoratory-0.9.1.18/Sources/decoratory/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,19 +136,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.2"
-__date__ = "2023-06-21"
-__time__ = "12:48:50"
+__version__ = "0.9.1.5"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 from functools import update_wrapper
 from typing import Union
@@ -200,23 +200,23 @@
             self (object): Wrapper decorator instance
         """
         self.__set__substitute(substitute)
         self.__set__before(before)
         self.__set__replace(replace)
         self.__set__after(after)
 
-        # --- Decorator Arguments Pattern (1/2)
+        # --- Decorator Arguments Template (1/2)
         if self.__get__substitute() is not None:
             # Decoration without parameter(s)
             self.__set__substitute(
                 F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
     def __call__(self, *args, **kwargs):
-        # --- Decorator Arguments Pattern (2/2)
+        # --- Decorator Arguments Template (2/2)
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
         else:  # *** Wrapper ***
             # Action BEFORE
```

### Comparing `decoratory-0.9.0.6/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.9.1.18/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.0.6
+Version: 0.9.1.18
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
-License: PSF
+License: MIT
 Project-URL: Projekt, http://evation.eu
 Project-URL: Release Notes, http://evation.eu
 Project-URL: Download, http://evation.eu
 Keywords: decorator singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation
-Classifier: License :: OSI Approved :: Python Software Foundation License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -49,30 +49,30 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu"
     __copyright__ = f"(c) copyright 2020-2023, {__company__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.0.7"
-    __date__ = "2023-06-23"
-    __time__ = "09:04:18"
+    __version__ = "0.9.1.13"
+    __date__ = "2023-06-27"
+    __time__ = "14:10:25"
     __state__ = "Beta"
-    __license__ = "PSF"
+    __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
 ==============================================================================
 
 
 **Introduction**
 
-The *decoratory package* is based on the `Decorator Arguments Pattern`_, an
+The *decoratory package* is based on the `Decorator Arguments Template`_, an
 integrated concept for Python decorators with and without parameters. In
 addition, all decorators created with it support complex arguments, e.g.
 lists of values and functions, without unnecessarily complicating the
 decoration of simple cases by these extensions. All implementation details
 are described on the `project homepage`_.
 
 
@@ -121,15 +121,15 @@
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of
 a class to a single (unique) instance. This is useful when exactly one unique
 object is needed i.e. to manage an expensive resource or coordinate actions
 across module boundaries.
 
 As a simple example serves the decoration of the class  ``Animal`` as a
-singleton. In the context of the `Decorator Arguments Pattern`_, this can be
+singleton. In the context of the `Decorator Arguments Template`_, this can be
 done both without brackets (decorator class) and with brackets (decorator
 instance), meaning both notations describe the same functional situation.
 
 .. code-block:: python
 
     # *** example_singleton.py - class Animal with Singleton decoration
 
@@ -175,15 +175,15 @@
     # Case 2: Dynamic decoration providing extra initial default values
     Animal = Singleton(Animal, 'Teddy')
     Animal()                        # Using the decorator's default 'Teddy'
     a = Animal(name='Roxie')        # Returns Teddy
     print(a)                        # Animal('Teddy')
 
 Quite generally, for all the following decorators based on this
-`Decorator Arguments Pattern`_, these two properties are always fulfilled:
+`Decorator Arguments Template`_, these two properties are always fulfilled:
 
 #. Decoration as a class (without parentheses) and Decoration as an instance
    (with empty parentheses) are equivalent
 #. For dynamic decoration, extra parameters can be passed, e.g. for the
    class constructor
 
 So far, this singleton implementation follows the concept of *once
@@ -1148,14 +1148,18 @@
 However, it bears the risk of losing track of all dependencies.
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.9.1.*, Build: 2023-06-27**
+
+- Switch from PSF License to MIT License
+
 **Version: 0.9.0.*, Build: 2023-06-23**
 
 - Unit test integration for Windows, Linux (and probably MacOS - feedback?)
 - Pre production state, version 0.9.* for module
     - observer [ ``python -m decoratory.observer --version`` ]
 - Pre production state, version 0.9.* for package
     - decoratory [ ``python -m decoratory --version`` ]
@@ -1206,9 +1210,9 @@
 
 
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Pattern: http://evation.eu
+.. _Decorator Arguments Template: http://evation.eu
```

### Comparing `decoratory-0.9.0.6/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.9.1.18/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 License.txt
 Readme.rst
+ReleaseNotes.txt
 Requirements.txt
 setup.py
 Sources/decoratory/__init__.py
 Sources/decoratory/__main__.py
 Sources/decoratory/banner.py
 Sources/decoratory/basic.py
 Sources/decoratory/multiton.py
```

### Comparing `decoratory-0.9.0.6/Unittest/test_basic.py` & `decoratory-0.9.1.18/Unittest/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.1"
-__date__ = "2023-06-21"
-__time__ = "18:42:36"
+__version__ = "0.9.1.3"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
 from decoratory.basic import (Activation, F, Parser, X)
```

### Comparing `decoratory-0.9.0.6/Unittest/test_multiton.py` & `decoratory-0.9.1.18/Unittest/test_multiton.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.1"
-__date__ = "2023-06-21"
-__time__ = "13:37:48"
+__version__ = "0.9.1.3"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
 from decoratory.multiton import Multiton
```

### Comparing `decoratory-0.9.0.6/Unittest/test_observer.py` & `decoratory-0.9.1.18/Unittest/test_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.2"
-__date__ = "2023-06-23"
-__time__ = "08:53:07"
+__version__ = "0.9.1.4"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
 from decoratory.observer import (BaseObservable, BaseObserver,
                                  Observable, Observer)
```

### Comparing `decoratory-0.9.0.6/Unittest/test_singleton.py` & `decoratory-0.9.1.18/Unittest/test_singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.1"
-__date__ = "2023-06-21"
-__time__ = "13:37:48"
+__version__ = "0.9.1.3"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
 from decoratory.singleton import Singleton, SemiSingleton
```

### Comparing `decoratory-0.9.0.6/Unittest/test_wrapper.py` & `decoratory-0.9.1.18/Unittest/test_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.1"
-__date__ = "2023-06-21"
-__time__ = "13:37:48"
+__version__ = "0.9.1.3"
+__date__ = "2023-06-27"
+__time__ = "13:42:36"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
 from decoratory.wrapper import Wrapper
 from decoratory.basic import F
```

### Comparing `decoratory-0.9.0.6/setup.py` & `decoratory-0.9.1.18/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.0.6"
-__date__ = "2023-06-23"
-__time__ = "09:10:15"
+__version__ = "0.9.1.18"
+__date__ = "2023-06-27"
+__time__ = "14:13:55"
 __state__ = "Beta"
-__license__ = "PSF"
+__license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
@@ -88,28 +88,29 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: Implementation',
-        'License :: OSI Approved :: Python Software Foundation License',
+        'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Topic :: Education',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Utilities'],
     # Modules, Files and Data
     # https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#finding-simple-packages
     packages=find_packages(where=src),
     package_dir={"": src},
     package_data={},
     py_modules=[],
     data_files=[(dta, ["License.txt",
                        "Readme.rst",
+                       "ReleaseNotes.txt",
                        "Requirements.txt"]),
                 (tst, ["Unittest/test_basic.py",
                        "Unittest/test_singleton.py",
                        "Unittest/test_multiton.py",
                        "Unittest/test_wrapper.py",
                        "Unittest/test_observer.py"])],
     entry_points={},
```

