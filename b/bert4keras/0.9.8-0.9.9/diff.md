# Comparing `tmp/bert4keras-0.9.8.tar.gz` & `tmp/bert4keras-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bert4keras-0.9.8.tar", last modified: Tue Jan 12 06:39:19 2021, max compression
+gzip compressed data, was "dist/bert4keras-0.9.9.tar", last modified: Sat Jan 30 03:26:36 2021, max compression
```

## Comparing `bert4keras-0.9.8.tar` & `bert4keras-0.9.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2021-01-12 06:39:19.000000 bert4keras-0.9.8/
--rw-rw-r--   0 you       (1000) you       (1000)       38 2021-01-12 06:39:19.000000 bert4keras-0.9.8/setup.cfg
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2021-01-12 06:39:19.000000 bert4keras-0.9.8/bert4keras/
--rw-rw-r--   0 you       (1000) you       (1000)    80089 2021-01-12 06:31:38.000000 bert4keras-0.9.8/bert4keras/models.py
--rw-rw-r--   0 you       (1000) you       (1000)       48 2021-01-12 06:31:38.000000 bert4keras-0.9.8/bert4keras/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)    15763 2021-01-12 06:31:38.000000 bert4keras-0.9.8/bert4keras/tokenizers.py
--rw-rw-r--   0 you       (1000) you       (1000)     9520 2021-01-12 06:31:38.000000 bert4keras-0.9.8/bert4keras/backend.py
--rw-rw-r--   0 you       (1000) you       (1000)    42285 2021-01-12 06:31:38.000000 bert4keras-0.9.8/bert4keras/optimizers.py
--rw-rw-r--   0 you       (1000) you       (1000)    25594 2021-01-12 06:31:38.000000 bert4keras-0.9.8/bert4keras/snippets.py
--rw-rw-r--   0 you       (1000) you       (1000)    42655 2021-01-12 06:31:38.000000 bert4keras-0.9.8/bert4keras/layers.py
--rw-rw-r--   0 you       (1000) you       (1000)    13849 2021-01-12 06:31:38.000000 bert4keras-0.9.8/README.md
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2021-01-12 06:39:19.000000 bert4keras-0.9.8/bert4keras.egg-info/
--rw-rw-r--   0 you       (1000) you       (1000)      347 2021-01-12 06:39:19.000000 bert4keras-0.9.8/bert4keras.egg-info/SOURCES.txt
--rw-rw-r--   0 you       (1000) you       (1000)        1 2021-01-12 06:39:19.000000 bert4keras-0.9.8/bert4keras.egg-info/dependency_links.txt
--rw-rw-r--   0 you       (1000) you       (1000)       11 2021-01-12 06:39:19.000000 bert4keras-0.9.8/bert4keras.egg-info/top_level.txt
--rw-rw-r--   0 you       (1000) you       (1000)       13 2021-01-12 06:39:19.000000 bert4keras-0.9.8/bert4keras.egg-info/requires.txt
--rw-rw-r--   0 you       (1000) you       (1000)      290 2021-01-12 06:39:19.000000 bert4keras-0.9.8/bert4keras.egg-info/PKG-INFO
--rw-rw-r--   0 you       (1000) you       (1000)      290 2021-01-12 06:39:19.000000 bert4keras-0.9.8/PKG-INFO
--rw-rw-r--   0 you       (1000) you       (1000)      449 2021-01-12 06:31:38.000000 bert4keras-0.9.8/setup.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2021-01-30 03:26:36.000000 bert4keras-0.9.9/
+-rw-rw-r--   0 you       (1000) you       (1000)       38 2021-01-30 03:26:36.000000 bert4keras-0.9.9/setup.cfg
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2021-01-30 03:26:36.000000 bert4keras-0.9.9/bert4keras/
+-rw-rw-r--   0 you       (1000) you       (1000)    80089 2021-01-30 03:24:45.000000 bert4keras-0.9.9/bert4keras/models.py
+-rw-rw-r--   0 you       (1000) you       (1000)       48 2021-01-30 03:24:45.000000 bert4keras-0.9.9/bert4keras/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)    15854 2021-01-30 03:24:45.000000 bert4keras-0.9.9/bert4keras/tokenizers.py
+-rw-rw-r--   0 you       (1000) you       (1000)     9520 2021-01-30 03:24:45.000000 bert4keras-0.9.9/bert4keras/backend.py
+-rw-rw-r--   0 you       (1000) you       (1000)    42285 2021-01-30 03:24:45.000000 bert4keras-0.9.9/bert4keras/optimizers.py
+-rw-rw-r--   0 you       (1000) you       (1000)    26522 2021-01-30 03:24:45.000000 bert4keras-0.9.9/bert4keras/snippets.py
+-rw-rw-r--   0 you       (1000) you       (1000)    42686 2021-01-30 03:24:45.000000 bert4keras-0.9.9/bert4keras/layers.py
+-rw-rw-r--   0 you       (1000) you       (1000)    14056 2021-01-30 03:24:45.000000 bert4keras-0.9.9/README.md
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2021-01-30 03:26:36.000000 bert4keras-0.9.9/bert4keras.egg-info/
+-rw-rw-r--   0 you       (1000) you       (1000)      347 2021-01-30 03:26:36.000000 bert4keras-0.9.9/bert4keras.egg-info/SOURCES.txt
+-rw-rw-r--   0 you       (1000) you       (1000)        1 2021-01-30 03:26:36.000000 bert4keras-0.9.9/bert4keras.egg-info/dependency_links.txt
+-rw-rw-r--   0 you       (1000) you       (1000)       11 2021-01-30 03:26:36.000000 bert4keras-0.9.9/bert4keras.egg-info/top_level.txt
+-rw-rw-r--   0 you       (1000) you       (1000)       13 2021-01-30 03:26:36.000000 bert4keras-0.9.9/bert4keras.egg-info/requires.txt
+-rw-rw-r--   0 you       (1000) you       (1000)      290 2021-01-30 03:26:36.000000 bert4keras-0.9.9/bert4keras.egg-info/PKG-INFO
+-rw-rw-r--   0 you       (1000) you       (1000)      290 2021-01-30 03:26:36.000000 bert4keras-0.9.9/PKG-INFO
+-rw-rw-r--   0 you       (1000) you       (1000)      449 2021-01-30 03:24:45.000000 bert4keras-0.9.9/setup.py
```

### Comparing `bert4keras-0.9.8/bert4keras/models.py` & `bert4keras-0.9.9/bert4keras/models.py`

 * *Files identical despite different names*

### Comparing `bert4keras-0.9.8/bert4keras/tokenizers.py` & `bert4keras-0.9.9/bert4keras/tokenizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,23 +182,26 @@
         raise NotImplementedError
 
 
 class Tokenizer(TokenizerBase):
     """Bert原生分词器
     纯Python实现，代码修改自keras_bert的tokenizer实现
     """
