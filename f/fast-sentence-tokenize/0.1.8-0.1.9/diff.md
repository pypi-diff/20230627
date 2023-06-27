# Comparing `tmp/fast-sentence-tokenize-0.1.8.tar.gz` & `tmp/fast-sentence-tokenize-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-sentence-tokenize-0.1.8.tar", max compression
+gzip compressed data, was "fast-sentence-tokenize-0.1.9.tar", max compression
```

## Comparing `fast-sentence-tokenize-0.1.8.tar` & `fast-sentence-tokenize-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1566 2022-10-26 23:22:27.330527 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/__init__.py
--rw-r--r--   0        0        0       34 2022-05-28 20:54:47.463119 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/bp/__init__.py
--rw-r--r--   0        0        0     2081 2022-10-26 23:30:12.719828 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/bp/ngrams.py
--rw-r--r--   0        0        0     1703 2022-10-26 22:27:20.714296 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/bp/tokenizer.py
--rw-r--r--   0        0        0      153 2022-10-26 22:27:22.141295 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/__init__.py
--rw-r--r--   0        0        0      260 2022-08-25 23:50:45.765850 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/__init__.py
--rw-r--r--   0        0        0     1378 2022-08-25 23:47:07.645771 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/abbreviations_kb.py
--rw-r--r--   0        0        0     1279 2022-05-28 20:54:47.467618 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/currency_kb.py
--rw-r--r--   0        0        0      151 2022-08-25 23:46:33.178670 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/dquotes_kb.py
--rw-r--r--   0        0        0     2139 2022-08-25 23:47:27.406964 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/enclictics.py
--rw-r--r--   0        0        0      488 2022-08-25 23:46:47.683233 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/hyphens_kb.py
--rw-r--r--   0        0        0      115 2022-08-25 23:46:01.562551 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/squotes_kb.py
--rw-r--r--   0        0        0     1681 2022-08-25 23:50:40.143420 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/stopwords_kb.py
--rw-r--r--   0        0        0     1275 2022-08-25 23:54:13.262464 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/find_dictionaries.py
--rw-r--r--   0        0        0     2130 2022-10-26 22:27:20.713795 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/find_pronouns.py
--rw-r--r--   0        0        0      719 2022-10-26 22:27:22.136294 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/find_stopwords.py
--rw-r--r--   0        0        0        0 2022-08-26 20:24:25.407172 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/dmo/__init__.py
--rw-r--r--   0        0        0      160 2022-10-26 23:22:27.343031 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/svc/__init__.py
--rw-r--r--   0        0        0     2034 2022-10-26 23:30:12.714328 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/svc/sliding_window_extract.py
--rw-r--r--   0        0        0     8325 2022-08-26 20:30:59.549589 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/svc/tokenize_use_graffl.py
--rw-r--r--   0        0        0      769 2022-10-26 22:27:20.714795 fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/svc/tokenize_use_spacy.py
--rw-r--r--   0        0        0     1476 2022-10-26 22:22:26.184879 fast-sentence-tokenize-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1014 2022-10-26 22:27:21.236795 fast-sentence-tokenize-0.1.8/README.md
--rw-r--r--   0        0        0     1922 2022-10-26 23:30:32.318152 fast-sentence-tokenize-0.1.8/setup.py
--rw-r--r--   0        0        0     1831 2022-10-26 23:30:32.318152 fast-sentence-tokenize-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1566 2022-10-26 23:22:27.330527 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/__init__.py
+-rw-r--r--   0        0        0       34 2022-05-28 20:54:47.463119 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/bp/__init__.py
+-rw-r--r--   0        0        0     2081 2022-10-26 23:30:12.719828 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/bp/ngrams.py
+-rw-r--r--   0        0        0     1703 2022-10-26 22:27:20.714296 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/bp/tokenizer.py
+-rw-r--r--   0        0        0      153 2022-10-26 22:27:22.141295 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/__init__.py
+-rw-r--r--   0        0        0      260 2022-08-25 23:50:45.765850 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/__init__.py
+-rw-r--r--   0        0        0     1378 2022-08-25 23:47:07.645771 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/abbreviations_kb.py
+-rw-r--r--   0        0        0     1279 2022-05-28 20:54:47.467618 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/currency_kb.py
+-rw-r--r--   0        0        0      151 2022-08-25 23:46:33.178670 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/dquotes_kb.py
+-rw-r--r--   0        0        0     2139 2022-08-25 23:47:27.406964 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/enclictics.py
+-rw-r--r--   0        0        0      488 2022-08-25 23:46:47.683233 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/hyphens_kb.py
+-rw-r--r--   0        0        0      115 2022-08-25 23:46:01.562551 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/squotes_kb.py
+-rw-r--r--   0        0        0     1681 2022-08-25 23:50:40.143420 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/stopwords_kb.py
+-rw-r--r--   0        0        0     1275 2022-08-25 23:54:13.262464 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/find_dictionaries.py
+-rw-r--r--   0        0        0     2130 2022-10-26 22:27:20.713795 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/find_pronouns.py
+-rw-r--r--   0        0        0      719 2022-10-26 22:27:22.136294 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/find_stopwords.py
+-rw-r--r--   0        0        0        0 2022-08-26 20:24:25.407172 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/dmo/__init__.py
+-rw-r--r--   0        0        0      160 2022-10-26 23:22:27.343031 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/svc/__init__.py
+-rw-r--r--   0        0        0     1586 2022-10-28 23:27:31.350030 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/svc/sliding_window_extract.py
+-rw-r--r--   0        0        0     8325 2022-08-26 20:30:59.549589 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/svc/tokenize_use_graffl.py
+-rw-r--r--   0        0        0      769 2022-10-26 22:27:20.714795 fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/svc/tokenize_use_spacy.py
+-rw-r--r--   0        0        0     1476 2022-10-28 23:26:09.125495 fast-sentence-tokenize-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1014 2022-10-26 22:27:21.236795 fast-sentence-tokenize-0.1.9/README.md
+-rw-r--r--   0        0        0     1922 2022-10-28 23:28:01.477457 fast-sentence-tokenize-0.1.9/setup.py
+-rw-r--r--   0        0        0     1831 2022-10-28 23:28:01.477957 fast-sentence-tokenize-0.1.9/PKG-INFO
```

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/__init__.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/__init__.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/bp/ngrams.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/bp/ngrams.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/bp/tokenizer.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/bp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/abbreviations_kb.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/abbreviations_kb.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/currency_kb.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/currency_kb.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/enclictics.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/enclictics.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/dto/stopwords_kb.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/dto/stopwords_kb.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/find_dictionaries.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/find_dictionaries.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/find_pronouns.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/find_pronouns.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/datablock/find_stopwords.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/datablock/find_stopwords.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/svc/sliding_window_extract.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/svc/sliding_window_extract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,29 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 """ Simple Sliding Window N-Gram Extractor """
 
 
 from typing import List
 
-from baseblock import BaseObject, Enforcer
+from baseblock import BaseObject, TextUtils
 
 
 class SlidingWindowExtract(BaseObject):
     """ Simple Sliding Window N-Gram Extractor """
 
     def __init__(self):
         """ Change Log
 
         Created:
             26-Oct-2022
             craigtrim@gmail.com
         """
         BaseObject.__init__(self, __name__)
 
-    def _extract(self,
-                 tokens: List[str],
-                 gram_level: int) -> list:
-
-        results = []
-        total_tokens = len(tokens)
-
-        for i in range(total_tokens):
-
-            buffer = []
-
-            x = 0
-            while x < gram_level:
-
-                pos = x + i
-                if pos < total_tokens:
-                    buffer.append(tokens[pos])
-
-                x += 1
-
-            if len(buffer) == gram_level:
-                results.append(buffer)
-                buffer = []
-
-        return results
-
     def process(self,
                 tokens: List[str],
                 gram_level: int,
                 skip_gram: bool = False) -> list:
         """ Extract Bigrams
 
         Args:
@@ -58,22 +32,29 @@
             skip_gram (bool, False): skip every other gram. Defaults to False.
 
         Returns:
             list: a list of bigrams (or skipgrams)
         """
 
         if not skip_gram:
-            return self._extract(tokens=tokens, gram_level=gram_level)
+            return TextUtils.sliding_window(
+                tokens=tokens,
+                window_size=gram_level)
 
         tokens_even = []
         tokens_odd = []
 
         for i in range(len(tokens)):
             if i % 2 != 0:
                 tokens_odd.append(tokens[i])
             else:
                 tokens_even.append(tokens[i])
 
-        grams_odd = self._extract(tokens=tokens_odd, gram_level=gram_level)
-        grams_even = self._extract(tokens=tokens_even, gram_level=gram_level)
+        grams_odd = TextUtils.sliding_window(
+            tokens=tokens_odd,
+            window_size=gram_level)
+
+        grams_even = TextUtils.sliding_window(
+            tokens=tokens_even,
+            window_size=gram_level)
 
         return grams_odd + grams_even
```

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/svc/tokenize_use_graffl.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/svc/tokenize_use_graffl.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/fast_sentence_tokenize/svc/tokenize_use_spacy.py` & `fast-sentence-tokenize-0.1.9/fast_sentence_tokenize/svc/tokenize_use_spacy.py`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/pyproject.toml` & `fast-sentence-tokenize-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Craig Trim <craigtrim@gmail.com>",
 ]
 
 description = "Fast and Efficient Sentence Tokenization"
 license = "None"
 name = "fast-sentence-tokenize"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 keywords = ["nlp", "nlu", "text", "classify", "classification"]
 repository = "https://github.com/craigtrim/fast-sentence-tokenize"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `fast-sentence-tokenize-0.1.8/README.md` & `fast-sentence-tokenize-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fast-sentence-tokenize-0.1.8/setup.py` & `fast-sentence-tokenize-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock', 'nltk', 'spacy==3.3']
 
 setup_kwargs = {
     'name': 'fast-sentence-tokenize',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Fast and Efficient Sentence Tokenization',
     'long_description': '# Fast Sentence Tokenizer (fast-sentence-tokenize)\nBest in class tokenizer\n\n## Usage\n\n### Import\n```python\nfrom fast_sentence_tokenize import fast_sentence_tokenize\n```\n\n### Call Tokenizer\n```python\nresults = fast_sentence_tokenize("isn\'t a test great!!?")\n```\n\n### Results\n```json\n[\n   "isn\'t",\n   "a",\n   "test",\n   "great",\n   "!",\n   "!",\n   "?"\n]\n```\nNote that whitespace is not preserved in the output by default.\n\nThis generally results in a more accurate parse from downstream components, but may make the reassembly of the original sentence more challenging.\n\n### Preserve Whitespace\n```python\nresults = fast_sentence_tokenize("isn\'t a test great!!?", eliminate_whitespace=False)\n```\n### Results\n```json\n[\n   "isn\'t ",\n   "a ",\n   "test ",\n   "great",\n   "!",\n   "!",\n   "?"\n]\n```\n\nThis option preserves whitespace.\n\nThis is useful if you want to re-assemble the tokens using the pre-existing spacing\n```python\nassert \'\'.join(tokens) == input_text\n```\n',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/fast-sentence-tokenize',
```

### Comparing `fast-sentence-tokenize-0.1.8/PKG-INFO` & `fast-sentence-tokenize-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-sentence-tokenize
-Version: 0.1.8
+Version: 0.1.9
 Summary: Fast and Efficient Sentence Tokenization
 Home-page: https://github.com/craigtrim/fast-sentence-tokenize
 License: None
 Keywords: nlp,nlu,text,classify,classification
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
```

