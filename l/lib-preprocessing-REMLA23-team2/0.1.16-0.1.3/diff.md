# Comparing `tmp/lib_preprocessing_REMLA23_team2-0.1.16.tar.gz` & `tmp/lib_preprocessing_REMLA23_team2-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_preprocessing_REMLA23_team2-0.1.16.tar", last modified: Tue Jun 27 00:56:45 2023, max compression
+gzip compressed data, was "lib_preprocessing_REMLA23_team2-0.1.3.tar", last modified: Mon Jun 26 10:52:15 2023, max compression
```

## Comparing `lib_preprocessing_REMLA23_team2-0.1.16.tar` & `lib_preprocessing_REMLA23_team2-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:56:45.574098 lib_preprocessing_REMLA23_team2-0.1.16/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-27 00:56:45.570098 lib_preprocessing_REMLA23_team2-0.1.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-27 00:56:31.000000 lib_preprocessing_REMLA23_team2-0.1.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:56:45.570098 lib_preprocessing_REMLA23_team2-0.1.16/lib_preproc/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 00:56:31.000000 lib_preprocessing_REMLA23_team2-0.1.16/lib_preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 00:56:31.000000 lib_preprocessing_REMLA23_team2-0.1.16/lib_preproc/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:56:45.570098 lib_preprocessing_REMLA23_team2-0.1.16/lib_preprocessing_REMLA23_team2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-27 00:56:45.000000 lib_preprocessing_REMLA23_team2-0.1.16/lib_preprocessing_REMLA23_team2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-27 00:56:45.000000 lib_preprocessing_REMLA23_team2-0.1.16/lib_preprocessing_REMLA23_team2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 00:56:45.000000 lib_preprocessing_REMLA23_team2-0.1.16/lib_preprocessing_REMLA23_team2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 00:56:45.000000 lib_preprocessing_REMLA23_team2-0.1.16/lib_preprocessing_REMLA23_team2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 00:56:45.000000 lib_preprocessing_REMLA23_team2-0.1.16/lib_preprocessing_REMLA23_team2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 00:56:45.574098 lib_preprocessing_REMLA23_team2-0.1.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-27 00:56:31.000000 lib_preprocessing_REMLA23_team2-0.1.16/setup.py
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

### Comparing `lib_preprocessing_REMLA23_team2-0.1.16/lib_preproc/preprocessing.py` & `lib_preprocessing_REMLA23_team2-0.1.3/lib_preproc/preprocessing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import re
 import nltk
 from nltk.corpus import stopwords
-from nltk.stem.porter import PorterStemmer
 
 nltk.download('stopwords')
 all_stopwords = stopwords.words('english')
 all_stopwords.remove('not')
 
-ps = PorterStemmer()
-
 def get_version():
     with open("VERSION", "r") as version_file:
         return version_file.read().strip()
 
 def process_review(review: str):
     review = re.sub('[^a-zA-Z]', ' ', review)
     review = review.lower()
```

### Comparing `lib_preprocessing_REMLA23_team2-0.1.16/setup.py` & `lib_preprocessing_REMLA23_team2-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,12 +11,8 @@
     packages=find_packages(),
     version=version,
     description='Library for preprocessing the data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='remla23_team2',
     license='MIT',
-    install_requires=[
-        'nltk',
-        're',
-    ],
 )
```

