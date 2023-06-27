# Comparing `tmp/langdash-1.5.1b1.tar.gz` & `tmp/langdash-1.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.5.1b1.tar", last modified: Thu Jun 22 20:29:58 2023, max compression
+gzip compressed data, was "langdash-1.6.0b0.tar", last modified: Tue Jun 27 20:26:38 2023, max compression
```

## Comparing `langdash-1.5.1b1.tar` & `langdash-1.6.0b0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:29:58.823359 langdash-1.5.1b1/
--rw-r--r--   0 user      (1000) user      (1000)    10786 2023-06-06 08:29:05.000000 langdash-1.5.1b1/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)       35 2023-06-06 08:29:05.000000 langdash-1.5.1b1/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     3726 2023-06-22 20:29:58.823359 langdash-1.5.1b1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2788 2023-06-22 20:23:51.000000 langdash-1.5.1b1/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:29:58.820026 langdash-1.5.1b1/langdash/
--rw-r--r--   0 user      (1000) user      (1000)       78 2023-06-22 20:29:19.000000 langdash-1.5.1b1/langdash/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:29:58.820026 langdash-1.5.1b1/langdash/chains/
--rw-r--r--   0 user      (1000) user      (1000)      178 2023-06-11 00:29:26.000000 langdash-1.5.1b1/langdash/chains/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    14686 2023-06-12 17:23:06.000000 langdash-1.5.1b1/langdash/chains/chains.py
--rw-r--r--   0 user      (1000) user      (1000)     9520 2023-06-15 22:53:06.000000 langdash-1.5.1b1/langdash/chains/nodes.py
--rw-r--r--   0 user      (1000) user      (1000)      253 2023-06-11 01:18:11.000000 langdash-1.5.1b1/langdash/chains/typing.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:29:58.820026 langdash-1.5.1b1/langdash/classify/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-06 08:44:18.000000 langdash-1.5.1b1/langdash/classify/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2032 2023-06-12 17:25:45.000000 langdash-1.5.1b1/langdash/classify/token_qa.py
--rw-r--r--   0 user      (1000) user      (1000)     6625 2023-06-15 18:51:05.000000 langdash-1.5.1b1/langdash/core.py
--rw-r--r--   0 user      (1000) user      (1000)     1321 2023-06-15 23:04:37.000000 langdash-1.5.1b1/langdash/infer.py
--rw-r--r--   0 user      (1000) user      (1000)     1555 2023-06-07 00:55:46.000000 langdash-1.5.1b1/langdash/llm.py
--rw-r--r--   0 user      (1000) user      (1000)     7473 2023-06-22 00:05:04.000000 langdash-1.5.1b1/langdash/llm_session.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:29:58.820026 langdash-1.5.1b1/langdash/models/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-13 06:46:41.000000 langdash-1.5.1b1/langdash/models/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:29:58.820026 langdash-1.5.1b1/langdash/models/_mixins/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-13 06:51:30.000000 langdash-1.5.1b1/langdash/models/_mixins/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3412 2023-06-20 01:17:39.000000 langdash-1.5.1b1/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:29:58.823359 langdash-1.5.1b1/langdash/models/_tokenizer/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-13 06:51:39.000000 langdash-1.5.1b1/langdash/models/_tokenizer/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1886 2023-06-13 06:51:21.000000 langdash-1.5.1b1/langdash/models/_tokenizer/_bpe.py
--rw-r--r--   0 user      (1000) user      (1000)     1532 2023-06-13 06:51:21.000000 langdash-1.5.1b1/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-r--r--   0 user      (1000) user      (1000)     2269 2023-06-20 00:04:11.000000 langdash-1.5.1b1/langdash/models/_tokenizer/hf_tokenizer.py
--rw-r--r--   0 user      (1000) user      (1000)     1546 2023-06-21 19:49:14.000000 langdash-1.5.1b1/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-r--r--   0 user      (1000) user      (1000)      664 2023-06-13 06:51:21.000000 langdash-1.5.1b1/langdash/models/_tokenizer/tokenizer.py
--rw-r--r--   0 user      (1000) user      (1000)     5084 2023-06-20 01:34:02.000000 langdash-1.5.1b1/langdash/models/ctransformers.py
--rw-r--r--   0 user      (1000) user      (1000)     4744 2023-06-13 06:51:21.000000 langdash-1.5.1b1/langdash/models/llama_cpp.py
--rw-r--r--   0 user      (1000) user      (1000)      689 2023-06-13 06:46:41.000000 langdash-1.5.1b1/langdash/models/mock.py
--rw-r--r--   0 user      (1000) user      (1000)     9027 2023-06-22 00:08:52.000000 langdash-1.5.1b1/langdash/models/rwkv_cpp.py
--rw-r--r--   0 user      (1000) user      (1000)     1005 2023-06-13 06:46:41.000000 langdash-1.5.1b1/langdash/models/sentence_transformers.py
--rw-r--r--   0 user      (1000) user      (1000)     5472 2023-06-13 06:51:21.000000 langdash-1.5.1b1/langdash/models/transformers.py
--rw-r--r--   0 user      (1000) user      (1000)      837 2023-06-07 00:55:46.000000 langdash-1.5.1b1/langdash/response.py
--rw-r--r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:38:13.000000 langdash-1.5.1b1/langdash/sampling.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:29:58.823359 langdash-1.5.1b1/langdash/search/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-06 08:44:18.000000 langdash-1.5.1b1/langdash/search/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1135 2023-06-12 17:46:13.000000 langdash-1.5.1b1/langdash/search/embedding_search.py
--rw-r--r--   0 user      (1000) user      (1000)     1118 2023-06-09 17:53:33.000000 langdash-1.5.1b1/langdash/search/engine.py
--rw-r--r--   0 user      (1000) user      (1000)     2861 2023-06-15 19:40:11.000000 langdash-1.5.1b1/langdash/search/multichoice_search.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-22 20:29:58.820026 langdash-1.5.1b1/langdash.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3726 2023-06-22 20:29:58.000000 langdash-1.5.1b1/langdash.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1188 2023-06-22 20:29:58.000000 langdash-1.5.1b1/langdash.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-22 20:29:58.000000 langdash-1.5.1b1/langdash.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      199 2023-06-22 20:29:58.000000 langdash-1.5.1b1/langdash.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        9 2023-06-22 20:29:58.000000 langdash-1.5.1b1/langdash.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-22 20:29:58.823359 langdash-1.5.1b1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1604 2023-06-22 20:29:50.000000 langdash-1.5.1b1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:26:38.106726 langdash-1.6.0b0/
+-rw-r--r--   0 user      (1000) user      (1000)    10786 2023-06-06 08:29:05.000000 langdash-1.6.0b0/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)       35 2023-06-06 08:29:05.000000 langdash-1.6.0b0/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3726 2023-06-27 20:26:38.106726 langdash-1.6.0b0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2788 2023-06-22 20:30:22.000000 langdash-1.6.0b0/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:26:38.103393 langdash-1.6.0b0/langdash/
+-rw-r--r--   0 user      (1000) user      (1000)       78 2023-06-27 20:25:25.000000 langdash-1.6.0b0/langdash/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:26:38.106726 langdash-1.6.0b0/langdash/chains/
+-rw-r--r--   0 user      (1000) user      (1000)      177 2023-06-27 19:02:29.000000 langdash-1.6.0b0/langdash/chains/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    14993 2023-06-27 20:04:56.000000 langdash-1.6.0b0/langdash/chains/chains.py
+-rw-r--r--   0 user      (1000) user      (1000)     9520 2023-06-22 20:30:16.000000 langdash-1.6.0b0/langdash/chains/nodes.py
+-rw-r--r--   0 user      (1000) user      (1000)      253 2023-06-11 01:18:11.000000 langdash-1.6.0b0/langdash/chains/typing.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:26:38.106726 langdash-1.6.0b0/langdash/classify/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-06 08:44:18.000000 langdash-1.6.0b0/langdash/classify/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2032 2023-06-12 17:25:45.000000 langdash-1.6.0b0/langdash/classify/token_qa.py
+-rw-r--r--   0 user      (1000) user      (1000)     6625 2023-06-22 20:30:16.000000 langdash-1.6.0b0/langdash/core.py
+-rw-r--r--   0 user      (1000) user      (1000)     1321 2023-06-22 20:30:16.000000 langdash-1.6.0b0/langdash/infer.py
+-rw-r--r--   0 user      (1000) user      (1000)     1555 2023-06-07 00:55:46.000000 langdash-1.6.0b0/langdash/llm.py
+-rw-r--r--   0 user      (1000) user      (1000)     8853 2023-06-27 19:06:16.000000 langdash-1.6.0b0/langdash/llm_session.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:26:38.106726 langdash-1.6.0b0/langdash/models/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-13 06:46:41.000000 langdash-1.6.0b0/langdash/models/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:26:38.106726 langdash-1.6.0b0/langdash/models/_mixins/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-13 06:51:30.000000 langdash-1.6.0b0/langdash/models/_mixins/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3412 2023-06-22 20:30:16.000000 langdash-1.6.0b0/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:26:38.106726 langdash-1.6.0b0/langdash/models/_tokenizer/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-13 06:51:39.000000 langdash-1.6.0b0/langdash/models/_tokenizer/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1886 2023-06-13 06:51:21.000000 langdash-1.6.0b0/langdash/models/_tokenizer/_bpe.py
+-rw-r--r--   0 user      (1000) user      (1000)     1532 2023-06-13 06:51:21.000000 langdash-1.6.0b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-r--r--   0 user      (1000) user      (1000)     2269 2023-06-22 20:30:16.000000 langdash-1.6.0b0/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-r--r--   0 user      (1000) user      (1000)     1546 2023-06-22 20:30:16.000000 langdash-1.6.0b0/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-r--r--   0 user      (1000) user      (1000)      664 2023-06-13 06:51:21.000000 langdash-1.6.0b0/langdash/models/_tokenizer/tokenizer.py
+-rw-r--r--   0 user      (1000) user      (1000)     5280 2023-06-27 19:02:29.000000 langdash-1.6.0b0/langdash/models/ctransformers.py
+-rw-r--r--   0 user      (1000) user      (1000)     4932 2023-06-27 19:02:29.000000 langdash-1.6.0b0/langdash/models/llama_cpp.py
+-rw-r--r--   0 user      (1000) user      (1000)      689 2023-06-13 06:46:41.000000 langdash-1.6.0b0/langdash/models/mock.py
+-rw-r--r--   0 user      (1000) user      (1000)     8993 2023-06-27 19:05:22.000000 langdash-1.6.0b0/langdash/models/rwkv_cpp.py
+-rw-r--r--   0 user      (1000) user      (1000)     1005 2023-06-13 06:46:41.000000 langdash-1.6.0b0/langdash/models/sentence_transformers.py
+-rw-r--r--   0 user      (1000) user      (1000)     5632 2023-06-27 19:02:29.000000 langdash-1.6.0b0/langdash/models/transformers.py
+-rw-r--r--   0 user      (1000) user      (1000)      837 2023-06-07 00:55:46.000000 langdash-1.6.0b0/langdash/response.py
+-rw-r--r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:38:13.000000 langdash-1.6.0b0/langdash/sampling.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:26:38.106726 langdash-1.6.0b0/langdash/search/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-06-06 08:44:18.000000 langdash-1.6.0b0/langdash/search/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1135 2023-06-12 17:46:13.000000 langdash-1.6.0b0/langdash/search/embedding_search.py
+-rw-r--r--   0 user      (1000) user      (1000)     1118 2023-06-09 17:53:33.000000 langdash-1.6.0b0/langdash/search/engine.py
+-rw-r--r--   0 user      (1000) user      (1000)     2861 2023-06-22 20:30:16.000000 langdash-1.6.0b0/langdash/search/multichoice_search.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-27 20:26:38.106726 langdash-1.6.0b0/langdash.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3726 2023-06-27 20:26:38.000000 langdash-1.6.0b0/langdash.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1188 2023-06-27 20:26:38.000000 langdash-1.6.0b0/langdash.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-27 20:26:38.000000 langdash-1.6.0b0/langdash.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      199 2023-06-27 20:26:38.000000 langdash-1.6.0b0/langdash.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        9 2023-06-27 20:26:38.000000 langdash-1.6.0b0/langdash.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-27 20:26:38.106726 langdash-1.6.0b0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1604 2023-06-22 20:30:45.000000 langdash-1.6.0b0/setup.py
```

### Comparing `langdash-1.5.1b1/LICENSE.txt` & `langdash-1.6.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/PKG-INFO` & `langdash-1.6.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.5.1b1
+Version: 1.6.0b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.5.1b1/README.md` & `langdash-1.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/chains/chains.py` & `langdash-1.6.0b0/langdash/chains/chains.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from collections import OrderedDict
-from typing import Generator, Dict, Any, List, Union, Optional, Tuple, FrozenSet, TYPE_CHECKING, cast
+from typing import Generator, Dict, Any, List, Union, Optional, Tuple, FrozenSet, Set, TYPE_CHECKING, cast
 import re
 import copy
 import warnings
 
 from langdash.response import Response, RespInfer, RespInject, RespReturns
 from .nodes import LDNode, LDText, LDFormatArg, LDArg, LDReturns, LDChoice, LDRepeat
 from .typing import Type, TypeDict
