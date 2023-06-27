# Comparing `tmp/Kanon4txt-0.1.2.tar.gz` & `tmp/Kanon4txt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kanon4txt-0.1.2.tar", last modified: Tue Jun 27 10:00:27 2023, max compression
+gzip compressed data, was "Kanon4txt-0.1.3.tar", last modified: Tue Jun 27 10:25:37 2023, max compression
```

## Comparing `Kanon4txt-0.1.2.tar` & `Kanon4txt-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 10:00:27.337807 Kanon4txt-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-27 10:00:27.295810 Kanon4txt-0.1.2/Kanon4txt/
--rw-rw-rw-   0        0        0       56 2023-06-27 08:41:29.000000 Kanon4txt-0.1.2/Kanon4txt/__init__.py
--rw-rw-rw-   0        0        0     9280 2023-06-27 09:55:54.000000 Kanon4txt-0.1.2/Kanon4txt/k_anonym_text.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:00:27.335808 Kanon4txt-0.1.2/Kanon4txt/utils/
--rw-rw-rw-   0        0        0      421 2023-06-26 10:40:14.000000 Kanon4txt-0.1.2/Kanon4txt/utils/__init__.py
--rw-rw-rw-   0        0        0    19915 2023-06-19 08:12:01.000000 Kanon4txt-0.1.2/Kanon4txt/utils/anonym_utils.py
--rw-rw-rw-   0        0        0    13766 2023-06-19 08:12:01.000000 Kanon4txt-0.1.2/Kanon4txt/utils/cluster_utils.py
--rw-rw-rw-   0        0        0     7107 2023-06-19 08:12:01.000000 Kanon4txt-0.1.2/Kanon4txt/utils/llm_utils.py
--rw-rw-rw-   0        0        0      485 2023-06-19 08:12:01.000000 Kanon4txt-0.1.2/Kanon4txt/utils/models.py
--rw-rw-rw-   0        0        0    13040 2023-06-19 08:12:01.000000 Kanon4txt-0.1.2/Kanon4txt/utils/nlp_utils.py
--rw-rw-rw-   0        0        0     6458 2023-06-19 08:12:01.000000 Kanon4txt-0.1.2/Kanon4txt/utils/utilization_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:00:27.314863 Kanon4txt-0.1.2/Kanon4txt.egg-info/
--rw-rw-rw-   0        0        0      724 2023-06-27 10:00:27.000000 Kanon4txt-0.1.2/Kanon4txt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-06-27 10:00:27.000000 Kanon4txt-0.1.2/Kanon4txt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 10:00:27.000000 Kanon4txt-0.1.2/Kanon4txt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-06-27 10:00:27.000000 Kanon4txt-0.1.2/Kanon4txt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 10:00:27.000000 Kanon4txt-0.1.2/Kanon4txt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-06 20:01:19.000000 Kanon4txt-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      724 2023-06-27 10:00:27.338808 Kanon4txt-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4499 2023-06-21 09:41:31.000000 Kanon4txt-0.1.2/README.md
--rw-rw-rw-   0        0        0       86 2023-06-27 10:00:27.341814 Kanon4txt-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1407 2023-06-27 09:57:29.000000 Kanon4txt-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:25:37.592560 Kanon4txt-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-06-27 10:25:37.521826 Kanon4txt-0.1.3/Kanon4txt/
+-rw-rw-rw-   0        0        0       45 2023-06-27 10:06:52.000000 Kanon4txt-0.1.3/Kanon4txt/__init__.py
+-rw-rw-rw-   0        0        0     9280 2023-06-27 09:55:54.000000 Kanon4txt-0.1.3/Kanon4txt/k_anonym_text.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:25:37.590563 Kanon4txt-0.1.3/Kanon4txt/utils/
+-rw-rw-rw-   0        0        0      277 2023-06-27 10:09:15.000000 Kanon4txt-0.1.3/Kanon4txt/utils/__init__.py
+-rw-rw-rw-   0        0        0    19915 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/anonym_utils.py
+-rw-rw-rw-   0        0        0    13766 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/cluster_utils.py
+-rw-rw-rw-   0        0        0     7107 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/llm_utils.py
+-rw-rw-rw-   0        0        0      485 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/models.py
+-rw-rw-rw-   0        0        0    13040 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/nlp_utils.py
+-rw-rw-rw-   0        0        0     6458 2023-06-19 08:12:01.000000 Kanon4txt-0.1.3/Kanon4txt/utils/utilization_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:25:37.567825 Kanon4txt-0.1.3/Kanon4txt.egg-info/
+-rw-rw-rw-   0        0        0      724 2023-06-27 10:25:37.000000 Kanon4txt-0.1.3/Kanon4txt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-06-27 10:25:37.000000 Kanon4txt-0.1.3/Kanon4txt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 10:25:37.000000 Kanon4txt-0.1.3/Kanon4txt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-06-27 10:25:37.000000 Kanon4txt-0.1.3/Kanon4txt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 10:25:37.000000 Kanon4txt-0.1.3/Kanon4txt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-06 20:01:19.000000 Kanon4txt-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      724 2023-06-27 10:25:37.593567 Kanon4txt-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4499 2023-06-21 09:41:31.000000 Kanon4txt-0.1.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-27 10:25:37.597556 Kanon4txt-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2023-06-27 10:25:16.000000 Kanon4txt-0.1.3/setup.py
```

### Comparing `Kanon4txt-0.1.2/Kanon4txt/k_anonym_text.py` & `Kanon4txt-0.1.3/Kanon4txt/k_anonym_text.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.2/Kanon4txt/utils/anonym_utils.py` & `Kanon4txt-0.1.3/Kanon4txt/utils/anonym_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.2/Kanon4txt/utils/cluster_utils.py` & `Kanon4txt-0.1.3/Kanon4txt/utils/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.2/Kanon4txt/utils/llm_utils.py` & `Kanon4txt-0.1.3/Kanon4txt/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.2/Kanon4txt/utils/nlp_utils.py` & `Kanon4txt-0.1.3/Kanon4txt/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.2/Kanon4txt/utils/utilization_utils.py` & `Kanon4txt-0.1.3/Kanon4txt/utils/utilization_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.2/Kanon4txt.egg-info/PKG-INFO` & `Kanon4txt-0.1.3/Kanon4txt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Kanon4txt
-Version: 0.1.2
+Version: 0.1.3
 Summary: K Anonymity for Text first Try
 Home-page: https://github.com/LiorTrieman/Kanon4txt/tree/maine
-Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.2.tar.gz
+Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.3.tar.gz
 Author: Lior Trieman
 Author-email: <liortr30@gmail.com>
 License: MIT
 Keywords: python,corpus,stopwords,DBSCAN,generalization,reduction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Kanon4txt-0.1.2/LICENSE` & `Kanon4txt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.2/PKG-INFO` & `Kanon4txt-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Kanon4txt
-Version: 0.1.2
+Version: 0.1.3
 Summary: K Anonymity for Text first Try
 Home-page: https://github.com/LiorTrieman/Kanon4txt/tree/maine
-Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.2.tar.gz
+Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.3.tar.gz
 Author: Lior Trieman
 Author-email: <liortr30@gmail.com>
 License: MIT
 Keywords: python,corpus,stopwords,DBSCAN,generalization,reduction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Kanon4txt-0.1.2/README.md` & `Kanon4txt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.2/setup.py` & `Kanon4txt-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'K Anonymity for Text first Try'
 LONG_DESCRIPTION = 'A package that takes a dataframe with a corpus and return an anonymized corpus'
 
 # Setting up
 setup(
     name="Kanon4txt",
     version=VERSION,
     author="Lior Trieman",
     author_email="<liortr30@gmail.com>",
     url='https://github.com/LiorTrieman/Kanon4txt/tree/maine',
-    download_url='https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.2.tar.gz',  # I explain this later on
+    download_url='https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.3.tar.gz',  # I explain this later on
 
     license='MIT',
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     # NEED TO ADD HERE ALL REQUIREMENTS!!!!!
```

