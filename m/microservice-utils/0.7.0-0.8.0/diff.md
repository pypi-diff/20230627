# Comparing `tmp/microservice-utils-0.7.0.tar.gz` & `tmp/microservice-utils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservice-utils-0.7.0.tar", last modified: Fri Mar 31 18:42:50 2023, max compression
+gzip compressed data, was "microservice-utils-0.8.0.tar", last modified: Tue Jun 27 18:48:07 2023, max compression
```

## Comparing `microservice-utils-0.7.0.tar` & `microservice-utils-0.8.0.tar`

### file list

```diff
@@ -1,35 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:50.860133 microservice-utils-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-31 18:42:50.860133 microservice-utils-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:50.856133 microservice-utils-0.7.0/microservice_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:50.860133 microservice-utils-0.7.0/microservice_utils/google_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/google_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:50.860133 microservice-utils-0.7.0/microservice_utils/google_cloud/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/google_cloud/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/google_cloud/adapters/cloud_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/google_cloud/adapters/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/google_cloud/adapters/cloud_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/google_cloud/adapters/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/google_cloud/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/microservice_utils/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:50.860133 microservice-utils-0.7.0/microservice_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-31 18:42:50.000000 microservice-utils-0.7.0/microservice_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-31 18:42:50.000000 microservice-utils-0.7.0/microservice_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 18:42:50.000000 microservice-utils-0.7.0/microservice_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-31 18:42:50.000000 microservice-utils-0.7.0/microservice_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-31 18:42:50.000000 microservice-utils-0.7.0/microservice_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 18:42:50.860133 microservice-utils-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:50.860133 microservice-utils-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:50.860133 microservice-utils-0.7.0/tests/google_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/tests/google_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/tests/google_cloud/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/tests/google_cloud/test_cloud_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/tests/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-03-31 18:42:41.000000 microservice-utils-0.7.0/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:48:07.565721 microservice-utils-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-27 18:48:07.565721 microservice-utils-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:48:07.557721 microservice-utils-0.8.0/microservice_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:48:07.561721 microservice-utils-0.8.0/microservice_utils/google_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/google_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:48:07.561721 microservice-utils-0.8.0/microservice_utils/google_cloud/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/google_cloud/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/google_cloud/adapters/cloud_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/google_cloud/adapters/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/google_cloud/adapters/cloud_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/google_cloud/adapters/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/google_cloud/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:48:07.561721 microservice-utils-0.8.0/microservice_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/openai/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:48:07.561721 microservice-utils-0.8.0/microservice_utils/pinecone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/pinecone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/microservice_utils/pinecone/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:48:07.561721 microservice-utils-0.8.0/microservice_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-27 18:48:07.000000 microservice-utils-0.8.0/microservice_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-27 18:48:07.000000 microservice-utils-0.8.0/microservice_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:48:07.000000 microservice-utils-0.8.0/microservice_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 18:48:07.000000 microservice-utils-0.8.0/microservice_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 18:48:07.000000 microservice-utils-0.8.0/microservice_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:48:07.565721 microservice-utils-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:48:07.561721 microservice-utils-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:48:07.565721 microservice-utils-0.8.0/tests/google_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/tests/google_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/tests/google_cloud/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/tests/google_cloud/test_cloud_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/tests/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:48:07.565721 microservice-utils-0.8.0/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/tests/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/tests/openai/test_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-27 18:46:40.000000 microservice-utils-0.8.0/tests/test_events.py
```

### Comparing `microservice-utils-0.7.0/LICENSE` & `microservice-utils-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.7.0/PKG-INFO` & `microservice-utils-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: microservice-utils
-Version: 0.7.0
+Version: 0.8.0
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: events
 Provides-Extra: gcp_cloud_run
 Provides-Extra: gcp_cloud_tasks
 Provides-Extra: gcp_pubsub
+Provides-Extra: openai
+Provides-Extra: pinecone
 License-File: LICENSE
 
 # microservice-utils
 
 Utilities and adapters for speeding up microservice development.
 
 ## Optional Dependencies (Extras)
@@ -24,19 +26,21 @@
 
 **Available extras:**
 
 - **events**: Support for event-driven architectures using pydantic for data validation and parsing.
 - **gcp_cloud_run**: Support for Google Cloud Run with the google-cloud-run client library.
 - **gcp_cloud_tasks**: Support for Google Cloud Tasks with the google-cloud-tasks client library.
 - **gcp_pubsub**: Support for Google Cloud Pub/Sub using the google-cloud-pubsub client library and tenacity for retries.
+- **openai**: Support for completions with the OpenAI API.
+- **pinecone**: Support for semantic search with Pinecone.
 
 To install multiple extras, separate them with commas:
 
 ```bash
-pip install microservice-utils[events,gcp_cloud_run,gcp_cloud_tasks,gcp_pubsub]
+pip install microservice-utils[events,gcp_cloud_run,gcp_cloud_tasks,gcp_pubsub,openai,pinecone]
 ```
 
 ## GCP Pub/Sub
 You can subscribe to multiple subscriptions by subsequently calling `subscribe()`. `wait_for_shutdown` will block IO
 for all the subscriptions and wait for the app to be signaled to shut down.
 
 ```python
```

### Comparing `microservice-utils-0.7.0/README.md` & `microservice-utils-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 
 **Available extras:**
 
 - **events**: Support for event-driven architectures using pydantic for data validation and parsing.
 - **gcp_cloud_run**: Support for Google Cloud Run with the google-cloud-run client library.
 - **gcp_cloud_tasks**: Support for Google Cloud Tasks with the google-cloud-tasks client library.
 - **gcp_pubsub**: Support for Google Cloud Pub/Sub using the google-cloud-pubsub client library and tenacity for retries.
