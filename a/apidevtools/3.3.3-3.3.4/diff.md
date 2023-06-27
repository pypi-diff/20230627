# Comparing `tmp/apidevtools-3.3.3.tar.gz` & `tmp/apidevtools-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.3.3.tar", last modified: Fri May 26 17:49:22 2023, max compression
+gzip compressed data, was "apidevtools-3.3.4.tar", last modified: Tue Jun 27 19:31:58 2023, max compression
```

## Comparing `apidevtools-3.3.3.tar` & `apidevtools-3.3.4.tar`

### file list

```diff
@@ -1,41 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.394604 apidevtools-3.3.3/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3546 2023-05-26 17:49:22.393603 apidevtools-3.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-3.3.3/README.md
--rw-rw-rw-   0        0        0     2155 2023-05-26 17:11:55.000000 apidevtools-3.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 17:49:22.394604 apidevtools-3.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.188561 apidevtools-3.3.3/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.3.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.203674 apidevtools-3.3.3/src/apidevtools/
--rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-3.3.3/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0     1179 2023-05-13 20:33:43.000000 apidevtools-3.3.3/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.237056 apidevtools-3.3.3/src/apidevtools/media/
--rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.3.3/src/apidevtools/media/ARIALNB.TTF
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.3.3/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-3.3.3/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-3.3.3/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.244055 apidevtools-3.3.3/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.3.3/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0     1986 2023-05-26 17:48:06.000000 apidevtools-3.3.3/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.3.3/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.265182 apidevtools-3.3.3/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.344648 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4797 2023-05-12 15:05:27.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4450 2023-05-12 15:05:27.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3396 2023-05-12 15:06:13.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6748 2023-05-12 15:03:15.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.389079 apidevtools-3.3.3/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/types/schema.py
--rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.3.3/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.221907 apidevtools-3.3.3/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3546 2023-05-26 17:49:22.000000 apidevtools-3.3.3/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-05-26 17:49:22.000000 apidevtools-3.3.3/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 17:49:22.000000 apidevtools-3.3.3/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      245 2023-05-26 17:49:22.000000 apidevtools-3.3.3/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-26 17:49:22.000000 apidevtools-3.3.3/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.749070 apidevtools-3.3.4/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3546 2023-06-27 19:31:58.748070 apidevtools-3.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-3.3.4/README.md
+-rw-rw-rw-   0        0        0     2155 2023-06-27 19:31:42.000000 apidevtools-3.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 19:31:58.749070 apidevtools-3.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.555249 apidevtools-3.3.4/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.3.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.568247 apidevtools-3.3.4/src/apidevtools/
+-rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-3.3.4/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      731 2023-06-20 21:52:55.000000 apidevtools-3.3.4/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.600043 apidevtools-3.3.4/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.3.4/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.3.4/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-3.3.4/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-3.3.4/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.610091 apidevtools-3.3.4/src/apidevtools/orm/
+-rw-rw-rw-   0        0        0       47 2023-06-21 22:55:30.000000 apidevtools-3.3.4/src/apidevtools/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.643063 apidevtools-3.3.4/src/apidevtools/orm/_crud/
+-rw-rw-rw-   0        0        0      147 2023-06-21 20:51:32.000000 apidevtools-3.3.4/src/apidevtools/orm/_crud/__init__.py
+-rw-rw-rw-   0        0        0     2017 2023-06-21 23:39:38.000000 apidevtools-3.3.4/src/apidevtools/orm/_crud/_operation.py
+-rw-rw-rw-   0        0        0      204 2023-06-21 23:49:34.000000 apidevtools-3.3.4/src/apidevtools/orm/_crud/delete.py
+-rw-rw-rw-   0        0        0      661 2023-06-21 23:48:43.000000 apidevtools-3.3.4/src/apidevtools/orm/_crud/insert.py
+-rw-rw-rw-   0        0        0      357 2023-06-21 23:48:43.000000 apidevtools-3.3.4/src/apidevtools/orm/_crud/select.py
+-rw-rw-rw-   0        0        0      443 2023-06-21 23:49:34.000000 apidevtools-3.3.4/src/apidevtools/orm/_crud/update.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.674070 apidevtools-3.3.4/src/apidevtools/orm/connector/
+-rw-rw-rw-   0        0        0      305 2023-06-21 22:55:53.000000 apidevtools-3.3.4/src/apidevtools/orm/connector/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-06-21 23:45:31.000000 apidevtools-3.3.4/src/apidevtools/orm/connector/_connector.py
+-rw-rw-rw-   0        0        0     2858 2023-06-21 23:32:33.000000 apidevtools-3.3.4/src/apidevtools/orm/connector/mysql.py
+-rw-rw-rw-   0        0        0     2387 2023-06-21 23:32:33.000000 apidevtools-3.3.4/src/apidevtools/orm/connector/postgresql.py
+-rw-rw-rw-   0        0        0     2187 2023-06-21 23:32:33.000000 apidevtools-3.3.4/src/apidevtools/orm/connector/sqlite.py
+-rw-rw-rw-   0        0        0     1374 2023-06-21 23:55:13.000000 apidevtools-3.3.4/src/apidevtools/orm/orm.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.688070 apidevtools-3.3.4/src/apidevtools/orm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.3.4/src/apidevtools/orm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.3.4/src/apidevtools/orm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.3.4/src/apidevtools/orm/types/schema.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.697071 apidevtools-3.3.4/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.3.4/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-3.3.4/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.3.4/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.711104 apidevtools-3.3.4/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.742070 apidevtools-3.3.4/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4797 2023-05-12 15:05:27.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4450 2023-05-12 15:05:27.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3400 2023-06-19 22:41:58.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.747070 apidevtools-3.3.4/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.3.4/src/apidevtools/simpleorm/types/schema.py
+-rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.3.4/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:31:58.586247 apidevtools-3.3.4/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3546 2023-06-27 19:31:58.000000 apidevtools-3.3.4/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-06-27 19:31:58.000000 apidevtools-3.3.4/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 19:31:58.000000 apidevtools-3.3.4/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      245 2023-06-27 19:31:58.000000 apidevtools-3.3.4/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 19:31:58.000000 apidevtools-3.3.4/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.3.3/LICENSE.txt` & `apidevtools-3.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/PKG-INFO` & `apidevtools-3.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.3.3
+Version: 3.3.4
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.3.3/README.md` & `apidevtools-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/pyproject.toml` & `apidevtools-3.3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.3.3"
+version = "3.3.4"
 authors = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 maintainers = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 description = "All in one tools for API development."
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `apidevtools-3.3.3/src/apidevtools/media/ARIALNB.TTF` & `apidevtools-3.3.4/src/apidevtools/media/ARIALNB.TTF`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/src/apidevtools/media/imgproc.py` & `apidevtools-3.3.4/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/src/apidevtools/media/telegraph.py` & `apidevtools-3.3.4/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/src/apidevtools/security/encryptor.py` & `apidevtools-3.3.4/src/apidevtools/security/encryptor.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 # add base64 ?
 # review types of `material`, `masterkey`, `authdata`, `raw`
 
 def keygen(material: Any = None) -> bytes:
     if not material:
         return _token_bytes(32)
