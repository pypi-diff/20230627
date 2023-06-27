# Comparing `tmp/lilyponddist-0.3.0.tar.gz` & `tmp/lilyponddist-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilyponddist-0.3.0.tar", last modified: Tue Apr 18 16:00:21 2023, max compression
+gzip compressed data, was "lilyponddist-0.4.0.tar", last modified: Tue Jun 27 14:55:13 2023, max compression
```

## Comparing `lilyponddist-0.3.0.tar` & `lilyponddist-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 16:00:21.126271 lilyponddist-0.3.0/
--rw-r--r--   0 em        (1000) em        (1000)     2079 2023-04-17 21:56:53.000000 lilyponddist-0.3.0/LICENSE
--rw-rw-r--   0 em        (1000) em        (1000)      965 2023-04-18 16:00:21.126271 lilyponddist-0.3.0/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      688 2023-04-18 15:30:21.000000 lilyponddist-0.3.0/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 16:00:21.124271 lilyponddist-0.3.0/lilyponddist/
--rw-rw-r--   0 em        (1000) em        (1000)     6872 2023-04-18 16:00:13.000000 lilyponddist-0.3.0/lilyponddist/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 16:00:21.125271 lilyponddist-0.3.0/lilyponddist.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)      965 2023-04-18 16:00:21.000000 lilyponddist-0.3.0/lilyponddist.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      245 2023-04-18 16:00:21.000000 lilyponddist-0.3.0/lilyponddist.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-18 16:00:21.000000 lilyponddist-0.3.0/lilyponddist.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       20 2023-04-18 16:00:21.000000 lilyponddist-0.3.0/lilyponddist.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       13 2023-04-18 16:00:21.000000 lilyponddist-0.3.0/lilyponddist.egg-info/top_level.txt
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-18 16:00:21.127271 lilyponddist-0.3.0/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)      720 2023-04-18 15:49:06.000000 lilyponddist-0.3.0/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 16:00:21.126271 lilyponddist-0.3.0/test/
--rw-r--r--   0 em        (1000) em        (1000)      328 2023-04-18 15:58:18.000000 lilyponddist-0.3.0/test/test1.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 14:55:13.087331 lilyponddist-0.4.0/
+-rw-r--r--   0 em        (1000) em        (1000)     2079 2023-04-17 21:56:53.000000 lilyponddist-0.4.0/LICENSE
+-rw-rw-r--   0 em        (1000) em        (1000)     1008 2023-06-27 14:55:13.087331 lilyponddist-0.4.0/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      731 2023-04-25 09:31:19.000000 lilyponddist-0.4.0/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 14:55:13.082331 lilyponddist-0.4.0/lilyponddist/
+-rw-rw-r--   0 em        (1000) em        (1000)     7121 2023-06-27 14:54:47.000000 lilyponddist-0.4.0/lilyponddist/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 14:55:13.086331 lilyponddist-0.4.0/lilyponddist.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     1008 2023-06-27 14:55:13.000000 lilyponddist-0.4.0/lilyponddist.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      245 2023-06-27 14:55:13.000000 lilyponddist-0.4.0/lilyponddist.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-06-27 14:55:13.000000 lilyponddist-0.4.0/lilyponddist.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       20 2023-06-27 14:55:13.000000 lilyponddist-0.4.0/lilyponddist.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       13 2023-06-27 14:55:13.000000 lilyponddist-0.4.0/lilyponddist.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-06-27 14:55:13.087331 lilyponddist-0.4.0/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)      720 2023-04-18 15:49:06.000000 lilyponddist-0.4.0/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-06-27 14:55:13.086331 lilyponddist-0.4.0/test/
+-rw-r--r--   0 em        (1000) em        (1000)      328 2023-04-18 15:58:18.000000 lilyponddist-0.4.0/test/test1.py
```

### Comparing `lilyponddist-0.3.0/LICENSE` & `lilyponddist-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lilyponddist-0.3.0/PKG-INFO` & `lilyponddist-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilyponddist
-Version: 0.3.0
+Version: 0.4.0
 Summary: Distribute lilypond as a pypi package
 Home-page: https://github.com/gesellkammer/lilyponddist
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 lilyponddist
@@ -32,7 +32,12 @@
 .. code:: python
 
     import lilyponddist
     import subprocess
 
     subprocess.call([lilyponddist.lilypondbin(), '/path/to/score.ly', '--pdf', '-o', '/path/to/output'])
 
