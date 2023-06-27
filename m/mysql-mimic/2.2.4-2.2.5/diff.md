# Comparing `tmp/mysql-mimic-2.2.4.tar.gz` & `tmp/mysql-mimic-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-mimic-2.2.4.tar", last modified: Fri Jun 23 21:35:51 2023, max compression
+gzip compressed data, was "mysql-mimic-2.2.5.tar", last modified: Tue Jun 27 18:47:36 2023, max compression
```

## Comparing `mysql-mimic-2.2.4.tar` & `mysql-mimic-2.2.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/mysql_mimic/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/charset.py
--rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/intercept.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/prepared.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/mysql_mimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-23 21:35:51.000000 mysql-mimic-2.2.4/mysql_mimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-23 21:35:51.000000 mysql-mimic-2.2.4/mysql_mimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:35:51.000000 mysql-mimic-2.2.4/mysql_mimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 21:35:51.000000 mysql-mimic-2.2.4/mysql_mimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 21:35:51.000000 mysql-mimic-2.2.4/mysql_mimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28243 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:47:36.082422 mysql-mimic-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-27 18:47:36.078422 mysql-mimic-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:47:36.078422 mysql-mimic-2.2.5/mysql_mimic/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/charset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/mysql_mimic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:47:36.078422 mysql-mimic-2.2.5/mysql_mimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-27 18:47:36.000000 mysql-mimic-2.2.5/mysql_mimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-27 18:47:36.000000 mysql-mimic-2.2.5/mysql_mimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:47:36.000000 mysql-mimic-2.2.5/mysql_mimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 18:47:36.000000 mysql-mimic-2.2.5/mysql_mimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 18:47:36.000000 mysql-mimic-2.2.5/mysql_mimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:47:36.082422 mysql-mimic-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:47:36.078422 mysql-mimic-2.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28686 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-27 18:46:53.000000 mysql-mimic-2.2.5/tests/test_version.py
```

### Comparing `mysql-mimic-2.2.4/LICENSE` & `mysql-mimic-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/PKG-INFO` & `mysql-mimic-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.4
+Version: 2.2.5
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.4/README.md` & `mysql-mimic-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/auth.py` & `mysql-mimic-2.2.5/mysql_mimic/auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/charset.py` & `mysql-mimic-2.2.5/mysql_mimic/charset.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/connection.py` & `mysql-mimic-2.2.5/mysql_mimic/connection.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/constants.py` & `mysql-mimic-2.2.5/mysql_mimic/constants.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/errors.py` & `mysql-mimic-2.2.5/mysql_mimic/errors.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/intercept.py` & `mysql-mimic-2.2.5/mysql_mimic/intercept.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/packets.py` & `mysql-mimic-2.2.5/mysql_mimic/packets.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/results.py` & `mysql-mimic-2.2.5/mysql_mimic/results.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/schema.py` & `mysql-mimic-2.2.5/mysql_mimic/schema.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/server.py` & `mysql-mimic-2.2.5/mysql_mimic/server.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/session.py` & `mysql-mimic-2.2.5/mysql_mimic/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
+from datetime import datetime, timezone as timezone_
 from typing import (
     Dict,
     List,
     TYPE_CHECKING,
     Optional,
     Callable,
     Awaitable,
@@ -30,15 +31,21 @@
     show_statement_to_info_schema_query,
     like_to_regex,
     BaseInfoSchema,
     ensure_info_schema,
 )
 from mysql_mimic.constants import INFO_SCHEMA
 from mysql_mimic.utils import find_dbs
-from mysql_mimic.variables import Variables, SessionVariables, GlobalVariables, DEFAULT
+from mysql_mimic.variables import (
+    Variables,
+    SessionVariables,
+    GlobalVariables,
+    DEFAULT,
+    parse_timezone,
+)
 from mysql_mimic.results import AllowedResult
 
 if TYPE_CHECKING:
     from mysql_mimic.connection import Connection
 
     Interceptor = Callable[[exp.Expression], Awaitable[AllowedResult]]
 
