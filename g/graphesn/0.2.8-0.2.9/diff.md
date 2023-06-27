# Comparing `tmp/graphesn-0.2.8.tar.gz` & `tmp/graphesn-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphesn-0.2.8.tar", last modified: Tue Mar 29 15:09:00 2022, max compression
+gzip compressed data, was "graphesn-0.2.9.tar", last modified: Wed Sep 28 15:57:34 2022, max compression
```

## Comparing `graphesn-0.2.8.tar` & `graphesn-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 domenico  (1000) domenico  (1000)        0 2022-03-29 15:09:00.814395 graphesn-0.2.8/
--rw-r--r--   0 domenico  (1000) domenico  (1000)     1110 2021-11-12 12:51:07.000000 graphesn-0.2.8/LICENSE
--rw-rw-r--   0 domenico  (1000) domenico  (1000)     3032 2022-03-29 15:09:00.814395 graphesn-0.2.8/PKG-INFO
--rw-r--r--   0 domenico  (1000) domenico  (1000)     2376 2021-12-02 09:37:08.000000 graphesn-0.2.8/README.md
--rw-r--r--   0 domenico  (1000) domenico  (1000)      103 2021-11-07 16:09:36.000000 graphesn-0.2.8/pyproject.toml
--rw-r--r--   0 domenico  (1000) domenico  (1000)      744 2022-03-29 15:09:00.815395 graphesn-0.2.8/setup.cfg
-drwxrwxr-x   0 domenico  (1000) domenico  (1000)        0 2022-03-29 15:09:00.807395 graphesn-0.2.8/src/
-drwxrwxr-x   0 domenico  (1000) domenico  (1000)        0 2022-03-29 15:09:00.813395 graphesn-0.2.8/src/graphesn/
--rw-r--r--   0 domenico  (1000) domenico  (1000)      312 2021-11-16 13:46:01.000000 graphesn-0.2.8/src/graphesn/__init__.py
--rw-r--r--   0 domenico  (1000) domenico  (1000)     3185 2021-11-12 16:45:05.000000 graphesn-0.2.8/src/graphesn/data.py
--rw-r--r--   0 domenico  (1000) domenico  (1000)    17177 2022-03-20 22:55:06.000000 graphesn-0.2.8/src/graphesn/dataset.py
--rw-r--r--   0 domenico  (1000) domenico  (1000)     4850 2022-03-29 14:43:48.000000 graphesn-0.2.8/src/graphesn/matrix.py
--rw-r--r--   0 domenico  (1000) domenico  (1000)     6537 2022-03-15 14:39:10.000000 graphesn-0.2.8/src/graphesn/readout.py
--rw-r--r--   0 domenico  (1000) domenico  (1000)    16386 2022-02-10 14:53:45.000000 graphesn-0.2.8/src/graphesn/reservoir.py
--rw-r--r--   0 domenico  (1000) domenico  (1000)     4043 2022-03-29 15:06:14.000000 graphesn-0.2.8/src/graphesn/util.py
-drwxrwxr-x   0 domenico  (1000) domenico  (1000)        0 2022-03-29 15:09:00.814395 graphesn-0.2.8/src/graphesn.egg-info/
--rw-rw-r--   0 domenico  (1000) domenico  (1000)     3032 2022-03-29 15:09:00.000000 graphesn-0.2.8/src/graphesn.egg-info/PKG-INFO
--rw-rw-r--   0 domenico  (1000) domenico  (1000)      350 2022-03-29 15:09:00.000000 graphesn-0.2.8/src/graphesn.egg-info/SOURCES.txt
--rw-rw-r--   0 domenico  (1000) domenico  (1000)        1 2022-03-29 15:09:00.000000 graphesn-0.2.8/src/graphesn.egg-info/dependency_links.txt
--rw-rw-r--   0 domenico  (1000) domenico  (1000)        9 2022-03-29 15:09:00.000000 graphesn-0.2.8/src/graphesn.egg-info/top_level.txt
+drwxr-xr-x   0 domenico  (1000) domenico  (1000)        0 2022-09-28 15:57:34.300857 graphesn-0.2.9/
+-rw-r--r--   0 domenico  (1000) domenico  (1000)     1110 2021-11-12 12:51:07.000000 graphesn-0.2.9/LICENSE
+-rw-r--r--   0 domenico  (1000) domenico  (1000)     2995 2022-09-28 15:57:34.300857 graphesn-0.2.9/PKG-INFO
+-rw-r--r--   0 domenico  (1000) domenico  (1000)     2376 2021-12-02 09:37:08.000000 graphesn-0.2.9/README.md
+-rw-r--r--   0 domenico  (1000) domenico  (1000)      103 2021-11-07 16:09:36.000000 graphesn-0.2.9/pyproject.toml
+-rw-r--r--   0 domenico  (1000) domenico  (1000)      744 2022-09-28 15:57:34.301857 graphesn-0.2.9/setup.cfg
+drwxr-xr-x   0 domenico  (1000) domenico  (1000)        0 2022-09-28 15:57:34.292857 graphesn-0.2.9/src/
+drwxr-xr-x   0 domenico  (1000) domenico  (1000)        0 2022-09-28 15:57:34.298857 graphesn-0.2.9/src/graphesn/
+-rw-r--r--   0 domenico  (1000) domenico  (1000)      312 2021-11-16 13:46:01.000000 graphesn-0.2.9/src/graphesn/__init__.py
+-rw-r--r--   0 domenico  (1000) domenico  (1000)     3185 2021-11-12 16:45:05.000000 graphesn-0.2.9/src/graphesn/data.py
+-rw-r--r--   0 domenico  (1000) domenico  (1000)    17177 2022-03-20 22:55:06.000000 graphesn-0.2.9/src/graphesn/dataset.py
+-rw-r--r--   0 domenico  (1000) domenico  (1000)     4850 2022-03-29 14:43:48.000000 graphesn-0.2.9/src/graphesn/matrix.py
+-rw-r--r--   0 domenico  (1000) domenico  (1000)     6537 2022-03-15 14:39:10.000000 graphesn-0.2.9/src/graphesn/readout.py
+-rw-r--r--   0 domenico  (1000) domenico  (1000)    18250 2022-09-28 15:48:48.000000 graphesn-0.2.9/src/graphesn/reservoir.py
+-rw-r--r--   0 domenico  (1000) domenico  (1000)     4043 2022-03-29 15:06:14.000000 graphesn-0.2.9/src/graphesn/util.py
+drwxr-xr-x   0 domenico  (1000) domenico  (1000)        0 2022-09-28 15:57:34.299857 graphesn-0.2.9/src/graphesn.egg-info/
+-rw-rw-r--   0 domenico  (1000) domenico  (1000)     2995 2022-09-28 15:57:34.000000 graphesn-0.2.9/src/graphesn.egg-info/PKG-INFO
+-rw-rw-r--   0 domenico  (1000) domenico  (1000)      350 2022-09-28 15:57:34.000000 graphesn-0.2.9/src/graphesn.egg-info/SOURCES.txt
+-rw-rw-r--   0 domenico  (1000) domenico  (1000)        1 2022-09-28 15:57:34.000000 graphesn-0.2.9/src/graphesn.egg-info/dependency_links.txt
+-rw-rw-r--   0 domenico  (1000) domenico  (1000)        9 2022-09-28 15:57:34.000000 graphesn-0.2.9/src/graphesn.egg-info/top_level.txt
```

### Comparing `graphesn-0.2.8/LICENSE` & `graphesn-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graphesn-0.2.8/PKG-INFO` & `graphesn-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: graphesn
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python implementation of Deep Graph Echo State Networks
 Home-page: https://github.com/dtortorella/graph-esn
 Author: Domenico Tortorella, Danilo Numeroso, Alessio Gravina
 Author-email: d.tortorella@phd.unipi.it, d.numeroso@phd.unipi.it, a.gravina@phd.unipi.it
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/dtortorella/graph-esn
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -60,9 +58,7 @@
 If you find a bug, please open an issue to report it, and we will do our best to solve it. For general or technical questions, please email us rather than opening an issue.
 
 ## References
 * C. Gallicchio, A. Micheli (2010). Graph Echo State Networks. The 2010 International Joint Conference on Neural Networks (IJCNN 2010), pp. 3967–3974.
 * C. Gallicchio, A. Micheli (2020). Fast and Deep Graph Neural Networks. The Thirty-Fourth AAAI Conference on Artificial Intelligence (AAAI-20).
 * C. Gallicchio, A. Micheli (2020). Ring Reservoir Neural Networks for Graphs. The 2020 International Joint Conference on Neural Networks (IJCNN 2020).
 * D. Tortorella, A. Micheli (2021). Dynamic Graph Echo State Networks. Proceedings of the 29th European Symposium on Artificial Neural Networks, Computational Intelligence and Machine Learning (ESANN 2021), pp. 99–104.
