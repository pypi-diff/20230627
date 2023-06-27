# Comparing `tmp/pathfind-0.0.8.tar.gz` & `tmp/pathfind-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathfind-0.0.8.tar", last modified: Mon Dec 19 04:14:15 2022, max compression
+gzip compressed data, was "pathfind-0.0.9.tar", last modified: Wed May 17 15:26:45 2023, max compression
```

## Comparing `pathfind-0.0.8.tar` & `pathfind-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,49 @@
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2022-12-19 04:14:15.937257 pathfind-0.0.8/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1063 2022-11-10 05:35:08.000000 pathfind-0.0.8/LICENSE
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3507 2022-12-19 04:14:15.937368 pathfind-0.0.8/PKG-INFO
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2980 2022-12-09 05:40:10.000000 pathfind-0.0.8/README.md
--rw-r--r--   0 morvanzhou   (501) staff       (20)       94 2022-11-07 07:33:46.000000 pathfind-0.0.8/pyproject.toml
--rw-r--r--   0 morvanzhou   (501) staff       (20)      757 2022-12-19 04:14:15.937745 pathfind-0.0.8/setup.cfg
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2022-12-19 04:14:15.931767 pathfind-0.0.8/src/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2022-12-19 04:14:15.932944 pathfind-0.0.8/src/pathfind/
--rw-r--r--   0 morvanzhou   (501) staff       (20)      204 2022-12-19 04:10:52.000000 pathfind-0.0.8/src/pathfind/__init__.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2022-12-19 04:14:15.934356 pathfind-0.0.8/src/pathfind/finder/
--rw-r--r--   0 morvanzhou   (501) staff       (20)      444 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/finder/__init__.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2022-12-19 04:14:15.936184 pathfind-0.0.8/src/pathfind/finder/alg/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1764 2022-12-19 04:10:52.000000 pathfind-0.0.8/src/pathfind/finder/alg/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      791 2022-11-16 09:15:14.000000 pathfind-0.0.8/src/pathfind/finder/alg/a_star.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)       65 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/finder/alg/ant_colony_optimization.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      672 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/finder/alg/breadth_first_search.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7311 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/finder/alg/d_star_lite.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      668 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/finder/alg/depth_first_search.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      592 2022-11-16 09:15:14.000000 pathfind-0.0.8/src/pathfind/finder/alg/dijkstra.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/finder/alg/genetic_algorithm.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      882 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/finder/alg/greedy_best_first.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7960 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/finder/alg/jump_point_search.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6447 2022-12-19 04:04:03.000000 pathfind-0.0.8/src/pathfind/finder/finder.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2049 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/finder/queue.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1182 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/finder/tool.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2022-12-19 04:14:15.936899 pathfind-0.0.8/src/pathfind/graph/
--rw-r--r--   0 morvanzhou   (501) staff       (20)      153 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/graph/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1941 2022-11-16 09:15:14.000000 pathfind-0.0.8/src/pathfind/graph/edge.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     9088 2022-12-09 05:36:22.000000 pathfind-0.0.8/src/pathfind/graph/graph.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3226 2022-12-06 07:54:27.000000 pathfind-0.0.8/src/pathfind/graph/node.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      807 2022-12-19 04:04:03.000000 pathfind-0.0.8/src/pathfind/graph/transform.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2022-12-19 04:14:15.933722 pathfind-0.0.8/src/pathfind.egg-info/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3507 2022-12-19 04:14:15.000000 pathfind-0.0.8/src/pathfind.egg-info/PKG-INFO
--rw-r--r--   0 morvanzhou   (501) staff       (20)      935 2022-12-19 04:14:15.000000 pathfind-0.0.8/src/pathfind.egg-info/SOURCES.txt
--rw-r--r--   0 morvanzhou   (501) staff       (20)        1 2022-12-19 04:14:15.000000 pathfind-0.0.8/src/pathfind.egg-info/dependency_links.txt
--rw-r--r--   0 morvanzhou   (501) staff       (20)       73 2022-12-19 04:14:15.000000 pathfind-0.0.8/src/pathfind.egg-info/requires.txt
--rw-r--r--   0 morvanzhou   (501) staff       (20)        9 2022-12-19 04:14:15.000000 pathfind-0.0.8/src/pathfind.egg-info/top_level.txt
+drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2023-05-17 15:26:45.087999 pathfind-0.0.9/
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1063 2022-11-10 05:35:08.000000 pathfind-0.0.9/LICENSE
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     3567 2023-05-17 15:26:45.088082 pathfind-0.0.9/PKG-INFO
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     2980 2022-12-09 05:40:10.000000 pathfind-0.0.9/README.md
+-rw-r--r--   0 morvanzhou   (501) staff       (20)       94 2022-11-07 07:33:46.000000 pathfind-0.0.9/pyproject.toml
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      830 2023-05-17 15:26:45.088409 pathfind-0.0.9/setup.cfg
+drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2023-05-17 15:26:45.077846 pathfind-0.0.9/src/
+drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2023-05-17 15:26:45.079351 pathfind-0.0.9/src/pathfind/
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      204 2022-12-19 04:10:52.000000 pathfind-0.0.9/src/pathfind/__init__.py
+drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2023-05-17 15:26:45.081235 pathfind-0.0.9/src/pathfind/finder/
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      444 2022-12-06 07:54:27.000000 pathfind-0.0.9/src/pathfind/finder/__init__.py
+drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2023-05-17 15:26:45.083557 pathfind-0.0.9/src/pathfind/finder/alg/
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1764 2022-12-19 04:10:52.000000 pathfind-0.0.9/src/pathfind/finder/alg/__init__.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      791 2023-05-17 15:16:04.000000 pathfind-0.0.9/src/pathfind/finder/alg/a_star.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      672 2023-05-17 15:13:59.000000 pathfind-0.0.9/src/pathfind/finder/alg/breadth_first_search.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     7311 2022-12-06 07:54:27.000000 pathfind-0.0.9/src/pathfind/finder/alg/d_star_lite.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      668 2022-12-06 07:54:27.000000 pathfind-0.0.9/src/pathfind/finder/alg/depth_first_search.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      592 2022-11-16 09:15:14.000000 pathfind-0.0.9/src/pathfind/finder/alg/dijkstra.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      882 2022-12-06 07:54:27.000000 pathfind-0.0.9/src/pathfind/finder/alg/greedy_best_first.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     7960 2022-12-06 07:54:27.000000 pathfind-0.0.9/src/pathfind/finder/alg/jump_point_search.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     6447 2023-05-17 15:07:53.000000 pathfind-0.0.9/src/pathfind/finder/finder.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1858 2023-05-17 15:24:56.000000 pathfind-0.0.9/src/pathfind/finder/queue.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1182 2022-12-06 07:54:27.000000 pathfind-0.0.9/src/pathfind/finder/tool.py
+drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2023-05-17 15:26:45.084939 pathfind-0.0.9/src/pathfind/graph/
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      153 2022-12-06 07:54:27.000000 pathfind-0.0.9/src/pathfind/graph/__init__.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1941 2022-11-16 09:15:14.000000 pathfind-0.0.9/src/pathfind/graph/edge.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     9088 2022-12-09 05:36:22.000000 pathfind-0.0.9/src/pathfind/graph/graph.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     2878 2023-05-17 15:09:14.000000 pathfind-0.0.9/src/pathfind/graph/node.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      807 2022-12-19 04:04:03.000000 pathfind-0.0.9/src/pathfind/graph/transform.py
+drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2023-05-17 15:26:45.080344 pathfind-0.0.9/src/pathfind.egg-info/
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     3567 2023-05-17 15:26:45.000000 pathfind-0.0.9/src/pathfind.egg-info/PKG-INFO
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1104 2023-05-17 15:26:45.000000 pathfind-0.0.9/src/pathfind.egg-info/SOURCES.txt
+-rw-r--r--   0 morvanzhou   (501) staff       (20)        1 2023-05-17 15:26:45.000000 pathfind-0.0.9/src/pathfind.egg-info/dependency_links.txt
+-rw-r--r--   0 morvanzhou   (501) staff       (20)       97 2023-05-17 15:26:45.000000 pathfind-0.0.9/src/pathfind.egg-info/requires.txt
+-rw-r--r--   0 morvanzhou   (501) staff       (20)        9 2023-05-17 15:26:45.000000 pathfind-0.0.9/src/pathfind.egg-info/top_level.txt
+drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2023-05-17 15:26:45.087838 pathfind-0.0.9/tests/
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1192 2022-12-06 07:54:27.000000 pathfind-0.0.9/tests/test_astar.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      487 2022-12-06 07:54:27.000000 pathfind-0.0.9/tests/test_bfs.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      542 2022-12-06 07:54:27.000000 pathfind-0.0.9/tests/test_dfs.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      551 2022-12-06 07:54:27.000000 pathfind-0.0.9/tests/test_dijkstra.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1977 2022-12-06 07:54:27.000000 pathfind-0.0.9/tests/test_dstart_lite.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     2257 2022-11-15 07:39:32.000000 pathfind-0.0.9/tests/test_edge.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     2431 2023-05-17 15:24:56.000000 pathfind-0.0.9/tests/test_find.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1026 2022-12-06 07:54:27.000000 pathfind-0.0.9/tests/test_graph.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      486 2022-12-06 07:54:27.000000 pathfind-0.0.9/tests/test_greedy.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     3168 2022-12-06 07:54:27.000000 pathfind-0.0.9/tests/test_jps.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)      354 2022-11-10 08:01:33.000000 pathfind-0.0.9/tests/test_node.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1322 2023-05-17 15:24:56.000000 pathfind-0.0.9/tests/test_queue.py
+-rw-r--r--   0 morvanzhou   (501) staff       (20)     1525 2022-12-06 07:54:27.000000 pathfind-0.0.9/tests/test_transform.py
```

### Comparing `pathfind-0.0.8/LICENSE` & `pathfind-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/PKG-INFO` & `pathfind-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pathfind
-Version: 0.0.8
+Version: 0.0.9
 Summary: path finding algorithms in python
 Home-page: https://github.com/MorvanZhou/pathfind
 Author: MorvanZhou
 Author-email: morvanzhou@hotmail.com
 Project-URL: Bug Tracker, https://github.com/MorvanZhou/pathfind/issues
