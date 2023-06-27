# Comparing `tmp/pinyin_jyutping-0.8.tar.gz` & `tmp/pinyin_jyutping-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinyin_jyutping-0.8.tar", last modified: Sun Apr 23 12:43:40 2023, max compression
+gzip compressed data, was "pinyin_jyutping-0.9.tar", last modified: Tue Jun 27 14:26:35 2023, max compression
```

## Comparing `pinyin_jyutping-0.8.tar` & `pinyin_jyutping-0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-23 12:43:40.358409 pinyin_jyutping-0.8/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)       81 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/MANIFEST.in
--rw-r--r--   0 luc       (1000) luc       (1000)     2655 2023-04-23 12:43:40.358409 pinyin_jyutping-0.8/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     2303 2023-04-23 12:42:22.000000 pinyin_jyutping-0.8/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-23 12:43:40.357409 pinyin_jyutping-0.8/pinyin_jyutping/
--rw-r--r--   0 luc       (1000) luc       (1000)     2148 2023-04-13 03:37:57.000000 pinyin_jyutping-0.8/pinyin_jyutping/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2883 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/cache.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8063 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7367 2023-04-23 12:42:22.000000 pinyin_jyutping-0.8/pinyin_jyutping/conversion.py
--rw-r--r--   0 luc       (1000) luc       (1000)      373 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/data.py
--rw-r--r--   0 luc       (1000) luc       (1000)  8583143 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/dict.txt.big
--rw-r--r--   0 luc       (1000) luc       (1000)      107 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    10976 2023-04-13 03:37:57.000000 pinyin_jyutping-0.8/pinyin_jyutping/logic.py
--rw-r--r--   0 luc       (1000) luc       (1000)    11907 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/parser.py
--rw-r--r--   0 luc       (1000) luc       (1000) 18950460 2023-04-23 12:43:38.000000 pinyin_jyutping-0.8/pinyin_jyutping/pinyin_jyutping.pkl
--rw-r--r--   0 luc       (1000) luc       (1000)     2411 2023-03-31 01:12:26.000000 pinyin_jyutping-0.8/pinyin_jyutping/syllables.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-04-23 12:43:40.358409 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)     2655 2023-04-23 12:43:39.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      578 2023-04-23 12:43:40.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-23 12:43:39.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-04-13 03:39:10.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/not-zip-safe
--rw-r--r--   0 luc       (1000) luc       (1000)        6 2023-04-23 12:43:40.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       16 2023-04-23 12:43:40.000000 pinyin_jyutping-0.8/pinyin_jyutping.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-04-23 12:43:40.358409 pinyin_jyutping-0.8/setup.cfg
--rw-r--r--   0 luc       (1000) luc       (1000)      796 2023-04-23 12:43:01.000000 pinyin_jyutping-0.8/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-06-27 14:26:35.763929 pinyin_jyutping-0.9/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)       81 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/MANIFEST.in
+-rw-r--r--   0 luc       (1000) luc       (1000)     2655 2023-06-27 14:26:35.763929 pinyin_jyutping-0.9/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     2303 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-06-27 14:26:35.763929 pinyin_jyutping-0.9/pinyin_jyutping/
+-rw-r--r--   0 luc       (1000) luc       (1000)     2148 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/pinyin_jyutping/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2883 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/pinyin_jyutping/cache.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8063 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/pinyin_jyutping/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7753 2023-06-27 14:26:04.000000 pinyin_jyutping-0.9/pinyin_jyutping/conversion.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      373 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/pinyin_jyutping/data.py
+-rw-r--r--   0 luc       (1000) luc       (1000)  8583143 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/pinyin_jyutping/dict.txt.big
+-rw-r--r--   0 luc       (1000) luc       (1000)      107 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/pinyin_jyutping/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    10976 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/pinyin_jyutping/logic.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    11907 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/pinyin_jyutping/parser.py
+-rw-r--r--   0 luc       (1000) luc       (1000) 18950460 2023-06-27 14:26:35.000000 pinyin_jyutping-0.9/pinyin_jyutping/pinyin_jyutping.pkl
+-rw-r--r--   0 luc       (1000) luc       (1000)     2411 2023-05-24 03:51:44.000000 pinyin_jyutping-0.9/pinyin_jyutping/syllables.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-06-27 14:26:35.763929 pinyin_jyutping-0.9/pinyin_jyutping.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)     2655 2023-06-27 14:26:35.000000 pinyin_jyutping-0.9/pinyin_jyutping.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      578 2023-06-27 14:26:35.000000 pinyin_jyutping-0.9/pinyin_jyutping.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-06-27 14:26:35.000000 pinyin_jyutping-0.9/pinyin_jyutping.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-06-27 14:26:35.000000 pinyin_jyutping-0.9/pinyin_jyutping.egg-info/not-zip-safe
+-rw-r--r--   0 luc       (1000) luc       (1000)       21 2023-06-27 14:26:35.000000 pinyin_jyutping-0.9/pinyin_jyutping.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       16 2023-06-27 14:26:35.000000 pinyin_jyutping-0.9/pinyin_jyutping.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-06-27 14:26:35.763929 pinyin_jyutping-0.9/setup.cfg
+-rw-r--r--   0 luc       (1000) luc       (1000)      824 2023-06-27 14:26:21.000000 pinyin_jyutping-0.9/setup.py
```

### Comparing `pinyin_jyutping-0.8/LICENSE` & `pinyin_jyutping-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/PKG-INFO` & `pinyin_jyutping-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinyin_jyutping
-Version: 0.8
+Version: 0.9
 Summary: Convert a Chinese sentence to Pinyin or Jyutping
 Home-page: https://github.com/Language-Tools/pinyin-jyutping
 Author: LucW
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pinyin_jyutping-0.8/README.rst` & `pinyin_jyutping-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping/__init__.py` & `pinyin_jyutping-0.9/pinyin_jyutping/__init__.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping/cache.py` & `pinyin_jyutping-0.9/pinyin_jyutping/cache.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping/constants.py` & `pinyin_jyutping-0.9/pinyin_jyutping/constants.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping/conversion.py` & `pinyin_jyutping-0.9/pinyin_jyutping/conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import jieba
+import hanzidentifier
 import logging
 import copy
 import pprint
 from . import syllables
 from . import logic
 from . import constants
 
