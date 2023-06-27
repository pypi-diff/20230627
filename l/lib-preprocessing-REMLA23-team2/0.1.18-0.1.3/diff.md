# Comparing `tmp/lib_preprocessing_REMLA23_team2-0.1.18.tar.gz` & `tmp/lib_preprocessing_REMLA23_team2-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_preprocessing_REMLA23_team2-0.1.18.tar", last modified: Tue Jun 27 12:31:58 2023, max compression
+gzip compressed data, was "lib_preprocessing_REMLA23_team2-0.1.3.tar", last modified: Mon Jun 26 10:52:15 2023, max compression
```

## Comparing `lib_preprocessing_REMLA23_team2-0.1.18.tar` & `lib_preprocessing_REMLA23_team2-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:31:58.648842 lib_preprocessing_REMLA23_team2-0.1.18/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-27 12:31:58.648842 lib_preprocessing_REMLA23_team2-0.1.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-27 12:31:47.000000 lib_preprocessing_REMLA23_team2-0.1.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:31:58.648842 lib_preprocessing_REMLA23_team2-0.1.18/lib_preproc/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 12:31:47.000000 lib_preprocessing_REMLA23_team2-0.1.18/lib_preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-27 12:31:47.000000 lib_preprocessing_REMLA23_team2-0.1.18/lib_preproc/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:31:58.648842 lib_preprocessing_REMLA23_team2-0.1.18/lib_preprocessing_REMLA23_team2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-27 12:31:58.000000 lib_preprocessing_REMLA23_team2-0.1.18/lib_preprocessing_REMLA23_team2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-27 12:31:58.000000 lib_preprocessing_REMLA23_team2-0.1.18/lib_preprocessing_REMLA23_team2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:31:58.000000 lib_preprocessing_REMLA23_team2-0.1.18/lib_preprocessing_REMLA23_team2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 12:31:58.000000 lib_preprocessing_REMLA23_team2-0.1.18/lib_preprocessing_REMLA23_team2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:31:58.648842 lib_preprocessing_REMLA23_team2-0.1.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-27 12:31:47.000000 lib_preprocessing_REMLA23_team2-0.1.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:52:15.104907 lib_preprocessing_REMLA23_team2-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-26 10:52:15.100906 lib_preprocessing_REMLA23_team2-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 10:52:02.000000 lib_preprocessing_REMLA23_team2-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:52:15.100906 lib_preprocessing_REMLA23_team2-0.1.3/lib_preproc/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 10:52:02.000000 lib_preprocessing_REMLA23_team2-0.1.3/lib_preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 10:52:02.000000 lib_preprocessing_REMLA23_team2-0.1.3/lib_preproc/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:52:15.100906 lib_preprocessing_REMLA23_team2-0.1.3/lib_preprocessing_REMLA23_team2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-26 10:52:15.000000 lib_preprocessing_REMLA23_team2-0.1.3/lib_preprocessing_REMLA23_team2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-26 10:52:15.000000 lib_preprocessing_REMLA23_team2-0.1.3/lib_preprocessing_REMLA23_team2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:52:15.000000 lib_preprocessing_REMLA23_team2-0.1.3/lib_preprocessing_REMLA23_team2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 10:52:15.000000 lib_preprocessing_REMLA23_team2-0.1.3/lib_preprocessing_REMLA23_team2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:52:15.104907 lib_preprocessing_REMLA23_team2-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-26 10:52:02.000000 lib_preprocessing_REMLA23_team2-0.1.3/setup.py
```

### Comparing `lib_preprocessing_REMLA23_team2-0.1.18/lib_preproc/preprocessing.py` & `lib_preprocessing_REMLA23_team2-0.1.3/lib_preproc/preprocessing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,18 @@
 import re
 import nltk
-import pkg_resources
 from nltk.corpus import stopwords
-from nltk.stem.porter import PorterStemmer
 
 nltk.download('stopwords')
 all_stopwords = stopwords.words('english')
 all_stopwords.remove('not')
 
-ps = PorterStemmer()
-
-# def get_version():
-#     with open("VERSION", "r") as version_file:
-#         return version_file.read().strip()
-    
-def get_version(package_name):
-    try:
-        return pkg_resources.get_distribution(package_name).version
-    except pkg_resources.DistributionNotFound:
-        return None
+def get_version():
+    with open("VERSION", "r") as version_file:
+        return version_file.read().strip()
 
 def process_review(review: str):
     review = re.sub('[^a-zA-Z]', ' ', review)
     review = review.lower()
     review = review.split()
     review = [ps.stem(word) for word in review if not word in set(all_stopwords)]
     review = ' '.join(review)
```

### Comparing `lib_preprocessing_REMLA23_team2-0.1.18/setup.py` & `lib_preprocessing_REMLA23_team2-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,12 +11,8 @@
     packages=find_packages(),
     version=version,
     description='Library for preprocessing the data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='remla23_team2',
     license='MIT',
-    # install_requires=[
-    #     'nltk',
-    #     're',
-    # ],
 )
```

