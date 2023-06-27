# Comparing `tmp/onnx_clip-3.0.0.tar.gz` & `tmp/onnx_clip-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx_clip-3.0.0.tar", max compression
+gzip compressed data, was "onnx_clip-3.1.0.tar", max compression
```

## Comparing `onnx_clip-3.0.0.tar` & `onnx_clip-3.1.0.tar`

### file list

```diff
@@ -1,13 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-05-26 14:28:02.956223 onnx_clip-3.0.0/LICENSE
--rw-r--r--   0        0        0     3521 2023-05-26 14:28:02.956375 onnx_clip-3.0.0/README.md
--rw-r--r--   0        0        0      393 2023-06-05 07:29:34.069013 onnx_clip-3.0.0/onnx_clip/__init__.py
--rw-r--r--   0        0        0       43 2023-05-26 14:28:02.956934 onnx_clip-3.0.0/onnx_clip/data/.gitattributes
--rw-r--r--   0        0        0   252444 2023-05-26 14:28:02.958500 onnx_clip-3.0.0/onnx_clip/data/CLIP.png
--rw-r--r--   0        0        0  1356917 2023-05-26 14:28:02.960272 onnx_clip-3.0.0/onnx_clip/data/bpe_simple_vocab_16e6.txt.gz
--rw-r--r--   0        0        0   602240 2023-05-26 14:28:02.962273 onnx_clip-3.0.0/onnx_clip/data/expected_preprocessed_image.npy
--rw-r--r--   0        0        0    80530 2023-05-26 14:28:02.962532 onnx_clip-3.0.0/onnx_clip/data/franz-kafka.jpg
--rw-r--r--   0        0        0    10985 2023-06-05 07:29:10.831158 onnx_clip-3.0.0/onnx_clip/model.py
--rw-r--r--   0        0        0     6955 2023-06-05 07:29:10.831843 onnx_clip-3.0.0/onnx_clip/preprocessor.py
--rw-r--r--   0        0        0     7659 2023-05-26 14:28:02.962928 onnx_clip-3.0.0/onnx_clip/tokenizer.py
--rw-r--r--   0        0        0      737 2023-06-05 07:29:10.832260 onnx_clip-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     4468 1970-01-01 00:00:00.000000 onnx_clip-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 08:11:42.387791 onnx_clip-3.1.0/LICENSE
+-rw-r--r--   0        0        0     3521 2023-06-27 08:11:42.387886 onnx_clip-3.1.0/README.md
+-rw-r--r--   0        0        0      393 2023-06-27 08:11:42.388122 onnx_clip-3.1.0/onnx_clip/__init__.py
+-rw-r--r--   0        0        0    11323 2023-06-27 11:22:25.428442 onnx_clip-3.1.0/onnx_clip/model.py
+-rw-r--r--   0        0        0     6955 2023-06-27 08:11:42.392667 onnx_clip-3.1.0/onnx_clip/preprocessor.py
+-rw-r--r--   0        0        0     7659 2023-06-27 08:11:42.392771 onnx_clip-3.1.0/onnx_clip/tokenizer.py
+-rw-r--r--   0        0        0      863 2023-06-27 11:30:56.865289 onnx_clip-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 onnx_clip-3.1.0/PKG-INFO
```

### Comparing `onnx_clip-3.0.0/LICENSE` & `onnx_clip-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx_clip-3.0.0/README.md` & `onnx_clip-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `onnx_clip-3.0.0/onnx_clip/model.py` & `onnx_clip-3.1.0/onnx_clip/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import errno
 import os
 import logging
+from pathlib import Path
 from typing import List, Tuple, Union, Iterable, Iterator, TypeVar, Optional
+import requests
 
 import numpy as np
 import onnxruntime as ort
 from PIL import Image
-import boto3
-from botocore import UNSIGNED
-from botocore.client import Config
 
 from onnx_clip import Preprocessor, Tokenizer
 
 
 def softmax(x: np.ndarray) -> np.ndarray:
     """
     Computes softmax values for each sets of scores in x.
@@ -180,27 +179,34 @@
             else:
                 raise FileNotFoundError(
                     errno.ENOENT,
                     os.strerror(errno.ENOENT),
                     path,
                 )
         except Exception:
+            s3_url = f"https://lakera-clip.s3.eu-west-1.amazonaws.com/{os.path.basename(path)}"
             if not silent:
                 logging.info(
                     f"The model file ({path}) doesn't exist "
                     f"or it is invalid. Downloading it from the public S3 "
-                    f"bucket: https://lakera-clip.s3.eu-west-1.amazonaws.com/{os.path.basename(path)}."  # noqa: E501
+                    f"bucket: {s3_url}."  # noqa: E501
                 )
-            # Download from S3
-            s3_client = boto3.client(
-                "s3", config=Config(signature_version=UNSIGNED)
-            )
-            s3_client.download_file(
-                "lakera-clip", os.path.basename(path), path
-            )
+
+            # Download from S3 
+            # Saving to a temporary file first to avoid corrupting the file
+            temporary_filename = Path(path).with_name(os.path.basename(path) + '.part')
+            with requests.get(s3_url, stream=True) as r:
+                r.raise_for_status()
+                with open(temporary_filename, 'wb') as f:
+                    for chunk in r.iter_content(chunk_size=8192): 
+                        f.write(chunk)
+                    f.flush()
+            # Finally move the temporary file to the correct location
+            temporary_filename.rename(path)
+
             # `providers` need to be set explicitly since ORT 1.9
             return ort.InferenceSession(
                 path, providers=ort.get_available_providers()
             )
 
     def get_image_embeddings(
         self,
```