@@ -57,14 +58,17 @@
 
 def solutions_array_for_word(word_map, word):
     entry = word_map.get(word, None)
     if entry != None:
         logger.debug(f'located {word} as word')
         return [mapping.syllables for mapping in entry]
     else:
+        if not hanzidentifier.has_chinese(word):
+            # not chinese text, return unmodified
+            return [[syllables.PassThroughSyllable(word)]]
         logger.debug(f'breaking down {word} into characters')
         return get_romanization_solutions_for_characters(word_map, word)    
 
 def render_solutions_array(solutions, tone_numbers, spaces):
     return [render_word(word, tone_numbers, spaces) for word in solutions]
 
 def render_all_romanization_solutions(word_map, word_list, tone_numbers, spaces):
@@ -84,14 +88,15 @@
     word_list = tokenize(text)
     word_list = improve_tokenization(word_map, word_list)
     return word_list
 
 def convert_to_romanization(word_map, text, tone_numbers, spaces):
     solution_list = []
     word_list = tokenize_to_word_list(word_map, text)
+    logger.debug(f'tokenization result: {pprint.pformat(word_list)}')
     solutions = render_all_romanization_solutions(word_map, word_list, tone_numbers, spaces)
     return {
         'word_list': word_list, 
         'solutions': solutions
     }
 
 def convert_single_solution(word_map, text, tone_numbers, spaces):
@@ -127,15 +132,19 @@
     # if the word is not found in the pinyin dictionary gives a better chance to find a good match.
     # for example with 投资银行, breaking down as 投资, 银行 is better
 
     iterations = 0
 
     final_word_list = []
     for word in word_list:
-        if len(word) == 1 or word in word_map:
+        #
+        if not hanzidentifier.has_chinese(word):
+            # word is not chinese
+            final_word_list.append(word)
+        elif len(word) == 1 or word in word_map:
             final_word_list.append(word)
         else:
             logger.debug(f'attempting improved tokenization for {word}')
             word_breakdown = []
             word_remaining_chars = word
             found_larger_matches = 0
             continue_iteration = True
```

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping/dict.txt.big` & `pinyin_jyutping-0.9/pinyin_jyutping/dict.txt.big`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping/logic.py` & `pinyin_jyutping-0.9/pinyin_jyutping/logic.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping/parser.py` & `pinyin_jyutping-0.9/pinyin_jyutping/parser.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping/pinyin_jyutping.pkl` & `pinyin_jyutping-0.9/pinyin_jyutping/pinyin_jyutping.pkl`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping/syllables.py` & `pinyin_jyutping-0.9/pinyin_jyutping/syllables.py`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping.egg-info/PKG-INFO` & `pinyin_jyutping-0.9/pinyin_jyutping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinyin-jyutping
-Version: 0.8
+Version: 0.9
 Summary: Convert a Chinese sentence to Pinyin or Jyutping
 Home-page: https://github.com/Language-Tools/pinyin-jyutping
 Author: LucW
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pinyin_jyutping-0.8/pinyin_jyutping.egg-info/SOURCES.txt` & `pinyin_jyutping-0.9/pinyin_jyutping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinyin_jyutping-0.8/setup.py` & `pinyin_jyutping-0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup
 
 # build instructions
 #  python3 setup.py sdist
 # twine upload dist/*
 
 setup(name='pinyin_jyutping',
-      version='0.8',
+      version='0.9',
       description='Convert a Chinese sentence to Pinyin or Jyutping',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/pinyin-jyutping',
       author='LucW',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Topic :: Text Processing :: Linguistic',
       ],      
       license='GPL',
       packages=['pinyin_jyutping'],
       install_requires=[
           'jieba',
+          'hanzidentifier'
       ],      
       zip_safe=False,
       include_package_data=True)
```

