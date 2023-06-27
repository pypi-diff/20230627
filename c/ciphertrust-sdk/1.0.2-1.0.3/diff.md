# Comparing `tmp/ciphertrust-sdk-1.0.2.tar.gz` & `tmp/ciphertrust-sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciphertrust-sdk-1.0.2.tar", last modified: Mon Jun 26 14:00:25 2023, max compression
+gzip compressed data, was "ciphertrust-sdk-1.0.3.tar", last modified: Tue Jun 27 12:44:39 2023, max compression
```

## Comparing `ciphertrust-sdk-1.0.2.tar` & `ciphertrust-sdk-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-26 14:00:25.462445 ciphertrust-sdk-1.0.2/
--rw-rw-r--   0 adamt      (501) staff       (20)     1064 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/LICENSE
--rw-r--r--   0 adamt      (501) staff       (20)     4532 2023-06-26 14:00:25.462011 ciphertrust-sdk-1.0.2/PKG-INFO
--rw-rw-r--   0 adamt      (501) staff       (20)     2849 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/README.md
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-26 14:00:25.457085 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/
--rw-r--r--   0 adamt      (501) staff       (20)     4532 2023-06-26 14:00:25.000000 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/PKG-INFO
--rw-r--r--   0 adamt      (501) staff       (20)      492 2023-06-26 14:00:25.000000 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-06-26 14:00:25.000000 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 adamt      (501) staff       (20)       94 2023-06-26 14:00:25.000000 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/requires.txt
--rw-r--r--   0 adamt      (501) staff       (20)       12 2023-06-26 14:00:25.000000 ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/top_level.txt
--rw-rw-r--   0 adamt      (501) staff       (20)     1054 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/pyproject.toml
--rw-r--r--   0 adamt      (501) staff       (20)       38 2023-06-26 14:00:25.462564 ciphertrust-sdk-1.0.2/setup.cfg
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-26 14:00:25.454062 ciphertrust-sdk-1.0.2/src/
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-26 14:00:25.461502 ciphertrust-sdk-1.0.2/src/ciphertrust/
--rw-rw-r--   0 adamt      (501) staff       (20)      134 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/_version.py
--rw-rw-r--   0 adamt      (501) staff       (20)     6353 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/api.py
--rw-rw-r--   0 adamt      (501) staff       (20)     8075 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/auth.py
--rw-rw-r--   0 adamt      (501) staff       (20)      248 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/config.py
--rw-rw-r--   0 adamt      (501) staff       (20)      471 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/exceptions.py
--rw-rw-r--   0 adamt      (501) staff       (20)     3721 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/models.py
--rw-rw-r--   0 adamt      (501) staff       (20)     9785 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/requestapi.py
--rw-rw-r--   0 adamt      (501) staff       (20)      417 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/static.py
--rw-rw-r--   0 adamt      (501) staff       (20)     6720 2023-06-26 13:57:22.000000 ciphertrust-sdk-1.0.2/src/ciphertrust/utils.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-27 12:44:39.448772 ciphertrust-sdk-1.0.3/
+-rw-rw-r--   0 adamt      (501) staff       (20)     1064 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/LICENSE
+-rw-r--r--   0 adamt      (501) staff       (20)     5082 2023-06-27 12:44:39.448326 ciphertrust-sdk-1.0.3/PKG-INFO
+-rw-rw-r--   0 adamt      (501) staff       (20)     3399 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/README.md
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-27 12:44:39.430820 ciphertrust-sdk-1.0.3/ciphertrust_sdk.egg-info/
+-rw-r--r--   0 adamt      (501) staff       (20)     5082 2023-06-27 12:44:39.000000 ciphertrust-sdk-1.0.3/ciphertrust_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 adamt      (501) staff       (20)      492 2023-06-27 12:44:39.000000 ciphertrust-sdk-1.0.3/ciphertrust_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-06-27 12:44:39.000000 ciphertrust-sdk-1.0.3/ciphertrust_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       94 2023-06-27 12:44:39.000000 ciphertrust-sdk-1.0.3/ciphertrust_sdk.egg-info/requires.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       12 2023-06-27 12:44:39.000000 ciphertrust-sdk-1.0.3/ciphertrust_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 adamt      (501) staff       (20)     1054 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/pyproject.toml
+-rw-r--r--   0 adamt      (501) staff       (20)       38 2023-06-27 12:44:39.448923 ciphertrust-sdk-1.0.3/setup.cfg
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-27 12:44:39.426306 ciphertrust-sdk-1.0.3/src/
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-27 12:44:39.447354 ciphertrust-sdk-1.0.3/src/ciphertrust/
+-rw-rw-r--   0 adamt      (501) staff       (20)      134 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/src/ciphertrust/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/src/ciphertrust/_version.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     6468 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/src/ciphertrust/api.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     8086 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/src/ciphertrust/auth.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      248 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/src/ciphertrust/config.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      471 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/src/ciphertrust/exceptions.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     3752 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/src/ciphertrust/models.py
+-rw-rw-r--   0 adamt      (501) staff       (20)    12016 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/src/ciphertrust/requestapi.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      417 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/src/ciphertrust/static.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     7229 2023-06-27 12:40:06.000000 ciphertrust-sdk-1.0.3/src/ciphertrust/utils.py
```

### Comparing `ciphertrust-sdk-1.0.2/LICENSE` & `ciphertrust-sdk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.2/PKG-INFO` & `ciphertrust-sdk-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciphertrust-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Thales CipherTrust SDK RestAPI
 Author-email: atav928 <dev@tavnets.com>
 License: MIT License
         
         Copyright (c) 2023 atav928
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -109,30 +109,43 @@
 | Version | Build | Changes |
 | ------- | ----- | ------- |
 | **0.0.1** | **final** | Test Relese; basic functionality |
 | **1.0.1** | **final** | Available Release with API and Auth functionality |
 | **1.0.2** | **a1** | Removed print |
 | **1.0.2** | **a2** | Added metrics in calls and additional awaits to call on mutliple calls |
 | **1.0.2** | **final** | See notes below |