@@ -19,15 +19,15 @@
 
 LDNodeGenerator = Generator[Response, None, None]
 LDNodeArgs = Dict[str, Any]
 LDNodeArgsFrozen = FrozenSet[Tuple[str, Any]]
 
 
 @dataclass(frozen=True)
-class CalledChain:
+class CalledNode:
   """
   Data class used to store info about nodes previously called.
   
   Attributes:
     node: Node object
     args: Arguments passed to the node (for LDFormatArg)
     tokens_used: Number of tokens the node used (either number of tokens injected, or generated)
@@ -133,17 +133,17 @@
     # filter
     pp_nodes = [node for node in pp_nodes if node is not None]
 
     return cast(List[LDNode], pp_nodes)
 
   def _node_pass(self, session: "LLMGenerationSession", args: LDNodeArgs):
     for node in self._nodes:
-      session.tokens_counter = 0
+      session._tokens_counter = 0
       yield node
-      session._append_called_chain(node, args, session.tokens_counter)
+      session._append_called_chain(node, args, session._tokens_counter)
 
   def _load_session(
     self, ctx: Union[str, "LLMGenerationSession"]
   ) -> "LLMGenerationSession":
     from langdash.llm_session import LLMGenerationSession
     if isinstance(ctx, LLMGenerationSession):
       return cast(LLMGenerationSession, ctx)
@@ -261,14 +261,16 @@
   _dict: _LDChainCacheStoreDict
   _model: str
   _model_kwargs: dict
 
 
 class LDChainCached(LDChain):
 
+  arguments_to_cache: Optional[Set[str]]
+
   def __init__(self, model: str, model_kwargs: dict, **kwargs):
     for k, v in kwargs.items():
       setattr(self, k, v)
 
     self._model = model
     self._model_kwargs = model_kwargs
 
@@ -289,21 +291,23 @@
         _arg_first_used_at[k] = self._any_arg_first_use
 
     self._arg_first_used_at: Dict[str, int] = _arg_first_used_at
     self._arg_first_used_at_ordered: List[str] = list(
       _arg_first_used_at.keys()
     )
     self._arg_first_used_at_ordered.sort(key=lambda k: _arg_first_used_at[k])
+    self.arguments_to_cache = None
 
     # cache session per argument use
     self._state_cache: _LDChainCacheStoreDict = OrderedDict()
     if len(self._args) == 0:
       self.max_states_to_cache = 1
     else:
       self.max_states_to_cache = min(len(self._args) + 2, 8)
+
     self._skip_nodes = 0
 
   # State cache functions
 
   def load_cache_store(self, cache_store: LDChainCacheStore):
     """
     Loads the cache store from previous inference time.
