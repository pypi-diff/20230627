# Comparing `tmp/product_key_memory-0.2.2.tar.gz` & `tmp/product_key_memory-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "product_key_memory-0.2.2.tar", last modified: Mon Jun 26 20:44:53 2023, max compression
+gzip compressed data, was "product_key_memory-0.2.3.tar", last modified: Tue Jun 27 18:53:33 2023, max compression
```

## Comparing `product_key_memory-0.2.2.tar` & `product_key_memory-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:44:53.793591 product_key_memory-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 20:44:43.000000 product_key_memory-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 20:44:53.793591 product_key_memory-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-26 20:44:43.000000 product_key_memory-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:44:53.793591 product_key_memory-0.2.2/product_key_memory/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 20:44:43.000000 product_key_memory-0.2.2/product_key_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-26 20:44:43.000000 product_key_memory-0.2.2/product_key_memory/product_key_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:44:53.793591 product_key_memory-0.2.2/product_key_memory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 20:44:53.000000 product_key_memory-0.2.2/product_key_memory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 20:44:53.000000 product_key_memory-0.2.2/product_key_memory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:44:53.000000 product_key_memory-0.2.2/product_key_memory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 20:44:53.000000 product_key_memory-0.2.2/product_key_memory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 20:44:53.000000 product_key_memory-0.2.2/product_key_memory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:44:53.793591 product_key_memory-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-26 20:44:43.000000 product_key_memory-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:33.735731 product_key_memory-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-27 18:53:22.000000 product_key_memory-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-27 18:53:33.735731 product_key_memory-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-27 18:53:22.000000 product_key_memory-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:33.731731 product_key_memory-0.2.3/product_key_memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-27 18:53:22.000000 product_key_memory-0.2.3/product_key_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-27 18:53:22.000000 product_key_memory-0.2.3/product_key_memory/product_key_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:33.735731 product_key_memory-0.2.3/product_key_memory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-27 18:53:33.000000 product_key_memory-0.2.3/product_key_memory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-27 18:53:33.000000 product_key_memory-0.2.3/product_key_memory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:53:33.000000 product_key_memory-0.2.3/product_key_memory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 18:53:33.000000 product_key_memory-0.2.3/product_key_memory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 18:53:33.000000 product_key_memory-0.2.3/product_key_memory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:53:33.735731 product_key_memory-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-27 18:53:22.000000 product_key_memory-0.2.3/setup.py
```

### Comparing `product_key_memory-0.2.2/LICENSE` & `product_key_memory-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.2/PKG-INFO` & `product_key_memory-0.2.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product_key_memory
-Version: 0.2.2
+Version: 0.2.3
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.2/README.md` & `product_key_memory-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.2/product_key_memory/product_key_memory.py` & `product_key_memory-0.2.3/product_key_memory/product_key_memory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import math
 import torch
 from torch import nn, einsum
 
 from einops import rearrange
 
+from colt5_attention import topk as differentiable_topk
+
 # helper functions
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
@@ -70,15 +72,15 @@
         dim_head = 128,
         input_dropout = 0.,
         query_dropout = 0.,
         value_dropout = 0.,
         attn_dropout = 0.,
         use_layernorm = True,
         pre_layernorm = False,
-
+        differentiable_topk = False
     ):
         super().__init__()
         self.topk = topk
         self.heads = heads
         self.num_keys = num_keys
 
         dim_query = dim_head * heads * 2
@@ -103,14 +105,18 @@
         init_(self.values.weight)
 
         self.input_dropout = nn.Dropout(input_dropout)
         self.query_dropout = nn.Dropout(query_dropout)
         self.value_dropout = nn.Dropout(value_dropout)
         self.attn_dropout = nn.Dropout(attn_dropout)
 
+        # use a differentiable topk, based on coordinate descent
+
+        self.differentiable_topk = differentiable_topk
+
     def forward(
         self,
         x,
         input_mask = None,
         **kwargs
     ):
         b, t, h = *x.shape[:2], self.heads
@@ -136,15 +142,20 @@
 
         # similarity to keys
 
         dots = einsum('p b t h d, h n p d -> b t h p n', queries, self.keys)
 
         # topk scores
 
-        scores, indices = dots.topk(k = self.topk, dim = -1)
+        if self.differentiable_topk:
+            scores, indices, *_ = differentiable_topk(dots, k = self.topk)
+        else:
+            scores, indices = dots.topk(k = self.topk, dim = -1)
+
+        # scores are factorized
 
         (scores_x, scores_y), (indices_x, indices_y) = map(lambda t: t.chunk(2, dim = 3), (scores, indices))
 
         all_topk = self.topk ** 2
 
         all_scores = rearrange((
             rearrange(scores_x, '... k -> ... k 1') +
```

### Comparing `product_key_memory-0.2.2/product_key_memory.egg-info/PKG-INFO` & `product_key_memory-0.2.3/product_key_memory.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product-key-memory
-Version: 0.2.2
+Version: 0.2.3
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

