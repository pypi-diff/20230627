# Comparing `tmp/onnx_clip-3.1.0.tar.gz` & `tmp/onnx_clip-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx_clip-3.1.0.tar", max compression
+gzip compressed data, was "onnx_clip-3.1.1.tar", max compression
```

## Comparing `onnx_clip-3.1.0.tar` & `onnx_clip-3.1.1.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-06-27 08:11:42.387791 onnx_clip-3.1.0/LICENSE
--rw-r--r--   0        0        0     3521 2023-06-27 08:11:42.387886 onnx_clip-3.1.0/README.md
--rw-r--r--   0        0        0      393 2023-06-27 08:11:42.388122 onnx_clip-3.1.0/onnx_clip/__init__.py
--rw-r--r--   0        0        0    11323 2023-06-27 11:22:25.428442 onnx_clip-3.1.0/onnx_clip/model.py
--rw-r--r--   0        0        0     6955 2023-06-27 08:11:42.392667 onnx_clip-3.1.0/onnx_clip/preprocessor.py
--rw-r--r--   0        0        0     7659 2023-06-27 08:11:42.392771 onnx_clip-3.1.0/onnx_clip/tokenizer.py
--rw-r--r--   0        0        0      863 2023-06-27 11:30:56.865289 onnx_clip-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 onnx_clip-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 08:11:42.387791 onnx_clip-3.1.1/LICENSE
+-rw-r--r--   0        0        0     3516 2023-06-27 12:30:58.417471 onnx_clip-3.1.1/README.md
+-rw-r--r--   0        0        0      393 2023-06-27 08:11:42.388122 onnx_clip-3.1.1/onnx_clip/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-27 12:26:18.353339 onnx_clip-3.1.1/onnx_clip/data/.gitattributes
+-rw-r--r--   0        0        0   252444 2023-06-27 12:26:10.421048 onnx_clip-3.1.1/onnx_clip/data/CLIP.png
+-rw-r--r--   0        0        0  1356917 2023-06-27 12:26:07.301289 onnx_clip-3.1.1/onnx_clip/data/bpe_simple_vocab_16e6.txt.gz
+-rw-r--r--   0        0        0   602240 2023-06-27 12:26:13.532135 onnx_clip-3.1.1/onnx_clip/data/expected_preprocessed_image.npy
+-rw-r--r--   0        0        0    80530 2023-06-27 12:26:15.682390 onnx_clip-3.1.1/onnx_clip/data/franz-kafka.jpg
+-rw-r--r--   0        0        0    11467 2023-06-27 12:29:00.465885 onnx_clip-3.1.1/onnx_clip/model.py
+-rw-r--r--   0        0        0     6955 2023-06-27 08:11:42.392667 onnx_clip-3.1.1/onnx_clip/preprocessor.py
+-rw-r--r--   0        0        0     7659 2023-06-27 08:11:42.392771 onnx_clip-3.1.1/onnx_clip/tokenizer.py
+-rw-r--r--   0        0        0      863 2023-06-27 12:29:51.647565 onnx_clip-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4466 1970-01-01 00:00:00.000000 onnx_clip-3.1.1/PKG-INFO
```

### Comparing `onnx_clip-3.1.0/LICENSE` & `onnx_clip-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx_clip-3.1.0/README.md` & `onnx_clip-3.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 First, remove/move the downloaded LFS files, so that they're not packaged with the code.
 Otherwise, this creates a huge `.whl` file that PyPI refuses and it causes confusing errors.
 
 Then, follow [this guide](https://towardsdatascience.com/how-to-publish-a-python-package-to-pypi-using-poetry-aa804533fc6f).
 tl;dr: go to the [PyPI account page](https://pypi.org/manage/account/), generate an API token
 and put it into the `$PYPI_PASSWORD` environment variable. Then run
 ```shell
-poetry publish --build --username "__token__" --password $PYPI_PASSWORD
+poetry publish --build --username lakera --password $PYPI_PASSWORD
 ```
 
 ## Help
 
 Please let us know how we can support you: [earlyaccess@lakera.ai](mailto:earlyaccess@lakera.ai).
 
 ## LICENSE
```

### Comparing `onnx_clip-3.1.0/onnx_clip/model.py` & `onnx_clip-3.1.1/onnx_clip/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,18 @@
                     f"or it is invalid. Downloading it from the public S3 "
                     f"bucket: {s3_url}."  # noqa: E501
                 )
 
             # Download from S3 
             # Saving to a temporary file first to avoid corrupting the file
             temporary_filename = Path(path).with_name(os.path.basename(path) + '.part')
+            
+            # Create any missing directories in the path
+            temporary_filename.parent.mkdir(parents=True, exist_ok=True)
+
             with requests.get(s3_url, stream=True) as r:
                 r.raise_for_status()
                 with open(temporary_filename, 'wb') as f:
                     for chunk in r.iter_content(chunk_size=8192): 
                         f.write(chunk)
                     f.flush()
             # Finally move the temporary file to the correct location
```

### Comparing `onnx_clip-3.1.0/onnx_clip/preprocessor.py` & `onnx_clip-3.1.1/onnx_clip/preprocessor.py`

 * *Files identical despite different names*

### Comparing `onnx_clip-3.1.0/onnx_clip/tokenizer.py` & `onnx_clip-3.1.1/onnx_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `onnx_clip-3.1.0/pyproject.toml` & `onnx_clip-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "onnx_clip"
-version = "3.1.0"
+version = "3.1.1"
 description = "CLIP with ONNX Runtime and without PyTorch dependencies."
 readme = "README.md"
 authors = ["Lakera AI <dev@lakera.ai>"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `onnx_clip-3.1.0/PKG-INFO` & `onnx_clip-3.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-clip
-Version: 3.1.0
+Version: 3.1.1
 Summary: CLIP with ONNX Runtime and without PyTorch dependencies.
 Author: Lakera AI
 Author-email: dev@lakera.ai
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -99,15 +99,15 @@
 First, remove/move the downloaded LFS files, so that they're not packaged with the code.
 Otherwise, this creates a huge `.whl` file that PyPI refuses and it causes confusing errors.
 
 Then, follow [this guide](https://towardsdatascience.com/how-to-publish-a-python-package-to-pypi-using-poetry-aa804533fc6f).
 tl;dr: go to the [PyPI account page](https://pypi.org/manage/account/), generate an API token
 and put it into the `$PYPI_PASSWORD` environment variable. Then run
 ```shell
-poetry publish --build --username "__token__" --password $PYPI_PASSWORD
+poetry publish --build --username lakera --password $PYPI_PASSWORD
 ```
 
 ## Help
 
 Please let us know how we can support you: [earlyaccess@lakera.ai](mailto:earlyaccess@lakera.ai).
 
 ## LICENSE
```

