# Comparing `tmp/xsskiller-1.0.0.tar.gz` & `tmp/xsskiller-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsskiller-1.0.0.tar", last modified: Tue Jun 27 01:55:58 2023, max compression
+gzip compressed data, was "xsskiller-1.0.1.tar", last modified: Tue Jun 27 03:00:09 2023, max compression
```

## Comparing `xsskiller-1.0.0.tar` & `xsskiller-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-27 01:55:58.549567 xsskiller-1.0.0/
--rwxrwxrwx   0 abel      (1000) abel      (1000)     1537 2023-06-27 01:55:58.549425 xsskiller-1.0.0/PKG-INFO
--rwxrwxrwx   0 abel      (1000) abel      (1000)      820 2023-06-25 04:47:42.000000 xsskiller-1.0.0/README.md
--rwxrwxrwx   0 abel      (1000) abel      (1000)       38 2023-06-27 01:55:58.549615 xsskiller-1.0.0/setup.cfg
--rwxrwxrwx   0 abel      (1000) abel      (1000)      997 2023-06-27 01:55:55.000000 xsskiller-1.0.0/setup.py
-drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-27 01:55:58.547450 xsskiller-1.0.0/xsskiller/
--rwxrwxrwx   0 abel      (1000) abel      (1000)       56 2023-06-25 05:04:58.000000 xsskiller-1.0.0/xsskiller/__init__.py
--rwxrwxrwx   0 abel      (1000) abel      (1000)     5696 2023-06-27 01:53:28.000000 xsskiller-1.0.0/xsskiller/xsskiller.py
-drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-27 01:55:58.549056 xsskiller-1.0.0/xsskiller.egg-info/
--rwxrwxrwx   0 abel      (1000) abel      (1000)     1537 2023-06-27 01:55:58.000000 xsskiller-1.0.0/xsskiller.egg-info/PKG-INFO
--rwxrwxrwx   0 abel      (1000) abel      (1000)      263 2023-06-27 01:55:58.000000 xsskiller-1.0.0/xsskiller.egg-info/SOURCES.txt
--rwxrwxrwx   0 abel      (1000) abel      (1000)        1 2023-06-27 01:55:58.000000 xsskiller-1.0.0/xsskiller.egg-info/dependency_links.txt
--rwxrwxrwx   0 abel      (1000) abel      (1000)       56 2023-06-27 01:55:58.000000 xsskiller-1.0.0/xsskiller.egg-info/entry_points.txt
--rwxrwxrwx   0 abel      (1000) abel      (1000)       18 2023-06-27 01:55:58.000000 xsskiller-1.0.0/xsskiller.egg-info/requires.txt
--rwxrwxrwx   0 abel      (1000) abel      (1000)       10 2023-06-27 01:55:58.000000 xsskiller-1.0.0/xsskiller.egg-info/top_level.txt
+drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-27 03:00:09.151005 xsskiller-1.0.1/
+-rwxrwxrwx   0 abel      (1000) abel      (1000)     1141 2023-06-27 03:00:09.150837 xsskiller-1.0.1/PKG-INFO
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      472 2023-06-27 02:58:18.000000 xsskiller-1.0.1/README.md
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       38 2023-06-27 03:00:09.151060 xsskiller-1.0.1/setup.cfg
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      997 2023-06-27 02:58:48.000000 xsskiller-1.0.1/setup.py
+drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-27 03:00:09.148804 xsskiller-1.0.1/xsskiller/
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       56 2023-06-27 02:58:37.000000 xsskiller-1.0.1/xsskiller/__init__.py
+-rwxrwxrwx   0 abel      (1000) abel      (1000)     5696 2023-06-27 01:53:28.000000 xsskiller-1.0.1/xsskiller/xsskiller.py
+drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-27 03:00:09.150492 xsskiller-1.0.1/xsskiller.egg-info/
+-rwxrwxrwx   0 abel      (1000) abel      (1000)     1141 2023-06-27 03:00:09.000000 xsskiller-1.0.1/xsskiller.egg-info/PKG-INFO
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      263 2023-06-27 03:00:09.000000 xsskiller-1.0.1/xsskiller.egg-info/SOURCES.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)        1 2023-06-27 03:00:09.000000 xsskiller-1.0.1/xsskiller.egg-info/dependency_links.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       56 2023-06-27 03:00:09.000000 xsskiller-1.0.1/xsskiller.egg-info/entry_points.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       18 2023-06-27 03:00:09.000000 xsskiller-1.0.1/xsskiller.egg-info/requires.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       10 2023-06-27 03:00:09.000000 xsskiller-1.0.1/xsskiller.egg-info/top_level.txt
```

### Comparing `xsskiller-1.0.0/setup.py` & `xsskiller-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="xsskiller",
-    version="1.0.0",
+    version="1.0.1",
     description="Automated tool scans URLS parameters to check if reflected XSS is vulnerable",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/abeljm/XSSKiller",
     author="Avelino Navarro",
     author_email="abeljm2017@gmail.com",
     classifiers=[
```

### Comparing `xsskiller-1.0.0/xsskiller/xsskiller.py` & `xsskiller-1.0.1/xsskiller/xsskiller.py`

 * *Files identical despite different names*

