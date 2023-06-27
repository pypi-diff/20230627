# Comparing `tmp/gremlin_python_tutorial-0.0.4.tar.gz` & `tmp/gremlin_python_tutorial-0.0.5.tar.gz`

## Comparing `gremlin_python_tutorial-0.0.4.tar` & `gremlin_python_tutorial-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.project
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.pydevproject
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.travis.yml
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/setServer.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.github/workflows/build.yaml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/config/DataStax.yaml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/config/Neo4j.yaml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/config/OrientDB.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/config/TinkerGraph.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/config/server.yaml
--rw-r--r--   0        0        0   192201 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/data/air-routes-small.xml
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/data/tinkerpop-modern.xml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/gremlin/__init__.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/gremlin/draw.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/gremlin/examples.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/gremlin/remote.py
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/install
--rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/installAndTest
--rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/run
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/runDataStax
--rwxr-xr-x   0        0        0     2120 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/runNeo4j
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/runOrientDB
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/base_gremlin_test.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/basetest.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_003_connection.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_004_io.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_005_graphviz.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_draw.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_examples.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_modern.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_server.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_tutorial.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/LICENSE
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/README.md
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.project
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.pydevproject
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.travis.yml
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/setServer.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/config/DataStax.yaml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/config/Neo4j.yaml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/config/OrientDB.yaml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/config/TinkerGraph.yaml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/config/server.yaml
+-rw-r--r--   0        0        0   192201 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/data/air-routes-small.xml
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/data/tinkerpop-modern.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/gremlin/__init__.py
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/gremlin/draw.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/gremlin/examples.py
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/gremlin/remote.py
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/install
+-rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/installAndTest
+-rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/run
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/runDataStax
+-rwxr-xr-x   0        0        0     2120 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/runNeo4j
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/runOrientDB
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/base_gremlin_test.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/basetest.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/jupyter.ipynb
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_003_connection.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_004_io.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_005_graphviz.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_draw.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_examples.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_modern.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_server.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_tutorial.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/README.md
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    15576 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/PKG-INFO
```

### Comparing `gremlin_python_tutorial-0.0.4/.project` & `gremlin_python_tutorial-0.0.5/.project`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/.travis.yml` & `gremlin_python_tutorial-0.0.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/setServer.py` & `gremlin_python_tutorial-0.0.5/setServer.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/.github/workflows/build.yaml` & `gremlin_python_tutorial-0.0.5/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/.github/workflows/upload-to-pypi.yml` & `gremlin_python_tutorial-0.0.5/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/data/air-routes-small.xml` & `gremlin_python_tutorial-0.0.5/data/air-routes-small.xml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/data/tinkerpop-modern.xml` & `gremlin_python_tutorial-0.0.5/data/tinkerpop-modern.xml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/gremlin/examples.py` & `gremlin_python_tutorial-0.0.5/gremlin/examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from os.path import abspath, dirname
 import urllib.request
 import os
 from pathlib import Path
+
+from gremlin_python.process.anonymous_traversal import GraphTraversalSource
 from gremlin.remote import RemoteTraversal
 from dataclasses import dataclass
 
 @dataclass
 class Volume:
     """
     map a local path on the client to a remote
@@ -35,53 +38,69 @@
         Returns:
             str: the remote path
         """
         path=f"{self.remote_path}/{file_name}"
         return path
         
     
-    @classmethod
-    def docker(cls)->"Volume":
+    @staticmethod
+    def docker()->"Volume":
         """
         get the default docker volume mapping
         
         Returns:
             Volume: the local_path/remote_path mapping
         """
         home = str(Path.home())
         local_path=f"{home}/.gremlin-examples"
         os.makedirs(local_path, exist_ok=True)  
         remote_path="/opt/gremlin-server/data/examples"
         volume=Volume(local_path=local_path,remote_path=remote_path)
         return volume
     
+    @staticmethod
+    def local() -> "Volume":
+        """
+        get the default local volume mapping
+
+        Returns:
+            Volume: the local_path/remote_path mapping
+        """
+        home = str(Path.home())
+        local_path=f"{home}/.gremlin-examples"
+        os.makedirs(local_path, exist_ok=True)
+        remote_path=str(abspath(f"{dirname(abspath(__file__))}/data"))
+        volume=Volume(local_path=local_path,remote_path=remote_path)
+        return volume
+    
 @dataclass
 class Example:
     name:str
     url:str
     
-    def __post_init__(self):
-        """
-        """
-    
-    def load(self,g,volume:Volume,force:bool=False,debug:bool=False):
+    def load(
+        self,
+        g: GraphTraversalSource,
+        volume: Volume,
+        force: bool = False,
+        debug: bool = False,
+    ) -> None:
         """
         download graph from remote_path to local_path depending on force flag
         and load graph into g
         
         Args:
-            g(GraphTraversal): the target 
+            g(GraphTraversalSource): the target graph (inout)
             volume:Volume
             force(bool): if True download even if local copy already exists
             debug(bool): if True show debugging information
         """
         self.download(volume.local_path, force=force,debug=debug)
         graph_xml=f"{volume.remote_path}/{self.name}.xml"
         RemoteTraversal.load(g, graph_xml)
-        pass
     
     def download(self,path,force:bool=False,debug:bool=False)->str:
         """
         load the graphml xml file from the given url and store it to the given file_name (prefix)
         
         Args:
             url(str): the url to use
@@ -109,15 +128,15 @@
         return graph_xml
     
 class Examples:
     """
     Examples 
     """
     
-    def __init__(self,volume,debug:bool=False):
+    def __init__(self,volume:Volume,debug:bool=False):
         """
         Constructor
         
         Args:
             volume:Volume
             debug(bool): if true switch on debugging
         
@@ -125,23 +144,27 @@
         self.debug=debug
         self.volume=volume
         self.examples_by_name={}
         for example in [
             Example(name="tinkerpop-modern",url="https://raw.githubusercontent.com/apache/tinkerpop/master/data/tinkerpop-modern.xml"),
             Example(name="grateful-dead",url="https://raw.githubusercontent.com/apache/tinkerpop/master/data/grateful-dead.xml"),
             Example(name="air-routes-small",url="https://raw.githubusercontent.com/krlawrence/graph/master/sample-data/air-routes-small.graphml"),
-            Example(name="air-routes-latest",url="https://raw.githubusercontent.com/krlawrence/graph/master/sample-data/air-routes-latest.graphml")        ]:
+            Example(name="air-routes-latest",url="https://raw.githubusercontent.com/krlawrence/graph/master/sample-data/air-routes-latest.graphml")
+        ]:
             self.examples_by_name[example.name]=example
         
-    def load_by_name(self,g,name:str):
+    def load_by_name(self, g: GraphTraversalSource, name: str) -> None:
         """
         load an example by name to the given graph
         
         Args:
-            g: the target graph
+            g(GraphTraversalSource): the target graph (inout)
             name(str): the name of the example
+
+        Raises:
+            Exception: if the example does not exist
         """
         if name in self.examples_by_name:
             example=self.examples_by_name[name]
             example.load(g,self.volume,debug=self.debug)
         else:
-            raise Exception(f"invalid example {name}")
+            raise Exception(f"invalid example {name}")
```

