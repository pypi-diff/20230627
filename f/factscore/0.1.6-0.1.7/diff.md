# Comparing `tmp/factscore-0.1.6.tar.gz` & `tmp/factscore-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factscore-0.1.6.tar", max compression
+gzip compressed data, was "factscore-0.1.7.tar", max compression
```

## Comparing `factscore-0.1.6.tar` & `factscore-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2023-06-24 22:10:15.165870 factscore-0.1.6/LICENSE
--rw-r--r--   0        0        0    10718 2023-06-27 14:25:12.317000 factscore-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-05-23 14:51:37.783672 factscore-0.1.6/factscore/__init__.py
--rw-r--r--   0        0        0     1768 2023-06-25 15:22:25.136628 factscore-0.1.6/factscore/abstain_detection.py
--rw-r--r--   0        0        0    13768 2023-06-25 15:11:45.270579 factscore-0.1.6/factscore/atomic_facts.py
--rw-r--r--   0        0        0     2868 2023-05-26 23:16:58.269806 factscore-0.1.6/factscore/clm.py
--rw-r--r--   0        0        0     6178 2023-05-26 23:16:58.269806 factscore-0.1.6/factscore/download_data.py
--rw-r--r--   0        0        0    15733 2023-06-27 14:25:12.321000 factscore-0.1.6/factscore/factscorer.py
--rw-r--r--   0        0        0     2022 2023-06-27 14:25:12.321000 factscore-0.1.6/factscore/lm.py
--rw-r--r--   0        0        0     7105 2023-05-23 19:37:35.506439 factscore-0.1.6/factscore/npm.py
--rw-r--r--   0        0        0     4090 2023-05-26 23:16:58.269806 factscore-0.1.6/factscore/openai_lm.py
--rw-r--r--   0        0        0     8201 2023-06-27 14:25:12.321000 factscore-0.1.6/factscore/retrieval.py
--rw-r--r--   0        0        0     4774 2023-05-23 14:51:37.783672 factscore-0.1.6/factscore/utils.py
--rw-r--r--   0        0        0      813 2023-06-27 14:28:08.057130 factscore-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    11839 1970-01-01 00:00:00.000000 factscore-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-24 22:10:15.165870 factscore-0.1.7/LICENSE
+-rw-r--r--   0        0        0    10718 2023-06-27 14:29:23.763463 factscore-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 14:51:37.783672 factscore-0.1.7/factscore/__init__.py
+-rw-r--r--   0        0        0     1768 2023-06-27 14:29:23.763463 factscore-0.1.7/factscore/abstain_detection.py
+-rw-r--r--   0        0        0    13768 2023-06-27 14:29:23.763463 factscore-0.1.7/factscore/atomic_facts.py
+-rw-r--r--   0        0        0     2868 2023-05-26 23:16:58.269806 factscore-0.1.7/factscore/clm.py
+-rw-r--r--   0        0        0     6178 2023-05-26 23:16:58.269806 factscore-0.1.7/factscore/download_data.py
+-rw-r--r--   0        0        0    15733 2023-06-27 14:29:23.763463 factscore-0.1.7/factscore/factscorer.py
+-rw-r--r--   0        0        0     2022 2023-06-27 14:29:23.763463 factscore-0.1.7/factscore/lm.py
+-rw-r--r--   0        0        0     7105 2023-05-23 19:37:35.506439 factscore-0.1.7/factscore/npm.py
+-rw-r--r--   0        0        0     4090 2023-05-26 23:16:58.269806 factscore-0.1.7/factscore/openai_lm.py
+-rw-r--r--   0        0        0     8201 2023-06-27 14:29:23.767463 factscore-0.1.7/factscore/retrieval.py
+-rw-r--r--   0        0        0     4774 2023-05-23 14:51:37.783672 factscore-0.1.7/factscore/utils.py
+-rw-r--r--   0        0        0      813 2023-06-27 14:30:37.853832 factscore-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    11839 1970-01-01 00:00:00.000000 factscore-0.1.7/PKG-INFO
```

### Comparing `factscore-0.1.6/LICENSE` & `factscore-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/README.md` & `factscore-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/factscore/abstain_detection.py` & `factscore-0.1.7/factscore/abstain_detection.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/factscore/atomic_facts.py` & `factscore-0.1.7/factscore/atomic_facts.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/factscore/clm.py` & `factscore-0.1.7/factscore/clm.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/factscore/download_data.py` & `factscore-0.1.7/factscore/download_data.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/factscore/factscorer.py` & `factscore-0.1.7/factscore/factscorer.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/factscore/lm.py` & `factscore-0.1.7/factscore/lm.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/factscore/npm.py` & `factscore-0.1.7/factscore/npm.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/factscore/openai_lm.py` & `factscore-0.1.7/factscore/openai_lm.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/factscore/retrieval.py` & `factscore-0.1.7/factscore/retrieval.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/factscore/utils.py` & `factscore-0.1.7/factscore/utils.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.6/pyproject.toml` & `factscore-0.1.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "factscore"
-version = "0.1.6"
+version = "0.1.7"
 description = "FactScore is an automatic evaluation metric for factual precision in long-form text generation. It uses large language models and retrieval to break down generations into atomic facts and then measure the correctness with respect to a knowledge source (like Wikipedia)."
 authors = ["Sewon Min <sewon@cs.washington.edu>", "Kalpesh Krishna <kalpesh@cs.umass.edu>", "Xinxi Lyu <alrope@cs.washington.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
```

### Comparing `factscore-0.1.6/PKG-INFO` & `factscore-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factscore
-Version: 0.1.6
+Version: 0.1.7
 Summary: FactScore is an automatic evaluation metric for factual precision in long-form text generation. It uses large language models and retrieval to break down generations into atomic facts and then measure the correctness with respect to a knowledge source (like Wikipedia).
 License: MIT
 Author: Sewon Min
 Author-email: sewon@cs.washington.edu
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

