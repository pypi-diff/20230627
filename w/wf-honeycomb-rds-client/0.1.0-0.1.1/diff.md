# Comparing `tmp/wf_honeycomb_rds_client-0.1.0.tar.gz` & `tmp/wf_honeycomb_rds_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_honeycomb_rds_client-0.1.0.tar", max compression
+gzip compressed data, was "wf_honeycomb_rds_client-0.1.1.tar", max compression
```

## Comparing `wf_honeycomb_rds_client-0.1.0.tar` & `wf_honeycomb_rds_client-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1088 2023-06-26 20:37:02.570215 wf_honeycomb_rds_client-0.1.0/LICENSE
--rw-r--r--   0        0        0      560 2023-06-26 20:41:41.572706 wf_honeycomb_rds_client-0.1.0/README.md
--rw-r--r--   0        0        0      429 2023-06-26 20:37:02.570215 wf_honeycomb_rds_client-0.1.0/honeycomb_rds_client/__init__.py
--rw-r--r--   0        0        0     6995 2023-06-26 20:59:58.271561 wf_honeycomb_rds_client-0.1.0/honeycomb_rds_client/core.py
--rw-r--r--   0        0        0     1122 2023-06-26 20:57:04.414890 wf_honeycomb_rds_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 wf_honeycomb_rds_client-0.1.0/setup.py
--rw-r--r--   0        0        0     1697 1970-01-01 00:00:00.000000 wf_honeycomb_rds_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-26 20:37:02.570215 wf_honeycomb_rds_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0      560 2023-06-26 20:41:41.572706 wf_honeycomb_rds_client-0.1.1/README.md
+-rw-r--r--   0        0        0      555 2023-06-26 23:15:19.471852 wf_honeycomb_rds_client-0.1.1/honeycomb_rds_client/__init__.py
+-rw-r--r--   0        0        0     6995 2023-06-26 20:59:58.271561 wf_honeycomb_rds_client-0.1.1/honeycomb_rds_client/core.py
+-rw-r--r--   0        0        0     1122 2023-06-26 23:16:02.838966 wf_honeycomb_rds_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 wf_honeycomb_rds_client-0.1.1/setup.py
+-rw-r--r--   0        0        0     1697 1970-01-01 00:00:00.000000 wf_honeycomb_rds_client-0.1.1/PKG-INFO
```

### Comparing `wf_honeycomb_rds_client-0.1.0/LICENSE` & `wf_honeycomb_rds_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_honeycomb_rds_client-0.1.0/README.md` & `wf_honeycomb_rds_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wf_honeycomb_rds_client-0.1.0/honeycomb_rds_client/core.py` & `wf_honeycomb_rds_client-0.1.1/honeycomb_rds_client/core.py`

 * *Files identical despite different names*

### Comparing `wf_honeycomb_rds_client-0.1.0/pyproject.toml` & `wf_honeycomb_rds_client-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-honeycomb-rds-client"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-honeycomb-rds-client"
-version = "0.1.0"
+version = "0.1.1"
 description = "A client for communicating with the RDS database underlying Honeycomb"
 authors = ["Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 readme = "README.md"
 keywords = []
 repository = "https://github.com/WildflowerSchools/wf-honeycomb-rds-client"
 license = "MIT"
```

### Comparing `wf_honeycomb_rds_client-0.1.0/setup.py` & `wf_honeycomb_rds_client-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['pandas>=1.5,<2.0',
  'toml>=0.10.2,<0.11.0',
  'wf-honeycomb-io>=2.1,<3.0',
  'wf-postgres-client>=0.1.0,<0.2.0']
 
 setup_kwargs = {
     'name': 'wf-honeycomb-rds-client',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A client for communicating with the RDS database underlying Honeycomb',
     'long_description': '# honeycomb_rds_client\n\nA client for communicating with the RDS database underlying Honeycomb\n\n## Installation\n\n`pip install wf-honeycomb-rds-client`\n\n## Development\n\n### Requirements\n\n* [Poetry](https://python-poetry.org/)\n* [just](https://github.com/casey/just)\n\n### Install\n\n`poetry install`\n\n\n#### Install w/ Python Version from PyEnv\n\n```\n# Specify pyenv python version\npyenv shell --unset\npyenv local <<VERSION>>\n\n# Set poetry python to pyenv version\npoetry env use $(pyenv which python)\npoetry cache clear . --all\npoetry install\n```\n\n## Task list\n* TBD\n',
     'author': 'Theodore Quinn',
     'author_email': 'ted.quinn@wildflowerschools.org',
     'maintainer': 'Theodore Quinn',
     'maintainer_email': 'ted.quinn@wildflowerschools.org',
     'url': 'https://github.com/WildflowerSchools/wf-honeycomb-rds-client',
```

### Comparing `wf_honeycomb_rds_client-0.1.0/PKG-INFO` & `wf_honeycomb_rds_client-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-honeycomb-rds-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A client for communicating with the RDS database underlying Honeycomb
 Home-page: https://github.com/WildflowerSchools/wf-honeycomb-rds-client
 License: MIT
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 Maintainer: Theodore Quinn
 Maintainer-email: ted.quinn@wildflowerschools.org
```