@@ -355,44 +359,51 @@
 
   # Inference functions
 
   def _node_pass(self, session: "LLMGenerationSession", args: LDNodeArgs):
     last_state_key: Optional[_LDChainCacheState] = None
     for i in range(self._skip_nodes, len(self._nodes)):
       node = self._nodes[i]
-      session.tokens_counter = 0
+      session._tokens_counter = 0
       yield node
       if isinstance(node, LDText) and last_state_key is not None:
         last_state_key.state = session.clone_state()
         last_state_key.skip_nodes = (i + 1)
       elif isinstance(node, LDArg) and self.max_states_to_cache > 0:
-        # TODO: there might be a faster way of doing this
-        # if the frozenset from _arg_subset_sorted_by_idx is used
+        if self.arguments_to_cache is not None and node._arg not in self.arguments_to_cache:
+          last_state_key = None
+          continue
+
+        # Do not update the cache if argument is injected the second time
         cached_idx = self._arg_first_used_at[node._arg]
         if i > cached_idx:
           last_state_key = None
           continue
+
+        # TODO: there might be a faster way of doing this
+        # if the frozenset from _arg_subset_sorted_by_idx is used
         current_keys = frozenset(
           (k, v)
           for k, v in args.items()
           if self._arg_first_used_at[k] <= cached_idx
         )