+| **1.0.3** | **final** | See notes below |
 
 ### Known Bugs/Futue Features
 
 __TODO:__
 
 * &#9745; Create a metrics fucntion to return
 * &#9745; Delete all private aand passwords being printed
 * &#9744; Add logging or streaming or none
 * &#9744; Add own metrics
   * &#9744; Generic metrics wrapper
   * &#9744; Logging metrics wrapper
 * &#9745; Create an average, mean, total time depending on calls being made for when you want to do a full list of keys
 * &#9745; Missing delete https action
+* &#9745; Create a download method to handle downlaoding files
 
 #### Release Notes
 
+#### v1.0.3
+
+* Fixed bug with headers returning a requests.exceptions.JSONDecodeError due to the way headers are formated.
+* Added more timeing metrics for quanitfying calls.
+* Added ability to request a download when stream=True is passed in call.
+
+__TODO:__
+
+* Need to build additional async requests when calling multiple items.
+* Build out ability to send multiple requests and hold the type of requests to make it easier to use the SDK.
+
 #### v1.0.2
 
 * Added Generic Metrics to each call with additional statistics that can be used.
 * Added async to handle multle requests; still need to take advantage of it.
 * Removed disclosure of secrets in debug prints.
 
 __Known Bugs:__
```

### Comparing `ciphertrust-sdk-1.0.2/README.md` & `ciphertrust-sdk-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -74,30 +74,43 @@
 | Version | Build | Changes |
 | ------- | ----- | ------- |
 | **0.0.1** | **final** | Test Relese; basic functionality |
 | **1.0.1** | **final** | Available Release with API and Auth functionality |
 | **1.0.2** | **a1** | Removed print |
 | **1.0.2** | **a2** | Added metrics in calls and additional awaits to call on mutliple calls |
 | **1.0.2** | **final** | See notes below |
