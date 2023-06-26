# Comparing `tmp/torch_grammar-0.2.1.tar.gz` & `tmp/torch_grammar-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_grammar-0.2.1.tar", max compression
+gzip compressed data, was "torch_grammar-0.3.0.tar", max compression
```

## Comparing `torch_grammar-0.2.1.tar` & `torch_grammar-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1916 2023-06-20 18:58:30.304068 torch_grammar-0.2.1/README.md
--rw-r--r--   0        0        0      588 2023-06-22 19:36:26.594443 torch_grammar-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.2.1/torch_grammar/__init__.py
--rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.2.1/torch_grammar/grammar_parser.py
--rw-r--r--   0        0        0     6363 2023-06-22 19:33:29.135187 torch_grammar-0.2.1/torch_grammar/grammar_sampler.py
--rw-r--r--   0        0        0     1208 2023-06-19 17:20:35.685343 torch_grammar-0.2.1/torch_grammar/token_trie.py
--rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 torch_grammar-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1946 2023-06-26 22:01:25.065253 torch_grammar-0.3.0/README.md
+-rw-r--r--   0        0        0      588 2023-06-26 22:01:54.186219 torch_grammar-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.3.0/torch_grammar/__init__.py
+-rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.3.0/torch_grammar/grammar_parser.py
+-rw-r--r--   0        0        0     6419 2023-06-26 21:03:33.486520 torch_grammar-0.3.0/torch_grammar/grammar_sampler.py
+-rw-r--r--   0        0        0     1949 2023-06-26 22:00:00.538471 torch_grammar-0.3.0/torch_grammar/token_trie.py
+-rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 torch_grammar-0.3.0/PKG-INFO
```

### Comparing `torch_grammar-0.2.1/README.md` & `torch_grammar-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 with open("examples/grammar.ebnf", "r") as file:
     input_text = file.read()
 grammar = GrammarSampler(input_text, "root", tokenizer)
 
 ids = [[1]]
 logits_processor = grammar.logits_processor()
 
+vocab_size = len(tokenizer.get_vocab())
 for i in range(10):
-  logits = torch.randn((1, tokenizer.vocab_size))
+  logits = torch.randn((1, vocab_size))
   logits = logits_processor(ids, logits)
   token = torch.argmax(logits).item()
   # logits_processor.accept_token(token)
   ids[0].append(token)
 print(f"\x1b[1mfirst 10 tokens: \x1b[1;35m{tokenizer.decode(ids[0])}\x1b[0m")
 ```
```

### Comparing `torch_grammar-0.2.1/torch_grammar/grammar_parser.py` & `torch_grammar-0.3.0/torch_grammar/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.2.1/torch_grammar/grammar_sampler.py` & `torch_grammar-0.3.0/torch_grammar/grammar_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
         return new_stacks
 
     def accept_token(self, token, stacks):
         if token == self.eos_token_id:
             if any(len(stack) == 0 for stack in stacks):
                 return []
-            assert False
+            raise Exception(f"EOS token not accepted with PDA stacks: {stacks}")
 
         for byte in self.token_trie.id2str(token):
             stacks = self.accept(byte, stacks)
             assert stacks != []
 
         return stacks
```

### Comparing `torch_grammar-0.2.1/PKG-INFO` & `torch_grammar-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-grammar
-Version: 0.2.1
+Version: 0.3.0
 Summary: Restrict LLM generations to a context-free grammar
 License: MIT
 Author: Burke Libbey
 Author-email: burke.libbey@shopify.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -35,16 +35,17 @@
 with open("examples/grammar.ebnf", "r") as file:
     input_text = file.read()
 grammar = GrammarSampler(input_text, "root", tokenizer)
 
 ids = [[1]]
 logits_processor = grammar.logits_processor()
 
+vocab_size = len(tokenizer.get_vocab())
 for i in range(10):
-  logits = torch.randn((1, tokenizer.vocab_size))
+  logits = torch.randn((1, vocab_size))
   logits = logits_processor(ids, logits)
   token = torch.argmax(logits).item()
   # logits_processor.accept_token(token)
   ids[0].append(token)
 print(f"\x1b[1mfirst 10 tokens: \x1b[1;35m{tokenizer.decode(ids[0])}\x1b[0m")
 ```
```

