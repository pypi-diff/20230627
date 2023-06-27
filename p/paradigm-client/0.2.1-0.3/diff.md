# Comparing `tmp/paradigm_client-0.2.1.tar.gz` & `tmp/paradigm_client-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm_client-0.2.1.tar", last modified: Thu Jun 15 09:09:12 2023, max compression
+gzip compressed data, was "paradigm_client-0.3.tar", last modified: Tue Jun 27 09:48:48 2023, max compression
```

## Comparing `paradigm_client-0.2.1.tar` & `paradigm_client-0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.871257 paradigm_client-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.871257 paradigm_client-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/.github/workflows/build-test-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.871257 paradigm_client-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/examples/create_endpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/examples/create_endpoint_batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/examples/mini_instruct_sagemaker_model_consumer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/examples/select_endpoint.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/paradigm_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/paradigm_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/paradigm_client/communicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/paradigm_client/remote_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/paradigm_client/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/paradigm_client/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/paradigm_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-15 09:09:12.000000 paradigm_client-0.2.1/paradigm_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-15 09:09:12.000000 paradigm_client-0.2.1/paradigm_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:09:12.000000 paradigm_client-0.2.1/paradigm_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 09:09:12.000000 paradigm_client-0.2.1/paradigm_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 09:09:12.000000 paradigm_client-0.2.1/paradigm_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/tests/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.109690 paradigm_client-0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-27 09:48:18.000000 paradigm_client-0.3/.github/workflows/build-test-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-27 09:48:18.000000 paradigm_client-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-27 09:48:18.000000 paradigm_client-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-27 09:48:48.113690 paradigm_client-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-27 09:48:18.000000 paradigm_client-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-27 09:48:18.000000 paradigm_client-0.3/examples/create_endpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-27 09:48:18.000000 paradigm_client-0.3/examples/create_endpoint_batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-06-27 09:48:18.000000 paradigm_client-0.3/examples/mini_instruct_sagemaker_model_consumer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-06-27 09:48:18.000000 paradigm_client-0.3/examples/select_endpoint.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/paradigm_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:18.000000 paradigm_client-0.3/paradigm_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-27 09:48:18.000000 paradigm_client-0.3/paradigm_client/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-06-27 09:48:18.000000 paradigm_client-0.3/paradigm_client/remote_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-27 09:48:18.000000 paradigm_client-0.3/paradigm_client/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-27 09:48:18.000000 paradigm_client-0.3/paradigm_client/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/paradigm_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-27 09:48:48.000000 paradigm_client-0.3/paradigm_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-27 09:48:48.000000 paradigm_client-0.3/paradigm_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:48:48.000000 paradigm_client-0.3/paradigm_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 09:48:48.000000 paradigm_client-0.3/paradigm_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 09:48:48.000000 paradigm_client-0.3/paradigm_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 09:48:18.000000 paradigm_client-0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:48:48.113690 paradigm_client-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-27 09:48:18.000000 paradigm_client-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:48:48.113690 paradigm_client-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-27 09:48:18.000000 paradigm_client-0.3/tests/example.py
```

### Comparing `paradigm_client-0.2.1/.github/workflows/build-test-deploy.yaml` & `paradigm_client-0.3/.github/workflows/build-test-deploy.yaml`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/.gitignore` & `paradigm_client-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/LICENSE` & `paradigm_client-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/PKG-INFO` & `paradigm_client-0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm_client
-Version: 0.2.1
+Version: 0.3
 Summary: Python client for LightOn Paradigm
 Home-page: https://github.com/lightonai/paradigm-client
 Author: LightOn AI
 Author-email: support@lighton.ai
 Keywords: NLP,API,AI,LLM
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paradigm_client-0.2.1/README.md` & `paradigm_client-0.3/README.md`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/examples/create_endpoint.ipynb` & `paradigm_client-0.3/examples/create_endpoint.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/examples/create_endpoint_batching.ipynb` & `paradigm_client-0.3/examples/create_endpoint_batching.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/examples/mini_instruct_sagemaker_model_consumer.ipynb` & `paradigm_client-0.3/examples/mini_instruct_sagemaker_model_consumer.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/examples/select_endpoint.ipynb` & `paradigm_client-0.3/examples/select_endpoint.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/paradigm_client/communicator.py` & `paradigm_client-0.3/paradigm_client/communicator.py`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/paradigm_client/remote_model.py` & `paradigm_client-0.3/paradigm_client/remote_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,19 +110,19 @@
         list[TokenizeResponse],
         ErrorResponse],
     ) -> Union[CreateResponse, AnalyseResponse, SelectResponse, TokenizeResponse, ErrorResponse]:
         return response if isinstance(response, ErrorResponse) else response[0]
 
     @validate_arguments
     def create(
-        self, prompt: str, params: Optional[CreateParameters] = None, show_progress: bool = False, **kwargs: Any
+        self, prompt: str, params: Optional[CreateParameters] = None, use_session: bool = True, show_progress: bool = False, **kwargs: Any
     ) -> Union[CreateResponse, ErrorResponse]:
         params = self._get_params(params, **kwargs)
         response = self._post(
-            {"text": prompt, "params": params},
+            {"text": prompt, "params": params, "use_session": use_session},
             Endpoint.create,
             num_tasks=params.get("n_completions", 1),
             show_progress=show_progress,
         )
         return self._format_single_request_output(response)
 
     @validate_arguments
```

### Comparing `paradigm_client-0.2.1/paradigm_client/request.py` & `paradigm_client-0.3/paradigm_client/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
     status: Status
     completed_task: int
 
 
 class CreateRequest(BaseModel):
     text: str
     params: Optional[CreateParameters] = None
+    use_session: bool = True,
     _validate_text = validator("text", allow_reuse=True)(check_text)
 
     @validator("params", always=True, pre=True)
     def check_params(cls, params, values) -> CreateParameters:
         if params is None:
             return CreateParameters()
         return params
```

### Comparing `paradigm_client-0.2.1/paradigm_client/response.py` & `paradigm_client-0.3/paradigm_client/response.py`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/paradigm_client.egg-info/PKG-INFO` & `paradigm_client-0.3/paradigm_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm-client
-Version: 0.2.1
+Version: 0.3
 Summary: Python client for LightOn Paradigm
 Home-page: https://github.com/lightonai/paradigm-client
 Author: LightOn AI
 Author-email: support@lighton.ai
 Keywords: NLP,API,AI,LLM
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paradigm_client-0.2.1/paradigm_client.egg-info/SOURCES.txt` & `paradigm_client-0.3/paradigm_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2.1/setup.py` & `paradigm_client-0.3/setup.py`

 * *Files identical despite different names*