@@ -127,28 +134,50 @@
         ]
 
         # Information functions.
         # These will be replaced in the AST with their corresponding values.
         self._functions = {
             "CONNECTION_ID": lambda: self.connection.connection_id,
             "USER": lambda: self.variables.get("external_user"),
-            "SYSTEM_USER": lambda: self.variables.get("external_user"),
-            "SESSION_USER": lambda: self.variables.get("external_user"),
             "CURRENT_USER": lambda: self.username,
             "VERSION": lambda: self.variables.get("version"),
             "DATABASE": lambda: self.database,
-            "SCHEMA": lambda: self.database,
+            "NOW": lambda: self.timestamp.strftime("%Y-%m-%d %H:%M:%S"),
+            "CURDATE": lambda: self.timestamp.strftime("%Y-%m-%d"),
+            "CURTIME": lambda: self.timestamp.strftime("%H:%M:%S"),
+        }
+        # Synonyms
+        self._functions.update(
+            {
+                "SYSTEM_USER": self._functions["USER"],
+                "SESSION_USER": self._functions["USER"],
+                "SCHEMA": self._functions["DATABASE"],
+                "CURRENT_TIMESTAMP": self._functions["NOW"],
+                "LOCALTIME": self._functions["NOW"],
+                "LOCALTIMESTAMP": self._functions["NOW"],
+                "CURRENT_DATE": self._functions["CURDATE"],
+                "CURRENT_TIME": self._functions["CURTIME"],
+            }
+        )
+        self._constants = {
+            "CURRENT_USER",
+            "CURRENT_TIME",
+            "CURRENT_TIMESTAMP",
+            "CURRENT_DATE",
         }
 
         # Current database
         self.database = None
 
         # Current authenticated user
         self.username = None
 