-    def __init__(self, token_dict, do_lower_case=False, **kwargs):
+    def __init__(
+        self, token_dict, do_lower_case=False, word_maxlen=200, **kwargs
+    ):
         super(Tokenizer, self).__init__(**kwargs)
         if is_string(token_dict):
             token_dict = load_vocab(token_dict)
 
         self._do_lower_case = do_lower_case
         self._token_dict = token_dict
         self._token_dict_inv = {v: k for k, v in token_dict.items()}
         self._vocab_size = len(token_dict)
+        self._word_maxlen = word_maxlen
 
         for token in ['pad', 'unk', 'mask', 'start', 'end']:
             try:
                 _token_id = token_dict[getattr(self, '_token_%s' % token)]
                 setattr(self, '_token_%s_id' % token, _token_id)
             except:
                 pass
@@ -281,32 +284,32 @@
             tokens.extend(self._word_piece_tokenize(word))
 
         return tokens
 
     def _word_piece_tokenize(self, word):
         """word内分成subword
         """
-        if word in self._token_dict:
+        if len(word) > self._word_maxlen:
             return [word]
 
-        tokens = []
-        start, stop = 0, 0
+        tokens, start, end = [], 0, 0
         while start < len(word):
-            stop = len(word)
-            while stop > start:
-                sub = word[start:stop]
+            end = len(word)
+            while end > start:
+                sub = word[start:end]
                 if start > 0:
                     sub = '##' + sub
                 if sub in self._token_dict:
                     break
