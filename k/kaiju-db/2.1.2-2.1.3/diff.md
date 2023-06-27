# Comparing `tmp/kaiju_db-2.1.2-py3-none-any.whl.zip` & `tmp/kaiju_db-2.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19507 bytes, number of entries: 12
--rw-r--r--  2.0 unx      183 b- defN 23-Jun-26 16:22 kaiju_db/__init__.py
--rw-r--r--  2.0 unx     3665 b- defN 23-Jun-26 16:22 kaiju_db/functions.py
--rw-r--r--  2.0 unx    57079 b- defN 23-Jun-26 16:22 kaiju_db/services.py
--rw-r--r--  2.0 unx      453 b- defN 23-Jun-26 16:22 kaiju_db/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:22 kaiju_db/tests/__init__.py
--rw-r--r--  2.0 unx     3240 b- defN 23-Jun-26 16:22 kaiju_db/tests/fixtures.py
--rw-r--r--  2.0 unx     4125 b- defN 23-Jun-26 16:22 kaiju_db/tests/test_db.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-26 16:22 kaiju_db-2.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3090 b- defN 23-Jun-26 16:22 kaiju_db-2.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 16:22 kaiju_db-2.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-26 16:22 kaiju_db-2.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      939 b- defN 23-Jun-26 16:22 kaiju_db-2.1.2.dist-info/RECORD
-12 files, 73485 bytes uncompressed, 17935 bytes compressed:  75.6%
+Zip file size: 19605 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-27 19:17 kaiju_db/__init__.py
+-rw-r--r--  2.0 unx     3665 b- defN 23-Jun-27 19:17 kaiju_db/functions.py
+-rw-r--r--  2.0 unx    57079 b- defN 23-Jun-27 19:17 kaiju_db/services.py
+-rw-r--r--  2.0 unx      453 b- defN 23-Jun-27 19:17 kaiju_db/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 19:17 kaiju_db/tests/__init__.py
+-rw-r--r--  2.0 unx     3240 b- defN 23-Jun-27 19:17 kaiju_db/tests/fixtures.py
+-rw-r--r--  2.0 unx     4832 b- defN 23-Jun-27 19:17 kaiju_db/tests/test_db.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-27 19:18 kaiju_db-2.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3090 b- defN 23-Jun-27 19:18 kaiju_db-2.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 19:18 kaiju_db-2.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-27 19:18 kaiju_db-2.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      939 b- defN 23-Jun-27 19:18 kaiju_db-2.1.3.dist-info/RECORD
+12 files, 74192 bytes uncompressed, 18033 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_db/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_db/tests/test_db.py
 Comment: 
 
-Filename: kaiju_db-2.1.2.dist-info/LICENSE
+Filename: kaiju_db-2.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_db-2.1.2.dist-info/METADATA
+Filename: kaiju_db-2.1.3.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_db-2.1.2.dist-info/WHEEL
+Filename: kaiju_db-2.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_db-2.1.2.dist-info/top_level.txt
+Filename: kaiju_db-2.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_db-2.1.2.dist-info/RECORD
+Filename: kaiju_db-2.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_db/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .types import *
 from .functions import *
 from .services import *
 
-__version__ = '2.1.2'
+__version__ = '2.1.3'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
 __service_package__ = True
```

## kaiju_db/tests/test_db.py

```diff
@@ -6,15 +6,15 @@
 import sqlalchemy.dialects.postgresql as sa_pg
 
 from kaiju_tools.encoding import dumps
 from kaiju_tools.tests.test_data_store import TestDataStore
 
 from kaiju_db.services import SQLService, DatabaseMigrationService
 
-__all__ = ['TestDatabaseService', 'TestMigrationService']
+__all__ = ['TestDatabaseService', 'TestMigrationService', 'TestSQLService', 'TestSQLServiceCompKey']
 
 
 @pytest.mark.asyncio
 @pytest.mark.docker
 class TestDatabaseService:
     """Test postgres connector."""
 
@@ -86,28 +86,53 @@
         value = await database_service.fetchval(test_table.select().with_only_columns(test_table.c.new_column_2))
         assert value is True
 
 
 @pytest.mark.asyncio
 @pytest.mark.docker
 class TestSQLService(TestDataStore):
-    @pytest.fixture
-    def _test_table(self, _row, test_table):
-        row_id, _ = _row()
-        test_table.append_column(sa.Column('uuid', sa_pg.UUID, primary_key=isinstance(row_id, tuple)))
-        return test_table
+    """Test SQL service methods."""
 
