# Comparing `tmp/esoteric-sigdigs-0.1.1.tar.gz` & `tmp/esoteric-sigdigs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esoteric-sigdigs-0.1.1.tar", last modified: Tue Jun 27 17:21:28 2023, max compression
+gzip compressed data, was "esoteric-sigdigs-0.1.2.tar", last modified: Tue Jun 27 17:56:33 2023, max compression
```

## Comparing `esoteric-sigdigs-0.1.1.tar` & `esoteric-sigdigs-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 17:21:28.522573 esoteric-sigdigs-0.1.1/
--rw-rw-rw-   0        0        0     1088 2023-06-27 04:47:18.000000 esoteric-sigdigs-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6489 2023-06-27 17:21:28.523572 esoteric-sigdigs-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5988 2023-06-27 16:52:57.000000 esoteric-sigdigs-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 17:21:28.521573 esoteric-sigdigs-0.1.1/esoteric_sigdigs.egg-info/
--rw-rw-rw-   0        0        0     6489 2023-06-27 17:21:28.000000 esoteric-sigdigs-0.1.1/esoteric_sigdigs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-27 17:21:28.000000 esoteric-sigdigs-0.1.1/esoteric_sigdigs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 17:21:28.000000 esoteric-sigdigs-0.1.1/esoteric_sigdigs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 17:21:28.000000 esoteric-sigdigs-0.1.1/esoteric_sigdigs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      109 2023-06-27 04:49:12.000000 esoteric-sigdigs-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      597 2023-06-27 17:21:28.526572 esoteric-sigdigs-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 17:56:33.027813 esoteric-sigdigs-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2023-06-27 04:47:18.000000 esoteric-sigdigs-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6588 2023-06-27 17:56:33.028814 esoteric-sigdigs-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6087 2023-06-27 17:55:37.000000 esoteric-sigdigs-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:56:33.013813 esoteric-sigdigs-0.1.2/esoteric_sigdigs.egg-info/
+-rw-rw-rw-   0        0        0     6588 2023-06-27 17:56:32.000000 esoteric-sigdigs-0.1.2/esoteric_sigdigs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-27 17:56:32.000000 esoteric-sigdigs-0.1.2/esoteric_sigdigs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:56:32.000000 esoteric-sigdigs-0.1.2/esoteric_sigdigs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:56:32.000000 esoteric-sigdigs-0.1.2/esoteric_sigdigs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      109 2023-06-27 04:49:12.000000 esoteric-sigdigs-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      597 2023-06-27 17:56:33.048819 esoteric-sigdigs-0.1.2/setup.cfg
```

### Comparing `esoteric-sigdigs-0.1.1/LICENSE` & `esoteric-sigdigs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esoteric-sigdigs-0.1.1/PKG-INFO` & `esoteric-sigdigs-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esoteric-sigdigs
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package that detects and rounds numbers to significant digits.
 Home-page: https://github.com/ericli3690/esoteric-sigdigs/
 Author: Eric Li
 Author-email: ericli3690@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,18 +15,23 @@
 # esoteric-sigdigs
 **🐍 A Python package that detects and rounds numbers to significant digits.**
 
 This package aims to provide easy-to-use functions to work with significant digits (also known as significant figures).
 
 ⚠ Please note that this package is almost certainly laced with bugs, so use it at your own risk! Additionally, the significant digit rules used may not be exactly what you are looking for; I have designed this package to fit the likely-esoteric way I have been taught to use significant digits. Sorry! If you encounter any issues, please create an issue on GitHub (*https://github.com/ericli3690/esoteric-sigdigs*) or email me at *ericli3690@gmail.com*.
 
-## 🛠 Installation
+## 🛠 Installation and Use
 
 `>> pip install esoteric-sigdigs`
 
+```python
+from sigdigs import sigdigs
+sigdigs.function_name_here(arguments_here)
+```
+
 ## 🧪 What is Scientific Notation?
 
 Scientific notation is often used by this package, a string formatting of numbers which takes the following form:
 
 `a.bcdEf`
 
 And which can be written in standard formatting as
```

### Comparing `esoteric-sigdigs-0.1.1/README.md` & `esoteric-sigdigs-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 # esoteric-sigdigs
 **🐍 A Python package that detects and rounds numbers to significant digits.**
 
 This package aims to provide easy-to-use functions to work with significant digits (also known as significant figures).
 
 ⚠ Please note that this package is almost certainly laced with bugs, so use it at your own risk! Additionally, the significant digit rules used may not be exactly what you are looking for; I have designed this package to fit the likely-esoteric way I have been taught to use significant digits. Sorry! If you encounter any issues, please create an issue on GitHub (*https://github.com/ericli3690/esoteric-sigdigs*) or email me at *ericli3690@gmail.com*.
 
-## 🛠 Installation
+## 🛠 Installation and Use
 
 `>> pip install esoteric-sigdigs`
 
+```python
+from sigdigs import sigdigs
+sigdigs.function_name_here(arguments_here)
+```
+
 ## 🧪 What is Scientific Notation?
 
 Scientific notation is often used by this package, a string formatting of numbers which takes the following form:
 
 `a.bcdEf`
 
 And which can be written in standard formatting as
```

### Comparing `esoteric-sigdigs-0.1.1/esoteric_sigdigs.egg-info/PKG-INFO` & `esoteric-sigdigs-0.1.2/esoteric_sigdigs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esoteric-sigdigs
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package that detects and rounds numbers to significant digits.
 Home-page: https://github.com/ericli3690/esoteric-sigdigs/
 Author: Eric Li
 Author-email: ericli3690@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,18 +15,23 @@
 # esoteric-sigdigs
 **🐍 A Python package that detects and rounds numbers to significant digits.**
 
 This package aims to provide easy-to-use functions to work with significant digits (also known as significant figures).
 
 ⚠ Please note that this package is almost certainly laced with bugs, so use it at your own risk! Additionally, the significant digit rules used may not be exactly what you are looking for; I have designed this package to fit the likely-esoteric way I have been taught to use significant digits. Sorry! If you encounter any issues, please create an issue on GitHub (*https://github.com/ericli3690/esoteric-sigdigs*) or email me at *ericli3690@gmail.com*.
 
-## 🛠 Installation
+## 🛠 Installation and Use
 
 `>> pip install esoteric-sigdigs`
 
+```python
+from sigdigs import sigdigs
+sigdigs.function_name_here(arguments_here)
+```
+
 ## 🧪 What is Scientific Notation?
 
 Scientific notation is often used by this package, a string formatting of numbers which takes the following form:
 
 `a.bcdEf`
 
 And which can be written in standard formatting as
```

### Comparing `esoteric-sigdigs-0.1.1/setup.cfg` & `esoteric-sigdigs-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 736f 7465 7269 632d 7369 6764   = esoteric-sigd
 00000020: 6967 730d 0a76 6572 7369 6f6e 203d 2030  igs..version = 0
-00000030: 2e31 2e31 0d0a 6175 7468 6f72 203d 2045  .1.1..author = E
+00000030: 2e31 2e32 0d0a 6175 7468 6f72 203d 2045  .1.2..author = E
 00000040: 7269 6320 4c69 0d0a 6175 7468 6f72 5f65  ric Li..author_e
 00000050: 6d61 696c 203d 2065 7269 636c 6933 3639  mail = ericli369
 00000060: 3040 676d 6169 6c2e 636f 6d0d 0a64 6573  0@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2041 2050 7974  cription = A Pyt
 00000080: 686f 6e20 7061 636b 6167 6520 7468 6174  hon package that
 00000090: 2064 6574 6563 7473 2061 6e64 2072 6f75   detects and rou
 000000a0: 6e64 7320 6e75 6d62 6572 7320 746f 2073  nds numbers to s
```

