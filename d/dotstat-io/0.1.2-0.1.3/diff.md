# Comparing `tmp/dotstat_io-0.1.2.tar.gz` & `tmp/dotstat_io-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotstat_io-0.1.2.tar", max compression
+gzip compressed data, was "dotstat_io-0.1.3.tar", max compression
```

## Comparing `dotstat_io-0.1.2.tar` & `dotstat_io-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-02 17:04:57.103457 dotstat_io-0.1.2/dotstat_io/__init__.py
--rw-r--r--   0        0        0    10527 2023-06-21 07:52:47.915175 dotstat_io-0.1.2/dotstat_io/authentication.py
--rw-r--r--   0        0        0     9732 2023-06-21 07:52:47.935178 dotstat_io-0.1.2/dotstat_io/download_upload.py
--rw-r--r--   0        0        0      610 2023-06-20 14:44:00.381283 dotstat_io-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5638 2023-06-21 13:38:39.787339 dotstat_io-0.1.2/README.md
--rw-r--r--   0        0        0     6191 1970-01-01 00:00:00.000000 dotstat_io-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-02 17:04:57.103457 dotstat_io-0.1.3/dotstat_io/__init__.py
+-rw-r--r--   0        0        0    10527 2023-06-21 07:52:47.915175 dotstat_io-0.1.3/dotstat_io/authentication.py
+-rw-r--r--   0        0        0    10098 2023-06-27 13:03:05.856024 dotstat_io-0.1.3/dotstat_io/download_upload.py
+-rw-r--r--   0        0        0      610 2023-06-27 13:10:52.656847 dotstat_io-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5862 2023-06-22 09:57:29.580014 dotstat_io-0.1.3/README.md
+-rw-r--r--   0        0        0     6411 1970-01-01 00:00:00.000000 dotstat_io-0.1.3/PKG-INFO
```

### Comparing `dotstat_io-0.1.2/dotstat_io/authentication.py` & `dotstat_io-0.1.3/dotstat_io/authentication.py`

 * *Files identical despite different names*

### Comparing `dotstat_io-0.1.2/dotstat_io/download_upload.py` & `dotstat_io-0.1.3/dotstat_io/download_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # class to download or upload data from/to .Stat Suite
 class Download_upload():
 
     # Declare constants
     __ERROR  = "An error occurred: "
     __EXECUTION_IN_PROGRESS = "InProgress"
     __DOWNLOAD_SUCCESS = "Successful download"
-    __UPLOAD_SUCCESS = "The request was successfully processed"
+    __UPLOAD_SUCCESS = "The request was successfully processed "
+    __UPLOAD_FAILED = "The request failed with status code "
 
     __NAMESPACE_MESSAGE = "{http://www.sdmx.org/resources/sdmxml/schemas/v2_1/message}"
     __NAMESPACE_COMMON = "{http://www.sdmx.org/resources/sdmxml/schemas/v2_1/common}"
   
     # Initialise Download_upload
     def __init__(self, token):
         self.token = token
@@ -151,22 +152,19 @@
 
     # Upload a structure to .STAT
     def upload_structure(self, transfer_url: str, file_path: Path):
         try:
             Returned_Message = ""
 
             # Detect the encoding used in file 
-            file = open(file=file_path, mode="rb")
-            detected_encoding = chardet.detect(file.read(10000))
-            file.close()
+            detected_encoding = self.__detect_encode(file_path)
 
             # Read file as a string "r+" with the detected encoding
-            file = open(file=file_path, mode="r+", encoding=detected_encoding.get("encoding"))
-            xml_data = file.read()
-            file.close()
+            with open(file=file_path, mode="r+", encoding=detected_encoding.get("encoding")) as file:
+                xml_data = file.read()
 
             # Make sure the encoding is "utf-8"
             tree = ET.fromstring(xml_data)
             xml_data = ET.tostring(tree, encoding="utf-8", method='xml', xml_declaration=True)
 
             if (self.token == None):
                 Returned_Message = self.__ERROR  + "No token" + os.linesep
@@ -181,27 +179,42 @@
                     transfer_url, verify=True, headers=headers, data=xml_data)
         except Exception as err:
             Returned_Message = self.__ERROR  + str(err)
         else:
             try:
                 response.raise_for_status()
             except requests.exceptions.HTTPError as e:
-                Returned_Message = f'Request failed with status code {response.status_code}: {e}'
+                Returned_Message = f'{self.__UPLOAD_FAILED}{response.status_code}: {e}'
             else:
                 response_tree = ET.XML(response.content)
                 for error_message in response_tree.findall("./{0}ErrorMessage".format(self.__NAMESPACE_MESSAGE)):
                     text_element = error_message.find("./{0}Text".format(self.__NAMESPACE_COMMON))
                     if (text_element is not None):
                         if Returned_Message == "":
                             Returned_Message = self.__UPLOAD_SUCCESS + os.linesep
                         Returned_Message = Returned_Message + text_element.text + os.linesep
         finally:
             return Returned_Message
         
 
