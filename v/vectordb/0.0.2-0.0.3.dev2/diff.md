# Comparing `tmp/vectordb-0.0.2.tar.gz` & `tmp/vectordb-0.0.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vectordb-0.0.2.tar", last modified: Thu Jun 22 13:43:17 2023, max compression
+gzip compressed data, was "vectordb-0.0.3.dev2.tar", last modified: Tue Jun 27 14:29:38 2023, max compression
```

## Comparing `vectordb-0.0.2.tar` & `vectordb-0.0.3.dev2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:17.000000 vectordb-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-22 13:43:17.000000 vectordb-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-22 13:43:03.000000 vectordb-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:43:17.000000 vectordb-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-22 13:43:03.000000 vectordb-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:17.000000 vectordb-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:03.000000 vectordb-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-22 13:43:03.000000 vectordb-0.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:17.000000 vectordb-0.0.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:03.000000 vectordb-0.0.2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-22 13:43:03.000000 vectordb-0.0.2/tests/integration/test_hnswlib_vectordb_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-22 13:43:03.000000 vectordb-0.0.2/tests/integration/test_inmemory_vectordb_serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:17.000000 vectordb-0.0.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:03.000000 vectordb-0.0.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-06-22 13:43:03.000000 vectordb-0.0.2/tests/unit/test_hnswlib_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-22 13:43:03.000000 vectordb-0.0.2/tests/unit/test_inmemory_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb/db/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/db/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/db/executors/hnsw_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/db/executors/inmemory_exact_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/db/executors/typed_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/db/hnsw_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/db/inmemory_exact_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/db/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/utils/create_doc_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/utils/pass_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/utils/push_to_hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/utils/sort_matches_by_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-22 13:43:03.000000 vectordb-0.0.2/vectordb/utils/unify_input_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 13:43:17.000000 vectordb-0.0.2/vectordb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:38.257574 vectordb-0.0.3.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-27 14:29:38.257574 vectordb-0.0.3.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:29:38.257574 vectordb-0.0.3.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:38.253574 vectordb-0.0.3.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:38.253574 vectordb-0.0.3.dev2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/tests/integration/test_hnswlib_vectordb_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/tests/integration/test_inmemory_vectordb_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:38.257574 vectordb-0.0.3.dev2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/tests/unit/test_hnswlib_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/tests/unit/test_inmemory_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:38.257574 vectordb-0.0.3.dev2/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-27 14:29:37.000000 vectordb-0.0.3.dev2/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:38.257574 vectordb-0.0.3.dev2/vectordb/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:38.257574 vectordb-0.0.3.dev2/vectordb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:38.257574 vectordb-0.0.3.dev2/vectordb/db/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/db/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/db/executors/hnsw_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/db/executors/inmemory_exact_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/db/executors/typed_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/db/hnsw_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/db/inmemory_exact_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/db/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:38.257574 vectordb-0.0.3.dev2/vectordb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/utils/create_doc_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/utils/pass_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/utils/push_to_hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/utils/sort_matches_by_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-27 14:29:32.000000 vectordb-0.0.3.dev2/vectordb/utils/unify_input_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:29:38.257574 vectordb-0.0.3.dev2/vectordb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-27 14:29:38.000000 vectordb-0.0.3.dev2/vectordb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-27 14:29:38.000000 vectordb-0.0.3.dev2/vectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:29:38.000000 vectordb-0.0.3.dev2/vectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-27 14:29:38.000000 vectordb-0.0.3.dev2/vectordb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 14:29:38.000000 vectordb-0.0.3.dev2/vectordb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 14:29:38.000000 vectordb-0.0.3.dev2/vectordb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vectordb-0.0.2/PKG-INFO` & `vectordb-0.0.3.dev2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: vectordb
-Version: 0.0.2
+Version: 0.0.3.dev2
 Summary: The Python VectorDB. Build your vector database from working as a library to scaling as a database in the cloud
 Home-page: https://github.com/jina-ai/vectordb/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/vectordb/tags
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `vectordb-0.0.2/setup.py` & `vectordb-0.0.3.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/tests/integration/test_hnswlib_vectordb_serve.py` & `vectordb-0.0.3.dev2/tests/integration/test_hnswlib_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/tests/integration/test_inmemory_vectordb_serve.py` & `vectordb-0.0.3.dev2/tests/integration/test_inmemory_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/tests/unit/test_hnswlib_vectordb.py` & `vectordb-0.0.3.dev2/tests/unit/test_hnswlib_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/tests/unit/test_inmemory_vectordb.py` & `vectordb-0.0.3.dev2/tests/unit/test_inmemory_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/vectordb/__main__.py` & `vectordb-0.0.3.dev2/vectordb/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,18 @@
     default=1,
     help='Number of shards to use for the deployed VectorDB',
     required=False,
     show_default=True,
 )
 def deploy(db, protocol, shards):
     definition_file, _, obj_name = db.partition(":")
+    if not definition_file.endswith('.py'):
+        definition_file = f'{definition_file}.py'
     protocol = protocol.split(',')
-    VectorDB.deploy(protoocl=protocol,
+    VectorDB.deploy(protocol=protocol,
                     shards=shards,
                     definition_file=definition_file,
                     obj_name=obj_name)
 
 
 @vectordb.command(help='Deploy a vectorDB app to Jina AI Cloud')
 @click.option(
```

