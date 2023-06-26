# Comparing `tmp/ignoreexceptions-0.10.tar.gz` & `tmp/ignoreexceptions-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignoreexceptions-0.10.tar", last modified: Mon Jun 26 22:44:18 2023, max compression
+gzip compressed data, was "ignoreexceptions-0.11.tar", last modified: Mon Jun 26 23:16:11 2023, max compression
```

## Comparing `ignoreexceptions-0.10.tar` & `ignoreexceptions-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 22:44:18.408510 ignoreexceptions-0.10/
--rw-rw-rw-   0        0        0     1148 2023-06-26 22:44:12.000000 ignoreexceptions-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      119 2023-06-26 22:44:12.000000 ignoreexceptions-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     6410 2023-06-26 22:44:18.408510 ignoreexceptions-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     5704 2023-06-26 22:40:50.000000 ignoreexceptions-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 22:44:18.404521 ignoreexceptions-0.10/ignoreexceptions/
--rw-rw-rw-   0        0        0     5704 2023-06-26 22:40:50.000000 ignoreexceptions-0.10/ignoreexceptions/README.MD
--rw-rw-rw-   0        0        0     5041 2023-06-26 22:41:52.000000 ignoreexceptions-0.10/ignoreexceptions/__init__.py
--rw-rw-rw-   0        0        0       10 2023-06-26 22:44:17.000000 ignoreexceptions-0.10/ignoreexceptions/requirements.txt
--rw-rw-rw-   0        0        0     1248 2023-06-26 22:44:17.000000 ignoreexceptions-0.10/ignoreexceptions/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-06-26 22:44:18.407513 ignoreexceptions-0.10/ignoreexceptions.egg-info/
--rw-rw-rw-   0        0        0     6410 2023-06-26 22:44:18.000000 ignoreexceptions-0.10/ignoreexceptions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-26 22:44:18.000000 ignoreexceptions-0.10/ignoreexceptions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 22:44:18.000000 ignoreexceptions-0.10/ignoreexceptions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 22:44:18.000000 ignoreexceptions-0.10/ignoreexceptions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-26 22:44:18.000000 ignoreexceptions-0.10/ignoreexceptions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-06-26 22:44:18.409507 ignoreexceptions-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1369 2023-06-26 22:44:17.000000 ignoreexceptions-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 23:16:11.904120 ignoreexceptions-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-06-26 23:16:05.000000 ignoreexceptions-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      119 2023-06-26 23:16:04.000000 ignoreexceptions-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     6410 2023-06-26 23:16:11.905117 ignoreexceptions-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     5704 2023-06-26 22:40:50.000000 ignoreexceptions-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 23:16:11.901127 ignoreexceptions-0.11/ignoreexceptions/
+-rw-rw-rw-   0        0        0     5704 2023-06-26 22:40:50.000000 ignoreexceptions-0.11/ignoreexceptions/README.MD
+-rw-rw-rw-   0        0        0     5006 2023-06-26 23:14:33.000000 ignoreexceptions-0.11/ignoreexceptions/__init__.py
+-rw-rw-rw-   0        0        0       10 2023-06-26 23:16:11.000000 ignoreexceptions-0.11/ignoreexceptions/requirements.txt
+-rw-rw-rw-   0        0        0     1248 2023-06-26 23:16:11.000000 ignoreexceptions-0.11/ignoreexceptions/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-06-26 23:16:11.904120 ignoreexceptions-0.11/ignoreexceptions.egg-info/
+-rw-rw-rw-   0        0        0     6410 2023-06-26 23:16:11.000000 ignoreexceptions-0.11/ignoreexceptions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-26 23:16:11.000000 ignoreexceptions-0.11/ignoreexceptions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 23:16:11.000000 ignoreexceptions-0.11/ignoreexceptions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 23:16:11.000000 ignoreexceptions-0.11/ignoreexceptions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-26 23:16:11.000000 ignoreexceptions-0.11/ignoreexceptions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-26 23:16:11.905117 ignoreexceptions-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1369 2023-06-26 23:16:11.000000 ignoreexceptions-0.11/setup.py
```

### Comparing `ignoreexceptions-0.10/LICENSE.rst` & `ignoreexceptions-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ignoreexceptions-0.10/PKG-INFO` & `ignoreexceptions-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignoreexceptions
-Version: 0.10
+Version: 0.11
 Summary: Decorators that provide graceful exception handling, customization of error handling behavior, error logging
 Home-page: https://github.com/hansalemaos/ignoreexceptions
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: ignore,exceptions,decorator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ignoreexceptions-0.10/README.md` & `ignoreexceptions-0.11/README.md`

 * *Files identical despite different names*

### Comparing `ignoreexceptions-0.10/ignoreexceptions/README.MD` & `ignoreexceptions-0.11/ignoreexceptions/README.MD`

 * *Files identical despite different names*

### Comparing `ignoreexceptions-0.10/ignoreexceptions/__init__.py` & `ignoreexceptions-0.11/ignoreexceptions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,27 +68,27 @@
     def _decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             def handle_ex(ex):
                 nonlocal result
                 if print_exceptions:
                     print(ex)
+                    traceback.print_exc()
+
                 if not active:
                     raise ex
                 if logfile:
                     _write2logfile(logfile, traceback.format_exc())
                 result = v
 
             result = v
             try:
                 result = func(*args, **kwargs)
             except Exception as e:
                 handle_ex(e)
-            except BaseExceptionGroup as e:
-                handle_ex(e)
             except KeyboardInterrupt as e:
                 handle_ex(e)
             except SystemExit as e:
                 handle_ex(e)
             return result
 
         return wrapper
@@ -140,12 +140,12 @@
     return _decorator(f_py) if callable(f_py) else _decorator
 
 
 def _write2logfile(logfile, infos):
     if not os.path.exists(logfile):
         touch(logfile)
     with open(logfile, mode="a", encoding="utf-8") as f:
-        f.write(f"\n\n{get_timestamp()}\n{str(infos)}\n---------------------------")
+        f.write(f"\n\n{get_timestamp()}\n{infos}\n---------------------------")
 
 
 def get_timestamp():
     return datetime.datetime.now().strftime("%Y/%m/%d %H:%M:%S.%f")
```

### Comparing `ignoreexceptions-0.10/ignoreexceptions/thirdparty.json` & `ignoreexceptions-0.11/ignoreexceptions/thirdparty.json`

 * *Files identical despite different names*

### Comparing `ignoreexceptions-0.10/ignoreexceptions.egg-info/PKG-INFO` & `ignoreexceptions-0.11/ignoreexceptions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignoreexceptions
-Version: 0.10
+Version: 0.11
 Summary: Decorators that provide graceful exception handling, customization of error handling behavior, error logging
 Home-page: https://github.com/hansalemaos/ignoreexceptions
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: ignore,exceptions,decorator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ignoreexceptions-0.10/setup.py` & `ignoreexceptions-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Decorators that provide graceful exception handling, customization of error handling behavior, error logging'''
 
 # Setting up
 setup(
     name="ignoreexceptions",
     version=VERSION,
     license='MIT',
```

