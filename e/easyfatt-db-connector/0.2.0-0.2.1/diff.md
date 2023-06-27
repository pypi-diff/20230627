# Comparing `tmp/easyfatt_db_connector-0.2.0.tar.gz` & `tmp/easyfatt_db_connector-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfatt_db_connector-0.2.0.tar", max compression
+gzip compressed data, was "easyfatt_db_connector-0.2.1.tar", max compression
```

## Comparing `easyfatt_db_connector-0.2.0.tar` & `easyfatt_db_connector-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1092 2023-04-26 12:59:14.893885 easyfatt_db_connector-0.2.0/LICENSE
--rw-r--r--   0        0        0      676 2023-06-26 18:42:19.602373 easyfatt_db_connector-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2205 2023-06-26 18:42:58.676372 easyfatt_db_connector-0.2.0/README.md
--rw-r--r--   0        0        0       68 2023-05-05 17:04:51.361083 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/__init__.py
--rw-r--r--   0        0        0      227 2023-06-26 18:40:35.254373 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/constants.py
--rw-r--r--   0        0        0       52 2023-05-05 17:04:51.377081 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/__init__.py
--rw-r--r--   0        0        0      109 2023-06-26 18:40:35.471873 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/__init__.py
--rw-r--r--   0        0        0     6904 2023-06-26 18:40:35.472374 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/_base.py
--rw-r--r--   0        0        0     2974 2023-06-26 18:40:35.472374 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/_fdb.py
--rw-r--r--   0        0        0     5088 2023-06-26 18:40:35.478873 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/_sqlalchemy.py
--rw-r--r--   0        0        0      294 2023-05-05 17:04:51.438081 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/exceptions.py
--rw-r--r--   0        0        0       55 2023-05-06 15:37:53.636002 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/__init__.py
--rw-r--r--   0        0        0       22 2023-05-07 22:06:24.536129 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/dynamic/__init__.py
--rw-r--r--   0        0        0     1429 2023-05-08 13:00:10.987069 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/dynamic/factory.py
--rw-r--r--   0        0        0      410 2023-05-08 13:05:49.414570 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/static/__init__.py
--rw-r--r--   0        0        0    66243 2023-05-08 13:03:58.168072 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/static/models.py
--rw-r--r--   0        0        0        0 2023-06-26 18:40:35.330373 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/utils/__init__.py
--rw-r--r--   0        0        0      206 2023-06-26 18:40:35.412373 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/utils/decorators.py
--rw-r--r--   0        0        0     4397 2023-06-26 18:40:35.336373 easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/utils/downloader.py
--rw-r--r--   0        0        0     2842 1970-01-01 00:00:00.000000 easyfatt_db_connector-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-26 12:59:14.893885 easyfatt_db_connector-0.2.1/LICENSE
+-rw-r--r--   0        0        0      676 2023-06-27 16:02:56.358075 easyfatt_db_connector-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2205 2023-06-26 18:42:58.676372 easyfatt_db_connector-0.2.1/README.md
+-rw-r--r--   0        0        0       68 2023-05-05 17:04:51.361083 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/__init__.py
+-rw-r--r--   0        0        0      227 2023-06-26 18:40:35.254373 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/constants.py
+-rw-r--r--   0        0        0       52 2023-05-05 17:04:51.377081 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-26 18:40:35.471873 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/__init__.py
+-rw-r--r--   0        0        0     6880 2023-06-27 15:57:18.413422 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_base.py
+-rw-r--r--   0        0        0     3054 2023-06-27 16:02:10.307915 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_fdb.py
+-rw-r--r--   0        0        0     5088 2023-06-26 18:40:35.478873 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_sqlalchemy.py
+-rw-r--r--   0        0        0      294 2023-05-05 17:04:51.438081 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/exceptions.py
+-rw-r--r--   0        0        0       55 2023-05-06 15:37:53.636002 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-07 22:06:24.536129 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/dynamic/__init__.py
+-rw-r--r--   0        0        0     1429 2023-05-08 13:00:10.987069 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/dynamic/factory.py
+-rw-r--r--   0        0        0      410 2023-05-08 13:05:49.414570 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/static/__init__.py
+-rw-r--r--   0        0        0    66243 2023-05-08 13:03:58.168072 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/static/models.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:40:35.330373 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/utils/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-26 18:40:35.412373 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/utils/decorators.py
+-rw-r--r--   0        0        0     4397 2023-06-26 18:40:35.336373 easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/utils/downloader.py
+-rw-r--r--   0        0        0     2842 1970-01-01 00:00:00.000000 easyfatt_db_connector-0.2.1/PKG-INFO
```

### Comparing `easyfatt_db_connector-0.2.0/LICENSE` & `easyfatt_db_connector-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.0/pyproject.toml` & `easyfatt_db_connector-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyfatt-db-connector"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Luca Salvarani <lucasalvarani99@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "easyfatt_db_connector", from = "./src/"}]
 
 [tool.poetry.dependencies]