+
         if current_keys not in self._state_cache:
           self._set_state_cache(
             current_keys,
             _LDChainCacheState(
               state=session.clone_state(), skip_nodes=(cached_idx + 1)
             )
           )
         else:
           self._update_state_cache(current_keys)
         last_state_key = self._state_cache[current_keys]
       else:
         last_state_key = None
-      session._append_called_chain(node, args, session.tokens_counter)
+      session._append_called_chain(node, args, session._tokens_counter)
 
   def _create_new_session(self) -> "LLMGenerationSession":
     ctx = self._ld.session_for_model(self._model, **self._model_kwargs)
     from langdash.llm_session import LLMGenerationSession
     assert isinstance(
       ctx, LLMGenerationSession
     ), "context must be LLMGenerationSession"
```

### Comparing `langdash-1.5.1b1/langdash/chains/nodes.py` & `langdash-1.6.0b0/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/classify/token_qa.py` & `langdash-1.6.0b0/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/core.py` & `langdash-1.6.0b0/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/infer.py` & `langdash-1.6.0b0/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/llm.py` & `langdash-1.6.0b0/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/llm_session.py` & `langdash-1.6.0b0/langdash/llm_session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypeVar, Generic, Optional, List, Generator, Union, Tuple, TYPE_CHECKING
 import copy
 
 from langdash.response import RespInfer
