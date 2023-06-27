# Comparing `tmp/pysquril-0.3.2.tar.gz` & `tmp/pysquril-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysquril-0.3.2.tar", max compression
+gzip compressed data, was "pysquril-0.3.3.tar", max compression
```

## Comparing `pysquril-0.3.2.tar` & `pysquril-0.3.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      524 2023-06-26 18:24:52.115152 pysquril-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-22 08:13:57.003868 pysquril-0.3.2/pysquril/__init__.py
--rw-r--r--   0        0        0    24893 2023-06-26 18:22:24.453542 pysquril-0.3.2/pysquril/backends.py
--rw-r--r--   0        0        0      136 2023-06-22 13:54:05.278837 pysquril-0.3.2/pysquril/exc.py
--rw-r--r--   0        0        0    21254 2023-06-20 11:11:42.555715 pysquril-0.3.2/pysquril/generator.py
--rw-r--r--   0        0        0     9452 2023-01-27 11:51:39.899603 pysquril-0.3.2/pysquril/parser.py
--rw-r--r--   0        0        0     1997 2022-11-21 13:00:47.589558 pysquril-0.3.2/pysquril/test_data.py
--rw-r--r--   0        0        0    20929 2023-06-26 18:23:11.351482 pysquril-0.3.2/pysquril/tests.py
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 pysquril-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      524 2023-06-27 12:19:07.707260 pysquril-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-22 08:13:57.003868 pysquril-0.3.3/pysquril/__init__.py
+-rw-r--r--   0        0        0    25249 2023-06-27 13:10:47.568080 pysquril-0.3.3/pysquril/backends.py
+-rw-r--r--   0        0        0      326 2023-06-27 12:18:06.880308 pysquril-0.3.3/pysquril/exc.py
+-rw-r--r--   0        0        0    21254 2023-06-20 11:11:42.555715 pysquril-0.3.3/pysquril/generator.py
+-rw-r--r--   0        0        0     9452 2023-01-27 11:51:39.899603 pysquril-0.3.3/pysquril/parser.py
+-rw-r--r--   0        0        0     1997 2022-11-21 13:00:47.589558 pysquril-0.3.3/pysquril/test_data.py
+-rw-r--r--   0        0        0    21429 2023-06-27 13:10:47.569189 pysquril-0.3.3/pysquril/tests.py
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 pysquril-0.3.3/PKG-INFO
```

### Comparing `pysquril-0.3.2/pyproject.toml` & `pysquril-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysquril"
-version = "0.3.2"
+version = "0.3.3"
 description = "Python implementation of structured URI query language"
 repository = "https://github.com/unioslo/pysquril"
 authors = [
     "Leon du Toit <l.c.d.toit@usit.uio.no>",
     "Eirik Haatveit <haatveit@uio.no>",
 ]
```

### Comparing `pysquril-0.3.2/pysquril/backends.py` & `pysquril-0.3.3/pysquril/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,24 @@
         """
         out = {}
         for k, v in target_entry.items():
             if current_entry.get(k) != v:
                 out[k] = v
         return out
 
+    def _get_pk_value(self, primary_key: str, entry: dict) -> Any:
+        keys = primary_key.split(".")
+        if len(keys) == 1:
+            return entry.get(primary_key)
+        else:
+            for key in keys:
+                nested_result = entry.get(key)
+                entry = nested_result
+            return nested_result
+
     def table_restore(self, table_name: str, uri_query: str) -> dict:
         """
         Restore rows to previous states, as recorded in the audit log.
 
         This can be either: undoing a delete, or updating a current
         record to a state prior to a specific update. The desired
         state is specified by means of a URI query. If the query
@@ -213,14 +223,15 @@
 
         When deleted rows are restored the event is recorded in the
         audit log as "restore" events. Such events are ignored by
         this function: that is, restore events are not restored,
         only updates and deletes.
 
         """
+        work_done = {"restores": [], "updates": []}
         # ensure we have enough information
         query_parts = uri_query.split("&")
         if not query_parts:
             raise ParseError("Missing query")
         if "restore" not in query_parts:
             raise ParseError("Missing restore directive")
         for part in query_parts:
@@ -245,29 +256,28 @@
             current_pks = []
         # fetch the desired state
         if "order" in query_parts:
             uri_query = uri_query.split("&order")[0]
         uri_query = f"{uri_query}&order=timestamp.asc" # sorted from old to new
         target_data = list(self.table_select(f"{table_name}_audit", uri_query))
         if not target_data:
-            return False # nothing to do
+            return work_done # nothing to do
         tsc = AuditTransaction(self.requestor)
         session_func = self._session_func()
         try:
             # ensure the table exists, may have been deleted
             with session_func(self.engine) as session:
                 self.table_create(table_name, session)
         except psycopg2.errors.DuplicateObject as e:
             pass # already exists
         handled = []
-        work_done = {"restores": [], "updates": []}
         with session_func(self.engine) as session:
             for entry in target_data:
                 target_entry = entry.get("previous")
-                pk_value = target_entry.get(primary_key) if target_entry else None
+                pk_value = self._get_pk_value(primary_key, target_entry) if target_entry else None
                 if pk_value in handled or entry.get("event") == "restore":
                     continue
                 target_entry = entry.get("previous")
                 pk_value = target_entry.get(primary_key)
                 result = list(
                     self.table_select(
                         table_name,
```

### Comparing `pysquril-0.3.2/pysquril/generator.py` & `pysquril-0.3.3/pysquril/generator.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.3.2/pysquril/parser.py` & `pysquril-0.3.3/pysquril/parser.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.3.2/pysquril/test_data.py` & `pysquril-0.3.3/pysquril/test_data.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.3.2/pysquril/tests.py` & `pysquril-0.3.3/pysquril/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -488,20 +488,28 @@
         # try to retrieve deleted table's audit table
         select = self.backend.table_select(table_name=f"{test_table}_audit", uri_query="")
         with self.assertRaises((sqlite3.OperationalError, psycopg2.errors.UndefinedTable)):
             next(select)
 
         # test deleting an entire table, without any updates
         # automatic audit table creation on delete
-        some_data = {"id": 0, "lol": None, "cat": [1, 2]}
+        # use a nested primary key, to test restores with such keys
+        some_data = {"pk": {"id": 0}, "lol": None, "cat": [1, 2]}
+        some_more_data = {"pk": {"id": 1}, "neither-lol-not-not-lol": None, "cat": []}
         some_table = "yay"
         self.backend.table_insert(table_name=some_table, data=some_data)
+        self.backend.table_insert(table_name=some_table, data=some_more_data)
         self.backend.table_delete(table_name=some_table, uri_query="")
         audit = list(self.backend.table_select(table_name=f"{some_table}_audit", uri_query=""))
-        self.assertEqual(audit[0].get("previous"), some_data)
+        self.assertTrue(len(audit), 2)
+        nested_result = self.backend.table_restore(
+            table_name=some_table, uri_query=f"restore&primary_key=pk.id"
+        )
+        self.assertEqual(len(nested_result.get("restores")), 2)
+        self.backend.table_delete(table_name=f"{some_table}_audit", uri_query="")
 
 
 class TestSqliteBackend(TestSqlBackend):
     __test__ = True
 
     def setUp(self) -> None:
         self.directory = tempfile.gettempdir()
```

### Comparing `pysquril-0.3.2/PKG-INFO` & `pysquril-0.3.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysquril
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python implementation of structured URI query language
 Home-page: https://github.com/unioslo/pysquril
 Author: Leon du Toit
 Author-email: l.c.d.toit@usit.uio.no
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

