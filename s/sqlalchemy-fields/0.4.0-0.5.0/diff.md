# Comparing `tmp/sqlalchemy_fields-0.4.0.tar.gz` & `tmp/sqlalchemy_fields-0.5.0.tar.gz`

## Comparing `sqlalchemy_fields-0.4.0.tar` & `sqlalchemy_fields-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/exceptions.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/__init__.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/base.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/filesystem.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/s3.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/utils.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/__init__.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/email.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/file.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/image.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/ip.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/url.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/uuid.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/README.md
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/exceptions.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/storages/__init__.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/storages/base.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/storages/filesystem.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/storages/s3.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/storages/utils.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/__init__.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/email.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/file.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/image.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/ip.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/url.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/uuid.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/README.md
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.5.0/PKG-INFO
```

### Comparing `sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/base.py` & `sqlalchemy_fields-0.5.0/sqlalchemy_fields/storages/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,22 @@
     def open(self, name: str) -> BinaryIO:
         ...
 
     def write(self, file: BinaryIO, name: str) -> str:
         ...
 
 
-class StorageFile:
+class StorageFile(str):
     """
     The file obect returned by the storage.
     """
 
+    def __new__(cls, name: str, storage: BaseStorage) -> "StorageFile":
+        return str.__new__(cls, storage.get_path(name))
+
     def __init__(self, *, name: str, storage: BaseStorage):
         self._name = name
         self._storage = storage
 
     @property
     def name(self) -> str:
         """File name including extension."""
@@ -64,14 +67,19 @@
 
 
 class StorageImage(StorageFile):
     """
     Inherits features of `StorageFile` and adds image specific properties.
     """
 
+    def __new__(
+        cls, name: str, storage: BaseStorage, height: int, width: int
+    ) -> "StorageImage":
+        return str.__new__(cls, storage.get_path(name))
+
     def __init__(
         self, *, name: str, storage: BaseStorage, height: int, width: int
     ) -> None:
         super().__init__(name=name, storage=storage)
         self._width = width
         self._height = height
```

### Comparing `sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/filesystem.py` & `sqlalchemy_fields-0.5.0/sqlalchemy_fields/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/s3.py` & `sqlalchemy_fields-0.5.0/sqlalchemy_fields/storages/s3.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,22 +11,35 @@
 from sqlalchemy_fields.storages.utils import secure_filename
 
 
 class S3Storage(BaseStorage):
     """
     Amazon S3 or any S3 compatible storage backend.
     You might want to use this with the `FileType` type.
-    Requires 'boto3' to be installed.
+    Requires `boto3` to be installed.
     """
 
     AWS_ACCESS_KEY_ID = os.environ.get("AWS_ACCESS_KEY_ID", "")
+    """AWS access key ID. Either set here or as an environment variable."""
+
     AWS_SECRET_ACCESS_KEY = os.environ.get("AWS_SECRET_ACCESS_KEY", "")
+    """AWS secret access key. Either set here or as an environment variable."""
+
     AWS_S3_BUCKET_NAME = ""
+    """AWS S3 bucket name to use."""
+
     AWS_S3_ENDPOINT_URL = ""
+    """AWS S3 endpoint URL."""
+
     AWS_S3_USE_SSL = True
+    """Indicate if SSL should be used."""
+
+    AWS_DEFAULT_ACL = ""
+    """Optional ACL set on the object like `public-read`.
+    By default file will be private."""
 
     def __init__(self) -> None:
         assert boto3 is not None, "'boto3' is not installed"
         assert not self.AWS_S3_ENDPOINT_URL.startswith(
             "http"
         ), "URL should not contain protocol"
 
@@ -69,9 +82,9 @@
     def write(self, file: BinaryIO, name: str) -> str:
         """
         Write input file which is opened in binary mode to destination.
         """
 
         file.seek(0, 0)
         key = self.get_name(name)
-        self._bucket.upload_fileobj(file, key)
+        self._bucket.upload_fileobj(file, key, ExtraArgs={"ACL": self.AWS_DEFAULT_ACL})
         return key
```

### Comparing `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/email.py` & `sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/email.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/file.py` & `sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/file.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/image.py` & `sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/image.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/ip.py` & `sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/ip.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/url.py` & `sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/url.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/uuid.py` & `sqlalchemy_fields-0.5.0/sqlalchemy_fields/types/uuid.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.4.0/.gitignore` & `sqlalchemy_fields-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.4.0/LICENSE.txt` & `sqlalchemy_fields-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.4.0/README.md` & `sqlalchemy_fields-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.4.0/pyproject.toml` & `sqlalchemy_fields-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -61,40 +61,37 @@
 [tool.hatch.envs.default]
 dependencies = [
   "black==22.10.0",
   "boto3~=1.25",
   "build==0.9.0",
   "coverage==6.5.0",
   "email-validator==1.3.0",
-  "isort==5.10.1",
   "moto==4.1.2",
   "mypy==0.982",
   "Pillow==9.4.0",
   "psycopg2-binary==2.9.5",
   "pytest==7.2.0",
   "ruff==0.0.237",
 ]
 
 [tool.hatch.envs.default.scripts]
 check = [
   "ruff .",
-  "isort --check --project=sqlalchemy_fields .",
   "black --check .",
   "mypy sqlalchemy_fields",
 ]
 cov = [
   "coverage report --show-missing --skip-covered --fail-under=99",
   "coverage xml",
 ]
 format = [
-  "isort --project=sqlalchemy_fields .",
   "black .",
   "ruff --fix .",
 ]
-test = "coverage run -a -m pytest"
+test = "coverage run -a -m pytest {args}"
 
 [tool.hatch.envs.docs]
 dependencies = [
   "mkdocs-material==8.5.7",
   "mkdocs==1.4.1",
   "mkdocstrings[python]==0.18.1",
 ]
@@ -106,17 +103,16 @@
 
 [tool.mypy]
 disallow_untyped_defs = true
 ignore_missing_imports = true
 show_error_codes = true
 no_implicit_optional = true
 
-[tool.isort]
-profile = "black"
-combine_as_imports = true
+[tool.ruff]
+select = ["E", "F", "I"]
 
 [tool.coverage.run]
 source_pkgs = [
   "sqlalchemy_fields",
   "tests",
 ]
```

### Comparing `sqlalchemy_fields-0.4.0/PKG-INFO` & `sqlalchemy_fields-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-fields
-Version: 0.4.0
+Version: 0.5.0
 Summary: SQLAlchemy fields
 Project-URL: Documentation, https://github.com/aminalaee/sqlalchemy-fields#readme
 Project-URL: Issues, https://github.com/aminalaee/sqlalchemy-fields/issues
 Project-URL: Source, https://github.com/aminalaee/sqlalchemy-fields
 Author-email: Amin Alaee <me@aminalaee.dev>
 License-Expression: MIT
 License-File: LICENSE.txt
```

