# Comparing `tmp/memphis-py-beta-1.0.5.tar.gz` & `tmp/memphis-py-beta-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/memphis-py-beta-1.0.5.tar", last modified: Thu Jun  1 07:02:56 2023, max compression
+gzip compressed data, was "dist/memphis-py-beta-1.0.6.tar", last modified: Tue Jun 27 07:00:11 2023, max compression
```

## Comparing `memphis-py-beta-1.0.5.tar` & `memphis-py-beta-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16488 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12575 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/memphis/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8079 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/consumer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/exceptions.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/headers.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    32675 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/memphis.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/message.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    14111 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/producer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/station.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/types.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16488 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/memphis_py_beta.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-06-01 07:02:56.000000 memphis-py-beta-1.0.5/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-06-01 07:02:55.000000 memphis-py-beta-1.0.5/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16856 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12847 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8079 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/consumer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/exceptions.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/headers.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    34977 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/memphis.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/message.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13568 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/producer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/station.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/types.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16856 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/setup.py
```

### Comparing `memphis-py-beta-1.0.5/PKG-INFO` & `memphis-py-beta-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 1.0.5
+Version: 1.0.6
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.5.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.6.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
@@ -179,15 +179,27 @@
         
         Destroying a station will remove all its resources (producers/consumers)
         
         ```python
         station.destroy()
         ```
         
-        ### Attaching a Schema to an Existing Station
+        ### Creating a New Schema 
+        
+        ```python
+        await memphis.create_schema("<schema-name>", "<schema-type>", "<schema-file-path>")
+        ```
+        
+        ### Enforcing a Schema on an Existing Station
+        
+        ```python
+        await memphis.enforce_schema("<schema-name>", "<station-name>")
+        ```
+        
+        ### Deprecated  - Attaching a Schema, use enforce_schema instead
         
         ```python
         await memphis.attach_schema("<schema-name>", "<station-name>")
         ```
         
         ### Detaching a Schema from Station
```

### Comparing `memphis-py-beta-1.0.5/README.md` & `memphis-py-beta-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,27 @@
 
 Destroying a station will remove all its resources (producers/consumers)
 
 ```python
 station.destroy()
 ```
 
-### Attaching a Schema to an Existing Station
+### Creating a New Schema 
+
+```python
+await memphis.create_schema("<schema-name>", "<schema-type>", "<schema-file-path>")
+```
+
+### Enforcing a Schema on an Existing Station
+
+```python
+await memphis.enforce_schema("<schema-name>", "<station-name>")
+```
+
+### Deprecated  - Attaching a Schema, use enforce_schema instead
 
 ```python
 await memphis.attach_schema("<schema-name>", "<station-name>")
 ```
 
 ### Detaching a Schema from Station
```

### Comparing `memphis-py-beta-1.0.5/memphis/__init__.py` & `memphis-py-beta-1.0.6/memphis/__init__.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.5/memphis/consumer.py` & `memphis-py-beta-1.0.6/memphis/consumer.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.5/memphis/exceptions.py` & `memphis-py-beta-1.0.6/memphis/exceptions.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.5/memphis/headers.py` & `memphis-py-beta-1.0.6/memphis/headers.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.5/memphis/memphis.py` & `memphis-py-beta-1.0.6/memphis/memphis.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import asyncio
 import copy
 import json
 import ssl
 from typing import Iterable, Union
 import uuid
 import base64
+import re
 
 import nats as broker
 from google.protobuf import descriptor_pb2, descriptor_pool
 from google.protobuf.message_factory import MessageFactory
 from graphql import build_schema as build_graphql_schema
 from memphis.consumer import Consumer
 from memphis.exceptions import MemphisConnectError, MemphisError
@@ -88,18 +89,16 @@
             raise MemphisError(err)
 
     async def get_broker_manager_connection(self, connection_opts):
         if "user" in connection_opts:
             async def ping_error_cb(e):
                 if "authorization violation" not in (str(e)).lower():
                     print(MemphisError(str(e)))
-            
             async def error_cb(e):
                 return
-            
             ping_connection_opts = copy.deepcopy(connection_opts)
             ping_connection_opts["allow_reconnect"] = False
             ping_connection_opts["error_cb"] = ping_error_cb
 
             try:
                 conn = await broker.connect(**ping_connection_opts)
                 await conn.close()
@@ -271,15 +270,25 @@
 
         except Exception as e:
             if str(e).find("already exist") != -1:
                 return Station(self, name.lower())
             raise MemphisError(str(e)) from e
 
     async def attach_schema(self, name, station_name):
