# Comparing `tmp/drupaljsonapiclient-1.0.7.tar.gz` & `tmp/drupaljsonapiclient-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drupaljsonapiclient-1.0.7.tar", max compression
+gzip compressed data, was "drupaljsonapiclient-1.0.8.tar", max compression
```

## Comparing `drupaljsonapiclient-1.0.7.tar` & `drupaljsonapiclient-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1690 2023-06-26 01:45:13.291513 drupaljsonapiclient-1.0.7/LICENSE
--rw-r--r--   0        0        0     1244 2023-06-26 01:45:13.291513 drupaljsonapiclient-1.0.7/README.md
--rw-r--r--   0        0        0      156 2023-06-26 01:45:13.291513 drupaljsonapiclient-1.0.7/drupaljsonapiclient/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-26 01:45:13.292513 drupaljsonapiclient-1.0.7/drupaljsonapiclient/common.py
--rw-r--r--   0        0        0     4383 2023-06-26 01:45:13.292513 drupaljsonapiclient-1.0.7/drupaljsonapiclient/document.py
--rw-r--r--   0        0        0      620 2023-06-26 01:45:13.292513 drupaljsonapiclient-1.0.7/drupaljsonapiclient/exceptions.py
--rw-r--r--   0        0        0     3145 2023-06-26 01:45:13.292513 drupaljsonapiclient-1.0.7/drupaljsonapiclient/filter.py
--rw-r--r--   0        0        0     4283 2023-06-26 01:45:13.292513 drupaljsonapiclient-1.0.7/drupaljsonapiclient/objects.py
--rw-r--r--   0        0        0    14266 2023-06-26 01:45:13.292513 drupaljsonapiclient-1.0.7/drupaljsonapiclient/relationships.py
--rw-r--r--   0        0        0    26615 2023-06-26 01:45:13.292513 drupaljsonapiclient-1.0.7/drupaljsonapiclient/resourceobject.py
--rw-r--r--   0        0        0    28104 2023-06-26 01:45:13.292513 drupaljsonapiclient-1.0.7/drupaljsonapiclient/session.py
--rw-r--r--   0        0        0     1008 2023-06-26 01:45:13.294513 drupaljsonapiclient-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1690 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1244 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/README.md
+-rw-r--r--   0        0        0      156 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/common.py
+-rw-r--r--   0        0        0     4383 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/document.py
+-rw-r--r--   0        0        0      620 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/exceptions.py
+-rw-r--r--   0        0        0     3145 2023-06-27 02:06:45.257616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/filter.py
+-rw-r--r--   0        0        0     4283 2023-06-27 02:06:45.258616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/objects.py
+-rw-r--r--   0        0        0    14266 2023-06-27 02:06:45.258616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/relationships.py
+-rw-r--r--   0        0        0    26615 2023-06-27 02:06:45.258616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/resourceobject.py
+-rw-r--r--   0        0        0    28112 2023-06-27 02:06:45.258616 drupaljsonapiclient-1.0.8/drupaljsonapiclient/session.py
+-rw-r--r--   0        0        0     1008 2023-06-27 02:06:45.259616 drupaljsonapiclient-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.8/PKG-INFO
```

### Comparing `drupaljsonapiclient-1.0.7/LICENSE` & `drupaljsonapiclient-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.7/README.md` & `drupaljsonapiclient-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.7/drupaljsonapiclient/common.py` & `drupaljsonapiclient-1.0.8/drupaljsonapiclient/common.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.7/drupaljsonapiclient/document.py` & `drupaljsonapiclient-1.0.8/drupaljsonapiclient/document.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.7/drupaljsonapiclient/exceptions.py` & `drupaljsonapiclient-1.0.8/drupaljsonapiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.7/drupaljsonapiclient/filter.py` & `drupaljsonapiclient-1.0.8/drupaljsonapiclient/filter.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.7/drupaljsonapiclient/objects.py` & `drupaljsonapiclient-1.0.8/drupaljsonapiclient/objects.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.7/drupaljsonapiclient/relationships.py` & `drupaljsonapiclient-1.0.8/drupaljsonapiclient/relationships.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.7/drupaljsonapiclient/resourceobject.py` & `drupaljsonapiclient-1.0.8/drupaljsonapiclient/resourceobject.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.7/drupaljsonapiclient/session.py` & `drupaljsonapiclient-1.0.8/drupaljsonapiclient/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         more_fields.update(fields)
 
         for key, value in more_fields.items():
             if key not in fields:
                 key = jsonify_attribute_name(key)
             props = schema['properties'].get(key, {})
             if 'relation' in props:
-                res_types = props['resource']
+                res_types = props.get('resource', [])
                 if isinstance(value, RESOURCE_TYPES + (str,)):
                     value = self._value_to_dict(value, res_types)
                 elif isinstance(value, collections.abc.Iterable):
                     value = [self._value_to_dict(id_, res_types) for id_ in value]
                 rels[key] = {'data': value}
             else:
                 key = key.split('.')
```

### Comparing `drupaljsonapiclient-1.0.7/pyproject.toml` & `drupaljsonapiclient-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drupaljsonapiclient"
-version = "1.0.7"
+version = "1.0.8"
 description = "Drupal CMS JSON:API client for Python."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drupaljsonapiclient"}]
 repository = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient"
 documentation = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient/-/blob/main/README.md"
```

### Comparing `drupaljsonapiclient-1.0.7/PKG-INFO` & `drupaljsonapiclient-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drupaljsonapiclient
-Version: 1.0.7
+Version: 1.0.8
 Summary: Drupal CMS JSON:API client for Python.
 Home-page: https://gitlab.com/martins-bruvelis/drupaljsonapiclient
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