+    # generates very weak password-based key, because of `salt` & `iterations`
     kdf = _PBKDF2HMAC(_SHA256(), 32, b'', 1, _default_backend())
     return kdf.derive(str(material).encode())
 
 
 def encrypt(
         raw: Any,
         key: bytes = keygen(),
```

### Comparing `apidevtools-3.3.3/src/apidevtools/security/hasher.py` & `apidevtools-3.3.4/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.3.4/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from abc import abstractmethod
 from typing import Any, MutableMapping
 
 from ..types import Relation
 
 
 class Connector:
-    def __init__(self, placeholder: str | None = '%s', constraint_wrapper: str | None = '', value_wrapper: str | None = "'"):
-        self.placeholder: str | None = placeholder
-        self.constraint_wrapper: str | None = constraint_wrapper
-        self.value_wrapper: str | None = value_wrapper
+    def __init__(self, placeholder: str = '%s', constraint_wrapper: str = '', value_wrapper: str = '\''):
+        self.placeholder: str = placeholder
+        self.constraint_wrapper: str = constraint_wrapper
+        self.value_wrapper: str = value_wrapper
 
     @abstractmethod
     async def create_pool(self) -> bool:
         ...
 
     @abstractmethod
     async def close_pool(self) -> bool:
@@ -53,15 +53,15 @@
     async def _constructor__insert_instance(
             self,
             instance: dict, tablename: str
     ) -> tuple[str, tuple[Any, ...]]:
         p, c, v = self.placeholder, self.constraint_wrapper, self.value_wrapper
 
         placeholders = ', '.join([p for _ in range(len(instance.keys()))])
-        columns, values = str(tuple(instance.keys())).replace("'", v), tuple(instance.values())
+        columns, values = str(tuple(instance.keys())).replace('\'', v), tuple(instance.values())
         return f'INSERT INTO {c}{tablename}{c} {columns} VALUES ({placeholders}) RETURNING *;', values
 
     @abstractmethod
     async def _constructor__update_instances(
             self,
             instance: dict, tablename: str, where: dict[str, Any]
     ) -> tuple[str, tuple[Any, ...]]:
```

### Comparing `apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.3.4/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.3.4/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.3.4/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from ._connector import Connector
 from ...logman import LoggerManager, Logger
 
 
 class SQLite(Connector):
     __memory = ':memory:'
 
-    def __init__(self, database: str = __memory,
+    def __init__(self, database: str = ':memory:',
                  logger: Logger = LoggerManager.logger()):
         self.database: str = database if database.endswith(('.sqlite', '.db')) or database == self.__memory else f'{database}.sqlite'
 
         self.logger: Logger = logger
         self.pool: _aiosqlite.Connection | None = None
 
-        super().__init__(placeholder='?', constraint_wrapper='"', value_wrapper="'")
+        super().__init__(placeholder='?', constraint_wrapper="\"", value_wrapper='\'')
 
     async def create_pool(self) -> bool:
         try:
             self.pool = await _aiosqlite.connect(database=self.database)
             return True
         except Exception as error:
             self.logger.error(error)
```

### Comparing `apidevtools-3.3.3/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.3.4/src/apidevtools/simpleorm/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Any
 import inspect as _inspect
 
 from ..utils import INF, is_dict as _is_dict
 from .types import RecordType, Record, Schema, Records, Relation, Instance
 from .connectors._connector import Connector
-from ..logman import LoggerManager, Logger
+from .. import logman
 
 
 class ORM:
-    def __init__(self, connector: Connector, logger: Logger = LoggerManager.logger()):
+    def __init__(self, connector: Connector, logger: logman.Logger = logman.logger):
         self.connector: Connector = connector
-        self.logger: Logger = logger
+        self.logger: logman.Logger = logger
 
     async def create_pool(self) -> bool:
         try:
             is_created = await self.connector.create_pool()
             self.logger.info(f'`ORM.connector: {self.connector.__class__.__name__}` pool created')
             return is_created
         except Exception as error:
```

### Comparing `apidevtools-3.3.3/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.3.4/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.3.4/src/apidevtools/orm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.3.4/src/apidevtools/orm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/src/apidevtools/utils.py` & `apidevtools-3.3.4/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.3/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.3.4/src/apidevtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.3.3
+Version: 3.3.4
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.3.3/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-3.3.4/src/apidevtools.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,30 @@
 src/apidevtools.egg-info/dependency_links.txt
 src/apidevtools.egg-info/requires.txt
 src/apidevtools.egg-info/top_level.txt
 src/apidevtools/media/ARIALNB.TTF
 src/apidevtools/media/__init__.py
 src/apidevtools/media/imgproc.py
 src/apidevtools/media/telegraph.py
+src/apidevtools/orm/__init__.py
+src/apidevtools/orm/orm.py
+src/apidevtools/orm/_crud/__init__.py
+src/apidevtools/orm/_crud/_operation.py
+src/apidevtools/orm/_crud/delete.py
+src/apidevtools/orm/_crud/insert.py
+src/apidevtools/orm/_crud/select.py
+src/apidevtools/orm/_crud/update.py
+src/apidevtools/orm/connector/__init__.py
+src/apidevtools/orm/connector/_connector.py
+src/apidevtools/orm/connector/mysql.py
+src/apidevtools/orm/connector/postgresql.py
+src/apidevtools/orm/connector/sqlite.py
+src/apidevtools/orm/types/__init__.py
+src/apidevtools/orm/types/records.py
+src/apidevtools/orm/types/schema.py
 src/apidevtools/security/__init__.py
 src/apidevtools/security/encryptor.py
 src/apidevtools/security/hasher.py
 src/apidevtools/simpleorm/__init__.py
 src/apidevtools/simpleorm/orm.py
 src/apidevtools/simpleorm/redis.py
 src/apidevtools/simpleorm/connectors/__init__.py
```

