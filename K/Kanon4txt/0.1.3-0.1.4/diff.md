# Comparing `tmp/Kanon4txt-0.1.3.tar.gz` & `tmp/Kanon4txt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kanon4txt-0.1.3.tar", last modified: Tue Jun 27 10:25:37 2023, max compression
+gzip compressed data, was "Kanon4txt-0.1.4.tar", last modified: Tue Jun 27 10:39:11 2023, max compression
```

## Comparing `Kanon4txt-0.1.3.tar` & `Kanon4txt-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 10:25:37.592560 Kanon4txt-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-06-27 10:25:37.521826 Kanon4txt-0.1.3/Kanon4txt/
--rw-rw-rw-   0        0        0       45 2023-06-27 10:06:52.000000 Kanon4txt-0.1.3/Kanon4txt/__init__.py
--rw-rw-rw-   0        0        0     9280 2023-06-27 09:55:54.000000 Kanon4txt-0.1.3/Kanon4txt/k_anonym_text.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:25:37.590563 Kanon4txt-0.1.3/Kanon4txt/utils/
--rw-rw-rw-   0        0        0      277 2023-06-27 10:09:15.000000 Kanon4txt-0.1.3/Kanon4txt/utils/__init__.py
--rw-rw-rw-   0        0        0    19915 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/anonym_utils.py
--rw-rw-rw-   0        0        0    13766 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/cluster_utils.py
--rw-rw-rw-   0        0        0     7107 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/llm_utils.py
--rw-rw-rw-   0        0        0      485 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/models.py
--rw-rw-rw-   0        0        0    13040 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/nlp_utils.py
--rw-rw-rw-   0        0        0     6458 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/utilization_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:25:37.567825 Kanon4txt-0.1.3/Kanon4txt.egg-info/
--rw-rw-rw-   0        0        0      724 2023-06-27 10:25:37.000000 Kanon4txt-0.1.3/Kanon4txt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-06-27 10:25:37.000000 Kanon4txt-0.1.3/Kanon4txt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 10:25:37.000000 Kanon4txt-0.1.3/Kanon4txt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-06-27 10:25:37.000000 Kanon4txt-0.1.3/Kanon4txt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 10:25:37.000000 Kanon4txt-0.1.3/Kanon4txt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-06 20:01:19.000000 Kanon4txt-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      724 2023-06-27 10:25:37.593567 Kanon4txt-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4499 2023-06-21 09:41:31.000000 Kanon4txt-0.1.3/README.md
--rw-rw-rw-   0        0        0       86 2023-06-27 10:25:37.597556 Kanon4txt-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1407 2023-06-27 10:25:16.000000 Kanon4txt-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:39:10.978064 Kanon4txt-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-06-27 10:39:10.908077 Kanon4txt-0.1.4/Kanon4txt/
+-rw-rw-rw-   0        0        0       45 2023-06-27 10:06:52.000000 Kanon4txt-0.1.4/Kanon4txt/__init__.py
+-rw-rw-rw-   0        0        0     9280 2023-06-27 09:55:54.000000 Kanon4txt-0.1.4/Kanon4txt/k_anonym_text.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:39:10.976068 Kanon4txt-0.1.4/Kanon4txt/utils/
+-rw-rw-rw-   0        0        0      373 2023-06-27 10:37:22.000000 Kanon4txt-0.1.4/Kanon4txt/utils/__init__.py
+-rw-rw-rw-   0        0        0    19915 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/anonym_utils.py
+-rw-rw-rw-   0        0        0    13766 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/cluster_utils.py
+-rw-rw-rw-   0        0        0     7107 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/llm_utils.py
+-rw-rw-rw-   0        0        0      485 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/models.py
+-rw-rw-rw-   0        0        0    13040 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/nlp_utils.py
+-rw-rw-rw-   0        0        0     6458 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/utilization_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:39:10.949066 Kanon4txt-0.1.4/Kanon4txt.egg-info/
+-rw-rw-rw-   0        0        0      724 2023-06-27 10:39:10.000000 Kanon4txt-0.1.4/Kanon4txt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-06-27 10:39:10.000000 Kanon4txt-0.1.4/Kanon4txt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 10:39:10.000000 Kanon4txt-0.1.4/Kanon4txt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-06-27 10:39:10.000000 Kanon4txt-0.1.4/Kanon4txt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 10:39:10.000000 Kanon4txt-0.1.4/Kanon4txt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-06 20:01:19.000000 Kanon4txt-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      724 2023-06-27 10:39:10.979063 Kanon4txt-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4499 2023-06-21 09:41:31.000000 Kanon4txt-0.1.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-27 10:39:10.982067 Kanon4txt-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2023-06-27 10:39:00.000000 Kanon4txt-0.1.4/setup.py
```

### Comparing `Kanon4txt-0.1.3/Kanon4txt/k_anonym_text.py` & `Kanon4txt-0.1.4/Kanon4txt/k_anonym_text.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.3/Kanon4txt/utils/anonym_utils.py` & `Kanon4txt-0.1.4/Kanon4txt/utils/anonym_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.3/Kanon4txt/utils/cluster_utils.py` & `Kanon4txt-0.1.4/Kanon4txt/utils/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.3/Kanon4txt/utils/llm_utils.py` & `Kanon4txt-0.1.4/Kanon4txt/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.3/Kanon4txt/utils/nlp_utils.py` & `Kanon4txt-0.1.4/Kanon4txt/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.3/Kanon4txt/utils/utilization_utils.py` & `Kanon4txt-0.1.4/Kanon4txt/utils/utilization_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.3/Kanon4txt.egg-info/PKG-INFO` & `Kanon4txt-0.1.4/Kanon4txt.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Kanon4txt
-Version: 0.1.3
+Version: 0.1.4
 Summary: K Anonymity for Text first Try
 Home-page: https://github.com/LiorTrieman/Kanon4txt/tree/maine
-Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.3.tar.gz
+Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.4.tar.gz
 Author: Lior Trieman
 Author-email: <liortr30@gmail.com>
 License: MIT
 Keywords: python,corpus,stopwords,DBSCAN,generalization,reduction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Kanon4txt-0.1.3/LICENSE` & `Kanon4txt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.3/PKG-INFO` & `Kanon4txt-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Kanon4txt
-Version: 0.1.3
+Version: 0.1.4
 Summary: K Anonymity for Text first Try
 Home-page: https://github.com/LiorTrieman/Kanon4txt/tree/maine
-Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.3.tar.gz
+Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.4.tar.gz
 Author: Lior Trieman
 Author-email: <liortr30@gmail.com>
 License: MIT
 Keywords: python,corpus,stopwords,DBSCAN,generalization,reduction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Kanon4txt-0.1.3/README.md` & `Kanon4txt-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.3/setup.py` & `Kanon4txt-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 from setuptools import setup, find_packages
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'K Anonymity for Text first Try'
 LONG_DESCRIPTION = 'A package that takes a dataframe with a corpus and return an anonymized corpus'
 
 # Setting up
 setup(
     name="Kanon4txt",
     version=VERSION,
     author="Lior Trieman",
     author_email="<liortr30@gmail.com>",
     url='https://github.com/LiorTrieman/Kanon4txt/tree/maine',
-    download_url='https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.3.tar.gz',  # I explain this later on
+    download_url='https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.4.tar.gz',  # I explain this later on
 
     license='MIT',
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     # NEED TO ADD HERE ALL REQUIREMENTS!!!!!
```

