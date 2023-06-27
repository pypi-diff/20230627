# Comparing `tmp/matan-0.1.5.2.7.3.dev3.tar.gz` & `tmp/MatAn-0.1.5.2.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matan-0.1.5.2.7.3.dev3.tar", last modified: Tue Jun 27 14:46:41 2023, max compression
+gzip compressed data, was "MatAn-0.1.5.2.7.dev1.tar", last modified: Tue Jun 27 13:59:08 2023, max compression
```

## Comparing `matan-0.1.5.2.7.3.dev3.tar` & `MatAn-0.1.5.2.7.dev1.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 14:46:41.791850 matan-0.1.5.2.7.3.dev3/
--rw-r--r--   0 uuu       (1000) uuu       (1000)    34670 2023-06-18 20:22:37.000000 matan-0.1.5.2.7.3.dev3/LICENSE
--rw-r--r--   0 uuu       (1000) uuu       (1000)     4257 2023-06-27 14:46:41.791850 matan-0.1.5.2.7.3.dev3/PKG-INFO
--rw-r--r--   0 uuu       (1000) uuu       (1000)     3337 2023-06-24 20:58:42.000000 matan-0.1.5.2.7.3.dev3/README.md
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 14:46:41.791850 matan-0.1.5.2.7.3.dev3/matan/
--rw-r--r--   0 uuu       (1000) uuu       (1000)       84 2023-06-19 18:03:25.000000 matan-0.1.5.2.7.3.dev3/matan/__init__.py
--rw-r--r--   0 uuu       (1000) uuu       (1000)      156 2023-06-19 18:03:25.000000 matan-0.1.5.2.7.3.dev3/matan/_misc.py
--rw-r--r--   0 uuu       (1000) uuu       (1000)     4960 2023-06-19 18:03:25.000000 matan-0.1.5.2.7.3.dev3/matan/files.py
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 14:46:41.791850 matan-0.1.5.2.7.3.dev3/matan/polymers/
--rw-r--r--   0 uuu       (1000) uuu       (1000)        0 2023-06-19 19:18:34.000000 matan-0.1.5.2.7.3.dev3/matan/polymers/__init__.py
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 14:46:41.791850 matan-0.1.5.2.7.3.dev3/matan/polymers/charpy/
--rw-r--r--   0 uuu       (1000) uuu       (1000)      815 2023-06-19 19:11:47.000000 matan-0.1.5.2.7.3.dev3/matan/polymers/charpy/__init__.py
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 14:46:41.791850 matan-0.1.5.2.7.3.dev3/matan/polymers/tensile/
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 14:46:41.791850 matan-0.1.5.2.7.3.dev3/matan/polymers/tensile/ISO527/
--rw-r--r--   0 uuu       (1000) uuu       (1000)     2710 2023-06-24 22:10:32.000000 matan-0.1.5.2.7.3.dev3/matan/polymers/tensile/ISO527/__init__.py
--rw-r--r--   0 uuu       (1000) uuu       (1000)    13537 2023-06-24 22:18:44.000000 matan-0.1.5.2.7.3.dev3/matan/polymers/tensile/__init__.py
--rw-r--r--   0 uuu       (1000) uuu       (1000)     8206 2023-06-24 22:14:15.000000 matan-0.1.5.2.7.3.dev3/matan/sample.py
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 14:46:41.791850 matan-0.1.5.2.7.3.dev3/matan.egg-info/
--rw-r--r--   0 uuu       (1000) uuu       (1000)     4257 2023-06-27 14:46:41.000000 matan-0.1.5.2.7.3.dev3/matan.egg-info/PKG-INFO
--rw-r--r--   0 uuu       (1000) uuu       (1000)      382 2023-06-27 14:46:41.000000 matan-0.1.5.2.7.3.dev3/matan.egg-info/SOURCES.txt
--rw-r--r--   0 uuu       (1000) uuu       (1000)        1 2023-06-27 14:46:41.000000 matan-0.1.5.2.7.3.dev3/matan.egg-info/dependency_links.txt
--rw-r--r--   0 uuu       (1000) uuu       (1000)       17 2023-06-27 14:46:41.000000 matan-0.1.5.2.7.3.dev3/matan.egg-info/requires.txt
--rw-r--r--   0 uuu       (1000) uuu       (1000)        6 2023-06-27 14:46:41.000000 matan-0.1.5.2.7.3.dev3/matan.egg-info/top_level.txt
--rw-r--r--   0 uuu       (1000) uuu       (1000)      103 2023-06-27 14:46:41.791850 matan-0.1.5.2.7.3.dev3/setup.cfg
--rw-r--r--   0 uuu       (1000) uuu       (1000)     1697 2023-06-27 14:46:40.000000 matan-0.1.5.2.7.3.dev3/setup.py
+drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 13:59:08.299691 MatAn-0.1.5.2.7.dev1/
+-rw-r--r--   0 uuu       (1000) uuu       (1000)    34670 2023-06-18 20:22:37.000000 MatAn-0.1.5.2.7.dev1/LICENSE
+-rw-r--r--   0 uuu       (1000) uuu       (1000)     4218 2023-06-27 13:59:08.299691 MatAn-0.1.5.2.7.dev1/PKG-INFO
+-rw-r--r--   0 uuu       (1000) uuu       (1000)     3337 2023-06-24 20:58:42.000000 MatAn-0.1.5.2.7.dev1/README.md
+drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 13:59:08.299691 MatAn-0.1.5.2.7.dev1/matan/
+drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 13:59:08.299691 MatAn-0.1.5.2.7.dev1/matan/MatAn.egg-info/
+-rw-r--r--   0 uuu       (1000) uuu       (1000)     4218 2023-06-27 13:59:08.000000 MatAn-0.1.5.2.7.dev1/matan/MatAn.egg-info/PKG-INFO
+-rw-r--r--   0 uuu       (1000) uuu       (1000)      348 2023-06-27 13:59:08.000000 MatAn-0.1.5.2.7.dev1/matan/MatAn.egg-info/SOURCES.txt
+-rw-r--r--   0 uuu       (1000) uuu       (1000)        1 2023-06-27 13:59:08.000000 MatAn-0.1.5.2.7.dev1/matan/MatAn.egg-info/dependency_links.txt
+-rw-r--r--   0 uuu       (1000) uuu       (1000)       17 2023-06-27 13:59:08.000000 MatAn-0.1.5.2.7.dev1/matan/MatAn.egg-info/requires.txt
+-rw-r--r--   0 uuu       (1000) uuu       (1000)        9 2023-06-27 13:59:08.000000 MatAn-0.1.5.2.7.dev1/matan/MatAn.egg-info/top_level.txt
+drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 13:59:08.299691 MatAn-0.1.5.2.7.dev1/matan/polymers/
+-rw-r--r--   0 uuu       (1000) uuu       (1000)        0 2023-06-19 19:18:34.000000 MatAn-0.1.5.2.7.dev1/matan/polymers/__init__.py
+drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 13:59:08.299691 MatAn-0.1.5.2.7.dev1/matan/polymers/charpy/
+-rw-r--r--   0 uuu       (1000) uuu       (1000)      815 2023-06-19 19:11:47.000000 MatAn-0.1.5.2.7.dev1/matan/polymers/charpy/__init__.py
+drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 13:59:08.299691 MatAn-0.1.5.2.7.dev1/matan/polymers/tensile/
+drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-27 13:59:08.299691 MatAn-0.1.5.2.7.dev1/matan/polymers/tensile/ISO527/
+-rw-r--r--   0 uuu       (1000) uuu       (1000)     2710 2023-06-24 22:10:32.000000 MatAn-0.1.5.2.7.dev1/matan/polymers/tensile/ISO527/__init__.py
+-rw-r--r--   0 uuu       (1000) uuu       (1000)    13537 2023-06-24 22:18:44.000000 MatAn-0.1.5.2.7.dev1/matan/polymers/tensile/__init__.py
+-rw-r--r--   0 uuu       (1000) uuu       (1000)      103 2023-06-27 13:59:08.303691 MatAn-0.1.5.2.7.dev1/setup.cfg
+-rw-r--r--   0 uuu       (1000) uuu       (1000)     1612 2023-06-27 13:54:24.000000 MatAn-0.1.5.2.7.dev1/setup.py
```

### Comparing `matan-0.1.5.2.7.3.dev3/LICENSE` & `MatAn-0.1.5.2.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `matan-0.1.5.2.7.3.dev3/PKG-INFO` & `MatAn-0.1.5.2.7.dev1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: matan
-Version: 0.1.5.2.7.3.dev3
+Name: MatAn
+Version: 0.1.5.2.7.dev1
 Summary: Material analysis package to plot or extract properties like tensile modulus etc. 
 Home-page: https://codeberg.org/309631/matan
 Author: Igor Cudnik
 Author-email: igor.cudnik@student.put.poznan.pl
 License: GPLv3
-Keywords: material analysis,ISO 527,ISO 527-1,polymers analysis,material analysis,tensile testcharpy
+Keywords: material analysis,ISO 527,ISO 527-1,polymers analysis
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `matan-0.1.5.2.7.3.dev3/README.md` & `MatAn-0.1.5.2.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `matan-0.1.5.2.7.3.dev3/matan/polymers/charpy/__init__.py` & `MatAn-0.1.5.2.7.dev1/matan/polymers/charpy/__init__.py`

 * *Files identical despite different names*