-    @pytest_asyncio.fixture
-    async def _store(self, app, _test_table, mock_data_store, database_service):
+    table_names = ['test_table']
 
-        async with app.services:
-            await database_service.execute(f'DROP TABLE IF EXISTS {_test_table.name};')
+    async def _remove_tables(self, database_service):
+        for t in self.table_names:
+            await database_service.execute(f'DROP TABLE IF EXISTS {t};')
+
+    @pytest.fixture
+    def _service(self, app, database_service, test_table):
+
+        test_table.append_column(sa.Column('uuid', sa_pg.UUID))
 
         class TestService(SQLService):
-            table = _test_table
+            table = test_table
 
-        service = TestService(app=app)
-        app.services.add_service(service)
+        return TestService(app=app, database_service=database_service)
 
+    @pytest_asyncio.fixture
+    async def _store(self, app, database_service, _service):
+        async with app.services:
+            await self._remove_tables(database_service)
+        app.services.add_service(_service)
         async with app.services:
-            yield service
-            await database_service.execute(f'DROP TABLE {_test_table.name};')
+            yield _service
+            await self._remove_tables(database_service)
+
+
+@pytest.mark.asyncio
+@pytest.mark.docker
+class TestSQLServiceCompKey(TestSQLService):
+    """Test SQL service with composite private key methods."""
+
+    primary_key = ['id', 'uuid']
+
+    @pytest.fixture
+    def _service(self, app, database_service, test_table):
+
+        test_table.append_column(sa.Column('uuid', sa_pg.UUID, primary_key=True))
+
+        class TestService(SQLService):
+            table = test_table
+
+        test_table.c.uuid.primary_key = True
+        s = TestService(app=app, database_service=database_service)
+        return s
```

## Comparing `kaiju_db-2.1.2.dist-info/LICENSE` & `kaiju_db-2.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_db-2.1.2.dist-info/METADATA` & `kaiju_db-2.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-db
-Version: 2.1.2
+Version: 2.1.3
 Summary: Postgresql db services and tools
 Home-page: https://gitlab.com/kaiju-python/kaiju-db
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `kaiju_db-2.1.2.dist-info/RECORD` & `kaiju_db-2.1.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-kaiju_db/__init__.py,sha256=sNhwNLlRyT73ileUc9FTyOCFRUBZfCjXQ4vEV51Cv0Q,183
+kaiju_db/__init__.py,sha256=cXI3RzSr_AqA5aHqR566leXQbhxuoszRva1THlXr16U,183
 kaiju_db/functions.py,sha256=0E7H85QZkRvPBMa6H5n9eC5tJlCvKXPvKT6e5O-nuGQ,3665
 kaiju_db/services.py,sha256=C8f_KK_q14xbtgjn-CsBkSRd226ONiZf6oHQKEK7OTA,57079
 kaiju_db/types.py,sha256=0ORvc2CaCcKUNibTR5o9EI5DOFQjM_uDg5S58aF8MyU,453
 kaiju_db/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kaiju_db/tests/fixtures.py,sha256=vkf27hrIx4meIa-A3uKbmXSmjkeih6QMUBpxQ-xwljI,3240
-kaiju_db/tests/test_db.py,sha256=V7rmNkGeDIOr_Wf_e6IaSqEkfK_wRDJ2nsJdcnDUU-8,4125
-kaiju_db-2.1.2.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_db-2.1.2.dist-info/METADATA,sha256=lrlsmg6ToSDBJ9P8cID-KEP4sWpgJogmV8JPygRQkcY,3090
-kaiju_db-2.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_db-2.1.2.dist-info/top_level.txt,sha256=-jcfPgSkIz8rxFCPp_XIg5g9tVsDmBd1wdxayb_mkNU,9
-kaiju_db-2.1.2.dist-info/RECORD,,
+kaiju_db/tests/test_db.py,sha256=Ln9GLkTrZI3LEEpjhSNeM3K_KYISyVoeNmznQirqxOg,4832
+kaiju_db-2.1.3.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_db-2.1.3.dist-info/METADATA,sha256=9294v4tY8JfFuUfDl7-cxeMhG8RLA3AcZZz5ff7SwH8,3090
+kaiju_db-2.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_db-2.1.3.dist-info/top_level.txt,sha256=-jcfPgSkIz8rxFCPp_XIg5g9tVsDmBd1wdxayb_mkNU,9
+kaiju_db-2.1.3.dist-info/RECORD,,
```

