# Comparing `tmp/grazier-0.0.1.tar.gz` & `tmp/grazier-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grazier-0.0.1.tar", last modified: Tue Jun 27 00:25:07 2023, max compression
+gzip compressed data, was "grazier-0.0.2.tar", last modified: Tue Jun 27 00:29:18 2023, max compression
```

## Comparing `grazier-0.0.1.tar` & `grazier-0.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:25:07.230774 grazier-0.0.1/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1181 2023-06-26 20:44:22.000000 grazier-0.0.1/LICENSE
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8545 2023-06-27 00:25:07.230774 grazier-0.0.1/PKG-INFO
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     6313 2023-06-27 00:23:42.000000 grazier-0.0.1/README.md
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:25:07.230774 grazier-0.0.1/grazier/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      216 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      764 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/cli.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:25:07.230774 grazier-0.0.1/grazier/engines/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:09:44.000000 grazier-0.0.1/grazier/engines/__init__.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:25:07.230774 grazier-0.0.1/grazier/engines/chat/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3418 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3411 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/anthropic_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      824 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/anthropic_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    11124 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/bard_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      760 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/bard_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8989 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/llama_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      818 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/llama_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2734 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/openai_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1014 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/openai_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4905 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/stable_lm_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      824 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/stable_lm_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3321 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/vertex_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      815 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/chat/vertex_engine_test.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:25:07.230774 grazier-0.0.1/grazier/engines/llm/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2189 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/llm/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4410 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/llm/huggingface_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      759 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/llm/huggingface_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3131 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/llm/llama_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      777 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/llm/llama_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2321 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/llm/openai_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      835 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/llm/openai_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1928 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/llm/vertex_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      574 2023-06-27 00:23:55.000000 grazier-0.0.1/grazier/engines/llm/vertex_engine_test.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:25:07.230774 grazier-0.0.1/grazier/utils/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:11:27.000000 grazier-0.0.1/grazier/utils/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2253 2023-06-26 20:25:42.000000 grazier-0.0.1/grazier/utils/python.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1123 2023-06-26 21:00:23.000000 grazier-0.0.1/grazier/utils/pytorch.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:25:07.230774 grazier-0.0.1/grazier.egg-info/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8545 2023-06-27 00:25:07.000000 grazier-0.0.1/grazier.egg-info/PKG-INFO
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1239 2023-06-27 00:25:07.000000 grazier-0.0.1/grazier.egg-info/SOURCES.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        1 2023-06-27 00:25:07.000000 grazier-0.0.1/grazier.egg-info/dependency_links.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       45 2023-06-27 00:25:07.000000 grazier-0.0.1/grazier.egg-info/entry_points.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      171 2023-06-27 00:25:07.000000 grazier-0.0.1/grazier.egg-info/requires.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        8 2023-06-27 00:25:07.000000 grazier-0.0.1/grazier.egg-info/top_level.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2575 2023-06-27 00:24:58.000000 grazier-0.0.1/pyproject.toml
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       38 2023-06-27 00:25:07.230774 grazier-0.0.1/setup.cfg
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:29:18.927517 grazier-0.0.2/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1181 2023-06-26 20:44:22.000000 grazier-0.0.2/LICENSE
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8735 2023-06-27 00:29:18.927517 grazier-0.0.2/PKG-INFO
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     6313 2023-06-27 00:23:42.000000 grazier-0.0.2/README.md
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:29:18.923517 grazier-0.0.2/grazier/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      216 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      764 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/cli.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:29:18.923517 grazier-0.0.2/grazier/engines/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:09:44.000000 grazier-0.0.2/grazier/engines/__init__.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:29:18.923517 grazier-0.0.2/grazier/engines/chat/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3418 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3411 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/anthropic_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      824 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/anthropic_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    11124 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/bard_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      760 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/bard_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8989 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/llama_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      818 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/llama_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2734 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/openai_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1014 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/openai_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4905 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/stable_lm_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      824 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/stable_lm_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3321 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/vertex_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      815 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/chat/vertex_engine_test.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:29:18.927517 grazier-0.0.2/grazier/engines/llm/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2189 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/llm/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4410 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/llm/huggingface_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      759 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/llm/huggingface_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3131 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/llm/llama_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      777 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/llm/llama_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2321 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/llm/openai_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      835 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/llm/openai_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1928 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/llm/vertex_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      574 2023-06-27 00:23:55.000000 grazier-0.0.2/grazier/engines/llm/vertex_engine_test.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:29:18.927517 grazier-0.0.2/grazier/utils/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:11:27.000000 grazier-0.0.2/grazier/utils/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2253 2023-06-26 20:25:42.000000 grazier-0.0.2/grazier/utils/python.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1123 2023-06-26 21:00:23.000000 grazier-0.0.2/grazier/utils/pytorch.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-06-27 00:29:18.923517 grazier-0.0.2/grazier.egg-info/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8735 2023-06-27 00:29:18.000000 grazier-0.0.2/grazier.egg-info/PKG-INFO
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1239 2023-06-27 00:29:18.000000 grazier-0.0.2/grazier.egg-info/SOURCES.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        1 2023-06-27 00:29:18.000000 grazier-0.0.2/grazier.egg-info/dependency_links.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       45 2023-06-27 00:29:18.000000 grazier-0.0.2/grazier.egg-info/entry_points.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      171 2023-06-27 00:29:18.000000 grazier-0.0.2/grazier.egg-info/requires.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        8 2023-06-27 00:29:18.000000 grazier-0.0.2/grazier.egg-info/top_level.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2751 2023-06-27 00:27:56.000000 grazier-0.0.2/pyproject.toml
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       38 2023-06-27 00:29:18.927517 grazier-0.0.2/setup.cfg
```

### Comparing `grazier-0.0.1/LICENSE` & `grazier-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/PKG-INFO` & `grazier-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: grazier
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for calling (and calling out to) large language models.
 Author-email: David Chan <davidchan@berkeley.edu>
 License: 
         Copyright 2023, Regents of the University of California
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
         THIS SOFTWARE AND/OR DATA WAS DEPOSITED IN THE BAIR OPEN RESEARCH COMMONS REPOSITORY ON 02/28/2023
         
