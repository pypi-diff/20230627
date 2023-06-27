# Comparing `tmp/m-filetypes-test-0.1.8.tar.gz` & `tmp/m-filetypes-test-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-filetypes-test-0.1.8.tar", last modified: Mon Mar 27 04:30:11 2023, max compression
+gzip compressed data, was "m-filetypes-test-0.1.9.tar", last modified: Tue Jun 27 14:45:58 2023, max compression
```

## Comparing `m-filetypes-test-0.1.8.tar` & `m-filetypes-test-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 04:30:11.913217 m-filetypes-test-0.1.8/
--rw-r--r--   0 root         (0) root         (0)     2061 2023-03-27 04:30:11.914217 m-filetypes-test-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      909 2023-03-27 04:28:24.000000 m-filetypes-test-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 04:30:11.908217 m-filetypes-test-0.1.8/m_filetypes_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2061 2023-03-27 04:30:11.000000 m-filetypes-test-0.1.8/m_filetypes_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      408 2023-03-27 04:30:11.000000 m-filetypes-test-0.1.8/m_filetypes_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 04:30:11.000000 m-filetypes-test-0.1.8/m_filetypes_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-27 04:30:11.000000 m-filetypes-test-0.1.8/m_filetypes_test.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 04:30:11.903217 m-filetypes-test-0.1.8/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 04:30:11.903217 m-filetypes-test-0.1.8/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 04:30:11.913217 m-filetypes-test-0.1.8/mobio/libs/filetypes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 04:28:24.000000 m-filetypes-test-0.1.8/mobio/libs/filetypes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1099 2023-03-27 04:28:24.000000 m-filetypes-test-0.1.8/mobio/libs/filetypes/common.py
--rw-r--r--   0 root         (0) root         (0)    40957 2023-03-27 04:28:24.000000 m-filetypes-test-0.1.8/mobio/libs/filetypes/custom_mimetypes.py
--rw-r--r--   0 root         (0) root         (0)     3514 2023-03-27 04:28:24.000000 m-filetypes-test-0.1.8/mobio/libs/filetypes/file.py
--rw-r--r--   0 root         (0) root         (0)    17852 2023-03-27 04:28:24.000000 m-filetypes-test-0.1.8/mobio/libs/filetypes/file_signature.json
--rw-r--r--   0 root         (0) root         (0)     2565 2023-03-27 04:28:24.000000 m-filetypes-test-0.1.8/mobio/libs/filetypes/utils.py
--rwxr-xr-x   0 root         (0) root         (0)      104 2023-03-27 04:28:24.000000 m-filetypes-test-0.1.8/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-03-27 04:30:11.915217 m-filetypes-test-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8819 2023-03-27 04:30:10.000000 m-filetypes-test-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:45:58.179519 m-filetypes-test-0.1.9/
+-rwxr-xr-x   0 root         (0) root         (0)     1073 2023-06-27 14:31:53.000000 m-filetypes-test-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-27 14:45:58.179519 m-filetypes-test-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      980 2023-06-27 14:31:53.000000 m-filetypes-test-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:45:58.173519 m-filetypes-test-0.1.9/m_filetypes_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-27 14:45:58.000000 m-filetypes-test-0.1.9/m_filetypes_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-27 14:45:58.000000 m-filetypes-test-0.1.9/m_filetypes_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 14:45:58.000000 m-filetypes-test-0.1.9/m_filetypes_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-27 14:45:58.000000 m-filetypes-test-0.1.9/m_filetypes_test.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:45:58.165518 m-filetypes-test-0.1.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:45:58.165518 m-filetypes-test-0.1.9/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:45:58.178519 m-filetypes-test-0.1.9/mobio/libs/filetypes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 14:31:53.000000 m-filetypes-test-0.1.9/mobio/libs/filetypes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-06-27 14:31:53.000000 m-filetypes-test-0.1.9/mobio/libs/filetypes/common.py
+-rw-r--r--   0 root         (0) root         (0)    40957 2023-06-27 14:31:53.000000 m-filetypes-test-0.1.9/mobio/libs/filetypes/custom_mimetypes.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2023-06-27 14:31:53.000000 m-filetypes-test-0.1.9/mobio/libs/filetypes/file.py
+-rw-r--r--   0 root         (0) root         (0)    17872 2023-06-27 14:31:53.000000 m-filetypes-test-0.1.9/mobio/libs/filetypes/file_signature.json
+-rw-r--r--   0 root         (0) root         (0)     2565 2023-06-27 14:31:53.000000 m-filetypes-test-0.1.9/mobio/libs/filetypes/utils.py
+-rwxr-xr-x   0 root         (0) root         (0)      104 2023-06-27 14:31:53.000000 m-filetypes-test-0.1.9/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)       38 2023-06-27 14:45:58.180519 m-filetypes-test-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8819 2023-06-27 14:45:57.000000 m-filetypes-test-0.1.9/setup.py
```

### Comparing `m-filetypes-test-0.1.8/PKG-INFO` & `m-filetypes-test-0.1.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 Metadata-Version: 2.1
 Name: m-filetypes-test
-Version: 0.1.8
+Version: 0.1.9
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

### Comparing `m-filetypes-test-0.1.8/README.md` & `m-filetypes-test-0.1.9/README.md`

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

### Comparing `m-filetypes-test-0.1.8/m_filetypes_test.egg-info/PKG-INFO` & `m-filetypes-test-0.1.9/m_filetypes_test.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 Metadata-Version: 2.1
 Name: m-filetypes-test
-Version: 0.1.8
+Version: 0.1.9
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

### Comparing `m-filetypes-test-0.1.8/mobio/libs/filetypes/common.py` & `m-filetypes-test-0.1.9/mobio/libs/filetypes/common.py`

 * *Files identical despite different names*

### Comparing `m-filetypes-test-0.1.8/mobio/libs/filetypes/custom_mimetypes.py` & `m-filetypes-test-0.1.9/mobio/libs/filetypes/custom_mimetypes.py`

 * *Files identical despite different names*

### Comparing `m-filetypes-test-0.1.8/mobio/libs/filetypes/file.py` & `m-filetypes-test-0.1.9/mobio/libs/filetypes/file.py`

 * *Files identical despite different names*

### Comparing `m-filetypes-test-0.1.8/mobio/libs/filetypes/file_signature.json` & `m-filetypes-test-0.1.9/mobio/libs/filetypes/file_signature.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999731182795699%*

 * *Differences: {"'xlsx'": "{'signs': {insert: [(1, '0,504B0304')]}}"}*

```diff
@@ -981,14 +981,15 @@
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

### Comparing `m-filetypes-test-0.1.8/mobio/libs/filetypes/utils.py` & `m-filetypes-test-0.1.9/mobio/libs/filetypes/utils.py`

 * *Files identical despite different names*

### Comparing `m-filetypes-test-0.1.8/setup.py` & `m-filetypes-test-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         :param filename:
         :return:
         """
         requirements = []
         return requirements
 
 
-version_dev='0.1.8'
+version_dev='0.1.9'
 version_prod='0.1.5'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -51,15 +51,15 @@
     name="m-filetypes" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.8',  # Required
+    version='0.1.9',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio Filetype Libs",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

