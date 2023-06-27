# Comparing `tmp/Kanon4txt-0.1.4.tar.gz` & `tmp/Kanon4txt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kanon4txt-0.1.4.tar", last modified: Tue Jun 27 10:39:11 2023, max compression
+gzip compressed data, was "Kanon4txt-0.1.5.tar", last modified: Tue Jun 27 10:55:07 2023, max compression
```

## Comparing `Kanon4txt-0.1.4.tar` & `Kanon4txt-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 10:39:10.978064 Kanon4txt-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-06-27 10:39:10.908077 Kanon4txt-0.1.4/Kanon4txt/
--rw-rw-rw-   0        0        0       45 2023-06-27 10:06:52.000000 Kanon4txt-0.1.4/Kanon4txt/__init__.py
--rw-rw-rw-   0        0        0     9280 2023-06-27 09:55:54.000000 Kanon4txt-0.1.4/Kanon4txt/k_anonym_text.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:39:10.976068 Kanon4txt-0.1.4/Kanon4txt/utils/
--rw-rw-rw-   0        0        0      373 2023-06-27 10:37:22.000000 Kanon4txt-0.1.4/Kanon4txt/utils/__init__.py
--rw-rw-rw-   0        0        0    19915 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/anonym_utils.py
--rw-rw-rw-   0        0        0    13766 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/cluster_utils.py
--rw-rw-rw-   0        0        0     7107 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/llm_utils.py
--rw-rw-rw-   0        0        0      485 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/models.py
--rw-rw-rw-   0        0        0    13040 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/nlp_utils.py
--rw-rw-rw-   0        0        0     6458 2023-06-19 08:12:01.000000 Kanon4txt-0.1.4/Kanon4txt/utils/utilization_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:39:10.949066 Kanon4txt-0.1.4/Kanon4txt.egg-info/
--rw-rw-rw-   0        0        0      724 2023-06-27 10:39:10.000000 Kanon4txt-0.1.4/Kanon4txt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-06-27 10:39:10.000000 Kanon4txt-0.1.4/Kanon4txt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 10:39:10.000000 Kanon4txt-0.1.4/Kanon4txt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-06-27 10:39:10.000000 Kanon4txt-0.1.4/Kanon4txt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 10:39:10.000000 Kanon4txt-0.1.4/Kanon4txt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-06 20:01:19.000000 Kanon4txt-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      724 2023-06-27 10:39:10.979063 Kanon4txt-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4499 2023-06-21 09:41:31.000000 Kanon4txt-0.1.4/README.md
--rw-rw-rw-   0        0        0       86 2023-06-27 10:39:10.982067 Kanon4txt-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1407 2023-06-27 10:39:00.000000 Kanon4txt-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:55:06.992105 Kanon4txt-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-06-27 10:55:06.925103 Kanon4txt-0.1.5/Kanon4txt/
+-rw-rw-rw-   0        0        0       45 2023-06-27 10:06:52.000000 Kanon4txt-0.1.5/Kanon4txt/__init__.py
+-rw-rw-rw-   0        0        0     9290 2023-06-27 10:41:13.000000 Kanon4txt-0.1.5/Kanon4txt/k_anonym_text.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:55:06.990102 Kanon4txt-0.1.5/Kanon4txt/utils/
+-rw-rw-rw-   0        0        0      373 2023-06-27 10:37:22.000000 Kanon4txt-0.1.5/Kanon4txt/utils/__init__.py
+-rw-rw-rw-   0        0        0    19915 2023-06-19 08:12:01.000000 Kanon4txt-0.1.5/Kanon4txt/utils/anonym_utils.py
+-rw-rw-rw-   0        0        0    13766 2023-06-19 08:12:01.000000 Kanon4txt-0.1.5/Kanon4txt/utils/cluster_utils.py
+-rw-rw-rw-   0        0        0     7107 2023-06-19 08:12:01.000000 Kanon4txt-0.1.5/Kanon4txt/utils/llm_utils.py
+-rw-rw-rw-   0        0        0      485 2023-06-19 08:12:01.000000 Kanon4txt-0.1.5/Kanon4txt/utils/models.py
+-rw-rw-rw-   0        0        0    13040 2023-06-19 08:12:01.000000 Kanon4txt-0.1.5/Kanon4txt/utils/nlp_utils.py
+-rw-rw-rw-   0        0        0     6458 2023-06-19 08:12:01.000000 Kanon4txt-0.1.5/Kanon4txt/utils/utilization_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:55:06.958103 Kanon4txt-0.1.5/Kanon4txt.egg-info/
+-rw-rw-rw-   0        0        0      724 2023-06-27 10:55:06.000000 Kanon4txt-0.1.5/Kanon4txt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-06-27 10:55:06.000000 Kanon4txt-0.1.5/Kanon4txt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 10:55:06.000000 Kanon4txt-0.1.5/Kanon4txt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-06-27 10:55:06.000000 Kanon4txt-0.1.5/Kanon4txt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 10:55:06.000000 Kanon4txt-0.1.5/Kanon4txt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-06 20:01:19.000000 Kanon4txt-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      724 2023-06-27 10:55:06.993104 Kanon4txt-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4499 2023-06-21 09:41:31.000000 Kanon4txt-0.1.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-27 10:55:07.004109 Kanon4txt-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2023-06-27 10:54:58.000000 Kanon4txt-0.1.5/setup.py
```

### Comparing `Kanon4txt-0.1.4/Kanon4txt/k_anonym_text.py` & `Kanon4txt-0.1.5/Kanon4txt/k_anonym_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
 
 # def run_anonym(arguments):
 def run_anonym(df: pd.DataFrame, k: int, col: str='txt', plot: bool=False, n_jobs: int = 1, verbose: int=0):
     """
     The main function. Runs the anonymization.
     """