+Project-URL: homepage, https://github.com/DavidMChan/grazier
+Project-URL: documentation, https://github.com/DavidMChan/grazier
+Project-URL: repository, https://github.com/DavidMChan/grazier
 Keywords: language-models,api,transformers,huggingface,openai,anthropic,gpt3,gpt-j,gpt-neo,gpt4,vertex,palm,bard
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `grazier-0.0.1/README.md` & `grazier-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/cli.py` & `grazier-0.0.2/grazier/cli.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/__init__.py` & `grazier-0.0.2/grazier/engines/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/anthropic_engine.py` & `grazier-0.0.2/grazier/engines/chat/anthropic_engine.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/anthropic_engine_test.py` & `grazier-0.0.2/grazier/engines/chat/anthropic_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/bard_engine.py` & `grazier-0.0.2/grazier/engines/chat/bard_engine.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/bard_engine_test.py` & `grazier-0.0.2/grazier/engines/chat/bard_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/llama_engine.py` & `grazier-0.0.2/grazier/engines/chat/llama_engine.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/llama_engine_test.py` & `grazier-0.0.2/grazier/engines/chat/llama_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/openai_engine.py` & `grazier-0.0.2/grazier/engines/chat/openai_engine.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/openai_engine_test.py` & `grazier-0.0.2/grazier/engines/chat/openai_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/stable_lm_engine.py` & `grazier-0.0.2/grazier/engines/chat/stable_lm_engine.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/stable_lm_engine_test.py` & `grazier-0.0.2/grazier/engines/chat/stable_lm_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/vertex_engine.py` & `grazier-0.0.2/grazier/engines/chat/vertex_engine.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/chat/vertex_engine_test.py` & `grazier-0.0.2/grazier/engines/chat/vertex_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/llm/__init__.py` & `grazier-0.0.2/grazier/engines/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/llm/huggingface_engine.py` & `grazier-0.0.2/grazier/engines/llm/huggingface_engine.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/llm/huggingface_engine_test.py` & `grazier-0.0.2/grazier/engines/llm/huggingface_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/llm/llama_engine.py` & `grazier-0.0.2/grazier/engines/llm/llama_engine.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/llm/llama_engine_test.py` & `grazier-0.0.2/grazier/engines/llm/llama_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/llm/openai_engine.py` & `grazier-0.0.2/grazier/engines/llm/openai_engine.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/llm/openai_engine_test.py` & `grazier-0.0.2/grazier/engines/llm/openai_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/llm/vertex_engine.py` & `grazier-0.0.2/grazier/engines/llm/vertex_engine.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/engines/llm/vertex_engine_test.py` & `grazier-0.0.2/grazier/engines/llm/vertex_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/utils/python.py` & `grazier-0.0.2/grazier/utils/python.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier/utils/pytorch.py` & `grazier-0.0.2/grazier/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/grazier.egg-info/PKG-INFO` & `grazier-0.0.2/grazier.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: grazier
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for calling (and calling out to) large language models.
 Author-email: David Chan <davidchan@berkeley.edu>
 License: 
         Copyright 2023, Regents of the University of California
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
         THIS SOFTWARE AND/OR DATA WAS DEPOSITED IN THE BAIR OPEN RESEARCH COMMONS REPOSITORY ON 02/28/2023
         
+Project-URL: homepage, https://github.com/DavidMChan/grazier
+Project-URL: documentation, https://github.com/DavidMChan/grazier
+Project-URL: repository, https://github.com/DavidMChan/grazier
 Keywords: language-models,api,transformers,huggingface,openai,anthropic,gpt3,gpt-j,gpt-neo,gpt4,vertex,palm,bard
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `grazier-0.0.1/grazier.egg-info/SOURCES.txt` & `grazier-0.0.2/grazier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grazier-0.0.1/pyproject.toml` & `grazier-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'grazier'
-version = '0.0.1'
+version = '0.0.2'
 description = 'A tool for calling (and calling out to) large language models.'
 authors = [
     {name='David Chan', email='davidchan@berkeley.edu'}
 ]
 dependencies=[
     # Base dependencies
     "click",
@@ -59,14 +59,19 @@
 [project.optional-dependencies]
 dev = ["pytest", "ruff", "mypy"]
 
 
 [project.scripts]
 grazier = "grazier.cli:main"
 
+[project.urls]
+homepage = "https://github.com/DavidMChan/grazier"
+documentation = "https://github.com/DavidMChan/grazier"
+repository = "https://github.com/DavidMChan/grazier"
+
 
 
 [tool.black]
 line-length = 120
 target_version =['py38']
 exclude = '''
```