+    # Detect the encoding used in file
+    def __detect_encode(self, file_path):
+        detector = chardet.UniversalDetector()
+        detector.reset()
+        with open(file=file_path, mode="rb") as file:
+            for row in file:
+                detector.feed(row)
+                if detector.done: 
+                    break
+
+        detector.close()
+
+        return detector.result
+
+
     # Check request sent to .STAT status
     # This is a recursive function to check the execution status
     def __check_request_status(self, transfer_url, requestId, space):
         try:
             Returned_Message = ""
 
             headers = {
```

### Comparing `dotstat_io-0.1.2/pyproject.toml` & `dotstat_io-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dotstat_io"
-version = "0.1.2"
+version = "0.1.3"
 description = "Utility to download or upload data from/to .Stat Suite using ADFS authentication to connect to it"
 license = "MIT"
 authors = ["Gyorgy Gyomai <gyorgy.gyomai@oecd.org>", "Abdel Aliaoui <abdel.aliaoui@oecd.org>"]
 readme = "README.md"
 packages = [{include = "dotstat_io"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dotstat_io-0.1.2/README.md` & `dotstat_io-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -81,43 +81,47 @@
 ```python
 token = [Authentication Object Name].get_token()
 ```
 
 ### In Download_upload module, four methods are available:
 #### 1. To download a file from .Stat:
 ```python
+from dotstat_io.download_upload import Download_upload
 with Download_upload(token) as Download_upload_obj:
     Returned_Message = Download_upload_obj.download_file(
         dotstat_url, content_format, Path(file_path))
 ```
 * `dotstat_url:` URL of data to be downloaded from .Stat Suite
 * `content_format:` Format of the downloaded content
 * `file_path:` The full path where the file will downloaded
 
 #### 2. To download streamed content from .Stat:
 ```python
+from dotstat_io.download_upload import Download_upload
 with Download_upload(token) as Download_upload_obj:
     Returned_Message = Download_upload_obj.download_stream(
         dotstat_url, content_format)
 ```
 * `dotstat_url:` URL of data to be downloaded from .Stat Suite
 * `content_format:` Format of the downloaded content
 
 #### 3. To upload a data file to .Stat:
 ```python
+from dotstat_io.download_upload import Download_upload
 with Download_upload(token) as Download_upload_obj:
     Returned_Message = Download_upload_obj.upload_file(
         transfer_url, Path(file_path), space)
 ```
 * `transfer_url:` URL of the transfer service
 * `file_path:` The full path of the SDMX-CSV file, which will be uploaded to .Stat Suite
 * `space:` Data space where the file will be uploaded
 
 #### 4. To upload a structure to .Stat:
 ```python
+from dotstat_io.download_upload import Download_upload
 with Download_upload(token) as Download_upload_obj:
     Returned_Message = Download_upload_obj.upload_structure(
         transfer_url, Path(file_path))
 ```
 * `transfer_url:` URL of the transfer service
 * `file_path:` The full path of the SDMX-ML file, which will be uploaded to .Stat Suite
```

### Comparing `dotstat_io-0.1.2/PKG-INFO` & `dotstat_io-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotstat-io
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utility to download or upload data from/to .Stat Suite using ADFS authentication to connect to it
 License: MIT
 Author: Gyorgy Gyomai
 Author-email: gyorgy.gyomai@oecd.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -99,43 +99,47 @@
 ```python
 token = [Authentication Object Name].get_token()
 ```
 
 ### In Download_upload module, four methods are available:
 #### 1. To download a file from .Stat:
 ```python
+from dotstat_io.download_upload import Download_upload
 with Download_upload(token) as Download_upload_obj:
     Returned_Message = Download_upload_obj.download_file(
         dotstat_url, content_format, Path(file_path))
 ```
 * `dotstat_url:` URL of data to be downloaded from .Stat Suite
 * `content_format:` Format of the downloaded content
 * `file_path:` The full path where the file will downloaded
 
 #### 2. To download streamed content from .Stat:
 ```python
+from dotstat_io.download_upload import Download_upload
 with Download_upload(token) as Download_upload_obj:
     Returned_Message = Download_upload_obj.download_stream(
         dotstat_url, content_format)
 ```
 * `dotstat_url:` URL of data to be downloaded from .Stat Suite
 * `content_format:` Format of the downloaded content
 
 #### 3. To upload a data file to .Stat:
 ```python
+from dotstat_io.download_upload import Download_upload
 with Download_upload(token) as Download_upload_obj:
     Returned_Message = Download_upload_obj.upload_file(
         transfer_url, Path(file_path), space)
 ```
 * `transfer_url:` URL of the transfer service
 * `file_path:` The full path of the SDMX-CSV file, which will be uploaded to .Stat Suite
 * `space:` Data space where the file will be uploaded
 
 #### 4. To upload a structure to .Stat:
 ```python
+from dotstat_io.download_upload import Download_upload
 with Download_upload(token) as Download_upload_obj:
     Returned_Message = Download_upload_obj.upload_structure(
         transfer_url, Path(file_path))
 ```
 * `transfer_url:` URL of the transfer service
 * `file_path:` The full path of the SDMX-ML file, which will be uploaded to .Stat Suite
```