+| **1.0.3** | **final** | See notes below |
 
 ### Known Bugs/Futue Features
 
 __TODO:__
 
 * &#9745; Create a metrics fucntion to return
 * &#9745; Delete all private aand passwords being printed
 * &#9744; Add logging or streaming or none
 * &#9744; Add own metrics
   * &#9744; Generic metrics wrapper
   * &#9744; Logging metrics wrapper
 * &#9745; Create an average, mean, total time depending on calls being made for when you want to do a full list of keys
 * &#9745; Missing delete https action
+* &#9745; Create a download method to handle downlaoding files
 
 #### Release Notes
 
+#### v1.0.3
+
+* Fixed bug with headers returning a requests.exceptions.JSONDecodeError due to the way headers are formated.
+* Added more timeing metrics for quanitfying calls.
+* Added ability to request a download when stream=True is passed in call.
+
+__TODO:__
+
+* Need to build additional async requests when calling multiple items.
+* Build out ability to send multiple requests and hold the type of requests to make it easier to use the SDK.
+
 #### v1.0.2
 
 * Added Generic Metrics to each call with additional statistics that can be used.
 * Added async to handle multle requests; still need to take advantage of it.
 * Removed disclosure of secrets in debug prints.
 
 __Known Bugs:__
```

### Comparing `ciphertrust-sdk-1.0.2/ciphertrust_sdk.egg-info/PKG-INFO` & `ciphertrust-sdk-1.0.3/ciphertrust_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciphertrust-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Thales CipherTrust SDK RestAPI
 Author-email: atav928 <dev@tavnets.com>
 License: MIT License
         
         Copyright (c) 2023 atav928
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -109,30 +109,43 @@
 | Version | Build | Changes |
 | ------- | ----- | ------- |
 | **0.0.1** | **final** | Test Relese; basic functionality |
 | **1.0.1** | **final** | Available Release with API and Auth functionality |
 | **1.0.2** | **a1** | Removed print |
 | **1.0.2** | **a2** | Added metrics in calls and additional awaits to call on mutliple calls |
 | **1.0.2** | **final** | See notes below |
+| **1.0.3** | **final** | See notes below |
 
 ### Known Bugs/Futue Features
 
 __TODO:__
 
 * &#9745; Create a metrics fucntion to return
 * &#9745; Delete all private aand passwords being printed
 * &#9744; Add logging or streaming or none
 * &#9744; Add own metrics
   * &#9744; Generic metrics wrapper
   * &#9744; Logging metrics wrapper
 * &#9745; Create an average, mean, total time depending on calls being made for when you want to do a full list of keys
 * &#9745; Missing delete https action
+* &#9745; Create a download method to handle downlaoding files
 
 #### Release Notes
 
+#### v1.0.3
+
+* Fixed bug with headers returning a requests.exceptions.JSONDecodeError due to the way headers are formated.
+* Added more timeing metrics for quanitfying calls.
+* Added ability to request a download when stream=True is passed in call.
+
+__TODO:__
+
+* Need to build additional async requests when calling multiple items.
+* Build out ability to send multiple requests and hold the type of requests to make it easier to use the SDK.
+
 #### v1.0.2
 
 * Added Generic Metrics to each call with additional statistics that can be used.
 * Added async to handle multle requests; still need to take advantage of it.
 * Removed disclosure of secrets in debug prints.
 
 __Known Bugs:__
