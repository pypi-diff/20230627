# Comparing `tmp/ieseg_credscore-0.23.1.tar.gz` & `tmp/ieseg_credscore-0.23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieseg_credscore-0.23.1.tar", last modified: Mon Jun 26 16:45:09 2023, max compression
+gzip compressed data, was "ieseg_credscore-0.23.2.tar", last modified: Tue Jun 27 12:13:59 2023, max compression
```

## Comparing `ieseg_credscore-0.23.1.tar` & `ieseg_credscore-0.23.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 16:45:09.148604 ieseg_credscore-0.23.1/
--rw-rw-rw-   0        0        0     1092 2023-06-26 15:40:57.000000 ieseg_credscore-0.23.1/LICENSE.rst
--rw-rw-rw-   0        0        0     2942 2023-06-26 16:45:09.148604 ieseg_credscore-0.23.1/PKG-INFO
--rw-rw-rw-   0        0        0     2606 2023-06-26 16:44:47.000000 ieseg_credscore-0.23.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 16:45:09.106749 ieseg_credscore-0.23.1/ieseg_credscore/
--rw-rw-rw-   0        0        0     4597 2022-02-04 14:15:05.000000 ieseg_credscore-0.23.1/ieseg_credscore/OBG.py
--rw-rw-rw-   0        0        0    45785 2022-04-29 08:07:32.000000 ieseg_credscore-0.23.1/ieseg_credscore/WOE.py
--rw-rw-rw-   0        0        0       26 2023-06-26 15:44:16.000000 ieseg_credscore-0.23.1/ieseg_credscore/__init__-PBORCHERT.py
--rw-rw-rw-   0        0        0        4 2022-02-03 18:45:50.000000 ieseg_credscore-0.23.1/ieseg_credscore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:45:09.143621 ieseg_credscore-0.23.1/ieseg_credscore.egg-info/
--rw-rw-rw-   0        0        0     2942 2023-06-26 16:45:08.000000 ieseg_credscore-0.23.1/ieseg_credscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-06-26 16:45:08.000000 ieseg_credscore-0.23.1/ieseg_credscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:45:08.000000 ieseg_credscore-0.23.1/ieseg_credscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-26 16:45:08.000000 ieseg_credscore-0.23.1/ieseg_credscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-26 16:45:08.000000 ieseg_credscore-0.23.1/ieseg_credscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-06-26 16:45:09.154586 ieseg_credscore-0.23.1/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-06-26 16:45:03.000000 ieseg_credscore-0.23.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:13:59.371712 ieseg_credscore-0.23.2/
+-rw-rw-rw-   0        0        0     1092 2023-06-26 15:40:57.000000 ieseg_credscore-0.23.2/LICENSE.rst
+-rw-rw-rw-   0        0        0     2942 2023-06-27 12:13:59.372706 ieseg_credscore-0.23.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2606 2023-06-26 16:44:47.000000 ieseg_credscore-0.23.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 12:13:59.256096 ieseg_credscore-0.23.2/ieseg_credscore/
+-rw-rw-rw-   0        0        0     4597 2022-02-04 14:15:05.000000 ieseg_credscore-0.23.2/ieseg_credscore/OBG.py
+-rw-rw-rw-   0        0        0    45785 2022-04-29 08:07:32.000000 ieseg_credscore-0.23.2/ieseg_credscore/WOE.py
+-rw-rw-rw-   0        0        0       80 2023-06-27 12:08:34.000000 ieseg_credscore-0.23.2/ieseg_credscore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:13:59.352777 ieseg_credscore-0.23.2/ieseg_credscore.egg-info/
+-rw-rw-rw-   0        0        0     2942 2023-06-27 12:13:58.000000 ieseg_credscore-0.23.2/ieseg_credscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-06-27 12:13:58.000000 ieseg_credscore-0.23.2/ieseg_credscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:13:58.000000 ieseg_credscore-0.23.2/ieseg_credscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 12:13:58.000000 ieseg_credscore-0.23.2/ieseg_credscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 12:13:58.000000 ieseg_credscore-0.23.2/ieseg_credscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-06-27 12:13:59.388653 ieseg_credscore-0.23.2/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-06-27 12:09:48.000000 ieseg_credscore-0.23.2/setup.py
```

### Comparing `ieseg_credscore-0.23.1/LICENSE.rst` & `ieseg_credscore-0.23.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.1/PKG-INFO` & `ieseg_credscore-0.23.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieseg_credscore
-Version: 0.23.1
+Version: 0.23.2
 Summary: Credit Scoring - IESEG School of Management
 Home-page: https://github.com/pnborchert
 Author: Philipp Borchert
 Author-email: p.borchert@ieseg.fr
 License: MIT
 Keywords: Credit Scoring IESEG
 Description-Content-Type: text/markdown
```

### Comparing `ieseg_credscore-0.23.1/README.md` & `ieseg_credscore-0.23.2/README.md`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.1/ieseg_credscore/OBG.py` & `ieseg_credscore-0.23.2/ieseg_credscore/OBG.py`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.1/ieseg_credscore/WOE.py` & `ieseg_credscore-0.23.2/ieseg_credscore/WOE.py`

 * *Files identical despite different names*

### Comparing `ieseg_credscore-0.23.1/ieseg_credscore.egg-info/PKG-INFO` & `ieseg_credscore-0.23.2/ieseg_credscore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieseg-credscore
-Version: 0.23.1
+Version: 0.23.2
 Summary: Credit Scoring - IESEG School of Management
 Home-page: https://github.com/pnborchert
 Author: Philipp Borchert
 Author-email: p.borchert@ieseg.fr
 License: MIT
 Keywords: Credit Scoring IESEG
 Description-Content-Type: text/markdown
```

### Comparing `ieseg_credscore-0.23.1/setup.py` & `ieseg_credscore-0.23.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ieseg_credscore',
-    version='0.23.1',
+    version='0.23.2',
     license='MIT',
     author="Philipp Borchert",
     author_email='p.borchert@ieseg.fr',
     packages=find_packages(),
     description = 'Credit Scoring - IESEG School of Management',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

