# Comparing `tmp/lilyponddist-0.4.0.tar.gz` & `tmp/lilyponddist-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilyponddist-0.4.0.tar", last modified: Tue Jun 27 14:55:13 2023, max compression
+gzip compressed data, was "lilyponddist-0.4.1.tar", last modified: Tue Jun 27 15:16:16 2023, max compression
```

## Comparing `lilyponddist-0.4.0.tar` & `lilyponddist-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 14:55:13.087331 lilyponddist-0.4.0/
--rw-r--r--   0 em        (1000) em        (1000)     2079 2023-04-17 21:56:53.000000 lilyponddist-0.4.0/LICENSE
--rw-rw-r--   0 em        (1000) em        (1000)     1008 2023-06-27 14:55:13.087331 lilyponddist-0.4.0/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      731 2023-04-25 09:31:19.000000 lilyponddist-0.4.0/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 14:55:13.082331 lilyponddist-0.4.0/lilyponddist/
--rw-rw-r--   0 em        (1000) em        (1000)     7121 2023-06-27 14:54:47.000000 lilyponddist-0.4.0/lilyponddist/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 14:55:13.086331 lilyponddist-0.4.0/lilyponddist.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     1008 2023-06-27 14:55:13.000000 lilyponddist-0.4.0/lilyponddist.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      245 2023-06-27 14:55:13.000000 lilyponddist-0.4.0/lilyponddist.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-06-27 14:55:13.000000 lilyponddist-0.4.0/lilyponddist.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       20 2023-06-27 14:55:13.000000 lilyponddist-0.4.0/lilyponddist.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       13 2023-06-27 14:55:13.000000 lilyponddist-0.4.0/lilyponddist.egg-info/top_level.txt
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-06-27 14:55:13.087331 lilyponddist-0.4.0/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)      720 2023-04-18 15:49:06.000000 lilyponddist-0.4.0/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 14:55:13.086331 lilyponddist-0.4.0/test/
--rw-r--r--   0 em        (1000) em        (1000)      328 2023-04-18 15:58:18.000000 lilyponddist-0.4.0/test/test1.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 15:16:16.027705 lilyponddist-0.4.1/
+-rw-r--r--   0 em        (1000) em        (1000)     2079 2023-04-17 21:56:53.000000 lilyponddist-0.4.1/LICENSE
+-rw-rw-r--   0 em        (1000) em        (1000)     1008 2023-06-27 15:16:16.027705 lilyponddist-0.4.1/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      731 2023-04-25 09:31:19.000000 lilyponddist-0.4.1/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 15:16:16.025705 lilyponddist-0.4.1/lilyponddist/
+-rw-rw-r--   0 em        (1000) em        (1000)     7383 2023-06-27 15:15:58.000000 lilyponddist-0.4.1/lilyponddist/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 15:16:16.026705 lilyponddist-0.4.1/lilyponddist.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     1008 2023-06-27 15:16:15.000000 lilyponddist-0.4.1/lilyponddist.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      245 2023-06-27 15:16:16.000000 lilyponddist-0.4.1/lilyponddist.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-06-27 15:16:15.000000 lilyponddist-0.4.1/lilyponddist.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       20 2023-06-27 15:16:15.000000 lilyponddist-0.4.1/lilyponddist.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       13 2023-06-27 15:16:15.000000 lilyponddist-0.4.1/lilyponddist.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-06-27 15:16:16.027705 lilyponddist-0.4.1/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)      720 2023-04-18 15:49:06.000000 lilyponddist-0.4.1/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 15:16:16.026705 lilyponddist-0.4.1/test/
+-rw-r--r--   0 em        (1000) em        (1000)      328 2023-04-18 15:58:18.000000 lilyponddist-0.4.1/test/test1.py
```

### Comparing `lilyponddist-0.4.0/LICENSE` & `lilyponddist-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lilyponddist-0.4.0/PKG-INFO` & `lilyponddist-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilyponddist
-Version: 0.4.0
+Version: 0.4.1
 Summary: Distribute lilypond as a pypi package
 Home-page: https://github.com/gesellkammer/lilyponddist
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 lilyponddist
```

### Comparing `lilyponddist-0.4.0/README.rst` & `lilyponddist-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `lilyponddist-0.4.0/lilyponddist/__init__.py` & `lilyponddist-0.4.1/lilyponddist/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 
 
-__VERSION__ = "0.4.0"
+__VERSION__ = "0.4.1"
 
 if __name__ == '__main__':
     if len(sys.argv) > 1 and sys.argv[1] == '--version':
         print(__VERSION__)
     sys.exit(0)
 
 
@@ -155,26 +155,26 @@
     if arch not in ('x64', 'x86_64'):
         logger.error(f"At the moment only x64 architecture is supported, got {arch}")
         return
 
     download_lilypond(osname=osname)
 
 
-def _get_platform() -> tuple[str, str]:
+def _get_platform(normalize=True) -> tuple[str, str]:
     """
     Return a string with current platform (system and machine architecture).
 
     This attempts to improve upon `sysconfig._get_platform` by fixing some
     issues when running a Python interpreter with a different architecture than
     that of the system (e.g. 32bit on 64bit system, or a multiarch build),
     which should return the machine architecture of the currently running
     interpreter rather than that of the system (which didn't seem to work
     properly). The reported machine architectures follow platform-specific
     naming conventions (e.g. "x86_64" on Linux, but "x64" on Windows).
-
+    Use normalize=True to reduce those labels (returns one of 'x86_64', 'arm64', 'x86')
     Example output strings for common platforms:
 
         darwin_(ppc|ppc64|i368|x86_64|arm64)
         linux_(i686|x86_64|armv7l|aarch64)
         windows_(x86|x64|arm32|arm64)
 
     """
@@ -205,14 +205,20 @@
     # some more fixes based on examples in https://en.wikipedia.org/wiki/Uname
     if not is_64bit and machine in ("x86_64", "amd64"):
         if any([x in system for x in ("cygwin", "mingw", "msys")]):
             machine = "i686"
         else:
             machine = "i386"
 
+    if normalize:
+        machine = {
+            'x64': 'x86_64',
+            'aarch64': 'arm64',
+            'amd64': 'x86_64'
+        }.get(machine, machine)
     return system, machine
 
 
 def lilypondroot() -> Path:
     return _lilyponddist_folder() / "lilypond-2.24.1"
```

### Comparing `lilyponddist-0.4.0/lilyponddist.egg-info/PKG-INFO` & `lilyponddist-0.4.1/lilyponddist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilyponddist
-Version: 0.4.0
+Version: 0.4.1
 Summary: Distribute lilypond as a pypi package
 Home-page: https://github.com/gesellkammer/lilyponddist
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 lilyponddist
```

### Comparing `lilyponddist-0.4.0/setup.py` & `lilyponddist-0.4.1/setup.py`

 * *Files identical despite different names*