```

### Comparing `ciphertrust-sdk-1.0.2/pyproject.toml` & `ciphertrust-sdk-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.2/src/ciphertrust/api.py` & `ciphertrust-sdk-1.0.3/src/ciphertrust/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,24 +75,26 @@
         :type url_path: str
         :return: _description_
         :rtype: dict[str, Any]
         """
         url: str = config.API_URL.format(self._parent_class.auth.hostname, # type: ignore
                                          url_path)
         params: dict[str,Any] = kwargs.pop("params", {})
+        stream: bool = kwargs.pop("stream", False)
         calls = {
             "standard": ctm_request,
             "list_all": asyn_get_all
         }
         get_all = "list_all" if kwargs.get("get_all", False) else "standard"
         response: dict[str,Any] = calls[get_all](auth=self._parent_class.auth, # type: ignore
                                                  url=url,
                                                  method=self.method, # type: ignore
                                                  params=params,
                                                  timeout=self._parent_class.auth.timeout, # type: ignore
+                                                 stream=stream,
                                                  verify=self._parent_class.auth.verify) # type: ignore
         return response
 
 
 class Post:
     """Calls generic POST requests for CipherTrust Manager
```

### Comparing `ciphertrust-sdk-1.0.2/src/ciphertrust/auth.py` & `ciphertrust-sdk-1.0.3/src/ciphertrust/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     @property
     def renew_refresh_token(self):
         return self.__renew_refresh_token
 
     @renew_refresh_token.setter
     def renew_refresh_token(self, value: bool):
-        if not isinstance(value, bool):
+        if not isinstance(value, bool):  # type: ignore
             raise CipherValueError(f"Invalid value for renew_refresh_token: {value}")
         self.__renew_refresh_token = value
 
     def _create_payload(self, payload: Dict[str, Any]) -> Dict[str, Any]:
         # print(f"{payload=}")
         response: Dict[str, Any] = default_payload(**payload)
         # print(f"createdpayload={response}")
@@ -131,15 +131,14 @@
         self.exec_time = exec_time
         self.exec_time_elapsed.append(exec_time)
         self.exec_time_min = min(self.exec_time_elapsed)
         self.exec_time_max = max(self.exec_time_elapsed)
         self.exec_time_stdev = 0.0 if len(
             self.exec_time_elapsed) <= 1 else statistics.stdev(
             self.exec_time_elapsed)
-    
 
     def _update_token_info(self, response_json: Dict[str, Any]):
         self.expiration = response_json["jwt_decode"]["exp"]
         self.issued_at = response_json["jwt_decode"]["iat"]
         self.refresh_token = response_json["refresh_token"]
         self.token = response_json["jwt"]
         self.token_type: str = response_json["token_type"]
```

### Comparing `ciphertrust-sdk-1.0.2/src/ciphertrust/models.py` & `ciphertrust-sdk-1.0.3/src/ciphertrust/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             raise CipherValueError(f"Invalid grant type: {self.grant_type=}")
         if not any([isinstance(self.verify, bool), isinstance(self.verify, str)]):
             raise CipherValueError(f"Invalid value: {self.verify=}")
         # TODO: Verify hostname is a valid domainname
         if not validate_domain(self.hostname):
             raise CipherValueError(f"Invlalid hostname: {self.hostname}")
 
-    def __new__(cls, *args, **kwargs):  # pylint: disable=unused-arguments
+    def __new__(cls, *args: Any, **kwargs: Any):  # pylint: disable=unused-arguments,unknown-option-value
         """Used to remove any unwatned arguments
 
         :return: _description_
         :rtype: _type_
         """
         try:
             initializer = cls.__initializer
```

### Comparing `ciphertrust-sdk-1.0.2/src/ciphertrust/requestapi.py` & `ciphertrust-sdk-1.0.3/src/ciphertrust/requestapi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,81 @@
 """Request API"""
 
 from typing import Any, Dict, List
+import json
+import os
 import time
+import datetime
 import statistics
 import asyncio
 import copy
 from functools import reduce
+from pathlib import Path
 
 import orjson
 import httpx
 import requests
 from requests import HTTPError, Response
 
 from ciphertrust.auth import (Auth, refresh_token)
 from ciphertrust.exceptions import (CipherAPIError, CipherMissingParam)
 from ciphertrust.static import (DEFAULT_HEADERS, ENCODE,
                                 DEFAULT_LIMITS_OVERRIDE, DEFAULT_TIMEOUT_CONFIG_OVERRIDE)