+        # Time when query started
+        self.timestamp: datetime = datetime.now()
+
         self._connection: Optional[Connection] = None
 
     async def query(
         self, expression: exp.Expression, sql: str, attrs: Dict[str, str]
     ) -> AllowedResult:
         """
         Process a SQL query.
@@ -203,14 +232,15 @@
     async def close(self) -> None:
         """
         Called when the client closes the connection.
         """
         self._connection = None
 
     async def handle_query(self, sql: str, attrs: Dict[str, str]) -> AllowedResult:
+        self.timestamp = datetime.now(tz=self.timezone())
         result = None
         for expression in self._parse(sql):
             if not expression:
                 continue
             with self._set_var_hint(expression):
                 result = await self._intercept(expression, sql, attrs)
                 if result is None:
@@ -311,16 +341,16 @@
                     func_name = node.name.upper()
                 else:
                     func_name = node.sql_name()
                 func = self._functions.get(func_name)
                 if func:
                     value = func()
                     new_node = value_to_expression(value)
-            elif isinstance(node, exp.Column) and node.sql() == "CURRENT_USER":
-                value = self._functions["CURRENT_USER"]()
+            elif isinstance(node, exp.Column) and node.sql() in self._constants:
+                value = self._functions[node.sql()]()
                 new_node = value_to_expression(value)
             elif isinstance(node, exp.SessionParameter):
                 value = self.variables.get(node.name)
                 new_node = value_to_expression(value)
 
             if (
                 new_node
@@ -470,7 +500,11 @@
         return [], ["Variable_name", "Value"]
 
     def _show_warnings(self, show: exp.Show) -> AllowedResult:
         return [], ["Level", "Code", "Message"]
 
     def _show_errors(self, show: exp.Show) -> AllowedResult:
         return [], ["Level", "Code", "Message"]
+
+    def timezone(self) -> timezone_:
+        tz = self.variables.get("time_zone")
+        return parse_timezone(tz)
```

### Comparing `mysql-mimic-2.2.4/mysql_mimic/stream.py` & `mysql-mimic-2.2.5/mysql_mimic/stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/types.py` & `mysql-mimic-2.2.5/mysql_mimic/types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/utils.py` & `mysql-mimic-2.2.5/mysql_mimic/utils.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/mysql_mimic/variables.py` & `mysql-mimic-2.2.5/mysql_mimic/variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
 
 import abc
+import re
+from datetime import timezone, timedelta
+from functools import lru_cache
 from typing import Any, Callable, Tuple
 
 from mysql_mimic.charset import CharacterSet, Collation
 from mysql_mimic.errors import MysqlError, ErrorCode
 
 
 class Default:
@@ -39,15 +42,15 @@
     "net_buffer_length": (int, 16384, True),
     "net_write_timeout": (int, 28800, True),
     "performance_schema": (bool, False, False),
     "sql_auto_is_null": (bool, False, True),
     "sql_mode": (str, "ANSI", True),
     "sql_select_limit": (int, None, True),
     "system_time_zone": (str, "UTC", False),
-    "time_zone": (str, "UTC", False),
+    "time_zone": (str, "UTC", True),
     "transaction_read_only": (bool, False, True),
     "transaction_isolation": (str, "READ-COMMITTED", True),
     "version": (str, "8.0.29", False),
     "version_comment": (str, "mysql-mimic", False),
     "wait_timeout": (int, 28800, True),
     "event_scheduler": (str, "OFF", True),
     "default_storage_engine": (str, "mysql-mimic", True),
@@ -117,7 +120,25 @@
     def __init__(self, global_variables: Variables):
         self.global_variables = global_variables
         super().__init__()
 
     @property
     def schema(self) -> dict[str, VariableSchema]:
         return self.global_variables.schema
+
+
+RE_TIMEZONE = re.compile(r"^(?P<sign>[+-])(?P<hours>\d\d):(?P<minutes>\d\d)")
+
+
+@lru_cache(maxsize=48)
+def parse_timezone(tz: str) -> timezone:
+    if tz.lower() == "utc":
+        return timezone.utc
+    match = RE_TIMEZONE.match(tz)
+    if not match:
+        raise MysqlError(msg=f"Invalid timezone: {tz}")
+    offset = timedelta(
+        hours=int(match.group("hours")), minutes=int(match.group("minutes"))
+    )
+    if match.group("sign") == "-":
+        offset = offset * -1
+    return timezone(offset)
```

### Comparing `mysql-mimic-2.2.4/mysql_mimic.egg-info/PKG-INFO` & `mysql-mimic-2.2.5/mysql_mimic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.4
+Version: 2.2.5
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.4/mysql_mimic.egg-info/SOURCES.txt` & `mysql-mimic-2.2.5/mysql_mimic.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 mysql_mimic.egg-info/top_level.txt
 tests/test_auth.py
 tests/test_query.py
 tests/test_result.py
 tests/test_ssl.py
 tests/test_stream.py
 tests/test_types.py
+tests/test_variables.py
 tests/test_version.py
```

### Comparing `mysql-mimic-2.2.4/setup.py` & `mysql-mimic-2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     extras_require={
         "dev": [
             "aiomysql",
             "mypy",
             "mysql-connector-python",
             "black",
             "coverage",
+            "freezegun",
             "gssapi",
             "k5test",
             "pylint",
             "pytest",
             "pytest-asyncio",
             "sphinx",
             "sqlalchemy",
```

### Comparing `mysql-mimic-2.2.4/tests/test_auth.py` & `mysql-mimic-2.2.5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/tests/test_query.py` & `mysql-mimic-2.2.5/tests/test_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pytest
 import pytest_asyncio
 from mysql.connector.abstracts import MySQLConnectionAbstract
 from sqlalchemy import text
 from sqlalchemy.ext.asyncio import AsyncEngine
 import aiomysql
+from freezegun import freeze_time
 
 from mysql_mimic import ResultColumn, ResultSet, MysqlServer, context
 from mysql_mimic.charset import CharacterSet
 from mysql_mimic.results import AllowedResult
 from mysql_mimic.constants import INFO_SCHEMA
 from mysql_mimic.types import ColumnType
 from tests.conftest import PreparedDictCursor, query, MockSession, ConnectFixture
@@ -775,25 +776,38 @@
                     "table_type": "TABLE",
                     "type_cat": None,
                     "type_name": None,
                     "type_schem": None,
                 },
             ],
         ),
+        # Timestamps
+        (
+            "select now(), curtime(), curdate(), current_time",
+            [
+                {
+                    "NOW()": "2023-01-01 00:00:00",
+                    "CURTIME()": "00:00:00",
+                    "CURDATE()": "2023-01-01",
+                    "CURRENT_TIME()": "00:00:00",
+                }
+            ],
+        ),
     ],
 )
 async def test_commands(
     session: MockSession,
     server: MysqlServer,
     query_fixture: QueryFixture,
     sql: str,
     expected: List[Dict[str, Any]],
 ) -> None:
-    result = await query_fixture(sql)
-    assert expected == list(result)
+    with freeze_time("2023-01-01"):
+        result = await query_fixture(sql)
+        assert expected == list(result)
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "sql,  msg",
     [
         (
```

### Comparing `mysql-mimic-2.2.4/tests/test_ssl.py` & `mysql-mimic-2.2.5/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/tests/test_stream.py` & `mysql-mimic-2.2.5/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.4/tests/test_types.py` & `mysql-mimic-2.2.5/tests/test_types.py`

 * *Files identical despite different names*