-                stop -= 1
-            if start == stop:
-                stop += 1
-            tokens.append(sub)
-            start = stop
+                end -= 1
+            if start == end:
+                return [word]
+            else:
+                tokens.append(sub)
+                start = end
 
         return tokens
 
     @staticmethod
     def stem(token):
         """获取token的“词干”（如果是##开头，则自动去掉##）
         """
```

### Comparing `bert4keras-0.9.8/bert4keras/backend.py` & `bert4keras-0.9.9/bert4keras/backend.py`

 * *Files identical despite different names*

### Comparing `bert4keras-0.9.8/bert4keras/optimizers.py` & `bert4keras-0.9.9/bert4keras/optimizers.py`

 * *Files identical despite different names*

### Comparing `bert4keras-0.9.8/bert4keras/snippets.py` & `bert4keras-0.9.9/bert4keras/snippets.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 import six
 import logging
 import numpy as np
 import re
 import sys
 from collections import defaultdict
 import json
-import keras
+import tensorflow as tf
+from bert4keras.backend import K, keras
 
 _open_ = open
 is_py2 = six.PY2
 
 if not is_py2:
     basestring = str
 
-    
+
 def to_array(*args):
     """批量转numpy的array
     """
     results = [np.array(a) for a in args]
     if len(args) == 1:
         return results[0]
     else:
@@ -326,14 +327,46 @@
         raise NotImplementedError
 
     def forfit(self, random=True):
         while True:
             for d in self.__iter__(random):
                 yield d
 
+    def to_dataset(self, types, shapes, names=None):
+        """转为tf.data.Dataset格式
+        如果传入names的话，自动把数据包装成dict形式。
+        """
+        if names is None:
+
+            generator = self.forfit
+
+        else:
+
+            if is_string(names):
+                warps = lambda k, v: {k: v}
+            elif is_string(names[0]):
+                warps = lambda k, v: dict(zip(k, v))
+            else:
+                warps = lambda k, v: tuple(
+                    dict(zip(i, j)) for i, j in zip(k, v)
+                )
+
+            def generator():
+                for d in self.forfit():
+                    yield warps(names, d)
+
+            types = warps(names, types)
+            shapes = warps(names, shapes)
+
+        dataset = tf.data.Dataset.from_generator(
+            generator, output_types=types, output_shapes=shapes
+        )
+        dataset = dataset.batch(self.batch_size)
+        return dataset
+
 
 class ViterbiDecoder(object):
     """Viterbi解码算法基类
     """
     def __init__(self, trans, starts=None, ends=None):
         self.trans = trans
         self.num_labels = len(trans)