### Comparing `onnx_clip-3.0.0/onnx_clip/preprocessor.py` & `onnx_clip-3.1.0/onnx_clip/preprocessor.py`

 * *Files identical despite different names*

### Comparing `onnx_clip-3.0.0/onnx_clip/tokenizer.py` & `onnx_clip-3.1.0/onnx_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `onnx_clip-3.0.0/pyproject.toml` & `onnx_clip-3.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "onnx_clip"
-version = "3.0.0"
+version = "3.1.0"
 description = "CLIP with ONNX Runtime and without PyTorch dependencies."
 readme = "README.md"
 authors = ["Lakera AI <dev@lakera.ai>"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/lakeraai/onnx_clip"
 
 [tool.poetry.dependencies]
 python = "^3.6.1"
-numpy = "^1.18.0"
+numpy = "^1.18.0,<1.24.0" # somehow 1.24 installation fails
 opencv-python-headless = "^4.0.1"
 onnxruntime = ">=1.4.0"
 pillow = "^8.4.0"
 ftfy = "^6.0.3"
 regex = "*"
-boto3 = "^1.23.10"
-importlib_metadata = ">=4.8"  # Supported by Python 3.6
+importlib_metadata = ">=4.8"  # Supported by Python 3.6
+requests = "^2.26.0" # Supported by Python 3.6
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^6.0.0"
```

### Comparing `onnx_clip-3.0.0/PKG-INFO` & `onnx_clip-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: onnx-clip
-Version: 3.0.0
+Version: 3.1.0
 Summary: CLIP with ONNX Runtime and without PyTorch dependencies.
 Author: Lakera AI
 Author-email: dev@lakera.ai
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: boto3 (>=1.23.10,<2.0.0)
 Requires-Dist: ftfy (>=6.0.3,<7.0.0)
 Requires-Dist: importlib_metadata (>=4.8)
-Requires-Dist: numpy (>=1.18.0,<2.0.0)
+Requires-Dist: numpy (>=1.18.0,<1.24.0)
 Requires-Dist: onnxruntime (>=1.4.0)
 Requires-Dist: opencv-python-headless (>=4.0.1,<5.0.0)
 Requires-Dist: pillow (>=8.4.0,<9.0.0)
 Requires-Dist: regex
+Requires-Dist: requests (>=2.26.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # onnx_clip
 
 An [ONNX](https://onnx.ai/)-based implementation of [CLIP](https://github.com/openai/CLIP) that doesn't
 depend on `torch` or `torchvision`.
 It also has a friendlier API than the original implementation.
```

