# Comparing `tmp/resotodatalink-1.1.0.tar.gz` & `tmp/resotodatalink-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotodatalink-1.1.0.tar", last modified: Mon Jun 19 19:54:43 2023, max compression
+gzip compressed data, was "resotodatalink-1.2.0.tar", last modified: Tue Jun 27 13:00:56 2023, max compression
```

## Comparing `resotodatalink-1.1.0.tar` & `resotodatalink-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/resotodatalink/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/resotodatalink/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/arrow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/arrow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/arrow/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/arrow/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/batch_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/collect_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/remote_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/show_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/resotodatalink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-19 19:54:43.000000 resotodatalink-1.1.0/resotodatalink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-19 19:54:43.000000 resotodatalink-1.1.0/resotodatalink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:54:43.000000 resotodatalink-1.1.0/resotodatalink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-19 19:54:43.000000 resotodatalink-1.1.0/resotodatalink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 19:54:43.000000 resotodatalink-1.1.0/resotodatalink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:00:56.680235 resotodatalink-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-27 13:00:56.680235 resotodatalink-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:00:56.676235 resotodatalink-1.2.0/resotodatalink/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:00:56.680235 resotodatalink-1.2.0/resotodatalink/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/arrow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/arrow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/arrow/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/arrow/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/batch_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/collect_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/remote_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/show_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-06-27 12:56:05.000000 resotodatalink-1.2.0/resotodatalink/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:00:56.676235 resotodatalink-1.2.0/resotodatalink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-27 13:00:56.000000 resotodatalink-1.2.0/resotodatalink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-27 13:00:56.000000 resotodatalink-1.2.0/resotodatalink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:00:56.000000 resotodatalink-1.2.0/resotodatalink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-27 13:00:56.000000 resotodatalink-1.2.0/resotodatalink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 13:00:56.000000 resotodatalink-1.2.0/resotodatalink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-27 13:00:56.680235 resotodatalink-1.2.0/setup.cfg
```

### Comparing `resotodatalink-1.1.0/LICENSE` & `resotodatalink-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.1.0/PKG-INFO` & `resotodatalink-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotodatalink
-Version: 1.1.0
+Version: 1.2.0
 Summary: Data Pipelines for Resoto infrastructure data.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotodatalink-1.1.0/pyproject.toml` & `resotodatalink-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotodatalink"
-version = "1.1.0"
+version = "1.2.0"
 authors = [{name="Some Engineering Inc."}]
 description = "Data Pipelines for Resoto infrastructure data."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -25,18 +25,18 @@
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 keywords = ["data source", "data sink", "data synchronization", "data pipeline"]
 
 dependencies = [
     "networkx",
-    "resotoclient",
+    "resotoclient>=1.5.0",
     "resotolib",
     "rich",
-    "sqlalchemy==1.4.45",
+    "sqlalchemy>=1.4.48,<2",
 ]
 
 [project.optional-dependencies]
 
 # The different database backends we have tested explicitly
 snowflake = [ "snowflake-sqlalchemy" ]
 mysql = [ "pymysql" ]
```

### Comparing `resotodatalink-1.1.0/requirements-all.txt` & `resotodatalink-1.2.0/requirements-all.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 asn1crypto==1.5.1
 astroid==2.15.5
 async-timeout==4.0.2
 attrs==23.1.0
 autocommand==2.2.2
 backoff==2.2.1
 black==23.3.0
-boto3==1.26.152
-botocore==1.29.152
+boto3==1.26.161
+botocore==1.29.161
 brotli==1.0.9
 build==0.10.0
 cachetools==5.3.1
 cattrs==23.1.2
 certifi==2023.5.7
 cffi==1.15.1
 chardet==5.1.0
@@ -25,105 +25,105 @@
 coverage[toml]==7.2.7
 cryptography==40.0.2
 dill==0.3.6
 distlib==0.3.6
 filelock==3.12.2
 flake8==6.0.0
 frozenlist==1.3.3
-google-api-core==2.11.0
-google-auth==2.19.1
+google-api-core==2.11.1
+google-auth==2.21.0
 google-cloud-core==2.3.2
-google-cloud-storage==2.9.0
+google-cloud-storage==2.10.0
 google-crc32c==1.5.0
 google-resumable-media==2.5.0
 googleapis-common-protos==1.59.1
-hypothesis==6.78.2
+hypothesis==6.79.3
 idna==3.4
 inflect==6.0.4
 iniconfig==2.0.0
 isort==5.12.0