### Comparing `matan-0.1.5.2.7.3.dev3/matan/polymers/tensile/ISO527/__init__.py` & `MatAn-0.1.5.2.7.dev1/matan/polymers/tensile/ISO527/__init__.py`

 * *Files identical despite different names*

### Comparing `matan-0.1.5.2.7.3.dev3/matan/polymers/tensile/__init__.py` & `MatAn-0.1.5.2.7.dev1/matan/polymers/tensile/__init__.py`

 * *Files identical despite different names*

### Comparing `matan-0.1.5.2.7.3.dev3/matan.egg-info/PKG-INFO` & `MatAn-0.1.5.2.7.dev1/matan/MatAn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: matan
-Version: 0.1.5.2.7.3.dev3
+Name: MatAn
+Version: 0.1.5.2.7.dev1
 Summary: Material analysis package to plot or extract properties like tensile modulus etc. 
 Home-page: https://codeberg.org/309631/matan
 Author: Igor Cudnik
 Author-email: igor.cudnik@student.put.poznan.pl
 License: GPLv3
-Keywords: material analysis,ISO 527,ISO 527-1,polymers analysis,material analysis,tensile testcharpy
+Keywords: material analysis,ISO 527,ISO 527-1,polymers analysis
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `matan-0.1.5.2.7.3.dev3/setup.py` & `MatAn-0.1.5.2.7.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,29 @@
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
-    name='matan',
-    version='0.1.5.2.7.3dev3',
+    name='MatAn',
+    version='0.1.5.2.7.dev1',
     license='GPLv3',
     author="Igor Cudnik",
     author_email='igor.cudnik@student.put.poznan.pl',
     description='Material analysis package to plot or extract properties like tensile modulus etc. ',
     long_description=readme(),
     long_description_content_type='text/markdown',
-    packages=find_packages(),
-    # package_dir={'': 'matan/'},
+    packages=find_packages('matan'),
+    package_dir={'': 'matan'},
     url='https://codeberg.org/309631/matan',
     keywords=['material analysis',
               'ISO 527',
               'ISO 527-1',
-              'polymers analysis',
-              'material analysis',
-              'tensile test'
-              'charpy'],
+              'polymers analysis'],
     install_requires=[
           'numpy',
         'matplotlib'
       ],
     classifiers=[
     # How mature is this project? Common values are
     #   3 - Alpha
```