+- **openai**: Support for completions with the OpenAI API.
+- **pinecone**: Support for semantic search with Pinecone.
 
 To install multiple extras, separate them with commas:
 
 ```bash
-pip install microservice-utils[events,gcp_cloud_run,gcp_cloud_tasks,gcp_pubsub]
+pip install microservice-utils[events,gcp_cloud_run,gcp_cloud_tasks,gcp_pubsub,openai,pinecone]
 ```
 
 ## GCP Pub/Sub
 You can subscribe to multiple subscriptions by subsequently calling `subscribe()`. `wait_for_shutdown` will block IO
 for all the subscriptions and wait for the app to be signaled to shut down.
 
 ```python
```

### Comparing `microservice-utils-0.7.0/microservice_utils/events.py` & `microservice-utils-0.8.0/microservice_utils/events.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.7.0/microservice_utils/google_cloud/adapters/cloud_logging.py` & `microservice-utils-0.8.0/microservice_utils/google_cloud/adapters/cloud_logging.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.7.0/microservice_utils/google_cloud/adapters/cloud_run.py` & `microservice-utils-0.8.0/microservice_utils/google_cloud/adapters/cloud_run.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.7.0/microservice_utils/google_cloud/adapters/cloud_tasks.py` & `microservice-utils-0.8.0/microservice_utils/google_cloud/adapters/cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.7.0/microservice_utils/google_cloud/adapters/pubsub.py` & `microservice-utils-0.8.0/microservice_utils/google_cloud/adapters/pubsub.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.7.0/microservice_utils/google_cloud/models.py` & `microservice-utils-0.8.0/microservice_utils/google_cloud/models.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.7.0/microservice_utils/graphql.py` & `microservice-utils-0.8.0/microservice_utils/graphql.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.7.0/microservice_utils.egg-info/PKG-INFO` & `microservice-utils-0.8.0/microservice_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: microservice-utils
-Version: 0.7.0
+Version: 0.8.0
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: events
 Provides-Extra: gcp_cloud_run
 Provides-Extra: gcp_cloud_tasks
 Provides-Extra: gcp_pubsub
+Provides-Extra: openai
+Provides-Extra: pinecone
 License-File: LICENSE
 
 # microservice-utils
 
 Utilities and adapters for speeding up microservice development.
 
 ## Optional Dependencies (Extras)
@@ -24,19 +26,21 @@
 
 **Available extras:**
 
 - **events**: Support for event-driven architectures using pydantic for data validation and parsing.
 - **gcp_cloud_run**: Support for Google Cloud Run with the google-cloud-run client library.
 - **gcp_cloud_tasks**: Support for Google Cloud Tasks with the google-cloud-tasks client library.
 - **gcp_pubsub**: Support for Google Cloud Pub/Sub using the google-cloud-pubsub client library and tenacity for retries.
+- **openai**: Support for completions with the OpenAI API.
+- **pinecone**: Support for semantic search with Pinecone.
 
 To install multiple extras, separate them with commas:
 
 ```bash
-pip install microservice-utils[events,gcp_cloud_run,gcp_cloud_tasks,gcp_pubsub]
+pip install microservice-utils[events,gcp_cloud_run,gcp_cloud_tasks,gcp_pubsub,openai,pinecone]
 ```
 
 ## GCP Pub/Sub
 You can subscribe to multiple subscriptions by subsequently calling `subscribe()`. `wait_for_shutdown` will block IO
 for all the subscriptions and wait for the app to be signaled to shut down.
 
 ```python
```

### Comparing `microservice-utils-0.7.0/microservice_utils.egg-info/SOURCES.txt` & `microservice-utils-0.8.0/microservice_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,13 +14,19 @@
 microservice_utils/google_cloud/__init__.py
 microservice_utils/google_cloud/models.py
 microservice_utils/google_cloud/adapters/__init__.py
 microservice_utils/google_cloud/adapters/cloud_logging.py
 microservice_utils/google_cloud/adapters/cloud_run.py
 microservice_utils/google_cloud/adapters/cloud_tasks.py
 microservice_utils/google_cloud/adapters/pubsub.py
+microservice_utils/openai/__init__.py
+microservice_utils/openai/adapters.py
+microservice_utils/pinecone/__init__.py
+microservice_utils/pinecone/adapters.py
 tests/__init__.py
 tests/graphql.py
 tests/test_events.py
 tests/google_cloud/__init__.py
 tests/google_cloud/test_cloud_run.py
-tests/google_cloud/test_cloud_tasks.py
+tests/google_cloud/test_cloud_tasks.py
+tests/openai/__init__.py
+tests/openai/test_adapters.py
```

### Comparing `microservice-utils-0.7.0/setup.py` & `microservice-utils-0.8.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     long_description_content_type="text/markdown",
     version=microservice_utils.__version__,
     extras_require={
         "events": ["pydantic>=1,<2"],
         "gcp_cloud_run": ["google-cloud-run<1"],
         "gcp_cloud_tasks": ["google-cloud-tasks>=2,<3"],
         "gcp_pubsub": ["google-cloud-pubsub>=2,<3", "tenacity>=8,<9"],
+        "openai": ["masked-ai>=1,<2", "numpy>=1,<2", "openai<1"],
+        "pinecone": ["pinecone-client>=2,<3"],
     },
     install_requires=[
         "ulid-py>=1,<2",
         "httpx==0.23.0",
     ],
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `microservice-utils-0.7.0/tests/google_cloud/test_cloud_run.py` & `microservice-utils-0.8.0/tests/google_cloud/test_cloud_run.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.7.0/tests/graphql.py` & `microservice-utils-0.8.0/tests/graphql.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.7.0/tests/test_events.py` & `microservice-utils-0.8.0/tests/test_events.py`

 * *Files identical despite different names*

