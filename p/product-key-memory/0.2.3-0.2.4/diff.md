# Comparing `tmp/product_key_memory-0.2.3.tar.gz` & `tmp/product_key_memory-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "product_key_memory-0.2.3.tar", last modified: Tue Jun 27 18:53:33 2023, max compression
+gzip compressed data, was "product_key_memory-0.2.4.tar", last modified: Tue Jun 27 18:55:55 2023, max compression
```

## Comparing `product_key_memory-0.2.3.tar` & `product_key_memory-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:33.735731 product_key_memory-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-27 18:53:22.000000 product_key_memory-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-27 18:53:33.735731 product_key_memory-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-27 18:53:22.000000 product_key_memory-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:33.731731 product_key_memory-0.2.3/product_key_memory/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-27 18:53:22.000000 product_key_memory-0.2.3/product_key_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-27 18:53:22.000000 product_key_memory-0.2.3/product_key_memory/product_key_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:33.735731 product_key_memory-0.2.3/product_key_memory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-27 18:53:33.000000 product_key_memory-0.2.3/product_key_memory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-27 18:53:33.000000 product_key_memory-0.2.3/product_key_memory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:53:33.000000 product_key_memory-0.2.3/product_key_memory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 18:53:33.000000 product_key_memory-0.2.3/product_key_memory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 18:53:33.000000 product_key_memory-0.2.3/product_key_memory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:53:33.735731 product_key_memory-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-27 18:53:22.000000 product_key_memory-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:55:55.158160 product_key_memory-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-27 18:55:45.000000 product_key_memory-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-27 18:55:55.158160 product_key_memory-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-27 18:55:45.000000 product_key_memory-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:55:55.154160 product_key_memory-0.2.4/product_key_memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-27 18:55:45.000000 product_key_memory-0.2.4/product_key_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-27 18:55:45.000000 product_key_memory-0.2.4/product_key_memory/product_key_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:55:55.158160 product_key_memory-0.2.4/product_key_memory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-27 18:55:55.000000 product_key_memory-0.2.4/product_key_memory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-27 18:55:55.000000 product_key_memory-0.2.4/product_key_memory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:55:55.000000 product_key_memory-0.2.4/product_key_memory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 18:55:55.000000 product_key_memory-0.2.4/product_key_memory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 18:55:55.000000 product_key_memory-0.2.4/product_key_memory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:55:55.158160 product_key_memory-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-27 18:55:45.000000 product_key_memory-0.2.4/setup.py
```

### Comparing `product_key_memory-0.2.3/LICENSE` & `product_key_memory-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.3/PKG-INFO` & `product_key_memory-0.2.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product_key_memory
-Version: 0.2.3
+Version: 0.2.4
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.3/README.md` & `product_key_memory-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.3/product_key_memory/product_key_memory.py` & `product_key_memory-0.2.4/product_key_memory/product_key_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 import torch
 from torch import nn, einsum
 
 from einops import rearrange
 
-from colt5_attention import topk as differentiable_topk
+from colt5_attention import topk as coor_descent_topk
 
 # helper functions
 
 def exists(val):
     return val is not None
 
 def default(val, d):
@@ -143,15 +143,15 @@
         # similarity to keys
 
         dots = einsum('p b t h d, h n p d -> b t h p n', queries, self.keys)
 
         # topk scores
 
         if self.differentiable_topk:
-            scores, indices, *_ = differentiable_topk(dots, k = self.topk)
+            scores, indices, *_ = coor_descent_topk(dots, k = self.topk, fused = True)
         else:
             scores, indices = dots.topk(k = self.topk, dim = -1)
 
         # scores are factorized
 
         (scores_x, scores_y), (indices_x, indices_y) = map(lambda t: t.chunk(2, dim = 3), (scores, indices))
```

### Comparing `product_key_memory-0.2.3/product_key_memory.egg-info/PKG-INFO` & `product_key_memory-0.2.4/product_key_memory.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product-key-memory
-Version: 0.2.3
+Version: 0.2.4
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.3/setup.py` & `product_key_memory-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'product_key_memory',
     packages = find_packages(),
-    version = '0.2.3',
+    version = '0.2.4',
     license = 'MIT',
     description = 'Product Key Memory',
     long_description_content_type = 'text/markdown',
     author = 'Aran Komatsuzaki, Phil Wang',
     author_email = 'aran1234321@gmail.com, lucidrains@gmail.com',
     url = 'https://github.com/lucidrains/product-key-memory',
     keywords = [
```

