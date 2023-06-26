# Comparing `tmp/wf_postgres_client-0.1.0.tar.gz` & `tmp/wf_postgres_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_postgres_client-0.1.0.tar", max compression
+gzip compressed data, was "wf_postgres_client-0.1.1.tar", max compression
```

## Comparing `wf_postgres_client-0.1.0.tar` & `wf_postgres_client-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1088 2023-05-27 00:02:23.477415 wf_postgres_client-0.1.0/LICENSE
--rw-r--r--   0        0        0      533 2023-05-27 00:13:58.563639 wf_postgres_client-0.1.0/README.md
--rw-r--r--   0        0        0      450 2023-06-26 19:15:53.275725 wf_postgres_client-0.1.0/postgres_client/__init__.py
--rw-r--r--   0        0        0     3200 2023-06-26 19:15:33.404097 wf_postgres_client-0.1.0/postgres_client/core.py
--rw-r--r--   0        0        0     5672 2023-06-26 19:15:43.395910 wf_postgres_client-0.1.0/postgres_client/utils.py
--rw-r--r--   0        0        0     1048 2023-06-25 23:46:16.031468 wf_postgres_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 wf_postgres_client-0.1.0/setup.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 wf_postgres_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-27 00:02:23.477415 wf_postgres_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0      533 2023-05-27 00:13:58.563639 wf_postgres_client-0.1.1/README.md
+-rw-r--r--   0        0        0      576 2023-06-26 23:12:51.174886 wf_postgres_client-0.1.1/postgres_client/__init__.py
+-rw-r--r--   0        0        0     3200 2023-06-26 19:15:33.404097 wf_postgres_client-0.1.1/postgres_client/core.py
+-rw-r--r--   0        0        0     5672 2023-06-26 19:15:43.395910 wf_postgres_client-0.1.1/postgres_client/utils.py
+-rw-r--r--   0        0        0     1048 2023-06-26 23:14:17.245124 wf_postgres_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 wf_postgres_client-0.1.1/setup.py
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 wf_postgres_client-0.1.1/PKG-INFO
```

### Comparing `wf_postgres_client-0.1.0/LICENSE` & `wf_postgres_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_postgres_client-0.1.0/README.md` & `wf_postgres_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wf_postgres_client-0.1.0/postgres_client/core.py` & `wf_postgres_client-0.1.1/postgres_client/core.py`

 * *Files identical despite different names*

### Comparing `wf_postgres_client-0.1.0/postgres_client/utils.py` & `wf_postgres_client-0.1.1/postgres_client/utils.py`

 * *Files identical despite different names*

### Comparing `wf_postgres_client-0.1.0/pyproject.toml` & `wf_postgres_client-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-postgres-client"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-postgres-client"
-version = "0.1.0"
+version = "0.1.1"
 description = "A client for communicating with PostgreSQL databases"
 authors = ["Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 readme = "README.md"
 keywords = []
 repository = "https://github.com/WildflowerSchools/wf-postgres-client"
 license = "MIT"
```

### Comparing `wf_postgres_client-0.1.0/setup.py` & `wf_postgres_client-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.5,<2.0', 'psycopg2>=2.9,<3.0', 'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'wf-postgres-client',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A client for communicating with PostgreSQL databases',
     'long_description': '# postgres_client\n\nA client for communicating with PostgreSQL databases\n\n## Installation\n\n`pip install wf-postgres-client`\n\n## Development\n\n### Requirements\n\n* [Poetry](https://python-poetry.org/)\n* [just](https://github.com/casey/just)\n\n### Install\n\n`poetry install`\n\n\n#### Install w/ Python Version from PyEnv\n\n```\n# Specify pyenv python version\npyenv shell --unset\npyenv local <<VERSION>>\n\n# Set poetry python to pyenv version\npoetry env use $(pyenv which python)\npoetry cache clear . --all\npoetry install\n```\n\n## Task list\n* TBD\n',
     'author': 'Theodore Quinn',
     'author_email': 'ted.quinn@wildflowerschools.org',
     'maintainer': 'Theodore Quinn',
     'maintainer_email': 'ted.quinn@wildflowerschools.org',
     'url': 'https://github.com/WildflowerSchools/wf-postgres-client',
```

### Comparing `wf_postgres_client-0.1.0/PKG-INFO` & `wf_postgres_client-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-postgres-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A client for communicating with PostgreSQL databases
 Home-page: https://github.com/WildflowerSchools/wf-postgres-client
 License: MIT
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 Maintainer: Theodore Quinn
 Maintainer-email: ted.quinn@wildflowerschools.org
```