@@ -656,16 +689,14 @@
     依赖：
         pip install bottle
         pip install paste
         （如果不用 server='paste' 的话，可以不装paste库）
     """
     def __init__(self, host='0.0.0.0', port=8000, server='paste'):
 
-        import tensorflow as tf
-        from bert4keras.backend import K
         import bottle
 
         self.host = host
         self.port = port
         self.server = server
         self.graph = tf.get_default_graph()
         self.sess = K.get_session()
```

### Comparing `bert4keras-0.9.8/bert4keras/layers.py` & `bert4keras-0.9.9/bert4keras/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,15 +536,15 @@
                 embeddings = K.gather(self.embeddings, position_ids)
             else:
                 embeddings = self.embeddings[None, :seq_len]
 
         if self.merge_mode == 'add':
             return inputs + embeddings
         elif self.merge_mode == 'mul':
-            return inputs * embeddings
+            return inputs * (embeddings + 1.0)
         else:
             if not self.custom_position_ids:
                 embeddings = K.tile(embeddings, [batch_size, 1, 1])
             return K.concatenate([inputs, embeddings])
 
     def compute_output_shape(self, input_shape):
         if self.custom_position_ids:
@@ -598,15 +598,15 @@
         embeddings = tf.einsum('bn,d->bnd', position_ids, indices)
         embeddings = K.stack([K.sin(embeddings), K.cos(embeddings)], axis=-1)
         embeddings = K.reshape(embeddings, (-1, seq_len, self.output_dim))
 
         if self.merge_mode == 'add':
             return inputs + embeddings
         elif self.merge_mode == 'mul':
-            return inputs * embeddings
+            return inputs * (embeddings + 1.0)
         else:
             if not self.custom_position_ids:
                 embeddings = K.tile(embeddings, [batch_size, 1, 1])
             return K.concatenate([inputs, embeddings])
 
     def compute_output_shape(self, input_shape):
         if self.custom_position_ids:
@@ -1124,15 +1124,15 @@
     """
     def __init__(self, output_axis=None, **kwargs):
         super(Loss, self).__init__(**kwargs)
         self.output_axis = output_axis
 
     def call(self, inputs, mask=None):
         loss = self.compute_loss(inputs, mask)
-        self.add_loss(loss)
+        self.add_loss(loss, inputs=inputs)
         if self.output_axis is None:
             return inputs
         elif isinstance(self.output_axis, list):
             return [inputs[i] for i in self.output_axis]
         else:
             return inputs[self.output_axis]
```

### Comparing `bert4keras-0.9.8/README.md` & `bert4keras-0.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 - <strong>Multilingual T5</strong>: https://github.com/google-research/multilingual-t5/
 
 <strong>注意事项</strong>
 - 注1：brightmart版albert的开源时间早于Google版albert，这导致早期brightmart版albert的权重与Google版的不完全一致，换言之两者不能直接相互替换。为了减少代码冗余，bert4keras的0.2.4及后续版本均只支持加载<u>Google版</u>以brightmart版中<u>带Google字眼</u>的权重。如果要加载早期版本的权重，请用<a href="https://github.com/bojone/bert4keras/releases/tag/v0.2.3">0.2.3版本</a>，或者考虑作者转换过的<a href="https://github.com/bojone/albert_zh">albert_zh</a>。
 - 注2：下载下来的ELECTRA权重，如果没有json配置文件的话，参考<a href="https://github.com/ymcui/Chinese-ELECTRA/issues/3">这里</a>自己改一个（需要加上`type_vocab_size`字段）。
 
 ## 更新
