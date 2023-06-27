# Comparing `tmp/m-filetypes-0.1.5.tar.gz` & `tmp/m-filetypes-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-filetypes-0.1.5.tar", last modified: Fri Jan 13 09:57:58 2023, max compression
+gzip compressed data, was "m-filetypes-0.1.6.tar", last modified: Tue Jun 27 14:52:24 2023, max compression
```

## Comparing `m-filetypes-0.1.5.tar` & `m-filetypes-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 09:57:58.535333 m-filetypes-0.1.5/
--rw-r--r--   0 root         (0) root         (0)     2056 2023-01-13 09:57:58.535333 m-filetypes-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      909 2023-01-03 11:23:52.000000 m-filetypes-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 09:57:58.530333 m-filetypes-0.1.5/m_filetypes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2056 2023-01-13 09:57:58.000000 m-filetypes-0.1.5/m_filetypes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      388 2023-01-13 09:57:58.000000 m-filetypes-0.1.5/m_filetypes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 09:57:58.000000 m-filetypes-0.1.5/m_filetypes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-13 09:57:58.000000 m-filetypes-0.1.5/m_filetypes.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 09:57:58.525333 m-filetypes-0.1.5/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 09:57:58.525333 m-filetypes-0.1.5/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 09:57:58.534333 m-filetypes-0.1.5/mobio/libs/filetypes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-03 10:16:27.000000 m-filetypes-0.1.5/mobio/libs/filetypes/__init__.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-01-13 09:56:48.000000 m-filetypes-0.1.5/mobio/libs/filetypes/common.py
--rw-r--r--   0 root         (0) root         (0)    40903 2023-01-03 10:16:27.000000 m-filetypes-0.1.5/mobio/libs/filetypes/custom_mimetypes.py
--rw-r--r--   0 root         (0) root         (0)     3375 2023-01-13 09:56:48.000000 m-filetypes-0.1.5/mobio/libs/filetypes/file.py
--rw-r--r--   0 root         (0) root         (0)    17485 2023-01-03 11:23:52.000000 m-filetypes-0.1.5/mobio/libs/filetypes/file_signature.json
--rw-r--r--   0 root         (0) root         (0)     2565 2023-01-03 10:16:27.000000 m-filetypes-0.1.5/mobio/libs/filetypes/utils.py
--rwxr-xr-x   0 root         (0) root         (0)      104 2023-01-03 10:16:27.000000 m-filetypes-0.1.5/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-01-13 09:57:58.537333 m-filetypes-0.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8814 2023-01-13 09:57:57.000000 m-filetypes-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:52:24.930247 m-filetypes-0.1.6/
+-rwxr-xr-x   0 root         (0) root         (0)     1073 2023-06-27 14:50:54.000000 m-filetypes-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-06-27 14:52:24.930247 m-filetypes-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      980 2023-06-27 14:50:54.000000 m-filetypes-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:52:24.925247 m-filetypes-0.1.6/m_filetypes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-06-27 14:52:24.000000 m-filetypes-0.1.6/m_filetypes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-27 14:52:24.000000 m-filetypes-0.1.6/m_filetypes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 14:52:24.000000 m-filetypes-0.1.6/m_filetypes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-27 14:52:24.000000 m-filetypes-0.1.6/m_filetypes.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:52:24.917247 m-filetypes-0.1.6/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:52:24.917247 m-filetypes-0.1.6/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:52:24.929247 m-filetypes-0.1.6/mobio/libs/filetypes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 14:50:54.000000 m-filetypes-0.1.6/mobio/libs/filetypes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-06-27 14:50:54.000000 m-filetypes-0.1.6/mobio/libs/filetypes/common.py
+-rw-r--r--   0 root         (0) root         (0)    40957 2023-06-27 14:50:54.000000 m-filetypes-0.1.6/mobio/libs/filetypes/custom_mimetypes.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2023-06-27 14:50:54.000000 m-filetypes-0.1.6/mobio/libs/filetypes/file.py
+-rw-r--r--   0 root         (0) root         (0)    17872 2023-06-27 14:50:54.000000 m-filetypes-0.1.6/mobio/libs/filetypes/file_signature.json
+-rw-r--r--   0 root         (0) root         (0)     2565 2023-06-27 14:50:54.000000 m-filetypes-0.1.6/mobio/libs/filetypes/utils.py
+-rwxr-xr-x   0 root         (0) root         (0)      104 2023-06-27 14:50:54.000000 m-filetypes-0.1.6/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)       38 2023-06-27 14:52:24.931247 m-filetypes-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-06-27 14:52:24.000000 m-filetypes-0.1.6/setup.py
```

### Comparing `m-filetypes-0.1.5/PKG-INFO` & `m-filetypes-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 Metadata-Version: 2.1
 Name: m-filetypes
