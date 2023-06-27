# Comparing `tmp/reasoner-pydantic-4.0.9.tar.gz` & `tmp/reasoner-pydantic-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-4.0.9.tar", last modified: Mon Jun 26 20:28:03 2023, max compression
+gzip compressed data, was "reasoner-pydantic-4.1.0.tar", last modified: Tue Jun 27 17:32:28 2023, max compression
```

## Comparing `reasoner-pydantic-4.0.9.tar` & `reasoner-pydantic-4.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:28:03.586345 reasoner-pydantic-4.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-26 20:28:03.586345 reasoner-pydantic-4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:28:03.582345 reasoner-pydantic-4.0.9/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:28:03.582345 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 20:28:03.000000 reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:28:03.586345 reasoner-pydantic-4.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-26 20:27:57.000000 reasoner-pydantic-4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:32:28.879103 reasoner-pydantic-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-27 17:32:28.879103 reasoner-pydantic-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:32:28.879103 reasoner-pydantic-4.1.0/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:32:28.879103 reasoner-pydantic-4.1.0/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-27 17:32:28.000000 reasoner-pydantic-4.1.0/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-27 17:32:28.000000 reasoner-pydantic-4.1.0/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:32:28.000000 reasoner-pydantic-4.1.0/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:32:28.000000 reasoner-pydantic-4.1.0/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 17:32:28.000000 reasoner-pydantic-4.1.0/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 17:32:28.000000 reasoner-pydantic-4.1.0/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:32:28.879103 reasoner-pydantic-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-27 17:32:22.000000 reasoner-pydantic-4.1.0/setup.py
```

### Comparing `reasoner-pydantic-4.0.9/PKG-INFO` & `reasoner-pydantic-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.9
+Version: 4.1.0
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.9/README.md` & `reasoner-pydantic-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/__init__.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/auxgraphs.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/base_model.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/message.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/message.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/metakg.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/results.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,16 +112,17 @@
     """Result."""
 
     node_bindings: HashableMapping[str, HashableSet[NodeBinding]] = Field(
         ...,
         title="list of node bindings",
     )
 
-    analyses: Optional[HashableSet[Analysis]] = Field(
-        None, title="list of anlysis blocks", nullable=True
+    analyses: HashableSet[Analysis] = Field(
+        ...,
+        title="list of anlysis blocks",
     )
 
     class Config:
         title = "result"
         extra = "allow"
 
     def update(self, other):
```

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/shared.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/utils.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic/workflow.py` & `reasoner-pydantic-4.1.0/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-4.1.0/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.9
+Version: 4.1.0
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.9/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-4.1.0/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.9/setup.py` & `reasoner-pydantic-4.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="4.0.9",
+    version="4.1.0",
     author="Abrar Mesbah",
     author_email="amesbah@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