-
-
```

### Comparing `graphesn-0.2.8/README.md` & `graphesn-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `graphesn-0.2.8/setup.cfg` & `graphesn-0.2.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = graphesn
-version = 0.2.8
+version = 0.2.9
 author = Domenico Tortorella, Danilo Numeroso, Alessio Gravina
 author_email = d.tortorella@phd.unipi.it, d.numeroso@phd.unipi.it, a.gravina@phd.unipi.it
 description = Python implementation of Deep Graph Echo State Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dtortorella/graph-esn
 project_urls =
```

### Comparing `graphesn-0.2.8/src/graphesn/data.py` & `graphesn-0.2.9/src/graphesn/data.py`

 * *Files identical despite different names*

### Comparing `graphesn-0.2.8/src/graphesn/dataset.py` & `graphesn-0.2.9/src/graphesn/dataset.py`

 * *Files identical despite different names*

### Comparing `graphesn-0.2.8/src/graphesn/matrix.py` & `graphesn-0.2.9/src/graphesn/matrix.py`

 * *Files identical despite different names*

### Comparing `graphesn-0.2.8/src/graphesn/readout.py` & `graphesn-0.2.9/src/graphesn/readout.py`

 * *Files identical despite different names*

### Comparing `graphesn-0.2.8/src/graphesn/reservoir.py` & `graphesn-0.2.9/src/graphesn/reservoir.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,38 +81,71 @@
     def in_features(self) -> int:
         """Input dimension"""
         return self.input_weight.shape[1]
 
     @property
     def out_features(self) -> int:
         """Reservoir state dimension"""
