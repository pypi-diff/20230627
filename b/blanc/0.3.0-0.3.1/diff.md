# Comparing `tmp/blanc-0.3.0.tar.gz` & `tmp/blanc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blanc-0.3.0.tar", last modified: Sun Nov 27 21:12:58 2022, max compression
+gzip compressed data, was "blanc-0.3.1.tar", last modified: Mon Jun 26 23:57:13 2023, max compression
```

## Comparing `blanc-0.3.0.tar` & `blanc-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2022-11-27 21:12:58.274495 blanc-0.3.0/
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2022-11-27 21:12:58.259091 blanc-0.3.0/.github/
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2022-11-27 21:12:58.260558 blanc-0.3.0/.github/workflows/
--rw-r--r--   0 olegvasilyev   (502) staff       (20)     2532 2022-11-20 20:03:24.000000 blanc-0.3.0/.github/workflows/codeql-analysis.yml
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)       54 2020-04-22 21:28:28.000000 blanc-0.3.0/.gitignore
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1049 2020-04-22 21:28:28.000000 blanc-0.3.0/LICENSE
--rw-r--r--   0 olegvasilyev   (502) staff       (20)    13913 2022-11-27 21:12:58.274266 blanc-0.3.0/PKG-INFO
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13478 2022-02-10 23:08:14.000000 blanc-0.3.0/README.md
--rw-r--r--   0 olegvasilyev   (502) staff       (20)     1629 2022-11-20 20:03:24.000000 blanc-0.3.0/SECURITY.md
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2022-11-27 21:12:58.262052 blanc-0.3.0/blanc/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      133 2022-02-10 23:08:14.000000 blanc-0.3.0/blanc/__init__.py
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    12173 2021-09-01 21:24:46.000000 blanc-0.3.0/blanc/__main__.py
--rw-r--r--   0 olegvasilyev   (502) staff       (20)       21 2022-11-27 06:46:03.000000 blanc-0.3.0/blanc/__version__.py
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    36885 2021-06-06 04:38:30.000000 blanc-0.3.0/blanc/blanc.py
--rw-r--r--   0 olegvasilyev   (502) staff       (20)    19293 2022-11-27 19:37:04.000000 blanc-0.3.0/blanc/estime.py
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    10428 2022-04-26 15:26:54.000000 blanc-0.3.0/blanc/shannon.py
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    16178 2021-03-11 01:31:26.000000 blanc-0.3.0/blanc/utils.py
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2022-11-27 21:12:58.262736 blanc-0.3.0/blanc.egg-info/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13913 2022-11-27 21:12:58.000000 blanc-0.3.0/blanc.egg-info/PKG-INFO
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      617 2022-11-27 21:12:58.000000 blanc-0.3.0/blanc.egg-info/SOURCES.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)        1 2022-11-27 21:12:58.000000 blanc-0.3.0/blanc.egg-info/dependency_links.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)       46 2022-11-27 21:12:58.000000 blanc-0.3.0/blanc.egg-info/entry_points.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)       98 2022-11-27 21:12:58.000000 blanc-0.3.0/blanc.egg-info/requires.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)        6 2022-11-27 21:12:58.000000 blanc-0.3.0/blanc.egg-info/top_level.txt
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2022-11-27 21:12:58.271118 blanc-0.3.0/data/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)  2779006 2020-11-22 22:52:16.000000 blanc-0.3.0/data/CNN_DailyMail_555.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1110748 2020-11-22 22:52:16.000000 blanc-0.3.0/data/DailyNews_300.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1257825 2020-11-22 22:52:16.000000 blanc-0.3.0/data/DailyNews_300_aspects.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1361 2021-04-04 18:11:32.000000 blanc-0.3.0/data/README.md
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      506 2020-04-22 21:28:28.000000 blanc-0.3.0/data/doc-summaries.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      363 2020-04-22 21:28:28.000000 blanc-0.3.0/data/pairs.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      149 2020-04-22 21:28:28.000000 blanc-0.3.0/data/single.json
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2022-11-27 21:12:58.271259 blanc-0.3.0/estime/
--rw-r--r--   0 olegvasilyev   (502) staff       (20)     3974 2022-11-27 20:17:26.000000 blanc-0.3.0/estime/README.md
--rw-r--r--   0 olegvasilyev   (502) staff       (20)       98 2022-11-21 01:28:17.000000 blanc-0.3.0/requirements.txt
--rw-r--r--   0 olegvasilyev   (502) staff       (20)       38 2022-11-27 21:12:58.274539 blanc-0.3.0/setup.cfg
--rw-r--r--   0 olegvasilyev   (502) staff       (20)      948 2022-11-27 20:13:31.000000 blanc-0.3.0/setup.py
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2022-11-27 21:12:58.274031 blanc-0.3.0/shannon/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      419 2022-11-27 18:48:19.000000 blanc-0.3.0/shannon/README.md
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)     3541 2022-02-01 01:02:52.000000 blanc-0.3.0/shannon/summeval_score.py
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.224611 blanc-0.3.1/
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.206010 blanc-0.3.1/.github/
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.208242 blanc-0.3.1/.github/workflows/
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)     2532 2022-11-20 20:03:24.000000 blanc-0.3.1/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)       54 2020-04-22 21:28:28.000000 blanc-0.3.1/.gitignore
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1049 2020-04-22 21:28:28.000000 blanc-0.3.1/LICENSE
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)    13913 2023-06-26 23:57:13.224436 blanc-0.3.1/PKG-INFO
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13478 2022-02-10 23:08:14.000000 blanc-0.3.1/README.md
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)     1629 2022-11-20 20:03:24.000000 blanc-0.3.1/SECURITY.md
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.210729 blanc-0.3.1/blanc/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      133 2022-02-10 23:08:14.000000 blanc-0.3.1/blanc/__init__.py
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    12173 2021-09-01 21:24:46.000000 blanc-0.3.1/blanc/__main__.py
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)       22 2023-06-26 23:53:08.000000 blanc-0.3.1/blanc/__version__.py
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    36885 2023-06-26 23:31:35.000000 blanc-0.3.1/blanc/blanc.py
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)    19293 2022-11-27 19:37:04.000000 blanc-0.3.1/blanc/estime.py
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)    11877 2023-06-26 23:53:08.000000 blanc-0.3.1/blanc/shannon.py
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    16178 2021-03-11 01:31:26.000000 blanc-0.3.1/blanc/utils.py
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.211997 blanc-0.3.1/blanc.egg-info/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13913 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/PKG-INFO
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      617 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/SOURCES.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)        1 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/dependency_links.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)       46 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/entry_points.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)       98 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/requires.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)        6 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/top_level.txt
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.223514 blanc-0.3.1/data/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)  2779006 2020-11-22 22:52:16.000000 blanc-0.3.1/data/CNN_DailyMail_555.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1110748 2020-11-22 22:52:16.000000 blanc-0.3.1/data/DailyNews_300.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1257825 2020-11-22 22:52:16.000000 blanc-0.3.1/data/DailyNews_300_aspects.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1361 2021-04-04 18:11:32.000000 blanc-0.3.1/data/README.md
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      506 2020-04-22 21:28:28.000000 blanc-0.3.1/data/doc-summaries.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      363 2020-04-22 21:28:28.000000 blanc-0.3.1/data/pairs.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      149 2020-04-22 21:28:28.000000 blanc-0.3.1/data/single.json
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.223657 blanc-0.3.1/estime/
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)     4053 2023-06-26 23:53:08.000000 blanc-0.3.1/estime/README.md
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)       98 2022-11-21 01:28:17.000000 blanc-0.3.1/requirements.txt
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)       38 2023-06-26 23:57:13.224649 blanc-0.3.1/setup.cfg
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)      948 2023-06-26 23:53:08.000000 blanc-0.3.1/setup.py
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.224135 blanc-0.3.1/shannon/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      419 2022-11-27 18:48:19.000000 blanc-0.3.1/shannon/README.md
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)     3541 2022-02-01 01:02:52.000000 blanc-0.3.1/shannon/summeval_score.py
```

### Comparing `blanc-0.3.0/.github/workflows/codeql-analysis.yml` & `blanc-0.3.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/LICENSE` & `blanc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/PKG-INFO` & `blanc-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blanc
-Version: 0.3.0
+Version: 0.3.1
 Summary: Human-free quality estimation of document summaries
 Home-page: https://github.com/PrimerAI/blanc
 Author: Primer AI
 Author-email: blanc@primer.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `blanc-0.3.0/README.md` & `blanc-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/SECURITY.md` & `blanc-0.3.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/blanc/__main__.py` & `blanc-0.3.1/blanc/__main__.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/blanc/blanc.py` & `blanc-0.3.1/blanc/blanc.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/blanc/estime.py` & `blanc-0.3.1/blanc/estime.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/blanc/shannon.py` & `blanc-0.3.1/blanc/shannon.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     ReformerTokenizer,
     XLMWithLMHeadModel,
     XLMTokenizer,
 )
 import numpy as np
 from nltk import sent_tokenize
 
-def get_model(name, size):
+def get_model(name, size, device='cuda'):
+    if device == 'cuda':
+        device = 'cuda' if torch.cuda.is_available() else 'cpu'
     if name == 'gpt2':
         t = GPT2Tokenizer.from_pretrained('gpt2')
         if size == 'base':
             g = GPT2LMHeadModel.from_pretrained('gpt2')
         else:
             g = GPT2LMHeadModel.from_pretrained(f'gpt2-{size}')
         eos = g.config.eos_token_id # '<|endoftext|>'
@@ -52,51 +54,81 @@
     elif name == 'xlm':
         t = XLMTokenizer.from_pretrained('xlm-clm-ende-1024')
         g = XLMWithLMHeadModel.from_pretrained('xlm-clm-ende-1024')
         g.config.lang_id = g.config.lang2id['en']
         eos = 4 # </s>
         max_input = 1024
 
-    g = g.to('cuda')
+    g = g.to(device)
     g.config.return_dict = False
     g.eval()
     return g, t, eos, max_input
 
+def prepare_inputs_for_generation(input_ids, past=None, **kwargs):
+    """Copied from gpt2 of huggingface transformers, but using it here separately, 
+    because in some versions this funciton worked differently, which caused errors."""
+    if past:  # only last token for inputs_ids if past is defined in kwargs
+        input_ids = input_ids[:, -1].unsqueeze(-1)
+
+    attention_mask = kwargs.get("attention_mask", None)
+    position_ids = kwargs.get("position_ids", None)
+
+    if attention_mask is not None and position_ids is None:
+        # create position_ids on the fly for batch generation
+        position_ids = attention_mask.long().cumsum(-1) - 1
+        position_ids.masked_fill_(attention_mask == 0, 1)
+        if past:
+            position_ids = position_ids[:, -1].unsqueeze(-1)
+    else:
+        position_ids = None
+    return {
+        "input_ids": input_ids,
+        "past_key_values": past,
+        "use_cache": kwargs.get("use_cache"),
+        "position_ids": position_ids,
+        "attention_mask": attention_mask,
+    }
+
 class Shannon:
     def __init__(
         self,
         verbose=False,
         language_model='gpt2',
         model_size='base',
         num_upstream=0,
         return_token_lls=False,
+        device='cuda'
     ):
         self.verbose = verbose
         self.language_model = language_model
         self.num_upstream = num_upstream
         self.return_token_lls = return_token_lls
-        self.g, self.t, self.eos, self.max_input = get_model(language_model, model_size)
+        self.device = device
+        if self.device == 'cuda':
+            self.device = 'cuda' if torch.cuda.is_available() else 'cpu'
+        self.g, self.t, self.eos, self.max_input = get_model(
+            language_model, model_size, self.device)
 
     def measure(self, doc_tokens, prompt):
-        eos = torch.LongTensor([self.eos]).to('cuda')
+        eos = torch.LongTensor([self.eos]).to(self.device)
         if prompt is None or (prompt.dim() == 1 and len(prompt) == 0):
-            prompt = torch.LongTensor([]).to('cuda')
+            prompt = torch.LongTensor([]).to(self.device)
 
         token_lls = []
         success = []
         past = None
         for i, token in enumerate(doc_tokens):
             upstream = doc_tokens[:i]
             if len(upstream) + len(prompt) + 1 > self.max_input:
                 upstream = upstream[-(self.max_input - 1 - len(prompt)):]
                 if past is not None:
                     past = [t[:, :, :, 1:, :] for t in past]
 
             prefix = torch.cat([eos, prompt, upstream]).unsqueeze(0)
-            inputs = self.g.prepare_inputs_for_generation(prefix, past=past, use_cache=True, use_mems=True)
+            inputs = prepare_inputs_for_generation(prefix, past=past, use_cache=True, use_mems=True)
             with torch.no_grad():
                 out = self.g(**inputs)
 
             if self.language_model in 'gpt2':
                 logits, past = out
             elif self.language_model in ['gpt1', 'reformer']:
                 logits, = out
@@ -130,16 +162,16 @@
         sents = sent_tokenize(doc)
         encode_args = {'return_tensors': 'pt'}
         if self.language_model == 'transformerxl':
             encode_args['add_space_before_punct_symbol'] = True
         if self.language_model in ['xlnet', 'xlm']:
             encode_args['add_special_tokens'] = False
 
-        sents_tokens = [self.t.encode(sent, **encode_args).to('cuda').view(-1) for sent in sents]
-        summ_tokens = self.t.encode(summ, **encode_args).to('cuda').view(-1)
+        sents_tokens = [self.t.encode(sent, **encode_args).to(self.device).view(-1) for sent in sents]
+        summ_tokens = self.t.encode(summ, **encode_args).to(self.device).view(-1)
         sents_tokens = [sent_tokens[:self.max_input - 1 - len(summ_tokens)] for sent_tokens in sents_tokens]
         doc_tokens = torch.cat(sents_tokens, dim=-1)
 
         if measure_t:
             ll, tries, success = 0, 0, []
             for sent_tokens in sents_tokens:
                 sent_ll, sent_tries, sent_success = self.measure(sent_tokens, sent_tokens)
@@ -157,15 +189,17 @@
             S = [[0, 0], [0, 0]]
             for sent_idx in range(len(sents_tokens)):
                 sent_tokens = sents_tokens[sent_idx]
                 upstream_tensors = sents_tokens[sent_idx-self.num_upstream:sent_idx]
                 if len(upstream_tensors) > 0:
                     upstream_context = torch.cat(upstream_tensors)
                 else:
-                    upstream_context = torch.LongTensor([]).cuda()
+                    upstream_context = torch.LongTensor([])
+                    if self.device == 'cuda':
+                        upstream_context = upstream_context.cuda()
 
                 base_prompt = upstream_context
                 help_prompt = torch.cat([summ_tokens, upstream_context])
                 full_prompt = torch.cat([upstream_context, sent_tokens, upstream_context])
 
                 base_sent_lls, base_sent_success = self.measure(sent_tokens, base_prompt)
                 help_sent_lls, help_sent_success = self.measure(sent_tokens, help_prompt)
```