### Comparing `vectordb-0.0.2/vectordb/client/client.py` & `vectordb-0.0.3.dev2/vectordb/client/client.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/vectordb/db/base.py` & `vectordb-0.0.3.dev2/vectordb/db/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             kwargs.pop('stateful')
 
         use_deployment = True
         if to_deploy:
             # here we would need to push the EXECUTOR TO HUBBLE AND CHANGE THE USES
             assert definition_file is not None, 'Trying to create a Jina Object for Deployment without the file where the vectordb object/class is defined'
             assert obj_name is not None, 'Trying to create a Jina Object for Deployment without the name of the vectordb object/class to deploy'
-            uses = f'jinaai+docker://{push_vectordb_to_hubble(vectordb_name=obj_name, definition_file_path=definition_file)}'
+            uses = f'{push_vectordb_to_hubble(vectordb_name=obj_name, definition_file_path=definition_file)}'
             use_deployment = False
 
         if 'websocket' in protocol_list:  # websocket not supported for Deployment
             use_deployment = False
 
         if (shards > 1 or stateful) and 'http' in protocol_list:  # http not supported for shards > 1 or stateful
             use_deployment = False
@@ -189,14 +189,15 @@
 
         executor_jcloud_config = {'resources': {'instance': 'C5', 'autoscale': {'min': 0, 'max': 1},
                                                 'storage': {'kind': 'ebs', 'size': '10G', 'retain': True}}}
         for executor in flow_dict['executors']:
             executor['jcloud'] = executor_jcloud_config
 
         global_jcloud_config = {
+            'docarray': '0.34.0',
             'labels': {
                 'app': 'vectordb',
             },
             'monitor': {
                 'traces': {
                     'enable': True,
                 },
@@ -209,14 +210,15 @@
         }
         flow_dict['jcloud'] = global_jcloud_config
         import tempfile
         from jcloud.flow import CloudFlow
 
         with tempfile.TemporaryDirectory() as tmpdir:
             flow_path = os.path.join(tmpdir, 'flow.yml')
+            print(f' flow_path {flow_path}')
             with open(flow_path, 'w') as f:
                 yaml.safe_dump(flow_dict, f, sort_keys=False)
 
             cloud_flow = CloudFlow(path=flow_path)
 
             async def _deploy():
                 await cloud_flow.__aenter__()
```

### Comparing `vectordb-0.0.2/vectordb/db/executors/hnsw_indexer.py` & `vectordb-0.0.3.dev2/vectordb/db/executors/hnsw_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/vectordb/db/executors/inmemory_exact_indexer.py` & `vectordb-0.0.3.dev2/vectordb/db/executors/inmemory_exact_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/vectordb/db/executors/typed_executor.py` & `vectordb-0.0.3.dev2/vectordb/db/executors/typed_executor.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/vectordb/db/service.py` & `vectordb-0.0.3.dev2/vectordb/db/service.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/vectordb/utils/create_doc_type.py` & `vectordb-0.0.3.dev2/vectordb/utils/create_doc_type.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/vectordb/utils/pass_parameters.py` & `vectordb-0.0.3.dev2/vectordb/utils/pass_parameters.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/vectordb/utils/push_to_hubble.py` & `vectordb-0.0.3.dev2/vectordb/utils/push_to_hubble.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,31 @@
         for key, val in self._env_keys_old.items():
             os.environ[key] = str(val)
         # Remove any newly added environment variables
         for key in self._env_keys_added.keys():
             os.unsetenv(key)
 
 
+def get_uri(id: str, tag: str):
+    import requests
+    from hubble import Auth
+
+    r = requests.get(
+        f"https://apihubble.jina.ai/v2/executor/getMeta?id={id}&tag={tag}",
+        headers={"Authorization": f"token {Auth.get_auth_token()}"},
+    )
+    _json = r.json()
+    if _json is None:
+        print(f'Could not find image with id {id} and tag {tag}')
+        return
+    _image_name = _json['data']['name']
+    _user_name = _json['meta']['owner']['name']
+    return f'jinaai+docker://{_user_name}/{_image_name}:{tag}'
+
+
 def get_random_tag():
     return 't-' + uuid.uuid4().hex[:5]
 
 
 def get_random_name():
     return 'n-' + uuid.uuid4().hex[:5]
 
@@ -106,8 +123,10 @@
         content = f.read()
 
     content = content.replace('vectordb_executor', f'vectordb_executor-{image_name}')
 
     with open(os.path.join(tmpdir, 'config.yml'), mode='w', encoding='utf-8') as f:
         f.write(content)
 
-    return _push_to_hubble(tmpdir, image_name, tag, True, False)
+    executor_id = _push_to_hubble(tmpdir, image_name, tag, True, False)
+    id, tag = executor_id.split(':')
+    return get_uri(id, tag)
```

### Comparing `vectordb-0.0.2/vectordb/utils/sort_matches_by_score.py` & `vectordb-0.0.3.dev2/vectordb/utils/sort_matches_by_score.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/vectordb/utils/unify_input_output.py` & `vectordb-0.0.3.dev2/vectordb/utils/unify_input_output.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.2/vectordb.egg-info/PKG-INFO` & `vectordb-0.0.3.dev2/vectordb.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: vectordb
-Version: 0.0.2
+Version: 0.0.3.dev2
 Summary: The Python VectorDB. Build your vector database from working as a library to scaling as a database in the cloud
 Home-page: https://github.com/jina-ai/vectordb/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/vectordb/tags
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `vectordb-0.0.2/vectordb.egg-info/SOURCES.txt` & `vectordb-0.0.3.dev2/vectordb.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/conftest.py
 tests/integration/__init__.py
 tests/integration/test_hnswlib_vectordb_serve.py
 tests/integration/test_inmemory_vectordb_serve.py
```