### Comparing `gremlin_python_tutorial-0.0.4/scripts/installAndTest` & `gremlin_python_tutorial-0.0.5/scripts/installAndTest`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/scripts/run` & `gremlin_python_tutorial-0.0.5/scripts/run`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/scripts/runNeo4j` & `gremlin_python_tutorial-0.0.5/scripts/runNeo4j`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/tests/base_gremlin_test.py` & `gremlin_python_tutorial-0.0.5/tests/base_gremlin_test.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/tests/basetest.py` & `gremlin_python_tutorial-0.0.5/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/tests/test_003_connection.py` & `gremlin_python_tutorial-0.0.5/tests/test_003_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 # see https://github.com/apache/tinkerpop/blob/master/gremlin-python/src/main/jython/tests/driver/test_client.py
+from os.path import abspath, dirname
 from gremlin_python.driver.request import RequestMessage
 from gremlin.remote import RemoteTraversal, Server
 from tests.basetest import Basetest
 
 class TestConnection(Basetest):
     """
     test connection handling
```

### Comparing `gremlin_python_tutorial-0.0.4/tests/test_004_io.py` & `gremlin_python_tutorial-0.0.5/tests/test_004_io.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/tests/test_005_graphviz.py` & `gremlin_python_tutorial-0.0.5/tests/test_005_graphviz.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/tests/test_draw.py` & `gremlin_python_tutorial-0.0.5/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/tests/test_examples.py` & `gremlin_python_tutorial-0.0.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/tests/test_modern.py` & `gremlin_python_tutorial-0.0.5/tests/test_modern.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/tests/test_tutorial.py` & `gremlin_python_tutorial-0.0.5/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/.gitignore` & `gremlin_python_tutorial-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/LICENSE` & `gremlin_python_tutorial-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/README.md` & `gremlin_python_tutorial-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.4/pyproject.toml` & `gremlin_python_tutorial-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 license = { file="LICENSE" }
 dependencies = [
 		# https://pypi.org/project/gremlinpython/
         'gremlinpython>=3.6.4',
         # https://pypi.org/project/graphviz/
         'graphviz>=0.20.1',
         # https://pypi.org/project/PyYAML/
-        'PyYAML>=6.0'
+        'PyYAML>=6.0',
+        # https://pypi.org/project/aenum/
+        'aenum>=3.1',
      ]
 
 requires-python = ">=3.8"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Programming Language :: Python :: 3 :: Only",
@@ -39,25 +41,29 @@
     "Operating System :: OS Independent",
     "Topic :: Software Development",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License"
     ]
 dynamic = ["version", "description"]
+
 [tool.hatch.version]
 path = "gremlin/__init__.py"
 
+[tool.hatch.build.targets.wheel]
+only-include = ["gremlin", "config", "data"]
+
+[tool.hatch.build.targets.wheel.sources]
+"gremlin" = "gremlin"
+"config" = "gremlin/config"
+"data" = "gremlin/data"
+
 [project.urls]
 Home = "https://github.com/WolfgangFahl/gremlin-python-tutorial"
 Documentation = "https://wiki.bitplan.com/index.php/Gremlin_python"
 Source = "https://github.com/WolfgangFahl/gremlin-python-tutorial"
 
 [project.optional-dependencies]
 test = [
   "green",
 ]
 
-[tool.hatch.build.targets.wheel]
-packages = [
-  "gremlin",
-]
-
```

### Comparing `gremlin_python_tutorial-0.0.4/PKG-INFO` & `gremlin_python_tutorial-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlin-python-tutorial
-Version: 0.0.4
+Version: 0.0.5
 Project-URL: Home, https://github.com/WolfgangFahl/gremlin-python-tutorial
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/Gremlin_python
 Project-URL: Source, https://github.com/WolfgangFahl/gremlin-python-tutorial
 Author-email: Wolfgang Fahl <wf@bitplan.com>, Julian Vollmer <julian.vollmer@rwth-aachen.de>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>, Julian Vollmer <julian.vollmer@rwth-aachen.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -217,14 +217,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
+Requires-Dist: aenum>=3.1
 Requires-Dist: graphviz>=0.20.1
 Requires-Dist: gremlinpython>=3.6.4
 Requires-Dist: pyyaml>=6.0
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
```