### Comparing `blanc-0.3.0/blanc/utils.py` & `blanc-0.3.1/blanc/utils.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/blanc.egg-info/PKG-INFO` & `blanc-0.3.1/blanc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blanc
-Version: 0.3.0
+Version: 0.3.1
 Summary: Human-free quality estimation of document summaries
 Home-page: https://github.com/PrimerAI/blanc
 Author: Primer AI
 Author-email: blanc@primer.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `blanc-0.3.0/blanc.egg-info/SOURCES.txt` & `blanc-0.3.1/blanc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/data/CNN_DailyMail_555.json` & `blanc-0.3.1/data/CNN_DailyMail_555.json`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/data/DailyNews_300.json` & `blanc-0.3.1/data/DailyNews_300.json`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/data/DailyNews_300_aspects.json` & `blanc-0.3.1/data/DailyNews_300_aspects.json`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/data/README.md` & `blanc-0.3.1/data/README.md`

 * *Files identical despite different names*

### Comparing `blanc-0.3.0/estime/README.md` & `blanc-0.3.1/estime/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 ```
 >>> estimator = Estime(output=['alarms', 'soft', 'coherence'])
 >>> estimator.evaluate_claims(text, [summary])
 [[5, 0.502, -0.25]]
 ```
 
-For more options, see comments in the source [estime](https://github.com/PrimerAI/blanc/blob/master/blanc/estime.py).
+For more options, see comments in the source [estime](https://github.com/PrimerAI/blanc/blob/master/blanc/estime.py), or see [estime](https://github.com/PrimerAI/primer-research/tree/main/estime).
 
 The table below is made in the same way as the Table 1 in [ESTIME](https://aclanthology.org/2021.eval4nlp-1.10/), except that the number of systems here is updated from 16 to 17, following the later version of [SummEval](https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00373/100686/SummEval-Re-evaluating-Summarization-Evaluation). This means that the correlations are taken here between arrays of 1700-length (100 texts x 17 summary generation systems).
 
 |model|consistency<br />Spearman|consistency<br />Kendall|relevance<br />Spearman|relevance<br />Kendall|coherence<br />Spearman|coherence<br />Kendall|fluency<br />Spearman|fluency<br />Kendall|
 |:--|--:|--:|--:|--:|--:|--:|--:|--:|
 BLANC-AXXL|0.19|0.09|0.21|0.15|0.11|0.08|0.10|0.06|
 BLANC-BLU|0.20|0.10|0.18|0.13|0.10|0.07|0.11|0.06|
```

### Comparing `blanc-0.3.0/setup.py` & `blanc-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import setuptools
 
-version = "0.3.0"
+version = "0.3.1"
 
 with open("README.md", encoding="utf-8") as reader:
     long_description = reader.read()
 
 with open("requirements.txt") as reader:
     requirements = [line.strip() for line in reader]
```

### Comparing `blanc-0.3.0/shannon/summeval_score.py` & `blanc-0.3.1/shannon/summeval_score.py`

 * *Files identical despite different names*

