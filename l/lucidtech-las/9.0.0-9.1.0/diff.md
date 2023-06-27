# Comparing `tmp/lucidtech-las-9.0.0.tar.gz` & `tmp/lucidtech-las-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidtech-las-9.0.0.tar", last modified: Thu Jun 15 08:08:49 2023, max compression
+gzip compressed data, was "lucidtech-las-9.1.0.tar", last modified: Tue Jun 27 13:37:45 2023, max compression
```

## Comparing `lucidtech-las-9.0.0.tar` & `lucidtech-las-9.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:08:49.455413 lucidtech-las-9.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-15 08:08:49.455413 lucidtech-las-9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:08:49.451413 lucidtech-las-9.0.0/las/
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/las/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/las/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)   101292 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/las/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/las/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:08:49.455413 lucidtech-las-9.0.0/lucidtech_las.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-15 08:08:49.000000 lucidtech-las-9.0.0/lucidtech_las.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-15 08:08:49.000000 lucidtech-las-9.0.0/lucidtech_las.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:08:49.000000 lucidtech-las-9.0.0/lucidtech_las.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 08:08:49.000000 lucidtech-las-9.0.0/lucidtech_las.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 08:08:49.000000 lucidtech-las-9.0.0/lucidtech_las.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 08:08:49.455413 lucidtech-las-9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-15 08:08:37.000000 lucidtech-las-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:37:45.657821 lucidtech-las-9.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-27 13:37:34.000000 lucidtech-las-9.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-27 13:37:34.000000 lucidtech-las-9.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-27 13:37:45.657821 lucidtech-las-9.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-27 13:37:34.000000 lucidtech-las-9.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:37:45.657821 lucidtech-las-9.1.0/las/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-27 13:37:34.000000 lucidtech-las-9.1.0/las/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-27 13:37:34.000000 lucidtech-las-9.1.0/las/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103653 2023-06-27 13:37:34.000000 lucidtech-las-9.1.0/las/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-27 13:37:34.000000 lucidtech-las-9.1.0/las/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:37:45.657821 lucidtech-las-9.1.0/lucidtech_las.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-27 13:37:45.000000 lucidtech-las-9.1.0/lucidtech_las.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-27 13:37:45.000000 lucidtech-las-9.1.0/lucidtech_las.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:37:45.000000 lucidtech-las-9.1.0/lucidtech_las.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 13:37:45.000000 lucidtech-las-9.1.0/lucidtech_las.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 13:37:45.000000 lucidtech-las-9.1.0/lucidtech_las.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 13:37:34.000000 lucidtech-las-9.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 13:37:45.657821 lucidtech-las-9.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-27 13:37:34.000000 lucidtech-las-9.1.0/setup.py
```

### Comparing `lucidtech-las-9.0.0/LICENSE.md` & `lucidtech-las-9.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lucidtech-las-9.0.0/PKG-INFO` & `lucidtech-las-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidtech-las
-Version: 9.0.0
+Version: 9.1.0
 Summary: Python SDK for Lucidtech AI Services
 Home-page: https://github.com/LucidtechAI/las-sdk-python
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: Magnus Aarskaug Rud
 Maintainer-email: magnus@lucidtech.ai
 License: Apache 2.0
```

### Comparing `lucidtech-las-9.0.0/README.md` & `lucidtech-las-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lucidtech-las-9.0.0/las/__init__.py` & `lucidtech-las-9.1.0/las/__init__.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-9.0.0/las/client.py` & `lucidtech-las-9.1.0/las/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,21 @@
     return {k: v for k, v in d.items() if v is not None}
 
 
 def _fatal_code(e):
     return 400 <= e.response.status_code < 500
 
 
-def _json_decode(response):
+def _decode_response(response, return_json=True):
     try:
         response.raise_for_status()
-        return response.json()
+        if return_json:
+            return response.json()
+        else:
+            return response.content
     except JSONDecodeError as e:
 
         if response.status_code == 204:
             return {'Your request executed successfully': '204'}
 
         logger.error('Status code {} body:\n{}'.format(response.status_code, response.text))
         raise e
@@ -81,53 +84,56 @@
 def _guess_content_type(raw):
     guessed_type = filetype.guess(raw)
     assert guessed_type, 'Could not determine content type of document. ' \
                          'Please provide it by specifying content_type'
     return guessed_type.mime
 
 