+- <strong>2021.01.30</strong>: 完善多GPU支持，增加多GPU例子：[task_seq2seq_autotitle_multigpu.py](https://github.com/bojone/bert4keras/blob/master/examples/task_seq2seq_autotitle_multigpu.py)。
 - <strong>2020.12.29</strong>: 增加`residual_attention_scores`参数来实现RealFormer，只需要在`build_transformer_model`中传入参数`residual_attention_scores=True`启用。
 - <strong>2020.12.04</strong>: `PositionEmbedding`引入层次分解，可以让BERT直接处理超长文本，在`build_transformer_model`中传入参数`hierarchical_position=True`启用。
 - <strong>2020.11.19</strong>: 支持GPT2模型，参考[CPM_LM_bert4keras](https://github.com/bojone/CPM_LM_bert4keras)项目。
 - <strong>2020.11.14</strong>: 新增分参数学习率`extend_with_parameter_wise_lr`，可用于给每层设置不同的学习率。
 - <strong>2020.10.27</strong>: 支持<a href="https://github.com/google-research/text-to-text-transfer-transformer/blob/master/released_checkpoints.md#t511">T5.1.1</a>和<a href="https://github.com/google-research/multilingual-t5/">Multilingual T5</a>。
 - <strong>2020.08.28</strong>: 支持<a href="https://github.com/bojone/CDial-GPT-tf">GPT_OpenAI</a>。
 - <strong>2020.08.22</strong>: 新增`WebServing`类，允许简单地将模型转换为Web接口，详情请参考该类的<a href="https://github.com/bojone/bert4keras/blob/8d55512a12e4677262363ac189ebf504fc451716/bert4keras/snippets.py#L580">说明</a>。
```

#### html2text {}

```diff
@@ -45,15 +45,17 @@
 /github.com/bojone/labse - Chinese-GENé¡¹ç®ä¸çæ¨¡å: https://github.com/
 bojone/chinese-gen - T5.1.1: https://github.com/google-research/text-to-text-
 transfer-transformer/blob/master/released_checkpoints.md#t511 - Multilingual
 T5: https://github.com/google-research/multilingual-t5/ æ³¨æäºé¡¹ -
 æ³¨1ï¼brightmartçalbertçå¼æºæ¶é´æ©äºGoogleçalbertï¼è¿å¯¼è´æ©æbrightmartçalbertçæéä¸Googleççä¸å®å¨ä¸è´ï¼æ¢è¨ä¹ä¸¤èä¸è½ç´æ¥ç¸äºæ¿æ¢ãä¸ºäºåå°ä»£ç åä½ï¼bert4kerasç0.2.4ååç»­çæ¬ååªæ¯æå è½½Googleçä»¥brightmartçä¸­å¸¦Googleå­ç¼çæéãå¦æè¦å è½½æ©æçæ¬çæéï¼è¯·ç¨0.2.3çæ¬ï¼æèèèä½èè½¬æ¢è¿çalbert_zhã
 -
 æ³¨2ï¼ä¸è½½ä¸æ¥çELECTRAæéï¼å¦ææ²¡æjsonéç½®æä»¶çè¯ï¼åèè¿éèªå·±æ¹ä¸ä¸ªï¼éè¦å ä¸`type_vocab_size`å­æ®µï¼ã
-## æ´æ° - 2020.12.29:
+## æ´æ° - 2021.01.30: å®åå¤GPUæ¯æï¼å¢å å¤GPUä¾å­ï¼
+[task_seq2seq_autotitle_multigpu.py](https://github.com/bojone/bert4keras/blob/
+master/examples/task_seq2seq_autotitle_multigpu.py)ã - 2020.12.29:
 å¢å `residual_attention_scores`åæ°æ¥å®ç°RealFormerï¼åªéè¦å¨`build_transformer_model`ä¸­ä¼ å¥åæ°`residual_attention_scores=True`å¯ç¨ã
 - 2020.12.04:
 `PositionEmbedding`å¼å¥å±æ¬¡åè§£ï¼å¯ä»¥è®©BERTç´æ¥å¤çè¶é¿ææ¬ï¼å¨`build_transformer_model`ä¸­ä¼ å¥åæ°`hierarchical_position=True`å¯ç¨ã
 - 2020.11.19: æ¯æGPT2æ¨¡åï¼åè[CPM_LM_bert4keras](https://github.com/
 bojone/CPM_LM_bert4keras)é¡¹ç®ã - 2020.11.14:
 æ°å¢ååæ°å­¦ä¹ ç`extend_with_parameter_wise_lr`ï¼å¯ç¨äºç»æ¯å±è®¾ç½®ä¸åçå­¦ä¹ çã
 - 2020.10.27: æ¯æT5.1.1åMultilingual_T5ã - 2020.08.28:
```