-from ciphertrust.utils import (reformat_exception, concat_resources)
+from ciphertrust.utils import (reformat_exception, concat_resources, verify_path_exists)
+
+
+def format_request(response: Response) -> dict[str, Any]:
+    """_summary_
+
+    :param response: _description_
+    :type response: Response
+    :return: _description_
+    :rtype: dict[str,Any]
+    """
+    api_raise_error(response=response)
+    json_response = {
+        "exec_time": response.elapsed.total_seconds(),
+        "headers": json.loads(orjson.dumps(response.headers.__dict__["_store"]).decode('utf-8')),
+        "exec_time_end": datetime.datetime.utcnow().isoformat()
+    }
+    return json_response
+
+
+def standard_request(**kwargs: Any) -> dict[str, Any]:
+    """_summary_
+
+    :return: _description_
+    :rtype: dict[str,Any]
+    """
+    resp: Response = requests.request(**kwargs)
+    response = {**resp.json(), **format_request(resp)}
+    return response
+
+
+def download_request(**kwargs: Any) -> dict[str, Any]:
+    """_summary_
+
+    :return: _description_
+    :rtype: Response
+    """
+    chunk_size = kwargs.pop("chunk_size", 128)
+    req: Response = requests.request(stream=True, **kwargs)
+    save_path = kwargs.pop("save_dir", os.path.expanduser('~'))
+    if not verify_path_exists(path_dir=save_path):
+        raise FileExistsError(f"{save_path} does not exist")
+        sys.exit()
+    save_filename = Path.joinpath(
+        Path(save_path) /
+        f"ciphertrust_log_{datetime.datetime.now().strftime('%Y%m%dT%H%M%S')}.tar.gz")
+    with open(save_filename, 'wb') as fd:
+        for chunk in req.iter_content(chunk_size=chunk_size):
+            fd.write(chunk)
+    response = {"message": "downloaded request completed", "location": str(save_filename)}
+    response = {**response, **format_request(req)}
+    return response
 
 
 @refresh_token
 def ctm_request(auth: Auth, **kwargs: Any) -> Dict[str, Any]:  # pylint: disable=too-many-locals
     """_summary_
 
     Args:
@@ -43,40 +98,38 @@
     try:
         method: str = kwargs.pop('method')  # type: ignore
         url: str = kwargs.pop('url')  # type: ignore
         timeout: int = kwargs.pop('timeout', 60)  # type: ignore
         verify: Any = kwargs.pop('verify', True)
         params: Dict[str, Any] = kwargs.pop('params', {})
         data: Any = kwargs.pop('data', None)  # type: ignore
+        stream: bool = kwargs.pop("stream", False)
         headers: Dict[str, Any] = kwargs.pop("headers", DEFAULT_HEADERS)
     except KeyError as err:
         error: str = reformat_exception(err)
         raise CipherMissingParam(error)  # pylint: disable=raise-missing-from
     if data:
         data: str = orjson.dumps(data).decode(ENCODE)  # pylint: disable=no-member
     # Add auth to header
     headers["Authorization"] = f"Bearer {auth.token}"
-    response: Response = requests.request(method=method,
-                                          url=url,
-                                          headers=headers,
-                                          data=data,
-                                          params=params,
-                                          verify=verify,
-                                          timeout=timeout)
-    # cipher_logger.debug("Response Code=%s|Full Response=%s",
-    #                     str(response.status_code), response.text.rstrip())
-    api_raise_error(response=response)
-    # Sample test
-    # TODO: Replace with logger
-    # print(f"status={response.status_code}|response={response.json()}")
-    json_response = {
-        "exec_time": response.elapsed.total_seconds(),
-        "headers": response.headers
+    request_type = {
+        "download": download_request,
+        "standard": standard_request
     }
-    return {**json_response, **response.json()}
+    start_time = datetime.datetime.utcnow().isoformat()
+    response: dict[str, Any] = request_type["standard" if not stream else "download"](method=method,
+                                                                                      url=url,
+                                                                                      headers=headers,
+                                                                                      data=data,
+                                                                                      params=params,
+                                                                                      verify=verify,
+                                                                                      timeout=timeout,
+                                                                                      **kwargs)
+    response["exec_time_start"] = start_time
+    return response
 
 
 @refresh_token
 async def ctm_request_async(auth: Auth, **kwargs: Any) -> Dict[str, Any]:  # pylint: disable=too-many-locals
     """_summary_
 
     Args:
@@ -150,27 +203,30 @@
         "exec_time_start": start_time,
         "iterations": copy.deepcopy(iterations),
     }
     full_listed_resp = []
     while iterations > 0:
         send_iterations = 10 if iterations <= 10 else iterations
         tmp_listed_resp = await split_up_req(auth=auth,
-                                             iterations=send_iterations,
-                                             limit=limit,
+                                             iterations=send_iterations,  # type: ignore
+                                             limit=limit,  # type: ignore
                                              **kwargs)
         full_listed_resp = full_listed_resp + tmp_listed_resp
         iterations -= 10
         print(f"One loop iteration completed new_iterations={iterations}")
-    response = {**response, **build_responsde(full_listed_resp=full_listed_resp)}
+    response = {**response, **build_responsde(full_listed_resp=full_listed_resp)}  # type: ignore
     response["exec_time"] = response["exec_time_end"] - start_time
+    response["exec_time_end"] = datetime.datetime.utcfromtimestamp(
+        response["exec_time_end"]).isoformat()
+    response["exec_time_start"] = datetime.datetime.utcfromtimestamp(start_time).isoformat()
     return response
 
 
 @refresh_token
-async def split_up_req(auth: Auth, iterations: int, limit: int, **kwargs) -> List[Dict[str, Any]]:
+async def split_up_req(auth: Auth, iterations: int, limit: int, **kwargs: Any) -> List[Dict[str, Any]]:
     """Splitting up requests due to too many being sent and cannot handle.
       Trying to adjust with timeout, but still causes errors on return.
 
     :param auth: _description_
     :type auth: Auth
     :param iterations: _description_
     :type iterations: int
@@ -188,16 +244,16 @@
             kwargs["params"] = {
                 "limit": limit,
                 "skip": (number*limit+1) if (number != 0) else 0
             }
             kwargs["client"] = client
             print(f"{number=}|{kwargs=}")
             tasks.append(asyncio.ensure_future(ctm_request_async(auth=auth, **kwargs)))
-        full_listed_resp: List[Dict[str, Any]] = await asyncio.gather(*tasks)
-    return full_listed_resp
+        full_listed_resp: List[Dict[str, Any]] = await asyncio.gather(*tasks)  # type: ignore
+    return full_listed_resp  # type: ignore
     # print(f"{full_listed_resp=}")
 
 
 def build_responsde(full_listed_resp: list[dict[str, Any]]) -> dict[str, Any]:
     response: Dict[str, Any] = {
         "exec_time_end": 0.0,
         "exec_time_min": 0.0,
```

### Comparing `ciphertrust-sdk-1.0.2/src/ciphertrust/utils.py` & `ciphertrust-sdk-1.0.3/src/ciphertrust/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """Utilities"""
 
-import time
 from typing import Dict, Any
+from pathlib import Path
 
 import validators
 
 from ciphertrust.exceptions import CipherValueError
 
-def concat_resources(dict1, dict2) -> list[dict[str,Any]]:
+
+def concat_resources(dict1, dict2) -> list[dict[str, Any]]:  # type: ignore
     """Use reduce to generate a list of resources
 
     :param dict1: _description_
     :type dict1: _type_
     :param dict2: _description_
     :type dict2: _type_
     :return: _description_
     :rtype: list[dict[str,Any]]
     """
-    for key in dict2:
+    for key in dict2:  # type: ignore
         if key in dict1 and key == "resources":
             dict1[key] += dict2[key]
-    return dict1
+    return dict1  # type: ignore
+
 
 def reformat_exception(error: Exception) -> str:
     """Reformates Exception to print out as a string pass for logging
 
     Args:
         error (Exception): _description_
 