-        return self.input_weight.shape[0]
+        return self.recurrent_weight.shape[0]
 
     def extra_repr(self) -> str:
         return f'in={self.in_features}, out={self.out_features}, bias={self.bias is not None}'
 
 
+class ReservoirEmbConvLayer(ReservoirConvLayer):
+    """
+    A Graph ESN convolution layer for categorical input features
+
+    :param input_features: Input categories
+    :param hidden_features: Reservoir dimension
+    :param bias: If bias term is present
+    :param activation: Activation function (default tanh)
+    """
+
+    def __init__(self, input_features: int, hidden_features: int, bias: bool = False,
+                 activation: Union[str, Callable[[Tensor], Tensor]] = 'tanh', **kwargs):
+        super().__init__(input_features, hidden_features, bias, activation, **kwargs)
+        self.input_weight = Parameter(torch.empty(input_features, hidden_features), requires_grad=False)
+
+    def forward(self, edge_index: Adj, input: Tensor, state: Tensor, edge_weight: OptTensor = None):
+        neighbour_aggr = self.propagate(edge_index=edge_index, x=state, edge_weight=edge_weight)
+        return self.leakage * self.activation(
+            F.embedding(input, self.input_weight) + F.linear(neighbour_aggr, self.recurrent_weight, self.bias)) \
+               + (1 - self.leakage) * state
+
+    @property
+    def in_features(self) -> int:
+        """Input categories"""
+        return self.input_weight.shape[0]
+
+
 class GraphReservoir(Module):
     """
     Base class for graph reservoirs
 
     :param num_layers: Reservoir layers
     :param in_features: Size of input
     :param hidden_features: Size of reservoir (i.e. number of hidden units per layer)
     :param bias: Whether bias term is present
+    :param categorical_input: Whether input features are categorical
     :param kwargs: Other `ReservoirConvLayer` arguments (activation, etc.)
     """
     layers: ModuleList
 
