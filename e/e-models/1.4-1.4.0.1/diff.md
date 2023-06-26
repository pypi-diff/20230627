# Comparing `tmp/e-models-1.4.tar.gz` & `tmp/e-models-1.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.4.tar", last modified: Mon Jun 26 14:30:46 2023, max compression
+gzip compressed data, was "e-models-1.4.0.1.tar", last modified: Mon Jun 26 22:58:57 2023, max compression
```

## Comparing `e-models-1.4.tar` & `e-models-1.4.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.338616 e-models-1.4/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.4/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3466 2023-06-26 14:30:46.338616 e-models-1.4/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-06-01 14:06:43.000000 e-models-1.4/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.334616 e-models-1.4/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3466 2023-06-26 14:30:46.000000 e-models-1.4/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      628 2023-06-26 14:30:46.000000 e-models-1.4/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-06-26 14:30:46.000000 e-models-1.4/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-06-26 14:30:46.000000 e-models-1.4/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-06-26 14:30:46.000000 e-models-1.4/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.334616 e-models-1.4/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       20 2023-06-26 13:32:53.000000 e-models-1.4/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.4/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.338616 e-models-1.4/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.4/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1818 2023-06-23 22:31:59.000000 e-models-1.4/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4716 2023-06-23 22:38:40.000000 e-models-1.4/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.338616 e-models-1.4/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35296 2023-06-08 13:46:29.000000 e-models-1.4/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.4/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.4/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.4/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.4/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.4/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.338616 e-models-1.4/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.4/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2544 2023-06-23 22:05:11.000000 e-models-1.4/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4351 2023-06-23 21:34:47.000000 e-models-1.4/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.4/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-06-26 14:30:46.338616 e-models-1.4/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      905 2023-06-26 13:32:42.000000 e-models-1.4/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 14:30:46.338616 e-models-1.4/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4948 2023-06-23 18:11:59.000000 e-models-1.4/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7475 2023-06-23 23:01:17.000000 e-models-1.4/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 22:58:57.205750 e-models-1.4.0.1/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.4.0.1/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3470 2023-06-26 22:58:57.205750 e-models-1.4.0.1/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-06-01 14:06:43.000000 e-models-1.4.0.1/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 22:58:57.201750 e-models-1.4.0.1/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3470 2023-06-26 22:58:57.000000 e-models-1.4.0.1/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      628 2023-06-26 22:58:57.000000 e-models-1.4.0.1/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-06-26 22:58:57.000000 e-models-1.4.0.1/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-06-26 22:58:57.000000 e-models-1.4.0.1/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-06-26 22:58:57.000000 e-models-1.4.0.1/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 22:58:57.201750 e-models-1.4.0.1/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2023-06-26 22:57:06.000000 e-models-1.4.0.1/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.4.0.1/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 22:58:57.205750 e-models-1.4.0.1/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.4.0.1/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1882 2023-06-26 22:53:37.000000 e-models-1.4.0.1/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4716 2023-06-23 22:38:40.000000 e-models-1.4.0.1/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 22:58:57.205750 e-models-1.4.0.1/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35296 2023-06-08 13:46:29.000000 e-models-1.4.0.1/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.4.0.1/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.4.0.1/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.4.0.1/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.4.0.1/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.4.0.1/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 22:58:57.205750 e-models-1.4.0.1/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.4.0.1/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2544 2023-06-23 22:05:11.000000 e-models-1.4.0.1/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4351 2023-06-23 21:34:47.000000 e-models-1.4.0.1/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.4.0.1/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-06-26 22:58:57.205750 e-models-1.4.0.1/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      909 2023-06-26 22:57:26.000000 e-models-1.4.0.1/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-26 22:58:57.205750 e-models-1.4.0.1/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4948 2023-06-23 18:11:59.000000 e-models-1.4.0.1/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7475 2023-06-23 23:01:17.000000 e-models-1.4.0.1/tests/test_scrapyutils.py
```

### Comparing `e-models-1.4/LICENSE` & `e-models-1.4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.4/PKG-INFO` & `e-models-1.4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.4
+Version: 1.4.0.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.4/README.md` & `e-models-1.4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.4/e_models.egg-info/PKG-INFO` & `e-models-1.4.0.1/e_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.4
+Version: 1.4.0.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.4/e_models.egg-info/SOURCES.txt` & `e-models-1.4.0.1/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.4/emodels/datasets/tokenizers.py` & `e-models-1.4.0.1/emodels/datasets/tokenizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     DatasetFilename,
     ResponseConverter,
     build_response_from_sample_data,
     Filename,
 )
 
 
+class TokenizerFilename(Filename):
+    pass
+
+
 def extract_dataset_text(
     dataset_filename: DatasetFilename, output_filename: Filename, response_converter_cls: type[ResponseConverter]
 ):
     """
     Extracts text from a dataset, suitable for usage in training tokenizer.
     The text is extracted using the specified ResponseConverter class, and saved into an output file
     for further tokenizer processing.
@@ -38,21 +42,21 @@
     with output_filename.open("w") as output:
         for data in dataset_filename:
             response = build_response_from_sample_data(data)
             text_pieces = converter.response_to_valid_text(response.text)
             print(" ".join(text_pieces), file=output)
 
 
-def train_tokenizer(tokenizer_training_text: Filename, model_filename: Filename):
+def train_tokenizer(tokenizer_training_text: Filename, model_filename: TokenizerFilename):
     """
     Train a tokenizer using tokenizer_training_text file as input.
     Saves the model into the specified model_filename.
     """
     model_prefix = os.path.splitext(model_filename.basename)[0]
     spm.SentencePieceTrainer.train(f"--input={tokenizer_training_text} --model_prefix={model_prefix} --vocab_size=2000")
     shutil.move(f"{model_prefix}.model", "/tmp/")
 
 
-def load_tokenizer(model_filename: Filename):
+def load_tokenizer(model_filename: TokenizerFilename):
     sp = spm.SentencePieceProcessor()
     sp.load(model_filename)
     return sp
```

### Comparing `e-models-1.4/emodels/datasets/utils.py` & `e-models-1.4.0.1/emodels/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.4/emodels/html2text/__init__.py` & `e-models-1.4.0.1/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.4/emodels/html2text/config.py` & `e-models-1.4.0.1/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.4/emodels/html2text/utils.py` & `e-models-1.4.0.1/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.4/emodels/scrapyutils/loader.py` & `e-models-1.4.0.1/emodels/scrapyutils/loader.py`

 * *Files identical despite different names*

### Comparing `e-models-1.4/emodels/scrapyutils/response.py` & `e-models-1.4.0.1/emodels/scrapyutils/response.py`

 * *Files identical despite different names*

### Comparing `e-models-1.4/setup.py` & `e-models-1.4.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.4',
+    version      = '1.4.0.1',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.4/tests/test_html2text.py` & `e-models-1.4.0.1/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.4/tests/test_scrapyutils.py` & `e-models-1.4.0.1/tests/test_scrapyutils.py`

 * *Files identical despite different names*