-Version: 0.1.5
+Version: 0.1.6
 Summary: Mobio Filetype Libs
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: ##  Thư viện kiểm tra file type.
-        
-        ### Cài đặt:
-        
-        ```bash
-         $ pip3 install m-filetype
-         ```
-        
-        ### Sử dụng
-        ```python
-        from mobio.sdks.filetype.file import File
-        from mobio.sdks.filetype.common import ExtensionImage
-        
-        File.check_filetype_by_file_extensions(
-            file_binary=file, # Check filetype của định dạng file binary.Mặc định None
-            file_path=file_path, # Check filetype của path file
-            extensions=[ExtensionImage.PNG] # Danh sách extension cần check.
-        )
-        
-        ```
-        
-        #### Lấy extensions support
-        - Extension Image:
-        ```python
-        from mobio.sdks.filetype.common import ExtensionImage
-        ExtensionImage.LIST_EXTENSION_SUPPORTED
-        ```
-        - Extension Document:
-        ```python
-        from mobio.sdks.filetype.common import ExtensionDocument
-        ExtensionDocument.LIST_EXTENSION_SUPPORTED
-        ```
-        - Extension Audio:
-        ```python
-        from mobio.sdks.filetype.common import ExtensionAudio
-        ExtensionAudio.LIST_EXTENSION_SUPPORTED
-        ```
 Keywords: mobio,filetype,contact spam
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+##  Thư viện kiểm tra file type.
+
+### Cài đặt:
+
+```bash
+ $ pip3 install m-filetype
+ ```
+
+Link chữ ký: https://en.wikipedia.org/wiki/List_of_file_signatures
+
+### Sử dụng
+```python
+from mobio.sdks.filetype.file import File
+from mobio.sdks.filetype.common import ExtensionImage
+
+File.check_filetype_by_file_extensions(
+    file_binary=file, # Check filetype của định dạng file binary.Mặc định None
+    file_path=file_path, # Check filetype của path file
+    extensions=[ExtensionImage.PNG] # Danh sách extension cần check.
+)
+
+```
+
+#### Lấy extensions support
+- Extension Image:
+```python
+from mobio.sdks.filetype.common import ExtensionImage
+ExtensionImage.LIST_EXTENSION_SUPPORTED
+```
+- Extension Document:
+```python
+from mobio.sdks.filetype.common import ExtensionDocument
+ExtensionDocument.LIST_EXTENSION_SUPPORTED
+```
+- Extension Audio:
+```python
+from mobio.sdks.filetype.common import ExtensionAudio
+ExtensionAudio.LIST_EXTENSION_SUPPORTED
+```
```

### Comparing `m-filetypes-0.1.5/README.md` & `m-filetypes-0.1.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 ### Cài đặt:
 
 ```bash
  $ pip3 install m-filetype
  ```
 
+Link chữ ký: https://en.wikipedia.org/wiki/List_of_file_signatures
+
 ### Sử dụng
 ```python
 from mobio.sdks.filetype.file import File
 from mobio.sdks.filetype.common import ExtensionImage
 
 File.check_filetype_by_file_extensions(
     file_binary=file, # Check filetype của định dạng file binary.Mặc định None
```