-    from utils import nlp_utils, cluster_utils, utilization_utils, anonym_utils
+    from Kanon4txt.utils import nlp_utils, cluster_utils, utilization_utils, anonym_utils
 
     # # getting the input arguments
     # input_file = arguments.file  # Input database
     # k = int(arguments.k)  # Desired k degree
     # stop_file = arguments.stop  # File with list of stop words
     # col = arguments.col  # The text columns  
     # n_jobs = args.n_jobs
```

### Comparing `Kanon4txt-0.1.4/Kanon4txt/utils/anonym_utils.py` & `Kanon4txt-0.1.5/Kanon4txt/utils/anonym_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.4/Kanon4txt/utils/cluster_utils.py` & `Kanon4txt-0.1.5/Kanon4txt/utils/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.4/Kanon4txt/utils/llm_utils.py` & `Kanon4txt-0.1.5/Kanon4txt/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.4/Kanon4txt/utils/nlp_utils.py` & `Kanon4txt-0.1.5/Kanon4txt/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.4/Kanon4txt/utils/utilization_utils.py` & `Kanon4txt-0.1.5/Kanon4txt/utils/utilization_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.4/Kanon4txt.egg-info/PKG-INFO` & `Kanon4txt-0.1.5/Kanon4txt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Kanon4txt
-Version: 0.1.4
+Version: 0.1.5
 Summary: K Anonymity for Text first Try
 Home-page: https://github.com/LiorTrieman/Kanon4txt/tree/maine
-Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.4.tar.gz
+Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.5.tar.gz
 Author: Lior Trieman
 Author-email: <liortr30@gmail.com>
 License: MIT
 Keywords: python,corpus,stopwords,DBSCAN,generalization,reduction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Kanon4txt-0.1.4/LICENSE` & `Kanon4txt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.4/PKG-INFO` & `Kanon4txt-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Kanon4txt
-Version: 0.1.4
+Version: 0.1.5
 Summary: K Anonymity for Text first Try
 Home-page: https://github.com/LiorTrieman/Kanon4txt/tree/maine
-Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.4.tar.gz
+Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.5.tar.gz
 Author: Lior Trieman
 Author-email: <liortr30@gmail.com>
 License: MIT
 Keywords: python,corpus,stopwords,DBSCAN,generalization,reduction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Kanon4txt-0.1.4/README.md` & `Kanon4txt-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.1.4/setup.py` & `Kanon4txt-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 from setuptools import setup, find_packages
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'K Anonymity for Text first Try'
 LONG_DESCRIPTION = 'A package that takes a dataframe with a corpus and return an anonymized corpus'
 
 # Setting up
 setup(
     name="Kanon4txt",
     version=VERSION,
     author="Lior Trieman",
     author_email="<liortr30@gmail.com>",
     url='https://github.com/LiorTrieman/Kanon4txt/tree/maine',
-    download_url='https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.4.tar.gz',  # I explain this later on
+    download_url='https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.1.5.tar.gz',  # I explain this later on
 
     license='MIT',
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     # NEED TO ADD HERE ALL REQUIREMENTS!!!!!
```