+Project-URL: Source, https://github.com/MorvanZhou/pathfind
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: build
 License-File: LICENSE
```

### Comparing `pathfind-0.0.8/README.md` & `pathfind-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/setup.cfg` & `pathfind-0.0.9/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [metadata]
 name = pathfind
-version = 0.0.8
+version = 0.0.9
 author = MorvanZhou
 author_email = morvanzhou@hotmail.com
 description = path finding algorithms in python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MorvanZhou/pathfind
 project_urls = 
 	Bug Tracker = https://github.com/MorvanZhou/pathfind/issues
+	Source=https://github.com/MorvanZhou/pathfind
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
@@ -25,15 +26,17 @@
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 build = 
 	tox==3.24.3
+	tox-conda
 	build
 	twine
 	pylint
+	line_profiler
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pathfind-0.0.8/src/pathfind/finder/alg/__init__.py` & `pathfind-0.0.9/src/pathfind/finder/alg/__init__.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/finder/alg/a_star.py` & `pathfind-0.0.9/src/pathfind/finder/alg/a_star.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/finder/alg/breadth_first_search.py` & `pathfind-0.0.9/src/pathfind/finder/alg/breadth_first_search.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/finder/alg/d_star_lite.py` & `pathfind-0.0.9/src/pathfind/finder/alg/d_star_lite.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/finder/alg/depth_first_search.py` & `pathfind-0.0.9/src/pathfind/finder/alg/depth_first_search.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/finder/alg/dijkstra.py` & `pathfind-0.0.9/src/pathfind/finder/alg/dijkstra.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/finder/alg/greedy_best_first.py` & `pathfind-0.0.9/src/pathfind/finder/alg/greedy_best_first.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/finder/alg/jump_point_search.py` & `pathfind-0.0.9/src/pathfind/finder/alg/jump_point_search.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/finder/finder.py` & `pathfind-0.0.9/src/pathfind/finder/finder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import typing as tp
 from abc import ABCMeta, abstractmethod
 
 from pathfind.graph.edge import INFINITY
 from pathfind.graph.graph import Graph, Node