### Comparing `m-filetypes-0.1.5/m_filetypes.egg-info/PKG-INFO` & `m-filetypes-0.1.6/m_filetypes.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 Metadata-Version: 2.1
 Name: m-filetypes
-Version: 0.1.5
+Version: 0.1.6
 Summary: Mobio Filetype Libs
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: ##  Thư viện kiểm tra file type.
-        
-        ### Cài đặt:
-        
-        ```bash
-         $ pip3 install m-filetype
-         ```
-        
-        ### Sử dụng
-        ```python
-        from mobio.sdks.filetype.file import File
-        from mobio.sdks.filetype.common import ExtensionImage
-        
-        File.check_filetype_by_file_extensions(
-            file_binary=file, # Check filetype của định dạng file binary.Mặc định None
-            file_path=file_path, # Check filetype của path file
-            extensions=[ExtensionImage.PNG] # Danh sách extension cần check.
-        )
-        
-        ```
-        
-        #### Lấy extensions support
-        - Extension Image:
-        ```python
-        from mobio.sdks.filetype.common import ExtensionImage
-        ExtensionImage.LIST_EXTENSION_SUPPORTED
-        ```
-        - Extension Document:
-        ```python
-        from mobio.sdks.filetype.common import ExtensionDocument
-        ExtensionDocument.LIST_EXTENSION_SUPPORTED
-        ```
-        - Extension Audio:
-        ```python
-        from mobio.sdks.filetype.common import ExtensionAudio
-        ExtensionAudio.LIST_EXTENSION_SUPPORTED
-        ```
 Keywords: mobio,filetype,contact spam
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+##  Thư viện kiểm tra file type.
+
+### Cài đặt:
+
+```bash
+ $ pip3 install m-filetype
+ ```
+
+Link chữ ký: https://en.wikipedia.org/wiki/List_of_file_signatures
+
+### Sử dụng
+```python
+from mobio.sdks.filetype.file import File
+from mobio.sdks.filetype.common import ExtensionImage
+
+File.check_filetype_by_file_extensions(
+    file_binary=file, # Check filetype của định dạng file binary.Mặc định None
+    file_path=file_path, # Check filetype của path file
+    extensions=[ExtensionImage.PNG] # Danh sách extension cần check.
+)
+
+```
+
+#### Lấy extensions support
+- Extension Image:
+```python
+from mobio.sdks.filetype.common import ExtensionImage
+ExtensionImage.LIST_EXTENSION_SUPPORTED
+```
+- Extension Document:
+```python
+from mobio.sdks.filetype.common import ExtensionDocument
+ExtensionDocument.LIST_EXTENSION_SUPPORTED
+```
+- Extension Audio:
+```python
+from mobio.sdks.filetype.common import ExtensionAudio
+ExtensionAudio.LIST_EXTENSION_SUPPORTED
+```
```

### Comparing `m-filetypes-0.1.5/mobio/libs/filetypes/common.py` & `m-filetypes-0.1.6/mobio/libs/filetypes/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 
 class ExtensionImage:
     GIF = "gif"
     JPG = "jpg"
     JPEG = "jpeg"
     PNG = "png"
+    HEIC = "heic"
+    HEIF = "heif"
 
-    LIST_EXTENSION_SUPPORTED = [GIF, JPEG, PNG, JPG]
+    LIST_EXTENSION_SUPPORTED = [GIF, JPEG, PNG, JPG, HEIC, HEIF]
 
 
 class ExtensionDocument:
     DOC = "doc"
     DOCX = "docx"
     XLS = "xls"
     XLSX = "xlsx"
@@ -38,14 +40,17 @@
     MPG = "mpg"
     OGV = "ogv"
     WEBM = "webm"
     FLV = "flv"
     MKV = "mkv"
     ASX = "asx"
     WMV = "wmv"