+
+TODO
+----
+
+* Reimplement this using pooch
```

### Comparing `lilyponddist-0.3.0/README.rst` & `lilyponddist-0.4.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -23,7 +23,12 @@
 .. code:: python
 
     import lilyponddist
     import subprocess
 
     subprocess.call([lilyponddist.lilypondbin(), '/path/to/score.ly', '--pdf', '-o', '/path/to/output'])
 
+
+TODO
+----
+
+* Reimplement this using pooch
```

### Comparing `lilyponddist-0.3.0/lilyponddist/__init__.py` & `lilyponddist-0.4.0/lilyponddist/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 
 
-__VERSION__ = "0.3.0"
+__VERSION__ = "0.4.0"
 
 if __name__ == '__main__':
     if len(sys.argv) > 1 and sys.argv[1] == '--version':
         print(__VERSION__)
     sys.exit(0)
 
 
@@ -18,14 +18,21 @@
 import tempfile
 import appdirs
 import shutil
 import progressbar
 from typing import Union
 
 
+urls = {
+    ('windows', 'x86_64'): "https://gitlab.com/lilypond/lilypond/-/releases/v2.24.1/downloads/lilypond-2.24.1-mingw-x86_64.zip",
+    ('linux', 'x86_64'): "https://gitlab.com/lilypond/lilypond/-/releases/v2.24.1/downloads/lilypond-2.24.1-linux-x86_64.tar.gz",
+    ('darwin', 'x86_64'): "https://gitlab.com/lilypond/lilypond/-/releases/v2.24.1/downloads/lilypond-2.24.1-darwin-x86_64.tar.gz"
+}
+    
+
 logger = logging.getLogger("lilyponddist")
 
 
 class _ProgressBar():
 
     def __init__(self):
         self.pbar = None
@@ -79,29 +86,31 @@
         raise RuntimeError(f"File format of {path} not supported")
 
 
 def _lilyponddist_folder() -> Path:
     return Path(appdirs.user_data_dir('lilyponddist'))
 
 
-def download_lilypond(osname: str, arch='x86_64', showprogress=True) -> Path:
+def download_lilypond(osname: str = '', arch='', showprogress=True) -> Path:
     """
     Downloads lilypond, expands it and returns the root path
 
     Args:
         osname: one of 'linux', 'windows', 'darwin'
         arch: one of 'x86_64', 'arm64'. At the moment only x86_64 is supported
 
     Returns:
         the destination folder. This will be something like '~/.local/share/lilyponddist/lilypond-2.24.1'
     """
-    urls = {
-        ('windows', 'x86_64'): "https://gitlab.com/lilypond/lilypond/-/releases/v2.24.1/downloads/lilypond-2.24.1-mingw-x86_64.zip",
-        ('linux', 'x86_64'): "https://gitlab.com/lilypond/lilypond/-/releases/v2.24.1/downloads/lilypond-2.24.1-linux-x86_64.tar.gz",
-    }
+    _osname, _arch = _get_platform()
+    if not osname:
+        osname = _osname 
+    if not arch:
+        arch = _arch
+        
     url = urls.get((osname, arch))
     if url is None:
         platforms = [f"{osname}-{arch}" for osname, arch in urls.keys()]
         raise KeyError(f"Platform {osname}-{arch} not supported. Possible platforms: {platforms}")
 
     tempdir = Path(tempfile.gettempdir())
     payload = _download(url, tempdir, showprogress=showprogress)
```

### Comparing `lilyponddist-0.3.0/lilyponddist.egg-info/PKG-INFO` & `lilyponddist-0.4.0/lilyponddist.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilyponddist
-Version: 0.3.0
+Version: 0.4.0
 Summary: Distribute lilypond as a pypi package
 Home-page: https://github.com/gesellkammer/lilyponddist
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 lilyponddist
@@ -32,7 +32,12 @@
 .. code:: python
 
     import lilyponddist
     import subprocess
 
     subprocess.call([lilyponddist.lilypondbin(), '/path/to/score.ly', '--pdf', '-o', '/path/to/output'])
 
+
+TODO
+----
+
+* Reimplement this using pooch
```

### Comparing `lilyponddist-0.3.0/setup.py` & `lilyponddist-0.4.0/setup.py`

 * *Files identical despite different names*