+def _parsed_content(raw, find_content_type, base_64_encode):
+    content_type = _guess_content_type(raw) if find_content_type else None
+    parsed_content = b64encode(raw).decode() if base_64_encode else raw
+    return parsed_content, content_type
+
+
 @singledispatch
-def parse_content(content, find_content_type=False):
+def parse_content(content, find_content_type=False, base_64_encode=True):
     raise TypeError(
         '\n'.join([
             f'Could not parse content {content} of type {type(content)}',
             'Specify content by using one of the options below:',
             '1. Path to a file either as a string or as a Path object',
             '2. Bytes object with b64encoding',
             '3. Bytes object without b64encoding',
             '4. IO Stream of either bytes or text',
         ])
     )
 
 
 @parse_content.register(str)
 @parse_content.register(Path)
-def _(content, find_content_type=False):
+def _(content, find_content_type=False, base_64_encode=True):
     raw = Path(content).read_bytes()
-    content_type = _guess_content_type(raw) if find_content_type else None
-    return b64encode(raw).decode(), content_type
+    return _parsed_content(raw, find_content_type, base_64_encode)
 
 
 @parse_content.register(bytes)
 @parse_content.register(bytearray)
-def _(content, find_content_type=False):
+def _(content, find_content_type=False, base_64_encode=True):
     try:
         raw = b64decode(content, validate=True)
     except binascii.Error:
         raw = content
-    content_type = _guess_content_type(raw) if find_content_type else None
-    return b64encode(raw).decode(), content_type
+    return _parsed_content(raw, find_content_type, base_64_encode)
 
 
 @parse_content.register(io.IOBase)
-def _(content, find_content_type=False):
+def _(content, find_content_type=False, base_64_encode=True):
     raw = content.read()
     raw = raw.encode() if isinstance(raw, str) else raw
-    content_type = _guess_content_type(raw) if find_content_type else None
-    return b64encode(raw).decode(), content_type
+    return _parsed_content(raw, find_content_type, base_64_encode)
 
 
 class EmptyRequestError(ValueError):
     """An EmptyRequestError is raised if the request body is empty when expected not to be empty."""
     pass
 
 
@@ -202,15 +208,40 @@
             **(extra_headers or {}),
         }
         response = requests_fn(
             url=uri.geturl(),
             headers=headers,
             **kwargs,
         )