-jaraco-collections==4.2.0
+jaraco-collections==4.3.0
 jaraco-context==4.3.0
-jaraco-functools==3.7.0
+jaraco-functools==3.8.0
 jaraco-text==3.11.1
 jmespath==1.0.1
 jsons==1.6.3
 lazy-object-proxy==1.9.0
 markdown-it-py==3.0.0
 mccabe==0.7.0
 mdurl==0.1.2
 monotonic==1.6
 more-itertools==9.1.0
 multidict==6.0.4
-mypy==1.3.0
+mypy==1.4.1
 mypy-extensions==1.0.0
 networkx==3.1
-numpy==1.24.3
+numpy==1.25.0
 oscrypto==1.3.0
 packaging==23.1
 parsy==2.1
 pathspec==0.11.1
 pep8-naming==0.13.3
 pint==0.22
 pip-tools==6.13.0
-platformdirs==3.5.3
-pluggy==1.0.0
+platformdirs==3.8.0
+pluggy==1.2.0
 portend==3.1.0
 posthog==3.0.1
 prometheus-client==0.17.0
-protobuf==4.23.2
+protobuf==4.23.3
 psutil==5.9.5
 psycopg2-binary==2.9.6
 pyarrow==12.0.1
 pyasn1==0.5.0
 pyasn1-modules==0.3.0
 pycares==4.3.0
 pycodestyle==2.10.0
 pycparser==2.21
 pycryptodomex==3.18.0
 pydantic==1.10.9
 pyflakes==3.0.1
 pygments==2.15.1
 pyjwt==2.7.0
 pylint==2.17.4
-pymysql==1.0.3
+pymysql==1.1.0
 pyopenssl==23.2.0
-pyproject-api==1.5.1
+pyproject-api==1.5.2
 pyproject-hooks==1.0.0
-pytest==7.3.2
+pytest==7.4.0
 pytest-asyncio==0.21.0
 pytest-cov==4.1.0
 pytest-runner==6.0.0
 python-dateutil==2.8.2
 pytz==2023.3
 pyyaml==6.0
 requests==2.31.0
-resoto-plugin-example-collector==3.5.2
-resotoclient==1.4.1
-resotolib==3.5.2
+resoto-plugin-example-collector==3.5.3
+resotoclient==1.5.0
+resotolib==3.5.3
 rich==13.4.2
 rsa==4.9
 s3transfer==0.6.1
 six==1.16.0
 snowflake-connector-python==3.0.4
 snowflake-sqlalchemy==1.4.7
 sortedcontainers==2.4.0
-sqlalchemy==1.4.45
-tempora==5.3.0
+sqlalchemy==1.4.48
+tempora==5.5.0
 tomlkit==0.11.8
-tox==4.6.0
+tox==4.6.3
 typeguard==4.0.0
 typing-extensions==4.6.3
 typish==1.9.3
 tzdata==2023.3
 tzlocal==5.0.1
 urllib3==1.26.16
-virtualenv==20.23.0
-websocket-client==1.5.3
+virtualenv==20.23.1
+websocket-client==1.6.1
 wheel==0.40.0
 wrapt==1.15.0
 yarl==1.9.2
 zc-lockfile==3.0.post1
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==23.1.2
-setuptools==67.8.0
+setuptools==68.0.0
```

### Comparing `resotodatalink-1.1.0/requirements.txt` & `resotodatalink-1.2.0/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 aiodns==3.0.0
 aiohttp[speedups]==3.8.4
 aiosignal==1.3.1
 asn1crypto==1.5.1
 async-timeout==4.0.2
 attrs==23.1.0
 autocommand==2.2.2
-boto3==1.26.152
-botocore==1.29.152
+boto3==1.26.161
+botocore==1.29.161
 brotli==1.0.9
 cachetools==5.3.1
 cattrs==23.1.2
 certifi==2023.5.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 cheroot==10.0.0
 cherrypy==18.8.0
 cryptography==40.0.2
 filelock==3.12.2
 frozenlist==1.3.3
-google-api-core==2.11.0
-google-auth==2.19.1
+google-api-core==2.11.1
+google-auth==2.21.0
 google-cloud-core==2.3.2
-google-cloud-storage==2.9.0
+google-cloud-storage==2.10.0
 google-crc32c==1.5.0
 google-resumable-media==2.5.0
 googleapis-common-protos==1.59.1
 idna==3.4
 inflect==6.0.4
-jaraco-collections==4.2.0
+jaraco-collections==4.3.0
 jaraco-context==4.3.0