-    def __init__(self, num_layers: int, in_features: int, hidden_features: int, bias: bool = False, **kwargs):
+    def __init__(self, num_layers: int, in_features: int, hidden_features: int, bias: bool = False,
+                 categorical_input: bool = False, **kwargs):
         super().__init__()
         assert num_layers > 0
         self.layers = ModuleList()
-        self.layers.append(
-            ReservoirConvLayer(input_features=in_features, hidden_features=hidden_features, bias=bias, **kwargs))
+        if categorical_input:
+            self.layers.append(
+                ReservoirEmbConvLayer(input_features=in_features, hidden_features=hidden_features, bias=bias, **kwargs))
+        else:
+            self.layers.append(
+                ReservoirConvLayer(input_features=in_features, hidden_features=hidden_features, bias=bias, **kwargs))
         for _ in range(1, num_layers):
             self.layers.append(
                 ReservoirConvLayer(input_features=hidden_features, hidden_features=hidden_features, bias=bias,
                                    **kwargs))
 
     def initialize_parameters(self, recurrent: Callable[[Size], Tensor], input: Callable[[Size], Tensor],
                               bias: Optional[Callable[[Size], Tensor]] = None, leakage: float = 1.0):
@@ -151,24 +184,26 @@
     :param in_features: Size of input
     :param hidden_features: Size of reservoir (i.e. number of hidden units per layer)
     :param bias: Whether bias term is present
     :param pooling: Graph pooling function (optional, default no pooling)
     :param fully: Whether to concatenate all layers' encodings, or use just final layer encoding
     :param max_iterations: Maximum number of iterations (optional, default infinity)
     :param epsilon: Convergence condition (default 1e-6)
+    :param categorical_input: Whether input features are categorical
     """
     pooling: Optional[Callable[[Tensor, Tensor], Tensor]]
     fully: bool
     max_iterations: Optional[int]
     epsilon: float
 
     def __init__(self, num_layers: int, in_features: int, hidden_features: int, bias: bool = False,
                  pooling: Optional[Callable[[Tensor, Tensor], Tensor]] = None, fully: bool = False,
-                 max_iterations: Optional[int] = None, epsilon: float = 1e-6, **kwargs):
-        super().__init__(num_layers, in_features, hidden_features, bias, **kwargs)
+                 max_iterations: Optional[int] = None, epsilon: float = 1e-6, categorical_input: bool = False,
+                 **kwargs):
+        super().__init__(num_layers, in_features, hidden_features, bias, categorical_input, **kwargs)
         self.pooling = pooling
         self.fully = fully
         self.max_iterations = max_iterations
         self.epsilon = epsilon
 
     def forward(self, edge_index: Adj, input: Tensor, initial_state: Optional[Union[List[Tensor], Tensor]] = None,
                 batch: OptTensor = None, edge_weight: OptTensor = None) -> Tensor:
@@ -179,15 +214,16 @@
         :param edge_weight: Edges weight (optional)
         :param input: Input graph signal (nodes × in_features)
         :param initial_state: Initial state (nodes × hidden_features) for all reservoir layers, default zeros
         :param batch: Batch index (optional)
         :return: Encoding (samples × dim)
         """
         if initial_state is None:
-            initial_state = [torch.zeros(input.shape[0], layer.out_features).to(input) for layer in self.layers]
+            initial_state = [torch.zeros(input.shape[0], layer.out_features).to(layer.recurrent_weight) for layer in
+                             self.layers]
         elif len(initial_state) != self.num_layers and initial_state.dim() == 2:
             initial_state = [initial_state] * self.num_layers
         embeddings = [self._embed(self.layers[0], edge_index, edge_weight, input, initial_state[0])]
         for i in range(1, self.num_layers):
             embeddings.append(self._embed(self.layers[i], edge_index, edge_weight, embeddings[-1], initial_state[i]))
         if self.fully:
             return torch.cat([self.pooling(x, batch) if self.pooling else x for x in embeddings], dim=-1)