```

### Comparing `easyfatt_db_connector-0.2.0/README.md` & `easyfatt_db_connector-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/_base.py` & `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,17 +133,17 @@
         except (fdb.DatabaseError, UnicodeDecodeError) as e:
             error_message = str(e)
             try:
                 sqlcode = e.args[1]
             except:
                 sqlcode = None
             
-            print(f"SQLCODE: {sqlcode} (error: {error_message})")
-            
-            if "codec can't decode byte" in error_message or "lock manager" in error_message:
+            if "codec can't decode byte" in error_message or "lock manager error" in error_message:
                 return True
             elif sqlcode == -902: # File used by another process (Error while connecting to database:\n- SQLCODE: -902\n- I/O error during "CreateFile (open)" operation for file "C:\\USERS\\{...}.EFT"\n- Error while trying to open file)
                 return True
             else:
                 raise
+        except Exception as e:
+            raise
         else:
             return False
```

### Comparing `easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/_fdb.py` & `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_fdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from contextlib import contextmanager
+import os
 import shutil
+import tempfile
 from typing import Any, Generator, Literal, Optional
 from pathlib import Path
 
 import fdb
 
 from easyfatt_db_connector.core.exceptions import FirebirdClientError
 from easyfatt_db_connector.core.connection._base import EasyfattDBGeneric
@@ -31,42 +33,44 @@
 
         Yields:
             TypedFDBConnection: The connection object.
         
         Raises:
             FirebirdClientError: If the database is locked.
         """
-        if self.is_locked():
-            raise FirebirdClientError(
-                f"The database '{self.archive_path}' is locked. Close Easyfatt and try again."
-            )
+        # if self.is_locked():
+        #     raise FirebirdClientError(
+        #         f"The database '{self.archive_path}' is locked. Close Easyfatt and try again."
+        #     )
         
-        temp_database = Path(f"{self.archive_path}.tmp~")
+        handle, path = tempfile.mkstemp(prefix=f"{self.archive_path.stem}-", suffix=".eft.tmp~")
+        os.close(handle)
+
+        temp_database = Path(path)
         shutil.copy(self.archive_path, temp_database)
 
         connection = None
         try:
             connection: TypedFDBConnection = fdb.connect(
-                database=str(self.archive_path),
+                database=str(temp_database),
                 user=self.db_username,
                 password=self.db_password if self.db_password else None,
                 charset=self.db_charset,
                 fb_library_name=str(self.firebird_path / "fbembed.dll"),
             )
             yield connection
-        
+
         except Exception:
             raise
 
         finally:
             if connection is not None:
                 connection.close()
 
-            if temp_database is not None:
-                temp_database.unlink(missing_ok=True)
+            temp_database.unlink(missing_ok=True)
 
 
 
 if __name__ == "__main__":
     database_path = Path("~/Documents/Danea Easyfatt/TestArchivio.eft").expanduser()
 
     db = EasyfattFDB(database_path)
```

### Comparing `easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/core/connection/_sqlalchemy.py` & `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/core/connection/_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/dynamic/factory.py` & `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/dynamic/factory.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/orm/static/models.py` & `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/orm/static/models.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.0/src/easyfatt_db_connector/utils/downloader.py` & `easyfatt_db_connector-0.2.1/src/easyfatt_db_connector/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.2.0/PKG-INFO` & `easyfatt_db_connector-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfatt-db-connector
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: MIT
 Author: Luca Salvarani
 Author-email: lucasalvarani99@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

