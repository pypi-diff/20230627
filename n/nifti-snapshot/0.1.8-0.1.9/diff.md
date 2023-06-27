# Comparing `tmp/nifti_snapshot-0.1.8.tar.gz` & `tmp/nifti_snapshot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifti_snapshot-0.1.8.tar", last modified: Mon Jan  3 16:16:25 2022, max compression
+gzip compressed data, was "nifti_snapshot-0.1.9.tar", last modified: Mon Jan  3 16:18:53 2022, max compression
```

## Comparing `nifti_snapshot-0.1.8.tar` & `nifti_snapshot-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kc244      (501) staff       (20)        0 2022-01-03 16:16:25.044228 nifti_snapshot-0.1.8/
--rw-r--r--   0 kc244      (501) staff       (20)     3320 2022-01-03 16:16:25.044327 nifti_snapshot-0.1.8/PKG-INFO
--rwxr-xr-x   0 kc244      (501) staff       (20)     2805 2021-03-22 15:13:04.000000 nifti_snapshot-0.1.8/README.md
--rw-r--r--   0 kc244      (501) staff       (20)      446 2021-03-22 15:13:04.000000 nifti_snapshot-0.1.8/enigma_download.sh
-drwxr-xr-x   0 kc244      (501) staff       (20)        0 2022-01-03 16:16:25.041909 nifti_snapshot-0.1.8/nifti_snapshot/
--rwxr-xr-x   0 kc244      (501) staff       (20)        0 2021-03-22 15:13:04.000000 nifti_snapshot-0.1.8/nifti_snapshot/__init__.py
--rwxr-xr-x   0 kc244      (501) staff       (20)    23983 2021-09-04 09:04:49.000000 nifti_snapshot-0.1.8/nifti_snapshot/nifti_snapshot.py
--rw-r--r--   0 kc244      (501) staff       (20)      717 2021-03-22 15:13:04.000000 nifti_snapshot-0.1.8/nifti_snapshot/nifti_snapshot_utils.py
-drwxr-xr-x   0 kc244      (501) staff       (20)        0 2022-01-03 16:16:25.043612 nifti_snapshot-0.1.8/nifti_snapshot.egg-info/
--rw-r--r--   0 kc244      (501) staff       (20)     3320 2022-01-03 16:16:25.000000 nifti_snapshot-0.1.8/nifti_snapshot.egg-info/PKG-INFO
--rw-r--r--   0 kc244      (501) staff       (20)      358 2022-01-03 16:16:25.000000 nifti_snapshot-0.1.8/nifti_snapshot.egg-info/SOURCES.txt
--rw-r--r--   0 kc244      (501) staff       (20)        1 2022-01-03 16:16:25.000000 nifti_snapshot-0.1.8/nifti_snapshot.egg-info/dependency_links.txt
--rw-r--r--   0 kc244      (501) staff       (20)       76 2022-01-03 16:16:25.000000 nifti_snapshot-0.1.8/nifti_snapshot.egg-info/requires.txt
--rw-r--r--   0 kc244      (501) staff       (20)       15 2022-01-03 16:16:25.000000 nifti_snapshot-0.1.8/nifti_snapshot.egg-info/top_level.txt
-drwxr-xr-x   0 kc244      (501) staff       (20)        0 2022-01-03 16:16:25.043932 nifti_snapshot-0.1.8/scripts/
--rwxr-xr-x   0 kc244      (501) staff       (20)     4627 2021-09-04 09:08:14.000000 nifti_snapshot-0.1.8/scripts/nifti_snapshot
--rw-r--r--   0 kc244      (501) staff       (20)       79 2022-01-03 16:16:25.044752 nifti_snapshot-0.1.8/setup.cfg
--rw-r--r--   0 kc244      (501) staff       (20)     1109 2022-01-03 16:16:16.000000 nifti_snapshot-0.1.8/setup.py
+drwxr-xr-x   0 kc244      (501) staff       (20)        0 2022-01-03 16:18:53.740634 nifti_snapshot-0.1.9/
+-rw-r--r--   0 kc244      (501) staff       (20)     3320 2022-01-03 16:18:53.740748 nifti_snapshot-0.1.9/PKG-INFO
+-rwxr-xr-x   0 kc244      (501) staff       (20)     2805 2021-03-22 15:13:04.000000 nifti_snapshot-0.1.9/README.md
+-rw-r--r--   0 kc244      (501) staff       (20)      446 2021-03-22 15:13:04.000000 nifti_snapshot-0.1.9/enigma_download.sh
+drwxr-xr-x   0 kc244      (501) staff       (20)        0 2022-01-03 16:18:53.738319 nifti_snapshot-0.1.9/nifti_snapshot/
+-rwxr-xr-x   0 kc244      (501) staff       (20)        0 2021-03-22 15:13:04.000000 nifti_snapshot-0.1.9/nifti_snapshot/__init__.py
+-rwxr-xr-x   0 kc244      (501) staff       (20)    23983 2021-09-04 09:04:49.000000 nifti_snapshot-0.1.9/nifti_snapshot/nifti_snapshot.py
+-rw-r--r--   0 kc244      (501) staff       (20)      717 2021-03-22 15:13:04.000000 nifti_snapshot-0.1.9/nifti_snapshot/nifti_snapshot_utils.py
+drwxr-xr-x   0 kc244      (501) staff       (20)        0 2022-01-03 16:18:53.740052 nifti_snapshot-0.1.9/nifti_snapshot.egg-info/
+-rw-r--r--   0 kc244      (501) staff       (20)     3320 2022-01-03 16:18:53.000000 nifti_snapshot-0.1.9/nifti_snapshot.egg-info/PKG-INFO
+-rw-r--r--   0 kc244      (501) staff       (20)      358 2022-01-03 16:18:53.000000 nifti_snapshot-0.1.9/nifti_snapshot.egg-info/SOURCES.txt
+-rw-r--r--   0 kc244      (501) staff       (20)        1 2022-01-03 16:18:53.000000 nifti_snapshot-0.1.9/nifti_snapshot.egg-info/dependency_links.txt
+-rw-r--r--   0 kc244      (501) staff       (20)       76 2022-01-03 16:18:53.000000 nifti_snapshot-0.1.9/nifti_snapshot.egg-info/requires.txt
+-rw-r--r--   0 kc244      (501) staff       (20)       15 2022-01-03 16:18:53.000000 nifti_snapshot-0.1.9/nifti_snapshot.egg-info/top_level.txt
+drwxr-xr-x   0 kc244      (501) staff       (20)        0 2022-01-03 16:18:53.740387 nifti_snapshot-0.1.9/scripts/
+-rwxr-xr-x   0 kc244      (501) staff       (20)     4627 2021-09-04 09:08:14.000000 nifti_snapshot-0.1.9/scripts/nifti_snapshot
+-rw-r--r--   0 kc244      (501) staff       (20)       79 2022-01-03 16:18:53.741186 nifti_snapshot-0.1.9/setup.cfg
+-rw-r--r--   0 kc244      (501) staff       (20)     1093 2022-01-03 16:18:48.000000 nifti_snapshot-0.1.9/setup.py
```

### Comparing `nifti_snapshot-0.1.8/PKG-INFO` & `nifti_snapshot-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti_snapshot
-Version: 0.1.8
+Version: 0.1.9
 Summary: First release to test pypi
 Home-page: https://github.com/pnlbwh/nifti-snapshot
 Author: kcho
 Author-email: kevincho@bwh.harvard.edu
 License: UNKNOWN
 Download-URL: https://github.com/pnlbwh/nifti-snapshot/archive/refs/tags/nifti-snapshot.zip
 Keywords: nifti,snapshot