-jaraco-functools==3.7.0
+jaraco-functools==3.8.0
 jaraco-text==3.11.1
 jmespath==1.0.1
 jsons==1.6.3
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==9.1.0
 multidict==6.0.4
 networkx==3.1
-numpy==1.24.3
+numpy==1.25.0
 oscrypto==1.3.0
 packaging==23.1
 parsy==2.1
 pint==0.22
 portend==3.1.0
 prometheus-client==0.17.0
-protobuf==4.23.2
+protobuf==4.23.3
 psutil==5.9.5
 psycopg2-binary==2.9.6
 pyarrow==12.0.1
 pyasn1==0.5.0
 pyasn1-modules==0.3.0
 pycares==4.3.0
 pycparser==2.21
 pycryptodomex==3.18.0
 pydantic==1.10.9
 pygments==2.15.1
 pyjwt==2.7.0
-pymysql==1.0.3
+pymysql==1.1.0
 pyopenssl==23.2.0
 python-dateutil==2.8.2
 pytz==2023.3
 pyyaml==6.0
 requests==2.31.0
-resotoclient==1.4.1
-resotolib==3.5.2
+resotoclient==1.5.0
+resotolib==3.5.3
 rich==13.4.2
 rsa==4.9
 s3transfer==0.6.1
 six==1.16.0
 snowflake-connector-python==3.0.4
 snowflake-sqlalchemy==1.4.7
 sortedcontainers==2.4.0
-sqlalchemy==1.4.45
-tempora==5.3.0
+sqlalchemy==1.4.48
+tempora==5.5.0
 typeguard==4.0.0
 typing-extensions==4.6.3
 typish==1.9.3
 tzdata==2023.3
 tzlocal==5.0.1
 urllib3==1.26.16
-websocket-client==1.5.3
+websocket-client==1.6.1
 yarl==1.9.2
 zc-lockfile==3.0.post1
 
 # The following packages are considered to be unsafe in a requirements file:
-setuptools==67.8.0
+setuptools==68.0.0
```

### Comparing `resotodatalink-1.1.0/resotodatalink/analytics.py` & `resotodatalink-1.2.0/resotodatalink/analytics.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.1.0/resotodatalink/arrow/config.py` & `resotodatalink-1.2.0/resotodatalink/arrow/config.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.1.0/resotodatalink/arrow/model.py` & `resotodatalink-1.2.0/resotodatalink/arrow/model.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.1.0/resotodatalink/arrow/type_converter.py` & `resotodatalink-1.2.0/resotodatalink/arrow/type_converter.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.1.0/resotodatalink/arrow/writer.py` & `resotodatalink-1.2.0/resotodatalink/arrow/writer.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.1.0/resotodatalink/batch_stream.py` & `resotodatalink-1.2.0/resotodatalink/batch_stream.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.1.0/resotodatalink/collect_plugins.py` & `resotodatalink-1.2.0/resotodatalink/collect_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
 from logging import getLogger
-from typing import List, Tuple, Set, Optional, AsyncIterator, Union, cast, Dict, TypeVar, Awaitable
+from typing import List, Tuple, Set, Optional, AsyncIterator, Union, cast, Dict, TypeVar, Awaitable, Any
 
 import jsons
 from resotoclient import Kind, Model
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.baseresources import BaseResource, EdgeType
 from resotolib.core.actions import CoreFeedback
 from resotolib.types import Json
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, text
 
 from resotodatalink import EngineConfig
 from resotodatalink.arrow.config import ArrowOutputConfig
 from resotodatalink.batch_stream import BatchStream
 from resotodatalink.sql import sql_updater
 
 try:
@@ -23,15 +23,15 @@
     ArrowModel = type(None)  # type: ignore
     ArrowWriter = type(None)  # type: ignore
 
 log = getLogger("resoto.datalink")
 T = TypeVar("T")
 
 