@@ -231,22 +267,23 @@
     :param num_layers: Reservoir layers
     :param in_features: Size of input
     :param hidden_features: Size of reservoir (i.e. number of hidden units per layer)
     :param bias: Whether bias term is present
     :param pooling: Graph pooling function (optional, default no pooling)
     :param fully: Whether to concatenate all layers' encodings, or use just final layer encoding
     :param return_sequences: Return the sequence of states instead of just the final states (default false)
+    :param categorical_input: Whether input features are categorical
     """
     pooling: Optional[Callable[[Tensor, Tensor], Tensor]]
     fully: bool
 
     def __init__(self, num_layers: int, in_features: int, hidden_features: int, bias: bool = False,
                  pooling: Optional[Callable[[Tensor, Tensor], Tensor]] = None, fully: bool = False,
-                 return_sequences: bool = False, **kwargs):
-        super().__init__(num_layers, in_features, hidden_features, bias, **kwargs)
+                 return_sequences: bool = False, categorical_input: bool = False, **kwargs):
+        super().__init__(num_layers, in_features, hidden_features, bias, categorical_input, **kwargs)
         self.pooling = pooling
         self.fully = fully
         self.return_sequences = return_sequences
 
     def forward(self, edge_index: Union[List[Adj], Adj], input: Union[Tensor, List[Tensor]],
                 initial_state: Optional[Union[List[Tensor], Tensor]] = None,
                 batch: OptTensor = None, edge_weight: Optional[Union[List[Tensor], Tensor]] = None,
@@ -260,15 +297,15 @@
         :param initial_state: Initial state (nodes × hidden_features) for all reservoir layers, default zeros
         :param batch: Batch index (optional)
         :param mask: Sequence of node masks (optional, useful for padding dynamic graphs with different lengths)
         :return: Encoding (samples × dim)
         """
         if initial_state is None:
             num_nodes = input[0].shape[0] if isinstance(input, list) else input.shape[1]
-            state = [torch.zeros(num_nodes, layer.out_features).to(input[0]) for layer in self.layers]
+            state = [torch.zeros(num_nodes, layer.out_features).to(layer.recurrent_weight) for layer in self.layers]
         elif len(initial_state) != self.num_layers and initial_state.dim() == 2:
             state = [initial_state.clone() for _ in range(self.num_layers)]
         else:
             state = [x.clone() for x in initial_state]
         if self.return_sequences:
             return self._embed_sequence(edge_index, edge_weight, input, state, mask, batch)
         else:
```

### Comparing `graphesn-0.2.8/src/graphesn/util.py` & `graphesn-0.2.9/src/graphesn/util.py`

 * *Files identical despite different names*

### Comparing `graphesn-0.2.8/src/graphesn.egg-info/PKG-INFO` & `graphesn-0.2.9/src/graphesn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: graphesn
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python implementation of Deep Graph Echo State Networks
 Home-page: https://github.com/dtortorella/graph-esn
 Author: Domenico Tortorella, Danilo Numeroso, Alessio Gravina
 Author-email: d.tortorella@phd.unipi.it, d.numeroso@phd.unipi.it, a.gravina@phd.unipi.it
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/dtortorella/graph-esn
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -60,9 +58,7 @@
 If you find a bug, please open an issue to report it, and we will do our best to solve it. For general or technical questions, please email us rather than opening an issue.
 
 ## References
 * C. Gallicchio, A. Micheli (2010). Graph Echo State Networks. The 2010 International Joint Conference on Neural Networks (IJCNN 2010), pp. 3967–3974.
 * C. Gallicchio, A. Micheli (2020). Fast and Deep Graph Neural Networks. The Thirty-Fourth AAAI Conference on Artificial Intelligence (AAAI-20).
 * C. Gallicchio, A. Micheli (2020). Ring Reservoir Neural Networks for Graphs. The 2020 International Joint Conference on Neural Networks (IJCNN 2020).
 * D. Tortorella, A. Micheli (2021). Dynamic Graph Echo State Networks. Proceedings of the 29th European Symposium on Artificial Neural Networks, Computational Intelligence and Machine Learning (ESANN 2021), pp. 99–104.
-
-
```