+from pathfind.graph.node import LinkedNode
 
 if tp.TYPE_CHECKING:
     from pathfind.finder.queue import BaseQueue
 
 NodeName = str
 Cost = float
 GMap = tp.Dict[NodeName, Cost]
@@ -179,27 +180,26 @@
             nodes.insert(0, parent_node.name)
             if parent_node.name == target_name:
                 break
             trace_start_name = parent_node.name
         return nodes
 
     @staticmethod
-    def successors(node: Node):
+    def successors(node: Node) -> tp.Iterator[LinkedNode]:
         """
         Return a generator for getting all successors from this node
 
         Args:
             node (Node): node
 
         Returns:
             a generator for getting successor nodes
         """
         for edge in node.edges.values():
-            successor_with_weight = node.get_successor_with_weight(edge)
-            yield successor_with_weight
+            yield node.successors[edge.id]
 
     @staticmethod
     def predecessors(node: Node):
         """
         Return a generator for getting all predecessors from this node
 
         Args:
```

### Comparing `pathfind-0.0.8/src/pathfind/finder/tool.py` & `pathfind-0.0.9/src/pathfind/finder/tool.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/graph/edge.py` & `pathfind-0.0.9/src/pathfind/graph/edge.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/graph/graph.py` & `pathfind-0.0.9/src/pathfind/graph/graph.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind/graph/node.py` & `pathfind-0.0.9/src/pathfind/graph/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,18 +25,15 @@
 class LinkedNode:
     node: Node
     edge: Edge
     back: bool
 
     @property
     def weight(self):
-        if self.back:
-            return self.edge.back_weight
-        else:
-            return self.edge.weight
+        return self.edge.back_weight if self.back else self.edge.weight
 
 
 @dataclass
 class Node:
     name: str = field(default_factory=_get_node_name)
     edges: tp.Dict[str, Edge] = field(default_factory=dict)
     successors: tp.Dict[str, LinkedNode] = field(default_factory=dict)
@@ -56,22 +53,14 @@
             if edge.back_weight >= 0:
                 self.predecessors[edge.id] = LinkedNode(node=edge.node1, edge=edge, back=True)
         else:
             raise ValueError(f"edge does not include this {self.name}")
 
         self.edges[edge.id] = edge
 
-    def get_successor(self, edge: tp.Union[str, Edge]) -> Node:
-        return self.get_successor_with_weight(edge).node
-
-    def get_successor_with_weight(self, edge: tp.Union[str, Edge]) -> LinkedNode:
-        if not isinstance(edge, str):
-            edge = edge.id
-        return self.successors[edge]
-
     def get_all_successors(self) -> tp.List[Node]:
         return [ln.node for ln in self.successors.values()]
 
     def get_all_successors_with_weight(self) -> tp.List[LinkedNode]:
         return list(self.successors.values())
 
     def get_predecessor(self, edge: tp.Union[str, Edge]) -> Node:
```

### Comparing `pathfind-0.0.8/src/pathfind/graph/transform.py` & `pathfind-0.0.9/src/pathfind/graph/transform.py`

 * *Files identical despite different names*

### Comparing `pathfind-0.0.8/src/pathfind.egg-info/PKG-INFO` & `pathfind-0.0.9/src/pathfind.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pathfind
-Version: 0.0.8
+Version: 0.0.9
 Summary: path finding algorithms in python
 Home-page: https://github.com/MorvanZhou/pathfind
 Author: MorvanZhou
 Author-email: morvanzhou@hotmail.com
 Project-URL: Bug Tracker, https://github.com/MorvanZhou/pathfind/issues
+Project-URL: Source, https://github.com/MorvanZhou/pathfind
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: build
 License-File: LICENSE
```