@@ -48,39 +50,39 @@
 # payload creation
 def set_refresh_lifetime(**kwargs: Dict[str, Any]) -> Dict[str, Any]:
     """Sets Refresh Lifetime if exists
 
     :return: _description_
     :rtype: Dict[str,Any]
     """
-    response = {}
+    response: Dict[str, Any] = {}
     if kwargs.get("refresh_token_lifetime"):
         response["refresh_token_lifetime"] = kwargs.get("refresh_token_lifetime")
     return response
 
 
 def set_refresh_token_revoke_unused_in(**kwargs: Dict[str, Any]) -> Dict[str, Any]:
     """Sets refresh_token_revoke_unused_in if exists
 
     :return: _description_
     :rtype: Dict[str,Any]
     """
-    response = {}
+    response: Dict[str, Any] = {}
     if kwargs.get("refresh_token_revoke_unused_in"):
         response["refresh_token_revoke_unused_in"] = kwargs.get("refresh_token_revoke_unused_in")
     return response
 
 
 def set_renew_refresh_token(**kwargs: Dict[str, Any]) -> Dict[str, Any]:
     """Sets renew_refresh_token default is False used to create new refresh token
 
     :return: _description_
     :rtype: Dict[str,Any]
     """
-    response = {}
+    response: Dict[str, Any] = {}
     response["renew_refresh_token"] = kwargs.get("renew_refresh_token", False)
     return response
 
 
 def set_user_cert(**kwargs: Dict[str, Any]) -> Dict[str, Any]:
     """Sets User Certificate when specified in grant type
 
@@ -113,15 +115,15 @@
         }
         response = {**response, **set_refresh_lifetime(**kwargs)}
         # only sets if password set
         response = {**response, **set_refresh_token_revoke_unused_in(**kwargs)}
         return response
     except KeyError as err:
         error: str = reformat_exception(err)
-        raise CipherValueError(f"Invalid value: {error}")
+        raise CipherValueError(f"Invalid value: {error}")  # pylint: disable=raise-missing-from
 
 
 def grant_refresh(**kwargs: Dict[str, Any]) -> Dict[str, Any]:
     """used to refresh grant token
 
     :raises CipherValueError: _description_
     :return: _description_
@@ -190,26 +192,43 @@
     "refresh_token": grant_refresh,
     "user_certificate": grant_user_cert,
     "client_credential": grant_client_creds
 }
 
 
 def default_payload(**kwargs: Dict[str, Any]) -> Dict[str, Any]:
+    """Set Default Payload
+
+    :raises CipherValueError: _description_
+    :return: _description_
+    :rtype: Dict[str, Any]
+    """
     try:
         response: Dict[str, Any] = {
             "grant_type": kwargs["grant_type"],
             "cookies": kwargs.get("cookies", False),
             "labels": kwargs.get("labels", []),
         }
         # returns the payload used to set up the AUTH Payload Body
         return {**response, **grant_options[response["grant_type"]](**kwargs)}
     except KeyError as err:
         error: str = reformat_exception(err)
         raise CipherValueError(f"Invalid value: {error}")
 
 
+def verify_path_exists(path_dir: str) -> bool:
+    """Checks if Path exists
+
+    :param path_dir: _description_
+    :type path_dir: str
+    :return: _description_
+    :rtype: bool
+    """
+    return Path(path_dir).exists()
+
+
 if __name__ == "__main__":
     valididate_list: list[str] = ["invalid", "valid-domain.example.com", "invalid_domain*.com"]
     # print(f"Checking domain validation against list: {', '.join(valididate_list)}")
     for _ in valididate_list:
         is_valid = validate_domain(_)
         # print(f"{_} is {str(is_valid)}")
```

