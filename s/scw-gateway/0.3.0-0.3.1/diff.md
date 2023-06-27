# Comparing `tmp/scw_gateway-0.3.0.tar.gz` & `tmp/scw_gateway-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_gateway-0.3.0.tar", max compression
+gzip compressed data, was "scw_gateway-0.3.1.tar", max compression
```

## Comparing `scw_gateway-0.3.0.tar` & `scw_gateway-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/__init__.py
--rw-r--r--   0        0        0     4952 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/cli.py
--rw-r--r--   0        0        0      352 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/client.py
--rw-r--r--   0        0        0     2465 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/conf.py
--rw-r--r--   0        0        0     5032 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/gateway.py
--rw-r--r--   0        0        0      281 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/infra/__init__.py
--rw-r--r--   0        0        0     1978 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/cockpit.py
--rw-r--r--   0        0        0     6009 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/container.py
--rw-r--r--   0        0        0      519 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/function.py
--rw-r--r--   0        0        0      317 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/image.py
--rw-r--r--   0        0        0    15463 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/manager.py
--rw-r--r--   0        0        0      999 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/rdb.py
--rw-r--r--   0        0        0     2515 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/secrets.py
--rw-r--r--   0        0        0     1037 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/model.py
--rw-r--r--   0        0        0      923 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 scw_gateway-0.3.0/setup.py
--rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 scw_gateway-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:20.419057 scw_gateway-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:20.419057 scw_gateway-0.3.1/cli/__init__.py
+-rw-r--r--   0        0        0     4952 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/cli.py
+-rw-r--r--   0        0        0      352 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/client.py
+-rw-r--r--   0        0        0     2465 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/conf.py
+-rw-r--r--   0        0        0     5707 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/gateway.py
+-rw-r--r--   0        0        0      281 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/__init__.py
+-rw-r--r--   0        0        0     1978 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/cockpit.py
+-rw-r--r--   0        0        0     6009 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/container.py
+-rw-r--r--   0        0        0      519 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/function.py
+-rw-r--r--   0        0        0      317 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/image.py
+-rw-r--r--   0        0        0    15463 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/manager.py
+-rw-r--r--   0        0        0      999 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/rdb.py
+-rw-r--r--   0        0        0     2515 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/secrets.py
+-rw-r--r--   0        0        0     1037 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/model.py
+-rw-r--r--   0        0        0      923 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 scw_gateway-0.3.1/setup.py
+-rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 scw_gateway-0.3.1/PKG-INFO
```

### Comparing `scw_gateway-0.3.0/cli/cli.py` & `scw_gateway-0.3.1/cli/cli.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.0/cli/conf.py` & `scw_gateway-0.3.1/cli/conf.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.0/cli/infra/cockpit.py` & `scw_gateway-0.3.1/cli/infra/cockpit.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.0/cli/infra/container.py` & `scw_gateway-0.3.1/cli/infra/container.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.0/cli/infra/function.py` & `scw_gateway-0.3.1/cli/infra/function.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.0/cli/infra/manager.py` & `scw_gateway-0.3.1/cli/infra/manager.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.0/cli/infra/rdb.py` & `scw_gateway-0.3.1/cli/infra/rdb.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.0/cli/infra/secrets.py` & `scw_gateway-0.3.1/cli/infra/secrets.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.0/cli/model.py` & `scw_gateway-0.3.1/cli/model.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.0/pyproject.toml` & `scw_gateway-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scw-gateway"
-version = "0.3.0"
+version = "0.3.1"
 description = "CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem"
 authors = ["Simon Shillaker <sshillaker@scaleway.com>"]
 readme = "README.md"
 packages = [{ include = "cli" }]
 
 [tool.poetry.dependencies]
 loguru = "0.6.0"
```

### Comparing `scw_gateway-0.3.0/setup.py` & `scw_gateway-0.3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'scaleway>=0.12.0,<0.13.0']
 
 entry_points = \
 {'console_scripts': ['scwgw = cli.cli:cli']}
 
 setup_kwargs = {
     'name': 'scw-gateway',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem',
     'long_description': '',
     'author': 'Simon Shillaker',
     'author_email': 'sshillaker@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scw_gateway-0.3.0/PKG-INFO` & `scw_gateway-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scw-gateway
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem
 Author: Simon Shillaker
 Author-email: sshillaker@scaleway.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

