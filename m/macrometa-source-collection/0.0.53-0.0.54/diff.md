# Comparing `tmp/macrometa-source-collection-0.0.53.tar.gz` & `tmp/macrometa-source-collection-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.53.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.54.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.53.tar` & `macrometa-source-collection-0.0.54.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11137 2023-06-23 08:18:35.489382 macrometa-source-collection-0.0.53/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0    10213 2023-06-23 08:18:35.489382 macrometa-source-collection-0.0.53/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-06-23 08:18:35.821417 macrometa-source-collection-0.0.53/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.53/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.53/PKG-INFO
+-rw-r--r--   0        0        0    11137 2023-06-27 10:51:43.928963 macrometa-source-collection-0.0.54/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0    10263 2023-06-27 10:51:43.928963 macrometa-source-collection-0.0.54/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-06-27 10:51:44.192968 macrometa-source-collection-0.0.54/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.54/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.54/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.53/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.54/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.53/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.54/macrometa_source_collection/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                 f"pulsar+ssl://{self._host}:6651/",
                 authentication=self._auth,
                 tls_allow_insecure_connection=False,
                 logger=_pulsar_logger,
             )
             _sub_name = self._wf_uuid if self._wf_uuid else f"cs_{uuid.uuid1()}"
             _topic = f"persistent://{self._tenant}/c8local.{self._fabric}/{self._collection}"
-            _consumer: pulsar.Consumer = _pulsar_client.subscribe(_topic, _sub_name)
+            _consumer: pulsar.Consumer = _pulsar_client.subscribe(_topic, _sub_name, initial_position=pulsar.InitialPosition.Earliest)
 
             # Load existing data
             self.load_existing_data(stream, columns, schema_properties)
             LOGGER.info("Full table sync completed.")
 
             # Change data capture
             while True:
```

### Comparing `macrometa-source-collection-0.0.53/pyproject.toml` & `macrometa-source-collection-0.0.54/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.53'
+version='0.0.54'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.53/setup.py` & `macrometa-source-collection-0.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.53',
+    'version': '0.0.54',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.53/PKG-INFO` & `macrometa-source-collection-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.53
+Version: 0.0.54
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