-from langdash.chains import CalledChain, LDNodeArgs, LDNode
+from langdash.chains import CalledNode, LDNodeArgs, LDNode
 from langdash.infer import InferArgs
 from langdash.llm import LLM
 
 if TYPE_CHECKING:
   from langdash.core import Langdash
 
 T_LLM = TypeVar("T_LLM", bound=LLM)
@@ -34,33 +34,67 @@
   """
   pass
 
 
 T_LLMState = TypeVar("T_LLMState", bound=LLMState)
 
 
+class LLMGenerationSessionEvents:
+
+  def on_before_node_append(
+    self, node: LDNode, args: LDNodeArgs, tokens_used: int,
+    session: "LLMGenerationSession"
+  ) -> Optional[bool]:
+    """
+    Event handler which fires after the node is run, but before node is appended to list of called nodes.
+    
+    Args:
+      node (LDNode): The node being added
+      args (LDNodeArgs): The arguments of the node
+      tokens_used (int): Number of tokens the node used
+      session (LLMGenerationSession): The current session
+    
+    Returns:
+      None or True if node should be appended, otherwise False if node should not be appended.
+    """
+    return None
+
+
 class LLMGenerationSession(LLMSession, Generic[T_LLM, T_LLMState]):
   """ Generation session for a language model. """
 
+  default_infer_args: InferArgs
+  """ Default inference arguments. """
+  called_nodes: Optional[List[CalledNode]]
+  """
+  List of called nodes.
+  If track_called_nodes is set to False in constructor, then this will be None.
+  """
+
+  # Event handlers
+  event_handlers: Optional[LLMGenerationSessionEvents]
+
   def __init__(
     self,
     llm: T_LLM,
     ld: "Langdash",
     default_infer_args: InferArgs = InferArgs(),
-    track_called_chains: bool = False,
+    track_called_nodes: bool = False,
     token_healing: bool = True,
-    global_args: LDNodeArgs = {}
+    global_args: LDNodeArgs = {},
+    event_handlers: Optional[LLMGenerationSessionEvents] = None,
   ):
     super().__init__(llm, ld)
     self.default_infer_args = default_infer_args
-    self.called_chains: Optional[List[CalledChain]
-                                ] = ([] if track_called_chains else None)
+    self.called_nodes = ([] if track_called_nodes else None)
     self.token_healing = token_healing
     self.global_args = global_args
-    self.tokens_counter = 0
+    self._tokens_counter = 0
+    self.tokens_used = 0
+    self.event_handlers = event_handlers
 
   def set_state(self, state: Optional[T_LLMState]):
     """
     Set the state of the language model.
 
     Args:
       state (Optional[T_LLMState]):
@@ -75,32 +109,36 @@
     raise NotImplementedError("clone_state")
 
   def clone(self) -> "LLMGenerationSession":
     session = self.__class__(
       llm=self._llm,
       ld=self._ld,
       default_infer_args=self.default_infer_args,
-      track_called_chains=False,
+      track_called_nodes=False,
       token_healing=self.token_healing,
       global_args=copy.copy(self.global_args)
     )
     session.set_state(self.clone_state())
