# Comparing `tmp/release-gitter-2.1.0.tar.gz` & `tmp/release-gitter-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "release-gitter-2.1.0.tar", last modified: Mon Jun  5 19:03:23 2023, max compression
+gzip compressed data, was "release-gitter-2.1.1.tar", last modified: Mon Jun 26 23:46:06 2023, max compression
```

## Comparing `release-gitter-2.1.0.tar` & `release-gitter-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:03:23.315115 release-gitter-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     1096 2023-06-05 19:02:51.000000 release-gitter-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5096 2023-06-05 19:03:23.315115 release-gitter-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4445 2023-06-05 19:02:51.000000 release-gitter-2.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     4691 2023-06-05 19:02:51.000000 release-gitter-2.1.0/pseudo_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 19:03:23.315115 release-gitter-2.1.0/release_gitter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5096 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-05 19:03:23.000000 release-gitter-2.1.0/release_gitter.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)    18423 2023-06-05 19:02:51.000000 release-gitter-2.1.0/release_gitter.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 19:03:23.315115 release-gitter-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1254 2023-06-05 19:02:51.000000 release-gitter-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 23:46:06.648733 release-gitter-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-06-26 23:45:34.000000 release-gitter-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-06-26 23:46:06.648733 release-gitter-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4445 2023-06-26 23:45:34.000000 release-gitter-2.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-06-26 23:45:34.000000 release-gitter-2.1.1/pseudo_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 23:46:06.648733 release-gitter-2.1.1/release_gitter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-06-26 23:46:06.000000 release-gitter-2.1.1/release_gitter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-26 23:46:06.000000 release-gitter-2.1.1/release_gitter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 23:46:06.000000 release-gitter-2.1.1/release_gitter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-26 23:46:06.000000 release-gitter-2.1.1/release_gitter.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-26 23:46:06.000000 release-gitter-2.1.1/release_gitter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-26 23:46:06.000000 release-gitter-2.1.1/release_gitter.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)    18578 2023-06-26 23:45:34.000000 release-gitter-2.1.1/release_gitter.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 23:46:06.648733 release-gitter-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-06-26 23:45:34.000000 release-gitter-2.1.1/setup.py
```

### Comparing `release-gitter-2.1.0/LICENSE` & `release-gitter-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `release-gitter-2.1.0/PKG-INFO` & `release-gitter-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: release-gitter
-Version: 2.1.0
+Version: 2.1.1
 Summary: Easily download releases from sites like Github and Gitea
 Home-page: https://git.iamthefij.com/iamthefij/release-gitter.git
 Download-URL: https://git.iamthefij.com/iamthefij/release-gitter.git/archive/master.tar.gz
 Author: iamthefij
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `release-gitter-2.1.0/README.md` & `release-gitter-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `release-gitter-2.1.0/pseudo_builder.py` & `release-gitter-2.1.1/pseudo_builder.py`

 * *Files identical despite different names*

### Comparing `release-gitter-2.1.0/release_gitter.egg-info/PKG-INFO` & `release-gitter-2.1.1/release_gitter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: release-gitter
-Version: 2.1.0
+Version: 2.1.1
 Summary: Easily download releases from sites like Github and Gitea
 Home-page: https://git.iamthefij.com/iamthefij/release-gitter.git
 Download-URL: https://git.iamthefij.com/iamthefij/release-gitter.git/archive/master.tar.gz
 Author: iamthefij
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `release-gitter-2.1.0/release_gitter.py` & `release-gitter-2.1.1/release_gitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,18 @@
         If the `file_names` list is empty, all files will be extracted"""
         if path is None:
             path = Path.cwd()
         if not members:
             self._package.extractall(path=path)
             return self.get_names()
 
+        missing_members = set(members) - set(self.get_names())
+        if missing_members:
+            raise ValueError(f"Missing members: {missing_members}")
+
         if isinstance(self._package, ZipFile):
             self._package.extractall(path=path, members=members)
         if isinstance(self._package, TarFile):
             self._package.extractall(
                 path=path, members=(TarInfo(name) for name in members)
             )
 
@@ -488,21 +492,21 @@
         "-c",
         help="Shell commands to execute after download or extraction. {} will be expanded to the downloaded asset name.",
     )
     parser.add_argument(
         "--extract-files",
         "-e",
         action="append",
-        help="A list of file names to extract from downloaded archive",
+        help="A list of file names to extract from the downloaded archive",
     )
     parser.add_argument(
         "--extract-all",
         "-x",
         action="store_true",
-        help="Shell commands to execute after download or extraction",
+        help="Extract all files from the downloaded archive",
     )
     parser.add_argument(
         "--url-only",
         action="store_true",
         help="Only print the URL and do not download",
     )
```

### Comparing `release-gitter-2.1.0/setup.py` & `release-gitter-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="release-gitter",
-    version="2.1.0",
+    version="2.1.1",
     description="Easily download releases from sites like Github and Gitea",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.iamthefij.com/iamthefij/release-gitter.git",
     download_url=(
         "https://git.iamthefij.com/iamthefij/release-gitter.git/archive/master.tar.gz"
     ),
```