-        return _json_decode(response)
+        return _decode_response(response)
+
+    @on_exception(expo, TooManyRequestsException, max_tries=4)
+    @on_exception(expo, RequestException, max_tries=3, giveup=_fatal_code)
+    def _make_fileserver_request(
+        self,
+        requests_fn: Callable,
+        file_url: str,
+        content: Optional[bytes] = None,
+        query_params: Optional[dict] = None,
+    ) -> Dict:
+        if not content and requests_fn == requests.put:
+            raise EmptyRequestError
+
+        kwargs = {'params': query_params}
+        if content:
+            kwargs.update({'data': content})
+        uri = urlparse(file_url)
+
+        headers = {'Authorization': f'Bearer {self.credentials.access_token}'}
+        response = requests_fn(
+            url=uri.geturl(),
+            headers=headers,
+            **kwargs,
+        )
+        return _decode_response(response, return_json=False)
 
     def create_app_client(
         self,
         generate_secret=True,
         logout_urls=None,
         callback_urls=None,
         login_urls=None,
@@ -621,46 +652,45 @@
         >>> from las.client import Client
         >>> client = Client()
         >>> client.create_document(b'<bytes data>', 'image/jpeg', consent_id='<consent id>')
 
         :param content: Content to POST
         :type content: Content
         :param content_type: MIME type for the document
-        :type content_type: str
+        :type content_type: str, optional
         :param consent_id: Id of the consent that marks the owner of the document
         :type consent_id: str, optional
         :param dataset_id: Id of the associated dataset
         :type dataset_id: str, optional
         :param ground_truth: List of items {'label': label, 'value': value} \
             representing the ground truth values for the document
         :type ground_truth: Sequence [ Dict [ str, Union [ str, bool ]  ] ], optional
+        :param retention_in_days: How many days the document should be stored
+        :type retention_in_days: int, optional
         :param metadata: Dictionary that can be used to store additional information
         :type metadata: dict, optional
         :return: Document response from REST API
         :rtype: dict
 
         :raises: :py:class:`~las.InvalidCredentialsException`, :py:class:`~las.TooManyRequestsException`,\
  :py:class:`~las.LimitExceededException`, :py:class:`requests.exception.RequestException`
         """
-        content_bytes, guessed_content_type = parse_content(content, True)
-
-        if content_type and content_type != guessed_content_type:
-            logger.warning(f'The specified content type does not match the observed content type:'
-                           f' {content_type} != {guessed_content_type}')
+        content_bytes, _ = parse_content(content, False, False)
 
         body = {
-            'content': content_bytes,
-            'contentType': content_type or guessed_content_type,
             'consentId': consent_id,
             'datasetId': dataset_id,
             'groundTruth': ground_truth,
-            'retentionInDays': retention_in_days,
             'metadata': metadata,
+            'retentionInDays': retention_in_days,
         }
-        return self._make_request(requests.post, '/documents', body=dictstrip(body))
+
+        document = self._make_request(requests.post, '/documents', body=dictstrip(body))
+        self._make_fileserver_request(requests.put, document['fileUrl'], content=content_bytes)
+        return document
 
     def list_documents(
         self,
         *,
         consent_id: Optional[Queryparam] = None,
         dataset_id: Optional[Queryparam] = None,
         max_results: Optional[int] = None,
@@ -753,30 +783,65 @@
                 intermediate_response = self._make_request(requests.delete, '/documents', params=params)
                 response['documents'].extend(intermediate_response.get('documents'))
                 params['nextToken'] = intermediate_response['nextToken']
                 logger.info(f'Deleted {len(response["documents"])} documents so far')
 
         return response
 
-    def get_document(self, document_id: str) -> Dict:
+    def get_document(
+        self,
+        document_id: str,
+        *,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        page: Optional[int] = None,
+        rotation: Optional[int] = None,
+        density: Optional[int] = None,
+    ) -> Dict:
         """Get document, calls the GET /documents/{documentId} endpoint.
 
         >>> from las.client import Client
         >>> client = Client()
         >>> client.get_document('<document id>')
 
         :param document_id: Id of the document
         :type document_id: str
+        :param width: Convert document file to JPEG with this px width
+        :type width: int, optional
+        :param height: Convert document file to JPEG with this px height
+        :type height: int, optional
+        :param page: Convert this page from PDF/TIFF document to JPEG, 0-indexed. Negative indices supported.
+        :type page: int, optional
+        :param rotation: Convert document file to JPEG and rotate it by rotation amount degrees
+        :type rotation: int, optional
+        :param density: Convert PDF/TIFF document to JPEG with this density setting
+        :type density: int, optional
         :return: Document response from REST API
         :rtype: dict
 
         :raises: :py:class:`~las.InvalidCredentialsException`, :py:class:`~las.TooManyRequestsException`,\
  :py:class:`~las.LimitExceededException`, :py:class:`requests.exception.RequestException`
         """
-        return self._make_request(requests.get, f'/documents/{document_id}')
+        document = self._make_request(requests.get, f'/documents/{document_id}')
+        query_params = dictstrip({
+            'width': width,
+            'height': height,
+            'page': page,
+            'rotation': rotation,
+            'density': density,
+        })
+
+        if query_params or 'content' not in document:
+            document['content'] = b64encode(self._make_fileserver_request(
+                requests_fn=requests.get,
+                file_url=document['fileUrl'],
+                query_params=query_params,
+            )).decode()
+
+        return document
 
     def update_document(
         self,
         document_id: str,
         ground_truth: Sequence[Dict[str, Union[Optional[str], bool]]] = None, # For backwards compatibility reasons, this is placed before the *
         *,
         metadata: Optional[dict] = None,
```

### Comparing `lucidtech-las-9.0.0/las/credentials.py` & `lucidtech-las-9.1.0/las/credentials.py`

 * *Files identical despite different names*

### Comparing `lucidtech-las-9.0.0/lucidtech_las.egg-info/PKG-INFO` & `lucidtech-las-9.1.0/lucidtech_las.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidtech-las
-Version: 9.0.0
+Version: 9.1.0
 Summary: Python SDK for Lucidtech AI Services
 Home-page: https://github.com/LucidtechAI/las-sdk-python
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: Magnus Aarskaug Rud
 Maintainer-email: magnus@lucidtech.ai
 License: Apache 2.0
```

### Comparing `lucidtech-las-9.0.0/setup.py` & `lucidtech-las-9.1.0/setup.py`

 * *Files identical despite different names*