+    HEVC = "hevc"
+    HDOT264 = "h.264"
 
-    LIST_EXTENSION_SUPPORTED = [MP3, MP4, MOV, AVI, THREE_GP, THREE_G2, M4V, MPEG, MPG, OGV, WEBM, FLV, MKV, ASX, WMV]
+    LIST_EXTENSION_SUPPORTED = [MP3, MP4, MOV, AVI, THREE_GP, THREE_G2, M4V, MPEG, MPG, OGV, WEBM, FLV, MKV, ASX, WMV,
+                                HEVC, HDOT264]
 
 
 class ParamFileSignature:
     SIGNS = "signs"
     MIME = "mime"
```

### Comparing `m-filetypes-0.1.5/mobio/libs/filetypes/custom_mimetypes.py` & `m-filetypes-0.1.6/mobio/libs/filetypes/custom_mimetypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,16 @@
     '.pbm': 'image/x-portable-bitmap',
     '.pgm': 'image/x-portable-graymap',
     '.ppm': 'image/x-portable-pixmap',
     '.rgb': 'image/x-rgb',
     '.xbm': 'image/x-xbitmap',
     '.xpm': 'image/x-xpixmap',
     '.xwd': 'image/x-xwindowdump',
+    '.heif': 'image/heif',
+    '.heic': 'image/heic',
     '.eml': 'message/rfc822',
     '.mht': 'message/rfc822',
     '.mhtml': 'message/rfc822',
     '.nws': 'message/rfc822',
     '.css': 'text/css',
     '.csv': 'text/csv',
     '.html': 'text/html',
```

### Comparing `m-filetypes-0.1.5/mobio/libs/filetypes/file.py` & `m-filetypes-0.1.6/mobio/libs/filetypes/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import os
 
-from mobio.libs.filetypes.common import ExtensionDocument, ExtensionAudio
+from mobio.libs.filetypes.common import ExtensionDocument, ExtensionAudio, ExtensionImage
 # from ..filetypes.utils import read_file_to_hex_data_by_path, load_signature_by_hex_data, \
 #     read_file_to_hex_data_by_file_binary, get_max_offset_extensions
 from mobio.libs.filetypes.utils import read_file_to_hex_data_by_path, load_signature_by_hex_data, \
     read_file_to_hex_data_by_file_binary, get_max_offset_extensions
+
 logger = logging.getLogger()
 logger.setLevel(logging.DEBUG)
 
 
 class File(object):
 
     def __init__(self):
@@ -31,24 +32,24 @@
         return
 
     @staticmethod
     def get_extension_by_filepath(filepath, max_offset_extensions):
         # Validate filepath
         File.validate_input_filepath(filepath)
         hex_data_file = read_file_to_hex_data_by_path(filepath, max_offset_extensions)
-        logger.debug("get_extension_by_filepath :: hex_data_file :: %s" % str(hex_data_file))
+        # logger.debug("get_extension_by_filepath :: hex_data_file :: %s" % str(hex_data_file))
         lst_extension = load_signature_by_hex_data(hex_data_file)
         logger.debug("get_extension_by_filepath :: lst_extension :: %s" % str(lst_extension))
         return lst_extension
 
     @staticmethod
     def get_extension_by_file_binary(file_binary, max_offset_extensions):
         # Validate filepath
         hex_data_file = read_file_to_hex_data_by_file_binary(file_binary, max_offset_extensions)
-        logger.debug("get_extension_by_file_binary :: hex_data_file :: %s" % str(hex_data_file))
+        # logger.debug("get_extension_by_file_binary :: hex_data_file :: %s" % str(hex_data_file))
         lst_extension = load_signature_by_hex_data(hex_data_file)
         logger.debug("get_extension_by_file_binary :: lst_extension :: %s" % str(lst_extension))
         return lst_extension
 
     @staticmethod
     def check_filetype_by_file_extensions(filepath=None, file_binary=None, extensions=None):
         File.validate_input_extension(extensions)