-    if self.called_chains is not None:
-      session.called_chains = copy.copy(self.called_chains)
+    if self.called_nodes is not None:
+      session.called_nodes = copy.copy(self.called_nodes)
     return session
 
   def _append_called_chain(
     self, node: LDNode, args: LDNodeArgs, tokens_used: int
   ):
-    if self.called_chains is None:
-      pass
-    else:
-      self.called_chains.append(
-        CalledChain(node=node, args=args, tokens_used=tokens_used)
+    if self.event_handlers is not None:
+      if self.event_handlers.on_before_node_append(
+        node, args, tokens_used, self
+      ) is False:
+        return
+    if self.called_nodes is not None:
+      self.called_nodes.append(
+        CalledNode(node=node, args=args, tokens_used=tokens_used)
       )
+    self.tokens_used += tokens_used
 
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
     """
     Tokenize the given text into a list of tokens.
 
     Args:
       text (str): The text to tokenize.
@@ -157,18 +195,26 @@
       Inference response
     """
     if not args:
       args = self.default_infer_args
     yield from self._infer(end=end, args=args, end_is_token=end_is_token)
 
   def inject(
-    self, text: Union[str, int, List[int]], add_special_tokens: bool = False
+    self,
+    text: Union[str, int, List[int]],
+    add_special_tokens: bool = False
   ) -> int:
     raise NotImplementedError("inject")
 
+  def get_context_length(self) -> int:
+    """
+    Returns the context length of the model, or zero for models that don't support one.
+    """
+    return 0
+
 
 T_Tensor = TypeVar("T_Tensor")
 
 
 class LLMGenerationSessionForRawText(
   LLMGenerationSession, Generic[T_LLM, T_LLMState, T_Tensor]
 ):
@@ -206,22 +252,24 @@
   def next_token_probs(self, *args, **kwargs) -> List[float]:
     raise NotImplementedError("next_token_probs")
 
   def _on_first_inject(self):
     return
 
   def inject(
-    self, text: Union[str, int, List[int]], add_special_tokens: bool = False
+    self,
+    text: Union[str, int, List[int]],
+    add_special_tokens: bool = False
   ) -> int:
     if isinstance(text, str):
       tokens = self.tokenize(text, add_special_tokens=add_special_tokens)
     elif isinstance(text, int):
       tokens = [text]
     else:
-      assert(isinstance(text, list))
+      assert (isinstance(text, list))
       tokens = text
     if not tokens:
       return 0
 
     if self._logits is None:
       self._on_first_inject()
```

### Comparing `langdash-1.5.1b1/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.6.0b0/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/models/_tokenizer/_bpe.py` & `langdash-1.6.0b0/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.6.0b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.6.0b0/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.6.0b0/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.6.0b0/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/models/ctransformers.py` & `langdash-1.6.0b0/langdash/models/ctransformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,18 @@
     self, session: "CTransformersSession", state: Optional[CTransformersState]
   ):
     self.enter_session(session)
     self.model.reset()
     if state is not None:
       self.model.set_state(state)
 
+  def get_context_length(self) -> int:
+    # self.enter_session(self)
+    return self.model.context_length
+
 
 class CTransformersSession(
   TensorBasedInferWithSessionMixin,
   LLMGenerationSessionForRawText["CTransformersModel", CTransformersState,
                                  torch.Tensor]
 ):
   """
@@ -134,14 +138,17 @@
       self._logits = None
     else:
       self._logits = self._model.load_logits_from_model()
 
   def clone_state(self) -> CTransformersState:
     return self._model.clone_state(self)
 
+  def get_context_length(self) -> int:
+    return self._model.get_context_length(self)
+
   # Wrapper for public functions to flush the old session states
 
   def inject(self, *a, **k):
     self._model.enter_session(self)
     return LLMGenerationSessionForRawText.inject(self, *a, **k)
 
   def flush_token(self, *a, **k):
```

### Comparing `langdash-1.5.1b1/langdash/models/llama_cpp.py` & `langdash-1.6.0b0/langdash/models/llama_cpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 
   def set_state(self, session: "LlamaCppSession", state: Optional[LlamaState]):
     self.enter_session(session)
     self.model.reset()
     if state is not None:
       self.model.load_state(state)
 
+  def get_context_length(self) -> int:
+    # self.enter_session(self)
+    return self.model.n_ctx()
+
 
 class LlamaCppSession(
   TensorBasedInferWithSessionMixin,
   LLMGenerationSessionForRawText["LlamaCppModel", LlamaState, torch.Tensor]
 ):
   """
   Session for llama.cpp model.