-        """Attaches a schema to an existing station.
+        """Deprecated - Use enforce_schema instead
+        Args:
+            name (str): schema name.
+            station_name (str): station name.
+        Raises:
+            Exception: _description_
+        """
+        await self.enforce_schema(name, station_name)
+
+    async def enforce_schema(self, name, station_name):
+        """Enforce a schema on an existing station.
         Args:
             name (str): schema name.
             station_name (str): station name.
         Raises:
             Exception: _description_
         """
         try:
@@ -706,14 +715,68 @@
             messages = await consumer.fetch(batch_size)
             if messages == None:
                 messages = []
             return messages
         except Exception as e:
             raise MemphisError(str(e)) from e
 
+    async def create_schema(self, schema_name, schema_type, schema_path):
+
+        """Creates a new schema.
+        Args:.
+            schema_name (str): the name of the schema.
+            schema_type (str): the type of the schema json / graphql / protobuf.
+            schema_path (str): the path for the schema file
+        """
+
+        if schema_type not in {'json', 'graphql', 'protobuf'}:
+            raise MemphisError("schema type not supported" + type)
+
+        try:
+            await self.schema_name_validation(schema_name)
+        except Exception as e:
+            raise e
+
+
+        schema_content = ""
+        with open(schema_path, "rt", encoding="utf-8") as f:
+            schema_content = f.read()
+
+        create_schema_req = {
+            "name": schema_name,
+            "type": schema_type,
+            "created_by_username": self.username,
+            "schema_content": schema_content,
+            "message_struct_name": ""
+        }
+
+        create_schema_req_bytes = json.dumps(create_schema_req, indent=2).encode("utf-8")
+
+        create_res = await self.broker_manager.request(
+            "$memphis_schema_creations", create_schema_req_bytes, timeout=5)
+
+        create_res = create_res.data.decode("utf-8")
+        create_res = json.loads(create_res)
+        if create_res["error"] != "":
+            raise MemphisError(create_res["error"])
+
+
+    async def schema_name_validation(self, schema_name):
+        if len(schema_name) == 0:
+            raise MemphisError("Schema name cannot be empty")
+
+        if len(schema_name) > 128:
+            raise MemphisError("Schema name should be under 128 characters")
+
+        if re.fullmatch(r'^[a-z0-9_.-]*$', schema_name) is None:
+            raise MemphisError("Only alphanumeric and the '_', '-', '.' characters are allowed in the schema name")
+
+        if not schema_name[0].isalnum() or not schema_name[-1].isalnum():
+            raise MemphisError("Schema name cannot start or end with a non-alphanumeric character")
+
     def is_connected(self):
         return self.broker_manager.is_connected
 
     def unset_cached_producer_station(self, station_name):
         try:
             internal_station_name = get_internal_name(station_name)
             for key in list(self.producers_map):
```

### Comparing `memphis-py-beta-1.0.5/memphis/message.py` & `memphis-py-beta-1.0.6/memphis/message.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.5/memphis/producer.py` & `memphis-py-beta-1.0.6/memphis/producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,27 +133,27 @@
                 msg = parse_graphql(message)
                 message = message.encode("utf-8")
             elif isinstance(message, graphql.language.ast.DocumentNode):
                 msg = message
                 message = str(msg.loc.source.body)
                 message = message.encode("utf-8")
             else:
-                raise MemphisError("Unsupported message type")
+                raise Exception("Unsupported message type")
             validate_res = validate_graphql(
                 schema=self.connection.graphql_schemas[self.internal_station_name],
                 document_ast=msg,
             )
             if len(validate_res) > 0:
                 raise Exception(
                     "Schema validation has failed: " + str(validate_res))
             return message
         except Exception as e:
             if "Syntax Error" in str(e):
                 e = "Invalid message format, expected GraphQL"
-            raise Exception("Schema validation has failed: " + str(e))
+            raise MemphisSchemaError("Schema validation has failed: " + str(e))
 
     async def produce(
         self,
         message,
         ack_wait_sec: int = 15,
         headers: Union[Headers, None] = None,
         async_produce: bool = False,
@@ -202,78 +202,79 @@
             else:
                 await self.connection.broker_connection.publish(
                     self.internal_station_name + ".final",
                     message,
                     timeout=ack_wait_sec,
                     headers=headers,
                 )
+        except MemphisSchemaError as e:
+            if self.connection.schema_updates_data[self.internal_station_name] != {}:
+                msg_to_send = ""
+                if hasattr(message, "SerializeToString"):
+                    msg_to_send = message.SerializeToString().decode("utf-8")
+                elif isinstance(message, bytearray):
+                    msg_to_send = str(message, "utf-8")
+                else:
+                    msg_to_send = str(message)
+
+                if self.connection.station_schemaverse_to_dls[
+                    self.internal_station_name
+                ]:
+                    unix_time = int(time.time())
+
+                    memphis_headers = {
+                        "$memphis_producedBy": self.producer_name,
+                        "$memphis_connectionId": self.connection.connection_id,
+                    }
+
+                    if headers != {} and not headers == None:
+                        headers = headers.headers
+                        headers.update(memphis_headers)
+                    else:
+                        headers = memphis_headers
+
+                    msg_to_send_encoded = msg_to_send.encode("utf-8")
+                    msg_hex = msg_to_send_encoded.hex()
+                    buf = {
+                        "station_name": self.internal_station_name,
+                        "producer": {
+                            "name": self.producer_name,
+                            "connection_id": self.connection.connection_id,
+                        },
+                        "creation_unix": unix_time,
+                        "message": {
+                            "data": msg_hex,
+                            "headers": headers,
+                        },
+                        "validation_error": str(e)
+                    }
+                    buf = json.dumps(buf).encode("utf-8")
+                    await self.connection.broker_manager.publish("$memphis_schemaverse_dls", buf)
+
+                if self.connection.cluster_configurations.get(
+                    "send_notification"
+                ):
+                    await self.connection.send_notification(
+                        "Schema validation has failed",
+                        "Station: "
+                        + self.station_name
+                        + "\nProducer: "
+                        + self.producer_name
+                        + "\nError:"
+                        + str(e),
+                        msg_to_send,
+                        schemaverse_fail_alert_type,
+                    )
+            raise e
         except Exception as e:
             if hasattr(e, "status_code") and e.status_code == "503":
                 raise MemphisError(
                     "Produce operation has failed, please check whether Station/Producer still exist"
                 )
             else:
-                if "Schema validation has failed" in str(
-                    e
-                ) or "Unsupported message type" in str(e):
-                    if self.connection.schema_updates_data[self.internal_station_name] != {}:
-                        msg_to_send = ""
-                        if hasattr(message, "SerializeToString"):
-                            msg_to_send = message.SerializeToString().decode("utf-8")
-                        elif isinstance(message, bytearray):
-                            msg_to_send = str(message, "utf-8")
-                        else:
-                            msg_to_send = str(message)
-                        if self.connection.station_schemaverse_to_dls[
-                            self.internal_station_name
-                        ]:
-                            unix_time = int(time.time())
-
-                            memphis_headers = {
-                                "$memphis_producedBy": self.producer_name,
-                                "$memphis_connectionId": self.connection.connection_id,
-                            }
-
-                            if headers != {} and not headers == None:
-                                headers = headers.headers
-                                headers.update(memphis_headers)
-                            else:
-                                headers = memphis_headers
-
-                            msg_to_send_encoded = msg_to_send.encode("utf-8")
-                            msg_hex = msg_to_send_encoded.hex()
-                            buf = {
-                                "station_name": self.internal_station_name,
-                                "producer": {
-                                    "name": self.producer_name,
-                                    "connection_id": self.connection.connection_id,
-                                },
-                                "creation_unix": unix_time,
-                                "message": {
-                                    "data": msg_hex,
-                                    "headers": headers,
-                                },
-                                "validation_error": str(e)
-                            }
-                            buf = json.dumps(buf).encode("utf-8")
-                            await self.connection.broker_manager.publish("$memphis_schemaverse_dls", buf)
-                            if self.connection.cluster_configurations.get(
-                                "send_notification"
-                            ):
-                                await self.connection.send_notification(
-                                    "Schema validation has failed",
-                                    "Station: "
-                                    + self.station_name
-                                    + "\nProducer: "
-                                    + self.producer_name
-                                    + "\nError:"
-                                    + str(e),
-                                    msg_to_send,
-                                    schemaverse_fail_alert_type,
-                                )
                 raise MemphisError(str(e)) from e
 
     async def destroy(self):
         """Destroy the producer."""
         try:
             destroy_producer_req = {
                 "name": self.producer_name,
```

### Comparing `memphis-py-beta-1.0.5/memphis/station.py` & `memphis-py-beta-1.0.6/memphis/station.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.5/memphis/types.py` & `memphis-py-beta-1.0.6/memphis/types.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.5/memphis/utils.py` & `memphis-py-beta-1.0.6/memphis/utils.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.5/memphis_py_beta.egg-info/PKG-INFO` & `memphis-py-beta-1.0.6/memphis_py_beta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 1.0.5
+Version: 1.0.6
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.5.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.6.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
@@ -179,15 +179,27 @@
         
         Destroying a station will remove all its resources (producers/consumers)
         
         ```python
         station.destroy()
         ```
         
-        ### Attaching a Schema to an Existing Station
+        ### Creating a New Schema 
+        
+        ```python
+        await memphis.create_schema("<schema-name>", "<schema-type>", "<schema-file-path>")
+        ```
+        
+        ### Enforcing a Schema on an Existing Station
+        
+        ```python
+        await memphis.enforce_schema("<schema-name>", "<station-name>")
+        ```
+        
+        ### Deprecated  - Attaching a Schema, use enforce_schema instead
         
         ```python
         await memphis.attach_schema("<schema-name>", "<station-name>")
         ```
         
         ### Detaching a Schema from Station
```

### Comparing `memphis-py-beta-1.0.5/setup.py` & `memphis-py-beta-1.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="memphis-py-beta",
     packages=["memphis"],
-    version="1.0.5",
+    version="1.0.6",
     license="Apache-2.0",
     description="A powerful messaging platform for modern developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author="Memphis.dev",
     author_email="team@memphis.dev",
     url="https://github.com/memphisdev/memphis.py",
-    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.5.tar.gz",
+    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.6.tar.gz",
     keywords=["message broker", "devtool", "streaming", "data"],
     install_requires=["asyncio", "nats-py", "protobuf", "jsonschema", "graphql-core"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "License :: OSI Approved :: GNU General Public License (GPL)",
```

