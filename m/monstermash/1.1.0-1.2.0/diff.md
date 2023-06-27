# Comparing `tmp/monstermash-1.1.0.tar.gz` & `tmp/monstermash-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstermash-1.1.0.tar", max compression
+gzip compressed data, was "monstermash-1.2.0.tar", max compression
```

## Comparing `monstermash-1.1.0.tar` & `monstermash-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0     1366 2023-06-25 04:39:34.307284 monstermash-1.1.0/README.md
--rw-r--r--   0        0        0     1080 2023-06-25 04:39:34.311284 monstermash-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-25 04:39:34.311284 monstermash-1.1.0/src/monstermash/__init__.py
--rw-r--r--   0        0        0     1646 2023-06-25 04:39:34.311284 monstermash-1.1.0/src/monstermash/__main__.py
--rw-r--r--   0        0        0     1772 2023-06-25 04:39:34.311284 monstermash-1.1.0/src/monstermash/crypt.py
--rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 monstermash-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1366 2023-06-27 12:20:06.360975 monstermash-1.2.0/README.md
+-rw-r--r--   0        0        0     1152 2023-06-27 12:20:06.360975 monstermash-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-06-27 12:20:06.360975 monstermash-1.2.0/src/monstermash/__init__.py
+-rw-r--r--   0        0        0     4196 2023-06-27 12:20:06.360975 monstermash-1.2.0/src/monstermash/__main__.py
+-rw-r--r--   0        0        0      365 2023-06-27 12:20:06.360975 monstermash-1.2.0/src/monstermash/config.py
+-rw-r--r--   0        0        0     1699 2023-06-27 12:20:06.360975 monstermash-1.2.0/src/monstermash/crypt.py
+-rw-r--r--   0        0        0      117 2023-06-27 12:20:06.360975 monstermash-1.2.0/src/monstermash/datamodels.py
+-rw-r--r--   0        0        0      406 2023-06-27 12:20:06.360975 monstermash-1.2.0/src/monstermash/parser.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:20:06.360975 monstermash-1.2.0/src/monstermash/utils/__init__.py
+-rw-r--r--   0        0        0      274 2023-06-27 12:20:06.360975 monstermash-1.2.0/src/monstermash/utils/file.py
+-rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 monstermash-1.2.0/PKG-INFO
```

### Comparing `monstermash-1.1.0/README.md` & `monstermash-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  🧟 Monstermash
 
-> 1️⃣ version: 1.1.0
+> 1️⃣ version: 1.2.0
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

### Comparing `monstermash-1.1.0/src/monstermash/crypt.py` & `monstermash-1.2.0/src/monstermash/crypt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from nacl.encoding import HexEncoder
 from nacl.public import Box, PrivateKey, PublicKey
-from pydantic import BaseModel, SecretStr
 
-
-class KeyPair(BaseModel):
-    private_key: SecretStr
-    public_key: str
+from monstermash.datamodels import KeyPair
 
 
 class Crypt:
     key_length: int = 32
 
     def __init__(self, private_key: bytes, msg_encoder=HexEncoder, key_encoder=HexEncoder):
         self.msg_encoder = msg_encoder
```

### Comparing `monstermash-1.1.0/PKG-INFO` & `monstermash-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstermash
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Author: Mitchell Lisle
 Author-email: m.lisle90@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pynacl (>=1.5.0,<2.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ##  🧟 Monstermash
 
-> 1️⃣ version: 1.1.0
+> 1️⃣ version: 1.2.0
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

