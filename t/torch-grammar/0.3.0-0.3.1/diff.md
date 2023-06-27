# Comparing `tmp/torch_grammar-0.3.0.tar.gz` & `tmp/torch_grammar-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_grammar-0.3.0.tar", max compression
+gzip compressed data, was "torch_grammar-0.3.1.tar", max compression
```

## Comparing `torch_grammar-0.3.0.tar` & `torch_grammar-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1946 2023-06-26 22:01:25.065253 torch_grammar-0.3.0/README.md
--rw-r--r--   0        0        0      588 2023-06-26 22:01:54.186219 torch_grammar-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.3.0/torch_grammar/__init__.py
--rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.3.0/torch_grammar/grammar_parser.py
--rw-r--r--   0        0        0     6419 2023-06-26 21:03:33.486520 torch_grammar-0.3.0/torch_grammar/grammar_sampler.py
--rw-r--r--   0        0        0     1949 2023-06-26 22:00:00.538471 torch_grammar-0.3.0/torch_grammar/token_trie.py
--rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 torch_grammar-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1890 2023-06-27 14:34:41.788242 torch_grammar-0.3.1/README.md
+-rw-r--r--   0        0        0      588 2023-06-27 14:35:12.424183 torch_grammar-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.3.1/torch_grammar/__init__.py
+-rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.3.1/torch_grammar/grammar_parser.py
+-rw-r--r--   0        0        0     6419 2023-06-26 21:03:33.486520 torch_grammar-0.3.1/torch_grammar/grammar_sampler.py
+-rw-r--r--   0        0        0     2626 2023-06-27 14:34:57.299812 torch_grammar-0.3.1/torch_grammar/token_trie.py
+-rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 torch_grammar-0.3.1/PKG-INFO
```

### Comparing `torch_grammar-0.3.0/README.md` & `torch_grammar-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,15 @@
   token = torch.argmax(logits).item()
   # logits_processor.accept_token(token)
   ids[0].append(token)
 print(f"\x1b[1mfirst 10 tokens: \x1b[1;35m{tokenizer.decode(ids[0])}\x1b[0m")
 ```
 
 `logits_processor` is meant to be passed to `model.generate` in a HuggingFace
-transformers model but this integration is not yet super clean. Take a look at
-the notebook in this repo for more info.
+transformers model but this integration is not yet super clean.
 
 ### TODO / possible features
 
 * UTF-8 support... a bit of fiddling but not terribly hard
 * More expressive grammars... lookahead would be challenging.
 * Easier integration with various tokenizers... LLaMA works well; T5 presents
   significant challenges; haven't even tried others.
```

### Comparing `torch_grammar-0.3.0/pyproject.toml` & `torch_grammar-0.3.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch-grammar"
-version = "0.3.0"
+version = "0.3.1"
 description = "Restrict LLM generations to a context-free grammar"
 authors = ["Burke Libbey <burke.libbey@shopify.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "torch_grammar"}]
 
 [tool.poetry.dependencies]
```

### Comparing `torch_grammar-0.3.0/torch_grammar/grammar_parser.py` & `torch_grammar-0.3.1/torch_grammar/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.3.0/torch_grammar/grammar_sampler.py` & `torch_grammar-0.3.1/torch_grammar/grammar_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.3.0/PKG-INFO` & `torch_grammar-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-grammar
-Version: 0.3.0
+Version: 0.3.1
 Summary: Restrict LLM generations to a context-free grammar
 License: MIT
 Author: Burke Libbey
 Author-email: burke.libbey@shopify.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -46,16 +46,15 @@
   token = torch.argmax(logits).item()
   # logits_processor.accept_token(token)
   ids[0].append(token)
 print(f"\x1b[1mfirst 10 tokens: \x1b[1;35m{tokenizer.decode(ids[0])}\x1b[0m")
 ```
 
 `logits_processor` is meant to be passed to `model.generate` in a HuggingFace
-transformers model but this integration is not yet super clean. Take a look at
-the notebook in this repo for more info.
+transformers model but this integration is not yet super clean.
 
 ### TODO / possible features
 
 * UTF-8 support... a bit of fiddling but not terribly hard
 * More expressive grammars... lookahead would be challenging.
 * Easier integration with various tokenizers... LLaMA works well; T5 presents
   significant challenges; haven't even tried others.
```