-def collect_to_file(
+async def collect_to_file(
     collector: BaseCollectorPlugin, feedback: CoreFeedback, output_config: ArrowOutputConfig
 ) -> Tuple[str, int, int]:
     # collect cloud data
     feedback.progress_done(collector.cloud, 0, 1)
     collector.collect()
     # read the kinds created from this collector
     # Note: Kind is a dataclass - from_json can only handle attrs
@@ -58,15 +58,15 @@
             return node_by_chksum[fr].kind, node_by_chksum[to].kind
         elif node["type"] == "node":
             return cast(str, node["reported"]["kind"])
         else:
             raise ValueError(f"Unknown node type {node['type']}")
 
     stream = BatchStream.from_graph(collector, key_fn, output_config.batch_size, len(collector.graph.nodes))
-    asyncio.run(write_file(output_config, model, stream, edges_by_kind, feedback, node_edge_count))
+    await write_file(output_config, model, stream, edges_by_kind, feedback, node_edge_count)
 
     feedback.progress_done(collector.cloud, 1, 1)
     return collector.cloud, len(collector.graph.nodes), len(collector.graph.edges)
 
 
 async def write_file(
     output_config: ArrowOutputConfig,
@@ -96,15 +96,15 @@
                     feedback.progress_done("sync_db", ne_current, node_edge_count)
         finally:
             writer.close()
 
     await __run_on_thread(run_on_thread())
 
 
-def collect_sql(
+async def collect_sql(
     collector: BaseCollectorPlugin,
     engine_config: EngineConfig,
     feedback: CoreFeedback,
     swap_temp_tables: bool = False,
     drop_existing_tables: bool = False,
 ) -> Tuple[str, int, int]:
     # collect cloud data
@@ -134,25 +134,23 @@
             return node_by_chksum[fr].kind, node_by_chksum[to].kind
         elif node["type"] == "node":
             return cast(str, node["reported"]["kind"])
         else:
             raise ValueError(f"Unknown node type {node['type']}")
 
     stream = BatchStream.from_graph(collector, key_fn, engine_config.batch_size, len(collector.graph.nodes))
-    asyncio.run(
-        update_sql(
-            engine_config,
-            model,
-            stream,
-            edges_by_kind,
-            swap_temp_tables,
-            drop_existing_tables,
-            feedback.with_context(collector.cloud),
-            len(collector.graph.nodes) + len(collector.graph.edges),
-        )
+    await update_sql(
+        engine_config,
+        model,
+        stream,
+        edges_by_kind,
+        swap_temp_tables,
+        drop_existing_tables,
+        feedback.with_context(collector.cloud),
+        len(collector.graph.nodes) + len(collector.graph.edges),
     )
     feedback.progress_done(collector.cloud, 1, 1)
     return collector.cloud, len(collector.graph.nodes), len(collector.graph.edges)
 
 
 async def update_sql(
     engine_config: EngineConfig,
@@ -215,14 +213,25 @@
 
             if swap_temp_tables:
                 updater.swap_temp_tables(conn, drop_existing_tables)
 
     await __run_on_thread(run_on_thread())
 
 
+async def execute_sql(
+    engine_config: EngineConfig, sql: str, bind_vars: Optional[Dict[str, Any]] = None
+) -> AsyncIterator[Json]:
+    engine = create_engine(engine_config.connection_string)
+    with engine.connect() as conn:
+        with conn.begin():
+            result_set = conn.execute(text(sql), bind_vars)
+            for row in result_set:
+                yield dict(row)
+
+
 async def __run_on_thread(awaitable: Awaitable[T]) -> T:
     """
     Run the async awaitable on a new thread.
     """
 
     def run_in_new_loop(lp: asyncio.AbstractEventLoop) -> T:
         asyncio.set_event_loop(lp)
```

### Comparing `resotodatalink-1.1.0/resotodatalink/remote_graph.py` & `resotodatalink-1.2.0/resotodatalink/remote_graph.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.1.0/resotodatalink/schema_utils.py` & `resotodatalink-1.2.0/resotodatalink/schema_utils.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.1.0/resotodatalink/show_progress.py` & `resotodatalink-1.2.0/resotodatalink/show_progress.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.1.0/resotodatalink/snowflake.py` & `resotodatalink-1.2.0/resotodatalink/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from resotodatalink.schema_utils import kind_properties, get_table_name
 from resotodatalink.sql import SqlDefaultUpdater, DialectUpdater
 
 log = logging.getLogger("resoto.datalink")
 
 
-def kind_to_snowflake_type(kind_name: str, model: Model) -> Any:  # Type[TypeEngine[Any]]
+def kind_to_snowflake_type(kind_name: str, model: Model, **kwargs: Any) -> Any:  # Type[TypeEngine[Any]]
     """
     Map internal kinds to snowflake types.
     More or less the default mapping, but with some special cases for OBJECT and ARRAY types.
     """
     kind = model.kinds.get(kind_name)
     if "[]" in kind_name:
         return ARRAY
```

### Comparing `resotodatalink-1.1.0/resotodatalink/sql.py` & `resotodatalink-1.2.0/resotodatalink/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Column,
     Float,
     Integer,
     JSON,
     MetaData,
     String,
     Table,
+    Text,
     DDL,
     DateTime,
     Date,
     TypeDecorator,
 )
 from sqlalchemy.engine import Engine, Connection, Dialect
 from sqlalchemy.sql.ddl import DropTable, DropConstraint
@@ -65,15 +66,15 @@
     def process_bind_param(self, value: Optional[str], dialect: Dialect) -> Optional[date]:
         return date.fromisoformat(value) if value else None
 
     def process_result_value(self, value: Optional[datetime], dialect: Dialect) -> Optional[str]:
         return value.strftime("%Y-%m-%d") if value else None
 
 
-def sql_kind_to_column_type(kind_name: str, model: Model) -> Any:  # Type[TypeEngine[Any]]
+def sql_kind_to_column_type(kind_name: str, model: Model, **kwargs: Any) -> Any:  # Type[TypeEngine[Any]]
     kind = model.kinds.get(kind_name)
     if "[]" in kind_name:
         return JSON
     elif kind_name.startswith("dict"):
         return JSON
     elif kind_name == "any":
         return JSON
@@ -84,18 +85,26 @@
     elif kind_name == "double":
         return Float  # use Double with sqlalchemy 2
     elif kind_name == "datetime":
         return DateTimeString
     elif kind_name == "date":
         return DateString
     elif kind_name in ("string", "duration"):
-        return String
+        if isinstance(str_len := kwargs.get("len"), int):
+            if str_len > 1024:
+                return Text
+            elif str_len < 32:
+                return String(32)
+            elif str_len >= 1:
+                return String(2 ** (str_len - 1).bit_length())
+        # if we come here no or invalid len was provided, default to 255 characters
+        return String(255)
     elif kind_name == "boolean":
         return Boolean
-    elif kind and kind.properties:  # complex kind
+    elif kind and kind.properties is not None:  # complex kind
         return JSON
     elif kind and kind.runtime_kind is not None:  # refined simple type like enum
         return sql_kind_to_column_type(kind.runtime_kind, model)
     else:
         raise ValueError(f"Not able to handle kind {kind_name}")
 
 
@@ -169,36 +178,31 @@
 
     def create_schema(self, connection: Connection, edges: List[Tuple[str, str]]) -> MetaData:
         log.info(f"Create schema for {len(self.table_kinds)} kinds and their relationships")
 
         def table_schema(kind: Kind) -> None:
             table_name = get_table_name(kind.fqn)
             if table_name not in self.metadata.tables:
-                properties, _ = kind_properties(kind, self.model, with_id=False)
-                Table(
-                    get_table_name(kind.fqn),
-                    self.metadata,
-                    *[
-                        Column("_id", String, primary_key=True),
-                        *[Column(p.name, self.column_types_fn(p.kind, self.model)) for p in properties],
-                    ],
-                )
+                pr, _ = kind_properties(kind, self.model, with_id=False)
+                columns = [Column(p.name, self.column_types_fn(p.kind, self.model, **(p.metadata or {}))) for p in pr]
+                idc = Column("_id", String(255), primary_key=True)
+                Table(get_table_name(kind.fqn), self.metadata, *[idc, *columns])
 
         def link_table_schema(from_kind: str, to_kind: str) -> None:
             from_table = get_table_name(from_kind)
             to_table = get_table_name(to_kind)
             link_table = get_link_table_name(from_kind, to_kind)
             if (
                 link_table not in self.metadata.tables
                 and from_table in self.metadata.tables
                 and to_table in self.metadata.tables
             ):
                 # defining a foreign key constraint on a table that does not exist yet, will fail
                 # defining it on the current tmp table setup is possible, but this will not reset during table rename
-                Table(link_table, self.metadata, Column("from_id", String), Column("to_id", String))
+                Table(link_table, self.metadata, Column("from_id", String(255)), Column("to_id", String(255)))
 
         def link_table_schema_from_successors(kind: Kind) -> None:
             _, successors = kind_properties(kind, self.model)
             # create link table for all linked entities
             for successor in successors:
                 link_table_schema(kind.fqn, successor)
```

### Comparing `resotodatalink-1.1.0/resotodatalink.egg-info/PKG-INFO` & `resotodatalink-1.2.0/resotodatalink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotodatalink
-Version: 1.1.0
+Version: 1.2.0
 Summary: Data Pipelines for Resoto infrastructure data.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotodatalink-1.1.0/resotodatalink.egg-info/SOURCES.txt` & `resotodatalink-1.2.0/resotodatalink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