@@ -124,14 +128,17 @@
   def decode(self, tokens: List[int]) -> str:
     return self._model.tokenizer.decode(tokens)
 
   def _on_first_inject(self):
     self._model.model.reset()
     self._eval(self._model.bos_token)
 
+  def get_context_length(self) -> int:
+    return self.model.get_context_length(self)
+
   # Wrapper for public functions to flush the old session states
 
   def inject(self, *a, **k):
     self._model.enter_session(self)
     return LLMGenerationSessionForRawText.inject(self, *a, **k)
 
   def flush_token(self, *a, **k):
```

### Comparing `langdash-1.5.1b1/langdash/models/mock.py` & `langdash-1.6.0b0/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/models/rwkv_cpp.py` & `langdash-1.6.0b0/langdash/models/rwkv_cpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     os.path.dirname(langdash.__file__), "extern/rwkv.cpp"
   )
 
   force_recompile = RWKV_CPP_FORCE_RECOMPILE
 
   git = shutil.which("git")
 
-  if not os.path.isdir(os.path.join(_rwkv_cpp_folder, ".git")):
+  if not os.path.isdir(_rwkv_cpp_folder):
     print("rwkv.cpp isn't installed, clone and install? (requires git, cmake)")
     do_install = input("Type 'y' (without quotes) to install: ") == "y"
     if not do_install:
       raise ImportError("rwkv.cpp is not installed")
     if git is None:
       raise ImportError("git is needed for compiling rwkv.cpp")
 
@@ -150,18 +150,15 @@
     self.eos_token = 0
 
   def eval(self, tokid: int, state: torch.Tensor,
            logits_out: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
     return self.model.eval(tokid, state, state, logits_out)
 
   def eval_mult(
-    self,
-    tokens: List[int],
-    state: torch.Tensor,
-    logits_out: torch.Tensor
+    self, tokens: List[int], state: torch.Tensor, logits_out: torch.Tensor
   ) -> Tuple[torch.Tensor, torch.Tensor]:
     if self.do_eval_sequence:
       batch_size = self.batch_size
       for i in range(0, len(tokens), batch_size):
         logits_out, state = self.model.eval_sequence(
           tokens[i:i + batch_size], state, state, logits_out
         )
```

### Comparing `langdash-1.5.1b1/langdash/models/sentence_transformers.py` & `langdash-1.6.0b0/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/models/transformers.py` & `langdash-1.6.0b0/langdash/models/transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,17 @@
       hf_tokenizer = llm._tokenizer
     self.tokenizer = HFTokenizer(hf_tokenizer)
     self.eos_token = hf_tokenizer.eos_token_id
 
   def forward(self, *a, **k):
     return self.model.forward(*a, **k)
 
+  def get_context_length(self) -> int:
+    return self.model.context_length
+
 
 class TransformersSession(
   TensorBasedInferMixin,
   LLMGenerationSessionForRawText["TransformersModel", TransformersState,
                                  torch.Tensor]
 ):
   """
@@ -147,14 +150,17 @@
 
   def next_token_logits(self) -> List[float]:
     return self._next_token_logits_raw().tolist()
 
   def next_token_probs(self) -> List[float]:
     return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
+  def get_context_length(self) -> int:
+    return self.model.get_context_length()
+
 
 class TransformersModel(LLM[TransformersSession]):
   """
   transformers model.
   """
   Session = TransformersSession
```

### Comparing `langdash-1.5.1b1/langdash/response.py` & `langdash-1.6.0b0/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/sampling.py` & `langdash-1.6.0b0/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/search/embedding_search.py` & `langdash-1.6.0b0/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/search/engine.py` & `langdash-1.6.0b0/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash/search/multichoice_search.py` & `langdash-1.6.0b0/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/langdash.egg-info/PKG-INFO` & `langdash-1.6.0b0/langdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.5.1b1
+Version: 1.6.0b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.5.1b1/langdash.egg-info/SOURCES.txt` & `langdash-1.6.0b0/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.5.1b1/setup.py` & `langdash-1.6.0b0/setup.py`

 * *Files identical despite different names*