@@ -68,9 +69,14 @@
             "status": len(result_merge_extension) > 0,
             "extension_of_file": lst_extension
         }
         return result
 
 
 if __name__ == '__main__':
-    File.check_filetype_by_file_extensions("/Users/tungdd/Downloads/call-vn-1-9N3L6CSU0J-1668541175511.mp3",
-                                           extensions=ExtensionAudio.LIST_EXTENSION_SUPPORTED)
+    lst_extension_support = ExtensionAudio.LIST_EXTENSION_SUPPORTED + ExtensionDocument.LIST_EXTENSION_SUPPORTED + ExtensionImage.LIST_EXTENSION_SUPPORTED
+
+    result = File.check_filetype_by_file_extensions(
+        "/Users/tungdd/Downloads/sample1.heif",
+        extensions=lst_extension_support
+    )
+    print(result)
```

### Comparing `m-filetypes-0.1.5/mobio/libs/filetypes/file_signature.json` & `m-filetypes-0.1.6/mobio/libs/filetypes/file_signature.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9739247311827958%*

 * *Differences: {"'hdot264'": "OrderedDict([('signs', ['0,0000000167']), ('mime', 'video/h.264')])",*

 * * "'heic'": "OrderedDict([('signs', ['0,000000206674797068656963']), ('mime', 'image/heic')])",*

 * * "'heif'": "OrderedDict([('signs', ['0,0000010000000048656966']), ('mime', 'image/heif')])",*

 * * "'hevc'": "OrderedDict([('signs', ['0,000000014201']), ('mime', 'video/mp4')])",*

 * * "'xlsx'": "{'signs': {insert: [(1, '0,504B0304')]}}"}*

```diff
@@ -270,21 +270,45 @@
     },
     "gz": {
         "mime": "application/gzip",
         "signs": [
             "0,1F8B08"
         ]
     },
+    "hdot264": {
+        "mime": "video/h.264",
+        "signs": [
+            "0,0000000167"
+        ]
+    },
     "hdr": {
         "mime": "image/vnd.radiance",
         "signs": [
             "0,233F52414449414E43450A",
             "0,49536328"
         ]
     },
+    "heic": {
+        "mime": "image/heic",
+        "signs": [
+            "0,000000206674797068656963"
+        ]
+    },
+    "heif": {
+        "mime": "image/heif",
+        "signs": [
+            "0,0000010000000048656966"
+        ]
+    },
+    "hevc": {
+        "mime": "video/mp4",
+        "signs": [
+            "0,000000014201"
+        ]
+    },
     "hqx": {
         "mime": "application/mac-binhex40",
         "signs": [
             "0,28546869732066696C65206D75737420626520636F6E76657274656420776974682042696E48657820"
         ]
     },
     "ico": {
@@ -957,14 +981,15 @@
             "512,FDFFFFFF20000000"
         ]
     },
     "xlsx": {
         "mime": "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
         "signs": [
             "0,504B030414000",
+            "0,504B0304",
             "-36,504B0506"
         ]
     },
     "xpi": {
         "mime": "application/x-xpinstall",
         "signs": [
             "0,504B0304"
```

### Comparing `m-filetypes-0.1.5/mobio/libs/filetypes/utils.py` & `m-filetypes-0.1.6/mobio/libs/filetypes/utils.py`

 * *Files identical despite different names*

### Comparing `m-filetypes-0.1.5/setup.py` & `m-filetypes-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         :param filename:
         :return:
         """
         requirements = []
         return requirements
 
 
-version_dev='0.1.7'
-version_prod='0.1.5'
+version_dev='0.1.9'
+version_prod='0.1.6'
 
 run_mode=''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -51,15 +51,15 @@
     name="m-filetypes" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.5',  # Required
+    version='0.1.6',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio Filetype Libs",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

