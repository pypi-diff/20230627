# Comparing `tmp/techiaith-tts-0.1.5.tar.gz` & `tmp/techiaith-tts-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techiaith-tts-0.1.5.tar", last modified: Wed May 17 14:04:04 2023, max compression
+gzip compressed data, was "techiaith-tts-0.1.6.tar", last modified: Tue Jun 27 05:41:31 2023, max compression
```

## Comparing `techiaith-tts-0.1.5.tar` & `techiaith-tts-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:04.605554 techiaith-tts-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-17 14:03:50.000000 techiaith-tts-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 14:04:04.605554 techiaith-tts-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-17 14:03:50.000000 techiaith-tts-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-17 14:03:50.000000 techiaith-tts-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:04:04.605554 techiaith-tts-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-17 14:03:50.000000 techiaith-tts-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:04.545554 techiaith-tts-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:04.545554 techiaith-tts-0.1.5/src/techiaith/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:03:50.000000 techiaith-tts-0.1.5/src/techiaith/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:04.545554 techiaith-tts-0.1.5/src/techiaith/tts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:04.545554 techiaith-tts-0.1.5/src/techiaith/tts/testun/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:04.545554 techiaith-tts-0.1.5/src/techiaith/tts/testun/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:03:50.000000 techiaith-tts-0.1.5/src/techiaith/tts/testun/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 56279604 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/src/techiaith/tts/testun/data/lecsicon_cc0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/src/techiaith/tts/testun/date_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/src/techiaith/tts/testun/known_phrases.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/src/techiaith/tts/testun/lexicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/src/techiaith/tts/testun/lookups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/src/techiaith/tts/testun/number_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/src/techiaith/tts/testun/time_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/src/techiaith/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:04.605554 techiaith-tts-0.1.5/src/techiaith_tts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 14:04:03.000000 techiaith-tts-0.1.5/src/techiaith_tts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-17 14:04:03.000000 techiaith-tts-0.1.5/src/techiaith_tts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:04:03.000000 techiaith-tts-0.1.5/src/techiaith_tts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-17 14:04:03.000000 techiaith-tts-0.1.5/src/techiaith_tts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 14:04:03.000000 techiaith-tts-0.1.5/src/techiaith_tts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:04.605554 techiaith-tts-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/tests/test_date_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/tests/test_known_phrase.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/tests/test_lecsicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/tests/test_number_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-17 14:03:51.000000 techiaith-tts-0.1.5/tests/test_time_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:41:31.159174 techiaith-tts-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-27 05:41:31.159174 techiaith-tts-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:41:31.159174 techiaith-tts-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:41:31.103173 techiaith-tts-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:41:31.103173 techiaith-tts-0.1.6/src/techiaith/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/src/techiaith/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:41:31.103173 techiaith-tts-0.1.6/src/techiaith/tts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:41:31.103173 techiaith-tts-0.1.6/src/techiaith/tts/testun/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:41:31.103173 techiaith-tts-0.1.6/src/techiaith/tts/testun/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/src/techiaith/tts/testun/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 56279604 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/src/techiaith/tts/testun/data/lecsicon_cc0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/src/techiaith/tts/testun/date_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/src/techiaith/tts/testun/known_phrases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/src/techiaith/tts/testun/lexicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/src/techiaith/tts/testun/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/src/techiaith/tts/testun/number_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/src/techiaith/tts/testun/time_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/src/techiaith/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:41:31.159174 techiaith-tts-0.1.6/src/techiaith_tts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-27 05:41:29.000000 techiaith-tts-0.1.6/src/techiaith_tts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-27 05:41:29.000000 techiaith-tts-0.1.6/src/techiaith_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:41:29.000000 techiaith-tts-0.1.6/src/techiaith_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-27 05:41:29.000000 techiaith-tts-0.1.6/src/techiaith_tts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 05:41:29.000000 techiaith-tts-0.1.6/src/techiaith_tts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:41:31.159174 techiaith-tts-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/tests/test_date_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/tests/test_known_phrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/tests/test_lecsicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/tests/test_number_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-27 05:41:15.000000 techiaith-tts-0.1.6/tests/test_time_norm.py
```

### Comparing `techiaith-tts-0.1.5/LICENSE` & `techiaith-tts-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/PKG-INFO` & `techiaith-tts-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: techiaith-tts
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/techiaith/techiaith-tts
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `techiaith-tts-0.1.5/README.md` & `techiaith-tts-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/setup.py` & `techiaith-tts-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/src/techiaith/tts/testun/data/lecsicon_cc0.txt` & `techiaith-tts-0.1.6/src/techiaith/tts/testun/data/lecsicon_cc0.txt`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/src/techiaith/tts/testun/date_norm.py` & `techiaith-tts-0.1.6/src/techiaith/tts/testun/date_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/src/techiaith/tts/testun/lexicon.py` & `techiaith-tts-0.1.6/src/techiaith/tts/testun/lexicon.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/src/techiaith/tts/testun/lookups.py` & `techiaith-tts-0.1.6/src/techiaith/tts/testun/lookups.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/src/techiaith/tts/testun/number_norm.py` & `techiaith-tts-0.1.6/src/techiaith/tts/testun/number_norm.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,20 +105,21 @@
     :param text:
     :param number:
     :return:
     """
     black_list = ["miliwn"]
     next_word = text.split(number, maxsplit=1)[-1].split(maxsplit=1)
     if next_word and next_word not in black_list:
-        info = lexicon[next_word[0]]
-        if "Fem" in info:
-            for num in number.split(" "):
-                for mut in fem_mu:
-                    if mut[0] == num:
-                        text = text.replace(mut[0], mut[1])
+        if next_word[0] in lexicon:
+            info = lexicon[next_word[0]]
+            if "Fem" in info:
+                for num in number.split(" "):
+                    for mut in fem_mu:
+                        if mut[0] == num:
+                            text = text.replace(mut[0], mut[1])
     return text
 
 
 def wordify(number):
     """
     convert a digit in string form into word form
     :param number:
```

### Comparing `techiaith-tts-0.1.5/src/techiaith/tts/testun/time_norm.py` & `techiaith-tts-0.1.6/src/techiaith/tts/testun/time_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/src/techiaith_tts.egg-info/PKG-INFO` & `techiaith-tts-0.1.6/src/techiaith_tts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: techiaith-tts
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/techiaith/techiaith-tts
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `techiaith-tts-0.1.5/src/techiaith_tts.egg-info/SOURCES.txt` & `techiaith-tts-0.1.6/src/techiaith_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/tests/test_date_norm.py` & `techiaith-tts-0.1.6/tests/test_date_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/tests/test_number_norm.py` & `techiaith-tts-0.1.6/tests/test_number_norm.py`

 * *Files identical despite different names*

### Comparing `techiaith-tts-0.1.5/tests/test_time_norm.py` & `techiaith-tts-0.1.6/tests/test_time_norm.py`

 * *Files identical despite different names*

