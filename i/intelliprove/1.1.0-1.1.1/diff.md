# Comparing `tmp/intelliprove-1.1.0.tar.gz` & `tmp/intelliprove-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelliprove-1.1.0.tar", max compression
+gzip compressed data, was "intelliprove-1.1.1.tar", max compression
```

## Comparing `intelliprove-1.1.0.tar` & `intelliprove-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1686 2023-06-01 13:49:57.540140 intelliprove-1.1.0/README.md
--rw-r--r--   0        0        0      185 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/__init__.py
--rw-r--r--   0        0        0     5513 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/api_service.py
--rw-r--r--   0        0        0      141 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/exceptions/__init__.py
--rw-r--r--   0        0        0      891 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/exceptions/api.py
--rw-r--r--   0        0        0      790 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/exceptions/media.py
--rw-r--r--   0        0        0      261 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/exceptions/uuid.py
--rw-r--r--   0        0        0     3522 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/intelliprove_api.py
--rw-r--r--   0        0        0      214 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/__init__.py
--rw-r--r--   0        0        0      214 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/dataclasses/__init__.py
--rw-r--r--   0        0        0      642 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/dataclasses/biomarkers.py
--rw-r--r--   0        0        0      250 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/dataclasses/quality.py
--rw-r--r--   0        0        0      785 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/dataclasses/settings.py
--rw-r--r--   0        0        0      343 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/enums.py
--rw-r--r--   0        0        0      164 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/responses/__init__.py
--rw-r--r--   0        0        0     1199 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/responses/biomarkers_response.py
--rw-r--r--   0        0        0      754 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/responses/quality_response.py
--rw-r--r--   0        0        0       91 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/utils/__init__.py
--rw-r--r--   0        0        0      169 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/utils/identifiers.py
--rw-r--r--   0        0        0     2459 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/utils/media.py
--rw-r--r--   0        0        0      426 2023-06-01 13:49:57.544140 intelliprove-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 intelliprove-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1686 2023-06-27 12:58:40.950506 intelliprove-1.1.1/README.md
+-rw-r--r--   0        0        0      185 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/__init__.py
+-rw-r--r--   0        0        0     5514 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/api_service.py
+-rw-r--r--   0        0        0      141 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/exceptions/__init__.py
+-rw-r--r--   0        0        0      891 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/exceptions/api.py
+-rw-r--r--   0        0        0      790 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/exceptions/media.py
+-rw-r--r--   0        0        0      261 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/exceptions/uuid.py
+-rw-r--r--   0        0        0     3522 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/intelliprove_api.py
+-rw-r--r--   0        0        0      214 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/models/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/models/dataclasses/__init__.py
+-rw-r--r--   0        0        0      642 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/models/dataclasses/biomarkers.py
+-rw-r--r--   0        0        0      250 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/models/dataclasses/quality.py
+-rw-r--r--   0        0        0      787 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/models/dataclasses/settings.py
+-rw-r--r--   0        0        0      343 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/models/enums.py
+-rw-r--r--   0        0        0      164 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/models/responses/__init__.py
+-rw-r--r--   0        0        0     1199 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/models/responses/biomarkers_response.py
+-rw-r--r--   0        0        0      754 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/models/responses/quality_response.py
+-rw-r--r--   0        0        0       91 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/utils/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/utils/identifiers.py
+-rw-r--r--   0        0        0     2459 2023-06-27 12:58:40.950506 intelliprove-1.1.1/intelliprove/api/utils/media.py
+-rw-r--r--   0        0        0      426 2023-06-27 12:58:40.950506 intelliprove-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 intelliprove-1.1.1/PKG-INFO
```

### Comparing `intelliprove-1.1.0/README.md` & `intelliprove-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `intelliprove-1.1.0/intelliprove/api/api_service.py` & `intelliprove-1.1.1/intelliprove/api/api_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         # Get result of processed upload by uuid
         if not is_valid_uuid(uuid):
             raise InvalidUuidException(uuid)
 
         uri = self.make_url(f"results/wait/{uuid}")
 
         resp = requests.get(uri, **self.request_kwargs)
-        self._check_status_code(resp, (200, 204))
+        self._check_status_code(resp, (200, 202))
         result = resp.json()
         return BiomarkersResponse.from_json(result) if resp.status_code == 200 and isinstance(result, dict) and len(result.keys()) > 0 else None
 
     def create_action_token(self, expires_in: int, metadata: dict) -> str:
         uri = self.make_url(f"auth/action-token")
 
         resp = requests.post(uri, data={
@@ -136,7 +136,8 @@
         if resp.status_code != expected if isinstance(expected, int) else resp.status_code not in expected:
             raise ApiException("Unexpected response from IntelliProve api.", resp.status_code)
 
     @staticmethod
     def _add_query_to_uri(uri, query: dict) -> str:
         # add dict query to uri and url encode
         return uri + "?" + urllib.parse.quote("&".join([f'{str(key)}={str(val)}' for key, val in query.items()]))
+
```

### Comparing `intelliprove-1.1.0/intelliprove/api/exceptions/api.py` & `intelliprove-1.1.1/intelliprove/api/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.1.0/intelliprove/api/exceptions/media.py` & `intelliprove-1.1.1/intelliprove/api/exceptions/media.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.1.0/intelliprove/api/intelliprove_api.py` & `intelliprove-1.1.1/intelliprove/api/intelliprove_api.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.1.0/intelliprove/api/models/dataclasses/biomarkers.py` & `intelliprove-1.1.1/intelliprove/api/models/dataclasses/biomarkers.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.1.0/intelliprove/api/models/dataclasses/settings.py` & `intelliprove-1.1.1/intelliprove/api/models/dataclasses/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 
     # Connection timeouts
     upload_timeout: float = 120.0  # Maximum timeout (s) that an upload may take before raising TimeoutError
     send_timeout: float = 30.0  # Maximum timeout (s) sending an HTTP request may take before raising TimeoutError
 
     @property
     def full_url(self) -> str:
-        return urljoin(self.base_url, self.version)
+        return urljoin(self.base_url, self.version)
+
```

### Comparing `intelliprove-1.1.0/intelliprove/api/models/responses/biomarkers_response.py` & `intelliprove-1.1.1/intelliprove/api/models/responses/biomarkers_response.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.1.0/intelliprove/api/models/responses/quality_response.py` & `intelliprove-1.1.1/intelliprove/api/models/responses/quality_response.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.1.0/intelliprove/api/utils/media.py` & `intelliprove-1.1.1/intelliprove/api/utils/media.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.1.0/PKG-INFO` & `intelliprove-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelliprove
-Version: 1.1.0
+Version: 1.1.1
 Summary: The Python SDK for using IntelliProve.
 Author: Seppe De Langhe
 Author-email: seppe.delanghe@intelliprove.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