```

### Comparing `nifti_snapshot-0.1.8/README.md` & `nifti_snapshot-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nifti_snapshot-0.1.8/nifti_snapshot/nifti_snapshot.py` & `nifti_snapshot-0.1.9/nifti_snapshot/nifti_snapshot.py`

 * *Files identical despite different names*

### Comparing `nifti_snapshot-0.1.8/nifti_snapshot/nifti_snapshot_utils.py` & `nifti_snapshot-0.1.9/nifti_snapshot/nifti_snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `nifti_snapshot-0.1.8/nifti_snapshot.egg-info/PKG-INFO` & `nifti_snapshot-0.1.9/nifti_snapshot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti-snapshot
-Version: 0.1.8
+Version: 0.1.9
 Summary: First release to test pypi
 Home-page: https://github.com/pnlbwh/nifti-snapshot
 Author: kcho
 Author-email: kevincho@bwh.harvard.edu
 License: UNKNOWN
 Download-URL: https://github.com/pnlbwh/nifti-snapshot/archive/refs/tags/nifti-snapshot.zip
 Keywords: nifti,snapshot
```

### Comparing `nifti_snapshot-0.1.8/scripts/nifti_snapshot` & `nifti_snapshot-0.1.9/scripts/nifti_snapshot`

 * *Files identical despite different names*

### Comparing `nifti_snapshot-0.1.8/setup.py` & `nifti_snapshot-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os.path import join
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='nifti_snapshot',
-    version='v0.1.8',
+    version='v0.1.9',
     description='First release to test pypi',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='kcho',
     author_email='kevincho@bwh.harvard.edu',
     url='https://github.com/pnlbwh/nifti-snapshot',
     download_url='https://github.com/pnlbwh/nifti-snapshot/archive/refs/tags/nifti-snapshot.zip',
@@ -24,10 +24,10 @@
     ],
     python_requires='>=3.7',
     install_requires=['matplotlib>=3.3.2',
                       'numpy>=1.19.2',
                       'scipy>=1.5.2',
                       'seaborn>=0.11.0',
                       'nibabel>=3.2.1'],
-    data_files=[('/usr/local/share/enigma_data', ['enigma_download.sh'])],
+    data_files=[('/enigma_data', ['enigma_download.sh'])],
     scripts=['scripts/nifti_snapshot']
 )
```

