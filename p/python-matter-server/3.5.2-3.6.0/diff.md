# Comparing `tmp/python-matter-server-3.5.2.tar.gz` & `tmp/python-matter-server-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.5.2.tar", last modified: Fri Jun 23 14:52:34 2023, max compression
+gzip compressed data, was "python-matter-server-3.6.0.tar", last modified: Tue Jun 27 14:03:15 2023, max compression
```

## Comparing `python-matter-server-3.5.2.tar` & `python-matter-server-3.6.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.369059 python-matter-server-3.5.2/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.369059 python-matter-server-3.5.2/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.369059 python-matter-server-3.5.2/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.369059 python-matter-server-3.5.2/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.369059 python-matter-server-3.5.2/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    26821 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-23 14:52:21.000000 python-matter-server-3.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-06-23 14:52:33.000000 python-matter-server-3.5.2/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-23 14:52:34.000000 python-matter-server-3.5.2/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:52:33.000000 python-matter-server-3.5.2/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 14:52:33.000000 python-matter-server-3.5.2/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:52:31.000000 python-matter-server-3.5.2/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-23 14:52:34.000000 python-matter-server-3.5.2/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 14:52:34.000000 python-matter-server-3.5.2/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:03:15.855467 python-matter-server-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-06-27 14:03:15.855467 python-matter-server-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:03:15.855467 python-matter-server-3.6.0/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:03:15.855467 python-matter-server-3.6.0/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:03:15.855467 python-matter-server-3.6.0/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:03:15.855467 python-matter-server-3.6.0/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:03:15.855467 python-matter-server-3.6.0/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:03:15.855467 python-matter-server-3.6.0/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:03:15.855467 python-matter-server-3.6.0/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-27 14:03:04.000000 python-matter-server-3.6.0/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-27 14:03:06.000000 python-matter-server-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:03:15.855467 python-matter-server-3.6.0/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-06-27 14:03:15.000000 python-matter-server-3.6.0/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-27 14:03:15.000000 python-matter-server-3.6.0/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:03:15.000000 python-matter-server-3.6.0/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 14:03:15.000000 python-matter-server-3.6.0/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:03:13.000000 python-matter-server-3.6.0/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-27 14:03:15.000000 python-matter-server-3.6.0/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 14:03:15.000000 python-matter-server-3.6.0/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-27 14:03:15.859467 python-matter-server-3.6.0/setup.cfg
```

### Comparing `python-matter-server-3.5.2/LICENSE` & `python-matter-server-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.2/PKG-INFO` & `python-matter-server-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.5.2
+Version: 3.6.0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -59,25 +59,25 @@
 relies on the networking managed by your operating system.
 
 ### Requirements to communicate with Wi-Fi/Ethernet based Thread devices
 
 Make sure your you run the container on the host network. The host network
 interface needs to be in the same network as the Android/iPhone device
 you are using for commissioning. Matter uses link-local multicast protocols
-which do not work accross different LANs or VLANs.
+which do not work across different LANs or VLANs.
 
 The host network interface needs IPv6 support enabled.
 
 ### Requirements to communicate with Thread devices through Thread border routers
 
 For communication through Thread border routers which are not running on the same
 host as the Matter Controller server to work, IPv6 routing needs to be properly
 working. IPv6 routing is largely setup automatically through the IPv6 Neighbor
 Discovery Protocol, specifically the Route Information Options (RIO). However,
-if IPv6 ND RIO's are processed, and processed correctly depends on the network
+if IPv6 Neighbor Discovery RIO's are processed, and processed correctly depends on the network
 management software your system is using. There may be bugs and cavats in
 processing this Route Information Options.
 
 In general, make sure the kernel option `CONFIG_IPV6_ROUTER_PREF` is enabled and
 that IPv6 forwarding is disabled (sysctl variable `net.ipv6.conf.all.forwarding`).
 If IPv6 forwarding is enabled, the Linux kernel doesn't employ reachability
 probing (RFC 4191), which can lead to longer outages (up to 30min) until
```

### Comparing `python-matter-server-3.5.2/README.md` & `python-matter-server-3.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,25 +40,25 @@
 relies on the networking managed by your operating system.
 
 ### Requirements to communicate with Wi-Fi/Ethernet based Thread devices
 
 Make sure your you run the container on the host network. The host network
 interface needs to be in the same network as the Android/iPhone device
 you are using for commissioning. Matter uses link-local multicast protocols
-which do not work accross different LANs or VLANs.
+which do not work across different LANs or VLANs.
 
 The host network interface needs IPv6 support enabled.
 
 ### Requirements to communicate with Thread devices through Thread border routers
 
 For communication through Thread border routers which are not running on the same
 host as the Matter Controller server to work, IPv6 routing needs to be properly
 working. IPv6 routing is largely setup automatically through the IPv6 Neighbor
 Discovery Protocol, specifically the Route Information Options (RIO). However,
-if IPv6 ND RIO's are processed, and processed correctly depends on the network
+if IPv6 Neighbor Discovery RIO's are processed, and processed correctly depends on the network
 management software your system is using. There may be bugs and cavats in
 processing this Route Information Options.
 
 In general, make sure the kernel option `CONFIG_IPV6_ROUTER_PREF` is enabled and
 that IPv6 forwarding is disabled (sysctl variable `net.ipv6.conf.all.forwarding`).
 If IPv6 forwarding is enabled, the Linux kernel doesn't employ reachability
 probing (RFC 4191), which can lead to longer outages (up to 30min) until
```

### Comparing `python-matter-server-3.5.2/matter_server/client/client.py` & `python-matter-server-3.6.0/matter_server/client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,18 @@
     ) -> Callable[[], None]:
         """
         Subscribe to node and server events.
 
         Optionally filter by specific events or node attributes.
         Returns:
             function to unsubscribe.
+
+        NOTE: To receive attribute changed events,
+        you must also register the attributes to subscribe to
+        with the `subscribe_attributes` method.
         """
         # for fast lookups we create a key based on the filters, allowing
         # a "catch all" with a wildcard (*).
         _event_filter: str
         if event_filter is None:
             _event_filter = SUB_WILDCARD
         else:
@@ -90,19 +94,19 @@
         self._subscribers[key].append(callback)
 
         def unsubscribe() -> None:
             self._subscribers[key].remove(callback)
 
         return unsubscribe
 
-    async def get_nodes(self) -> list[MatterNode]:
+    def get_nodes(self) -> list[MatterNode]:
         """Return all Matter nodes."""
         return list(self._nodes.values())
 
-    async def get_node(self, node_id: int) -> MatterNode:
+    def get_node(self, node_id: int) -> MatterNode:
         """Return Matter node by id."""
         return self._nodes[node_id]
 
     async def commission_with_code(self, code: str) -> MatterNodeData:
         """
         Commission a device using QRCode or ManualPairingCode.
 
@@ -160,15 +164,15 @@
     async def get_matter_fabrics(self, node_id: int) -> list[MatterFabricData]:
         """
         Get Matter fabrics from a device.
 
         Returns a list of MatterFabricData objects.
         """
 
-        node = await self.get_node(node_id)
+        node = self.get_node(node_id)
         fabrics: list[
             Clusters.OperationalCredentials.Structs.FabricDescriptor
         ] = node.get_attribute_value(
             0, None, Clusters.OperationalCredentials.Attributes.Fabrics
         )
 
         vendors_map = await self.send_command(
@@ -225,14 +229,30 @@
             interaction_timeout_ms=interaction_timeout_ms,
         )
 
     async def remove_node(self, node_id: int) -> None:
         """Remove a Matter node/device from the fabric."""
         await self.send_command(APICommand.REMOVE_NODE, node_id=node_id)
 
+    async def subscribe_attribute(
+        self, node_id: int, attribute_path: str | list[str]
+    ) -> None:
+        """
+        Subscribe to given AttributePath(s).
+
+        Either supply a single attribute path or a list of paths.
+        The given attribute path(s) will be added to the list of attributes that
+        are watched for the given node. This is persistent over restarts.
+        """
+        await self.send_command(
+            APICommand.SUBSCRIBE_ATTRIBUTE,
+            node_id=node_id,
+            attribute_path=attribute_path,
+        )
+
     async def send_command(
         self,
         command: str,
         require_schema: int | None = None,
         **kwargs: Any,
     ) -> Any:
         """Send a command and get a response."""
@@ -362,15 +382,14 @@
             if isinstance(msg, ErrorResultMessage):
                 exc = ERROR_MAP[msg.error_code]
                 future.set_exception(exc(msg.details))
                 return
 
         # handle EventMessage
         if isinstance(msg, EventMessage):
-            self.logger.debug("Received event: %s", msg)
             self._handle_event_message(msg)
             return
 
         # Log anything we can't handle here
         self.logger.debug(
             "Received message with unknown type '%s': %s",
             type(msg),
@@ -383,36 +402,64 @@
             # an update event can potentially arrive for a not yet known node
             node_data = dataclass_from_dict(MatterNodeData, msg.data)
             node = self._nodes.get(node_data.node_id)
             if node is None:
                 event = EventType.NODE_ADDED
                 node = MatterNode(node_data)
                 self._nodes[node.node_id] = node
+                self.logger.debug("New node added: %s", node.node_id)
             else:
                 event = EventType.NODE_UPDATED
                 node.update(node_data)
+                self.logger.debug("Node updated: %s", node.node_id)
             self._signal_event(event, data=node, node_id=node.node_id)
             return
-        if msg.event == EventType.NODE_DELETED:
+        if msg.event == EventType.NODE_REMOVED:
             node_id = msg.data
+            self.logger.debug("Node removed: %s", node_id)
+            self._signal_event(EventType.NODE_REMOVED, data=node_id, node_id=node_id)
+            # cleanup node only after signalling subscribers
             self._nodes.pop(node_id, None)
-            self._signal_event(EventType.NODE_DELETED, data=node_id, node_id=node_id)
+            return
+        if msg.event == EventType.ENDPOINT_REMOVED:
+            node_id = msg.data["node_id"]
+            endpoint_id = msg.data["endpoint_id"]
+            self.logger.debug("Endpoint removed: %s/%s", node_id, endpoint_id)
+            self._signal_event(
+                EventType.ENDPOINT_REMOVED, data=msg.data, node_id=node_id
+            )
+            # cleanup endpoint only after signalling subscribers
+            if node := self._nodes.get(node_id):
+                node.endpoints.pop(endpoint_id, None)
             return
         if msg.event == EventType.ATTRIBUTE_UPDATED:
             # data is tuple[node_id, attribute_path, new_value]
             node_id, attribute_path, new_value = msg.data
+            if self.logger.isEnabledFor(logging.DEBUG):
+                self.logger.debug(
+                    "Attribute updated: Node: %s - Attribute: %s - New value: %s",
+                    node_id,
+                    attribute_path,
+                    new_value,
+                )
             self._nodes[node_id].update_attribute(attribute_path, new_value)
             self._signal_event(
                 EventType.ATTRIBUTE_UPDATED,
                 data=new_value,
                 node_id=node_id,
                 attribute_path=attribute_path,
             )
             return
-        # TODO: handle any other events ?
+        if msg.event == EventType.ENDPOINT_ADDED:
+            node_id = msg.data["node_id"]
+            endpoint_id = msg.data["endpoint_id"]
+            self.logger.debug("Endpoint added: %s/%s", node_id, endpoint_id)
+        # simply forward all other events as-is
+        if self.logger.isEnabledFor(logging.DEBUG):
+            self.logger.debug("Received event: %s", msg)
         self._signal_event(msg.event, msg.data)
 
     def _signal_event(
         self,
         event: EventType,
         data: Any = None,
         node_id: Optional[int] = None,
```

### Comparing `python-matter-server-3.5.2/matter_server/client/connection.py` & `python-matter-server-3.6.0/matter_server/client/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Logic to manage the WebSocket connection to the Matter server."""
 from __future__ import annotations
 
 import asyncio
 import logging
+import os
 import pprint
 from typing import Any, Callable, Dict, Final, cast
 
 from aiohttp import ClientSession, ClientWebSocketResponse, WSMsgType, client_exceptions
 
 from matter_server.common.helpers.util import dataclass_from_dict
 
@@ -29,14 +30,15 @@
     InvalidServerVersion,
     InvalidState,
     NotConnected,
 )
 from .models.node import MatterNode
 
 LOGGER = logging.getLogger(f"{__package__}.connection")
+VERBOSE_LOGGER = os.environ.get("MATTER_VERBOSE_LOGGING")
 SUB_WILDCARD: Final = "*"
 
 
 class MatterClientConnection:
     """Manage a Matter server over WebSockets."""
 
     def __init__(
@@ -124,29 +126,29 @@
         try:
             msg = parse_message(json_loads(ws_msg.data))
         except TypeError as err:
             raise InvalidMessage(f"Received unsupported JSON: {err}") from err
         except ValueError as err:
             raise InvalidMessage("Received invalid JSON.") from err
 
-        if LOGGER.isEnabledFor(logging.DEBUG):
+        if VERBOSE_LOGGER and LOGGER.isEnabledFor(logging.DEBUG):
             LOGGER.debug("Received message:\n%s\n", pprint.pformat(ws_msg))
 
         return msg
 
     async def send_message(self, message: CommandMessage) -> None:
         """
         Send a CommandMessage to the server.
 
         Raises NotConnected if client not connected.
         """
         if not self.connected:
             raise NotConnected
 
-        if LOGGER.isEnabledFor(logging.DEBUG):
+        if VERBOSE_LOGGER and LOGGER.isEnabledFor(logging.DEBUG):
             LOGGER.debug("Publishing message:\n%s\n", pprint.pformat(message))
 
         assert self._ws_client
         assert isinstance(message, CommandMessage)
 
         await self._ws_client.send_json(message, dumps=json_dumps)
```

### Comparing `python-matter-server-3.5.2/matter_server/client/exceptions.py` & `python-matter-server-3.6.0/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.2/matter_server/client/models/device_types.py` & `python-matter-server-3.6.0/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.2/matter_server/client/models/node.py` & `python-matter-server-3.6.0/matter_server/client/models/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,14 @@
 
 class MatterNode:
     """Representation of a Matter Node."""
 
     def __init__(self, node_data: MatterNodeData) -> None:
         """Initialize MatterNode from MatterNodeData."""
         self.endpoints: dict[int, MatterEndpoint] = {}
-        self._is_bridge_device: bool = False
         # composed devices reference to other endpoints through the partsList attribute
         # create a mapping table
         self._composed_endpoints: dict[int, int] = {}
         self.update(node_data)
 
     @property
     def node_id(self) -> int:
@@ -247,15 +246,15 @@
         Returns BasicInformation from the Node itself (endpoint 0).
         """
         return self.get_cluster(0, Clusters.BasicInformation)
 
     @property
     def is_bridge_device(self) -> bool:
         """Return if this Node is a Bridge/Aggregator device."""
-        return self._is_bridge_device
+        return self.node_data.is_bridge
 
     def get_attribute_value(
         self,
         endpoint: int,
         cluster: type[_CLUSTER_T] | int | None,
         attribute: int | type[_ATTRIBUTE_T],
     ) -> Any:
@@ -306,18 +305,14 @@
         for endpoint_id, attributes_data in endpoint_data.items():
             if endpoint_id in self.endpoints:
                 self.endpoints[endpoint_id].update(attributes_data)
             else:
                 self.endpoints[endpoint_id] = MatterEndpoint(
                     endpoint_id=endpoint_id, attributes_data=attributes_data, node=self
                 )
-        # lookup if this is a bridge device
-        self._is_bridge_device = any(
-            Aggregator in x.device_types for x in self.endpoints.values()
-        )
         # composed devices reference to other endpoints through the partsList attribute
         # create a mapping table to quickly map this
         for endpoint in self.endpoints.values():
             if RootNode in endpoint.device_types:
                 # ignore root endpoint
                 continue
             if Aggregator in endpoint.device_types:
@@ -335,12 +330,15 @@
             if descriptor.partsList:  # type: ignore[unreachable]
                 for endpoint_id in descriptor.partsList:
                     self._composed_endpoints[endpoint_id] = endpoint.endpoint_id
 
     def update_attribute(self, attribute_path: str, new_value: Any) -> None:
         """Handle Attribute value update."""
         endpoint_id = int(attribute_path.split("/")[0])
+        if endpoint_id not in self.endpoints:
+            # race condition when a bridge is in the process of adding a new endpoint
+            return
         self.endpoints[endpoint_id].set_attribute_value(attribute_path, new_value)
 
     def __repr__(self) -> str:
         """Return the representation."""
         return f"<MatterNode {self.node_id}>"
```

### Comparing `python-matter-server-3.5.2/matter_server/common/errors.py` & `python-matter-server-3.6.0/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.2/matter_server/common/helpers/api.py` & `python-matter-server-3.6.0/matter_server/common/helpers/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     if args is None:
         args = {}
     final_args = {}
     # ignore extra args if not strict
     if strict:
         for key, value in args.items():
             if key not in func_sig.parameters:
-                raise KeyError("Invalid parameter: '%s'" % key)
+                raise KeyError(f"Invalid parameter: '{key}'")
     # parse arguments to correct type
     for name, param in func_sig.parameters.items():
         value = args.get(name)
         if param.default is inspect.Parameter.empty:
             default = MISSING
         else:
             default = param.default
```

### Comparing `python-matter-server-3.5.2/matter_server/common/helpers/json.py` & `python-matter-server-3.6.0/matter_server/common/helpers/json.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Helpers to work with (de)serializing of json."""
 
 from base64 import b64encode
 from dataclasses import is_dataclass
 from typing import Any
 
-from chip.clusters.Attribute import ValueDecodeFailure
 from chip.clusters.Types import Nullable
 from chip.tlv import float32, uint
 import orjson
 
 from .util import dataclass_to_dict
 
 JSON_ENCODE_EXCEPTIONS = (TypeError, ValueError)
@@ -18,16 +17,14 @@
 def json_encoder_default(obj: Any) -> Any:
     """Convert Special objects.
 
     Hand other objects to the original method.
     """
     if getattr(obj, "do_not_serialize", None):
         return None
-    if isinstance(obj, ValueDecodeFailure):
-        return None
     if isinstance(obj, (set, tuple)):
         return list(obj)
     if isinstance(obj, float32):
         return float(obj)
     if isinstance(obj, uint):
         return int(obj)
     if hasattr(obj, "as_dict"):
@@ -36,15 +33,15 @@
         return dataclass_to_dict(obj)
     if isinstance(obj, Nullable):
         return None
     if isinstance(obj, bytes):
         return b64encode(obj).decode("utf-8")
     if isinstance(obj, Exception):
         return str(obj)
-    if type(obj) == type:
+    if type(obj) == type:  # pylint: disable=unidiomatic-typecheck
         return f"{obj.__module__}.{obj.__qualname__}"
 
     raise TypeError
 
 
 def json_dumps(data: Any) -> str:
     """Dump json string."""
```

### Comparing `python-matter-server-3.5.2/matter_server/common/helpers/util.py` & `python-matter-server-3.6.0/matter_server/common/helpers/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 def parse_utc_timestamp(datetime_string: str) -> datetime:
     """Parse datetime from string."""
     return datetime.fromisoformat(datetime_string.replace("Z", "+00:00"))
 
 
 def parse_value(name: str, value: Any, value_type: Any, default: Any = MISSING) -> Any:
     """Try to parse a value from raw (json) data and type annotations."""
+    # pylint: disable=too-many-return-statements,too-many-branches
 
     if isinstance(value_type, str):
         # this shouldn't happen, but just in case
         value_type = get_type_hints(value_type, globals(), locals())
 
     if isinstance(value, dict):
         # always prefer classes that have a from_dict
@@ -101,32 +102,32 @@
         return None
     if value is None and value_type is Nullable:
         return None
     if is_dataclass(value_type) and isinstance(value, dict):
         return dataclass_from_dict(value_type, value)
     # get origin value type and inspect one-by-one
     origin: Any = get_origin(value_type)
-    if origin in (list, tuple) and isinstance(value, list | tuple):
+    if origin in (list, tuple, set) and isinstance(value, (list, tuple, set)):
         return origin(
             parse_value(name, subvalue, get_args(value_type)[0])
             for subvalue in value
             if subvalue is not None
         )
     # handle dictionary where we should inspect all values
-    elif origin is dict:
+    if origin is dict:
         subkey_type = get_args(value_type)[0]
         subvalue_type = get_args(value_type)[1]
         return {
             parse_value(subkey, subkey, subkey_type): parse_value(
                 f"{subkey}.value", subvalue, subvalue_type
             )
             for subkey, subvalue in value.items()
         }
     # handle Union type
-    elif origin is Union or origin is UnionType:
+    if origin is Union or origin is UnionType:
         # try all possible types
         sub_value_types = get_args(value_type)
         for sub_arg_type in sub_value_types:
             if value is NoneType and sub_arg_type is NoneType:
                 return value
             # try them all until one succeeds
             try:
@@ -139,28 +140,29 @@
             f"Value {value} of type {type(value)} is invalid for {name}, "
             f"expected value of type {value_type}"
         )
         if NoneType not in sub_value_types:
             # raise exception, we have no idea how to handle this value
             raise TypeError(err)
         # failed to parse the (sub) value but None allowed, log only
-        logging.getLogger(__name__).warn(err)
+        logging.getLogger(__name__).warning(err)
         return None
-    elif origin is type:
+    if origin is type:
         return get_type_hints(value, globals(), locals())
     # handle Any as value type (which is basically unprocessable)
     if value_type is Any:
         return value
     # raise if value is None and the value is required according to annotations
     if value is None and value_type is not NoneType:
         raise KeyError(f"`{name}` of type `{value_type}` is required.")
 
     try:
         if issubclass(value_type, Enum):
             # handle enums from the SDK that have a value that does not exist in the enum (sigh)
+            # pylint: disable=protected-access
             if value not in value_type._value2member_map_:
                 # we do not want to crash so we return the raw value
                 return value
             return value_type(value)
         if issubclass(value_type, datetime):
             return parse_utc_timestamp(value)
     except TypeError:
@@ -204,19 +206,18 @@
     """
     Create (instance of) a dataclass by providing a dict with values.
 
     Including support for nested structures and common type conversions.
     If strict mode enabled, any additional keys in the provided dict will result in a KeyError.
     """
     if strict:
-        extra_keys = dict_obj.keys() - set([f.name for f in fields(cls)])
+        extra_keys = dict_obj.keys() - {f.name for f in fields(cls)}
         if extra_keys:
             raise KeyError(
-                "Extra key(s) %s not allowed for %s"
-                % (",".join(extra_keys), (str(cls)))
+                f'Extra key(s) {",".join(extra_keys)} not allowed for {str(cls)}'
             )
     type_hints = get_type_hints(cls)
     return cls(
         **{
             field.name: parse_value(
                 f"{cls.__name__}.{field.name}",
                 dict_obj.get(field.name),
```

### Comparing `python-matter-server-3.5.2/matter_server/common/models.py` & `python-matter-server-3.6.0/matter_server/common/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 
 
 class EventType(Enum):
     """Enum with possible events sent from server to client."""
 
     NODE_ADDED = "node_added"
     NODE_UPDATED = "node_updated"
-    NODE_DELETED = "node_deleted"
+    NODE_REMOVED = "node_removed"
     NODE_EVENT = "node_event"
     ATTRIBUTE_UPDATED = "attribute_updated"
     SERVER_SHUTDOWN = "server_shutdown"
+    ENDPOINT_ADDED = "endpoint_added"
+    ENDPOINT_REMOVED = "endpoint_removed"
 
 
 class APICommand(str, Enum):
     """Enum with all known API commands."""
 
     START_LISTENING = "start_listening"
     SERVER_DIAGNOSTICS = "diagnostics"
@@ -34,14 +36,15 @@
     SET_THREAD_DATASET = "set_thread_dataset"
     OPEN_COMMISSIONING_WINDOW = "open_commissioning_window"
     DISCOVER = "discover"
     INTERVIEW_NODE = "interview_node"
     DEVICE_COMMAND = "device_command"
     REMOVE_NODE = "remove_node"
     GET_VENDOR_NAMES = "get_vendor_names"
+    SUBSCRIBE_ATTRIBUTE = "subscribe_attribute"
 
 
 EventCallBackType = Callable[[EventType, Any], None]
 
 # Generic model(s)
 
 
@@ -62,16 +65,23 @@
     """Matter node data as received from (and stored on) the server."""
 
     node_id: int
     date_commissioned: datetime
     last_interview: datetime
     interview_version: int
     available: bool = False
+    is_bridge: bool = False
     # attributes are stored in form of AttributePath: ENDPOINT/CLUSTER_ID/ATTRIBUTE_ID
     attributes: dict[str, Any] = field(default_factory=dict)
+    # all attribute subscriptions we need to persist for this node,
+    # a set of tuples in format (endpoint_id, cluster_id, attribute_id)
+    # where each value can also be a '*' for wildcard
+    attribute_subscriptions: set[tuple[int | str, int | str, int | str]] = field(
+        default_factory=set
+    )
 
 
 @dataclass
 class ServerDiagnostics:
     """Full dump of the server information and data."""
 
     info: ServerInfoMessage
```

### Comparing `python-matter-server-3.5.2/matter_server/server/__main__.py` & `python-matter-server-3.6.0/matter_server/server/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,14 +66,16 @@
     """Run main execution."""
     # configure logging
     handlers = None
     if args.log_file:
         handlers = [logging.FileHandler(args.log_file)]
     logging.basicConfig(handlers=handlers, level=args.log_level.upper())
     coloredlogs.install(level=args.log_level.upper())
+    if not logging.getLogger().isEnabledFor(logging.DEBUG):
+        logging.getLogger("chip").setLevel(logging.WARNING)
 
     # make sure storage path exists
     if not os.path.isdir(args.storage_path):
         os.mkdir(args.storage_path)
 
     # Init server
     server = MatterServer(
```

### Comparing `python-matter-server-3.5.2/matter_server/server/client_handler.py` & `python-matter-server-3.6.0/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.2/matter_server/server/const.py` & `python-matter-server-3.6.0/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.2/matter_server/server/device_controller.py` & `python-matter-server-3.6.0/matter_server/server/device_controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 from __future__ import annotations
 
 import asyncio
 from collections import deque
 from datetime import datetime
 from functools import partial
 import logging
-import time
-from typing import TYPE_CHECKING, Any, Callable, Coroutine, Deque, Type, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, Deque, Iterable, Type, TypeVar, cast
 
 from chip.ChipDeviceCtrl import CommissionableNode
 from chip.clusters import Attribute, Objects as Clusters
 from chip.clusters.Attribute import ValueDecodeFailure
-from chip.clusters.ClusterObjects import ALL_CLUSTERS, Cluster
+from chip.clusters.ClusterObjects import (
+    ALL_ATTRIBUTES,
+    ALL_CLUSTERS,
+    Cluster,
+    ClusterAttributeDescriptor,
+)
 from chip.exceptions import ChipStackError
 
 from ..common.const import SCHEMA_VERSION
 from ..common.errors import (
     NodeCommissionFailed,
     NodeInterviewFailed,
     NodeNotExists,
@@ -25,14 +29,15 @@
 )
 from ..common.helpers.api import api_command
 from ..common.helpers.json import json_dumps
 from ..common.helpers.util import (
     create_attribute_path,
     create_attribute_path_from_attribute,
     dataclass_from_dict,
+    parse_attribute_path,
 )
 from ..common.models import APICommand, EventType, MatterNodeData
 from .const import PAA_ROOT_CERTS_DIR
 from .helpers.paa_certificates import fetch_certificates
 
 if TYPE_CHECKING:
     from chip.ChipDeviceCtrl import ChipDeviceController
@@ -41,15 +46,23 @@
 
 _T = TypeVar("_T")
 
 DATA_KEY_NODES = "nodes"
 DATA_KEY_LAST_NODE_ID = "last_node_id"
 
 LOGGER = logging.getLogger(__name__)
-INTERVIEW_TASK_LIMIT = 10
+INTERVIEW_TASK_LIMIT = 5
+
+# a list of attributes we should always watch on all nodes
+DEFAULT_SUBSCRIBE_ATTRIBUTES: set[tuple[int | str, int | str, int | str]] = {
+    ("*", 0x001D, 0x00000000),  # all endpoints, descriptor cluster, deviceTypeList
+    ("*", 0x001D, 0x00000003),  # all endpoints, descriptor cluster, partsList
+    (0, 0x0028, "*"),  # endpoint 0, BasicInformation cluster, all attributes
+    ("*", 0x0039, "*"),  # BridgedDeviceBasicInformation
+}
 
 
 class MatterDeviceController:
     """Class that manages the Matter devices."""
 
     chip_controller: ChipDeviceController | None
 
@@ -58,19 +71,24 @@
         server: MatterServer,
     ):
         """Initialize the device controller."""
         self.server = server
         # we keep the last events in memory so we can include them in the diagnostics dump
         self.event_history: Deque[Attribute.EventReadResult] = deque(maxlen=25)
         self._subscriptions: dict[int, Attribute.SubscriptionTransaction] = {}
+        self._attr_subscriptions: dict[int, list[tuple[Any, ...]] | str] = {}
+        self._resub_timer: dict[int, asyncio.TimerHandle] = {}
         self._nodes: dict[int, MatterNodeData | None] = {}
         self.wifi_credentials_set: bool = False
         self.thread_credentials_set: bool = False
         self.compressed_fabric_id: int | None = None
-        self._interview_task: asyncio.Task | None = None
+        self._interview_limit: asyncio.Semaphore = asyncio.Semaphore(
+            INTERVIEW_TASK_LIMIT
+        )
+        self._node_lock: dict[int, asyncio.Lock] = {}
 
     async def initialize(self) -> None:
         """Async initialize of controller."""
         # (re)fetch all PAA certificates once at startup
         # NOTE: this must be done before initializing the controller
         await fetch_certificates()
         # Instantiate the underlying ChipDeviceController instance on the Fabric
@@ -93,19 +111,17 @@
             if node_dict and node_dict.get("interview_version") != SCHEMA_VERSION:
                 node = None
             else:
                 node = dataclass_from_dict(MatterNodeData, node_dict)
                 # always mark node as unavailable at startup until subscriptions are ready
                 node.available = False
             self._nodes[node_id] = node
-        # setup subscriptions and (re)interviews as task in the background
-        # as we do not want it to block our startup
-        self._interview_task = asyncio.create_task(
-            self._check_subscriptions_and_interviews()
-        )
+            # setup subscription and (re)interview as task in the background
+            # as we do not want it to block our startup
+            asyncio.create_task(self._check_interview_and_subscription(node_id))
         LOGGER.debug("Loaded %s nodes", len(self._nodes))
 
     async def stop(self) -> None:
         """Handle logic on server stop."""
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
 
@@ -156,15 +172,15 @@
             raise NodeCommissionFailed(
                 f"Commission with code failed for node {node_id}"
             )
 
         # full interview of the device
         await self.interview_node(node_id)
         # make sure we start a subscription for this newly added node
-        await self.subscribe_node(node_id)
+        await self._subscribe_node(node_id)
         # return full node object once we're complete
         return self.get_node(node_id)
 
     @api_command(APICommand.COMMISSION_ON_NETWORK)
     async def commission_on_network(
         self,
         setup_pin_code: int,
@@ -201,15 +217,15 @@
             raise NodeCommissionFailed(
                 f"Commission on network failed for node {node_id}"
             )
 
         # full interview of the device
         await self.interview_node(node_id)
         # make sure we start a subscription for this newly added node
-        await self.subscribe_node(node_id)
+        await self._subscribe_node(node_id)
         # return full node object once we're complete
         return self.get_node(node_id)
 
     @api_command(APICommand.SET_WIFI_CREDENTIALS)
     async def set_wifi_credentials(self, ssid: str, credentials: str) -> None:
         """Set WiFi credentials for commissioning to a (new) device."""
         if self.chip_controller is None:
@@ -241,16 +257,15 @@
         self,
         node_id: int,
         timeout: int = 300,
         iteration: int = 1000,
         option: int = 1,
         discriminator: int | None = None,
     ) -> tuple[int, str]:
-        """
-        Open a commissioning window to commission a device present on this controller to another.
+        """Open a commissioning window to commission a device present on this controller to another.
 
         Returns code to use as discriminator.
         """
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
 
         if discriminator is None:
@@ -284,19 +299,24 @@
         """Interview a node."""
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
 
         LOGGER.debug("Interviewing node: %s", node_id)
         try:
             await self._resolve_node(node_id=node_id)
-            read_response: Attribute.AsyncReadTransaction.ReadResponse = (
-                await self.chip_controller.Read(
-                    nodeid=node_id, attributes="*", events="*", fabricFiltered=False
-                )
-            )
+            async with self._interview_limit:
+                async with self._get_node_lock(node_id):
+                    read_response: Attribute.AsyncReadTransaction.ReadResponse = (
+                        await self.chip_controller.Read(
+                            nodeid=node_id,
+                            attributes="*",
+                            events="*",
+                            fabricFiltered=False,
+                        )
+                    )
         except (ChipStackError, NodeNotResolving) as err:
             raise NodeInterviewFailed(f"Failed to interview node {node_id}") from err
 
         is_new_node = node_id not in self._nodes
         existing_info = self._nodes.get(node_id)
         node = MatterNodeData(
             node_id=node_id,
@@ -306,27 +326,34 @@
             last_interview=datetime.utcnow(),
             interview_version=SCHEMA_VERSION,
             attributes=self._parse_attributes_from_read_result(
                 read_response.attributes
             ),
         )
 
+        if existing_info:
+            node.attribute_subscriptions = existing_info.attribute_subscriptions
+        # work out if the node is a bridge device by looking at the devicetype of endpoint 1
+        if attr_data := node.attributes.get("1/29/0"):
+            node.is_bridge = any(x.deviceType == 14 for x in attr_data)
+
         # save updated node data
         self._nodes[node_id] = node
         self.server.storage.set(
             DATA_KEY_NODES,
             subkey=str(node_id),
             value=node,
             force=not existing_info,
         )
         if is_new_node:
             # new node - first interview
             self.server.signal_event(EventType.NODE_ADDED, node)
         else:
             # existing node, signal node updated event
+            # TODO: maybe only signal this event if attributes actually changed ?
             self.server.signal_event(EventType.NODE_UPDATED, node)
 
         LOGGER.debug("Interview of node %s completed", node_id)
 
     @api_command(APICommand.DEVICE_COMMAND)
     async def send_device_command(
         self,
@@ -342,22 +369,23 @@
         """Send a command to a Matter node/device."""
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
 
         cluster_cls: Cluster = ALL_CLUSTERS[cluster_id]
         command_cls = getattr(cluster_cls.Commands, command_name)
         command = dataclass_from_dict(command_cls, payload)
-        return await self.chip_controller.SendCommand(
-            nodeid=node_id,
-            endpoint=endpoint_id,
-            payload=command,
-            responseType=response_type,
-            timedRequestTimeoutMs=timed_request_timeout_ms,
-            interactionTimeoutMs=interaction_timeout_ms,
-        )
+        async with self._get_node_lock(node_id):
+            return await self.chip_controller.SendCommand(
+                nodeid=node_id,
+                endpoint=endpoint_id,
+                payload=command,
+                responseType=response_type,
+                timedRequestTimeoutMs=timed_request_timeout_ms,
+                interactionTimeoutMs=interaction_timeout_ms,
+            )
 
     @api_command(APICommand.REMOVE_NODE)
     async def remove_node(self, node_id: int) -> None:
         """Remove a Matter node/device from the fabric."""
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
 
@@ -376,71 +404,200 @@
 
         attribute_path = create_attribute_path_from_attribute(
             0,
             Clusters.OperationalCredentials.Attributes.CurrentFabricIndex,
         )
         fabric_index = node.attributes[attribute_path]
 
-        self.server.signal_event(EventType.NODE_DELETED, node_id)
+        self.server.signal_event(EventType.NODE_REMOVED, node_id)
 
         await self.chip_controller.SendCommand(
             nodeid=node_id,
             endpoint=0,
             payload=Clusters.OperationalCredentials.Commands.RemoveFabric(
                 fabricIndex=fabric_index,
             ),
         )
 
-    async def subscribe_node(self, node_id: int) -> None:
+    @api_command(APICommand.SUBSCRIBE_ATTRIBUTE)
+    async def subscribe_attribute(
+        self, node_id: int, attribute_path: str | list[str]
+    ) -> None:
         """
-        Subscribe to all node state changes/events for an individual node.
+        Subscribe to given AttributePath(s).
 
-        Note that by using the listen command at server level, you will receive all node events.
+        Either supply a single attribute path or a list of paths.
+        The given attribute path(s) will be added to the list of attributes that
+        are watched for the given node. This is persistent over restarts.
         """
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
 
         if node_id not in self._nodes:
             raise NodeNotExists(
                 f"Node {node_id} does not exist or has not been interviewed."
             )
-        assert node_id not in self._subscriptions, "Already subscribed to node"
-        node_logger = LOGGER.getChild(str(node_id))
-        node_logger.debug("Setting up subscriptions...")
 
+        node = self._nodes[node_id]
+        assert node is not None
+
+        # work out added subscriptions
+        if not isinstance(attribute_path, list):
+            attribute_path = [attribute_path]
+        attribute_paths = {parse_attribute_path(x) for x in attribute_path}
+        prev_subs = set(node.attribute_subscriptions)
+        node.attribute_subscriptions.update(attribute_paths)
+        if prev_subs == node.attribute_subscriptions:
+            return  # nothing to do
+        # save updated node data
+        self.server.storage.set(
+            DATA_KEY_NODES,
+            subkey=str(node_id),
+            value=node,
+        )
+
+        # (re)setup node subscription
+        # this could potentially be called multiple times within a short timeframe
+        # so debounce it a bit
+        def resubscribe() -> None:
+            self._resub_timer.pop(node_id, None)
+            asyncio.create_task(self._subscribe_node(node_id))
+
+        if existing_timer := self._resub_timer.pop(node_id, None):
+            existing_timer.cancel()
+        assert self.server.loop is not None
+        self._resub_timer[node_id] = self.server.loop.call_later(5, resubscribe)
+
+    async def _subscribe_node(self, node_id: int) -> None:
+        """
+        Subscribe to all node state changes/events for an individual node.
+
+        Note that by using the listen command at server level,
+        you will receive all (subscribed) node events and attribute updates.
+        """
+        # pylint: disable=too-many-locals,too-many-statements
+        if self.chip_controller is None:
+            raise RuntimeError("Device Controller not initialized.")
+
+        if self._nodes.get(node_id) is None:
+            raise NodeNotExists(
+                f"Node {node_id} does not exist or has not been interviewed."
+            )
+
+        node_logger = LOGGER.getChild(f"[node {node_id}]")
+        node_lock = self._get_node_lock(node_id)
         node = cast(MatterNodeData, self._nodes[node_id])
-        node.available = False
         await self._resolve_node(node_id=node_id)
-        node.available = True
 
-        # we follow the pattern of apple and google here and
-        # just do a wildcard subscription for all clusters and properties
-        # the client will handle filtering of the events.
-        # if it turns out in the future that this is too much traffic (I don't think so now)
-        # we can revisit this choice and do some selected subscriptions.
-        sub: Attribute.SubscriptionTransaction = await self.chip_controller.Read(
-            nodeid=node_id,
-            attributes="*",
-            events=[("*", 1)],
-            reportInterval=(0, 120),
-            fabricFiltered=False,
-        )
+        # work out all (current) attribute subscriptions
+        attr_subscriptions: list[Any] = []
+        for (
+            endpoint_id,
+            cluster_id,
+            attribute_id,
+        ) in set.union(DEFAULT_SUBSCRIBE_ATTRIBUTES, node.attribute_subscriptions):
+            endpoint: int | None = None if endpoint_id == "*" else int(endpoint_id)
+            cluster: Type[Cluster] = ALL_CLUSTERS[cluster_id]
+            attribute: Type[ClusterAttributeDescriptor] | None = (
+                None
+                if attribute_id == "*"
+                else ALL_ATTRIBUTES[cluster_id][attribute_id]
+            )
+            if endpoint and attribute:
+                # Concrete path: specific endpoint, specific clusterattribute
+                attr_subscriptions.append((endpoint, attribute))
+            elif endpoint and cluster:
+                # Specific endpoint, Wildcard attribute id (specific cluster)
+                attr_subscriptions.append((endpoint, cluster))
+            elif attribute:
+                # Wildcard endpoint, specific attribute
+                attr_subscriptions.append(attribute)
+            elif cluster:
+                # Wildcard endpoint, specific cluster
+                attr_subscriptions.append(cluster)
+
+        if len(attr_subscriptions) > 50:
+            # prevent memory overload on node and fallback to wildcard sub if too many
+            # individual subscriptions
+            attr_subscriptions = "*"  # type: ignore[assignment]
+
+        # check if we already have an subscription for this node,
+        # if so, we need to unsubscribe first because a device can only maintain
+        # a very limited amount of concurrent subscriptions.
+        if prev_sub := self._subscriptions.pop(node_id, None):
+            if self._attr_subscriptions.get(node_id) == attr_subscriptions:
+                # the current subscription already matches, no need to re-setup
+                node_logger.debug("Re-using existing subscription.")
+                return
+            async with node_lock:
+                node_logger.debug("Unsubscribing from existing subscription.")
+                await self._call_sdk(prev_sub.Shutdown)
+
+        node_logger.debug("Setting up attributes and events subscription.")
+        self._attr_subscriptions[node_id] = attr_subscriptions
+        async with node_lock:
+            sub: Attribute.SubscriptionTransaction = await self.chip_controller.Read(
+                nodeid=node_id,
+                # In order to prevent network congestion due to wildcard subscriptions on all nodes,
+                # we keep a list of attributes we are explicitly interested in.
+                attributes=attr_subscriptions,
+                # simply subscribe to all (urgent and non urgent) device events
+                events=[("*", 1), ("*", 0)],
+                # Use a report interval of 0, 300 which means we want to receive state changes
+                # as soon as possible (the 0 as floor) but we want to receive a report
+                # at least once every 5 minutes (300 as ceiling).
+                # This is also used to detect the node is still alive.
+                # A resubscription will be initiated automatically by the sdk
+                # if there was no report within the interval.
+                reportInterval=(0, 300),
+                # Use fabricfiltered as False to detect changes made by other controllers
+                # and to be able to provide a list of all fabrics attached to the device
+                fabricFiltered=False,
+            )
 
         def attribute_updated_callback(
             path: Attribute.TypedAttributePath,
             transaction: Attribute.SubscriptionTransaction,
         ) -> None:
             assert self.server.loop is not None
             new_value = transaction.GetAttribute(path)
             # failsafe: ignore ValueDecodeErrors
             # these are set by the SDK if parsing the value failed miserably
             if isinstance(new_value, ValueDecodeFailure):
                 return
-            node_logger.debug("Attribute updated: %s - new value: %s", path, new_value)
+
             attr_path = str(path.Path)
+            old_value = node.attributes.get(attr_path)
+
+            node_logger.debug(
+                "Attribute updated: %s - old value: %s - new value: %s",
+                path,
+                old_value,
+                new_value,
+            )
+
+            # work out added/removed endpoints on bridges
+            if (
+                node.is_bridge
+                and path.Path.EndpointId == 0
+                and path.AttributeType == Clusters.Descriptor.Attributes.PartsList
+            ):
+                endpoints_removed = set(old_value or []) - set(new_value)
+                endpoints_added = set(new_value) - set(old_value or [])
+                if endpoints_removed:
+                    self.server.loop.call_soon_threadsafe(
+                        self._handle_endpoints_removed, node_id, endpoints_removed
+                    )
+                if endpoints_added:
+                    self.server.loop.create_task(
+                        self._handle_endpoints_added(node_id, endpoints_added)
+                    )
+                return
+
+            # store updated value in node attributes
             node.attributes[attr_path] = new_value
 
             # schedule save to persistent storage
             self.server.storage.set(
                 DATA_KEY_NODES,
                 subkey=str(node_id),
                 value=node,
@@ -456,15 +613,17 @@
 
         def event_callback(
             data: Attribute.EventReadResult,
             transaction: Attribute.SubscriptionTransaction,
         ) -> None:
             # pylint: disable=unused-argument
             assert self.server.loop is not None
-            node_logger.debug("Received node event: %s", data)
+            node_logger.debug(
+                "Received node event: %s - transaction: %s", data, transaction
+            )
             self.event_history.append(data)
             self.server.loop.call_soon_threadsafe(
                 self.server.signal_event, EventType.NODE_EVENT, data
             )
 
         def error_callback(
             chipError: int, transaction: Attribute.SubscriptionTransaction
@@ -474,44 +633,48 @@
 
         def resubscription_attempted(
             transaction: Attribute.SubscriptionTransaction,
             terminationError: int,
             nextResubscribeIntervalMsec: int,
         ) -> None:
             # pylint: disable=unused-argument, invalid-name
-            node_logger.debug(
+            node_logger.info(
                 "Previous subscription failed with Error: %s, re-subscribing in %s ms...",
                 terminationError,
                 nextResubscribeIntervalMsec,
             )
             # mark node as unavailable and signal consumers
             if node.available:
                 node.available = False
                 self.server.signal_event(EventType.NODE_UPDATED, node)
 
         def resubscription_succeeded(
             transaction: Attribute.SubscriptionTransaction,
         ) -> None:
             # pylint: disable=unused-argument, invalid-name
-            node_logger.debug("Re-Subscription succeeded")
+            node_logger.info("Re-Subscription succeeded")
             # mark node as available and signal consumers
             if not node.available:
                 node.available = True
                 self.server.signal_event(EventType.NODE_UPDATED, node)
 
         sub.SetAttributeUpdateCallback(attribute_updated_callback)
         sub.SetEventUpdateCallback(event_callback)
         sub.SetErrorCallback(error_callback)
         sub.SetResubscriptionAttemptedCallback(resubscription_attempted)
         sub.SetResubscriptionSucceededCallback(resubscription_succeeded)
         self._subscriptions[node_id] = sub
+
         # if we reach this point, it means the node could be resolved
         # and the initial subscription succeeded, mark the node available.
         node.available = True
-        node_logger.debug("Subscription succeeded")
+        node_logger.info("Subscription succeeded")
+        # update attributes with current state from read request
+        current_atributes = self._parse_attributes_from_read_result(sub.GetAttributes())
+        node.attributes.update(current_atributes)
         self.server.signal_event(EventType.NODE_UPDATED, node)
 
     def _get_next_node_id(self) -> int:
         """Return next node_id."""
         next_node_id = cast(int, self.server.storage.get(DATA_KEY_LAST_NODE_ID, 0)) + 1
         self.server.storage.set(DATA_KEY_LAST_NODE_ID, next_node_id, force=True)
         return next_node_id
@@ -525,96 +688,65 @@
             _T,
             await self.server.loop.run_in_executor(
                 None,
                 partial(func, *args, **kwargs),
             ),
         )
 
-    async def _check_subscriptions_and_interviews(self) -> None:
-        """Run subscriptions (and interviews) for known nodes."""
-        # Set default resubscribe interval to 1 hour
-        reschedule_interval = 3600
-        start_time = time.time()
-        tasks: list[Coroutine[Any, Any, None]] = []
-        task_limit: asyncio.Semaphore = asyncio.Semaphore(INTERVIEW_TASK_LIMIT)
-
-        for node_id, node in self._nodes.items():
-            # (re)interview node (only) if needed
-            if (
-                node is None
-                or node.interview_version < SCHEMA_VERSION
-                or (datetime.utcnow() - node.last_interview).days > 30
-            ):
-
-                async def _interview_node(node_id: int) -> None:
-                    """Run interview for node."""
-                    try:
-                        await self.interview_node(node_id)
-                    except NodeInterviewFailed as err:
-                        LOGGER.warning(
-                            "Unable to interview Node %s, we will retry later in the background.",
-                            node_id,
-                            exc_info=err,
-                        )
-                        raise err
-
-                tasks.append(_interview_node(node_id))
-                continue
+    async def _check_interview_and_subscription(
+        self, node_id: int, reschedule_interval: int = 300
+    ) -> None:
+        """Handle interview (if needed) and subscription for known node."""
 
-            # setup subscriptions for the node
-            if node_id in self._subscriptions:
-                continue
-
-            async def _subscribe_node(node_id: int) -> None:
-                """Subscribe to node events."""
-                try:
-                    await self.subscribe_node(node_id)
-                except NodeNotResolving as err:
-                    LOGGER.warning(
-                        "Unable to subscribe to Node %s, "
-                        "we will retry later in the background.",
-                        node_id,
-                        exc_info=err,
-                    )
-                    raise err
+        def reschedule() -> None:
+            """(Re)Schedule interview and/or initial subscription for a node."""
+            assert self.server.loop is not None
+            self.server.loop.call_later(
+                reschedule_interval,
+                asyncio.create_task,
+                self._check_interview_and_subscription(
+                    node_id,
+                    # increase interval at each attempt with maximum of 1 hour
+                    min(reschedule_interval + 300, 3600),
+                ),
+            )
+
+        # (re)interview node (only) if needed
+        node_data = self._nodes.get(node_id)
+        if (
+            node_data is None
+            # re-interview if the schema has changed
+            or node_data.interview_version < SCHEMA_VERSION
+            # re-interview every 30 days
+            or (datetime.utcnow() - node_data.last_interview).days > 30
+        ):
+            try:
+                await self.interview_node(node_id)
+            except NodeInterviewFailed:
+                LOGGER.warning(
+                    "Unable to interview Node %s, will retry later in the background.",
+                    node_id,
+                )
+                # reschedule self on error
+                reschedule()
+                return
 
-            tasks.append(_subscribe_node(node_id))
+        # setup subscriptions for the node
+        if node_id in self._subscriptions:
+            return
 
-        async def _run_task(task: Coroutine[Any, Any, None]) -> None:
-            """Run coroutine and release semaphore."""
-            async with task_limit:
-                await task
-
-        LOGGER.debug("Running %s tasks", len(tasks))
-        # wait for all tasks to finish
-        results: list[Exception | None] = await asyncio.gather(
-            *(_run_task(task) for task in tasks), return_exceptions=True
-        )
-        LOGGER.debug(
-            "Done running %s tasks in %s seconds",
-            len(results),
-            start_time - time.time(),
-        )
-        # check if any of the tasks failed
-        for result in results:
-            if isinstance(result, Exception):
-                # if any of the tasks failed, reschedule in 5 minutes
-                reschedule_interval = 300
-                break
-
-        # reschedule self to run every hour
-        def _schedule() -> None:
-            """Schedule task."""
-            self._interview_task = asyncio.create_task(
-                self._check_subscriptions_and_interviews()
-            )
-
-        LOGGER.debug("Rescheduling interviews in %s seconds", reschedule_interval)
-        loop = cast(asyncio.AbstractEventLoop, self.server.loop)
-        loop.call_later(reschedule_interval, _schedule)
+        try:
+            await self._subscribe_node(node_id)
+        except NodeNotResolving:
+            LOGGER.warning(
+                "Unable to subscribe to Node %s as it is unavailable, "
+                "will retry later in the background.",
+                node_id,
+            )
+            reschedule()
 
     @staticmethod
     def _parse_attributes_from_read_result(
         read_result: dict[int, dict[Type, dict[Type, Any]]]
     ) -> dict[str, Any]:
         """Parse attributes from ReadResult."""
         result = {}
@@ -654,31 +786,74 @@
                     result[attribute_path] = attr_value
         return result
 
     async def _resolve_node(
         self, node_id: int, retries: int = 3, allow_pase: bool = False
     ) -> None:
         """Resolve a Node on the network."""
+        node_lock = self._get_node_lock(node_id)
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
         try:
             if allow_pase:
                 # last attempt allows PASE connection (last resort)
                 LOGGER.debug(
                     "Attempting to resolve node %s (with PASE connection)", node_id
                 )
-                await self._call_sdk(
-                    self.chip_controller.GetConnectedDeviceSync,
-                    nodeid=node_id,
-                    allowPASE=True,
-                )
+                async with node_lock:
+                    await self._call_sdk(
+                        self.chip_controller.GetConnectedDeviceSync,
+                        nodeid=node_id,
+                        allowPASE=True,
+                        timeoutMs=30000,
+                    )
                 return
             LOGGER.debug("Resolving node %s", node_id)
             await self._call_sdk(self.chip_controller.ResolveNode, nodeid=node_id)
         except (ChipStackError, TimeoutError) as err:
             if not retries:
                 # when we're out of retries, raise NodeNotResolving
                 raise NodeNotResolving(f"Unable to resolve Node {node_id}") from err
-            await self._resolve_node(
-                node_id=node_id, retries=retries - 1, allow_pase=retries - 1 == 0
-            )
+            async with node_lock:
+                await self._resolve_node(
+                    node_id=node_id, retries=retries - 1, allow_pase=retries - 1 == 0
+                )
             await asyncio.sleep(2)
+
+    def _handle_endpoints_removed(self, node_id: int, endpoints: Iterable[int]) -> None:
+        """Handle callback for when bridge endpoint(s) get deleted."""
+        node = cast(MatterNodeData, self._nodes[node_id])
+        for endpoint_id in endpoints:
+            node.attributes = {
+                key: value
+                for key, value in node.attributes.items()
+                if not key.startswith(f"{endpoint_id}/")
+            }
+            self.server.signal_event(
+                EventType.ENDPOINT_REMOVED,
+                {"node_id": node_id, "endpoint_id": endpoint_id},
+            )
+        # schedule save to persistent storage
+        self.server.storage.set(
+            DATA_KEY_NODES,
+            subkey=str(node_id),
+            value=node,
+        )
+
+    async def _handle_endpoints_added(
+        self, node_id: int, endpoints: Iterable[int]
+    ) -> None:
+        """Handle callback for when bridge endpoint(s) get added."""
+        # we simply do a full interview of the node
+        await self.interview_node(node_id)
+        # signal event to consumers
+        for endpoint_id in endpoints:
+            self.server.signal_event(
+                EventType.ENDPOINT_ADDED,
+                {"node_id": node_id, "endpoint_id": endpoint_id},
+            )
+
+    def _get_node_lock(self, node_id: int) -> asyncio.Lock:
+        """Return lock for given node."""
+        if node_id not in self._node_lock:
+            self._node_lock[node_id] = asyncio.Lock()
+        return self._node_lock[node_id]
```

### Comparing `python-matter-server-3.5.2/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.6.0/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.2/matter_server/server/server.py` & `python-matter-server-3.6.0/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.2/matter_server/server/stack.py` & `python-matter-server-3.6.0/matter_server/server/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
         self.logger.info("Initializing CHIP/Matter Controller Stack...")
         storage_file = os.path.join(server.storage_path, "chip.json")
         self.logger.debug("Using storage file: %s", storage_file)
         chip.native.Init()
         chip.logging.RedirectToPythonLogging()
 
         self._chip_stack = ChipStack(
-            persistentStoragePath=storage_file, enableServerInteractions=False
+            persistentStoragePath=storage_file,
+            installDefaultLogHandler=False,
+            enableServerInteractions=False,
         )
 
         # Initialize Certificate Authority Manager
         # yeah this is a bit weird just to prevent a circular import in the underlying SDK
         self.certificate_authority_manager: CertificateAuthorityManager = (
             chip.CertificateAuthority.CertificateAuthorityManager(
                 chipStack=self._chip_stack
```

### Comparing `python-matter-server-3.5.2/matter_server/server/storage.py` & `python-matter-server-3.6.0/matter_server/server/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,24 +119,29 @@
         loop = asyncio.get_running_loop()
         self._data = await loop.run_in_executor(None, _load)
 
     def save(self, immediate: bool = False) -> None:
         """Schedule save of data to disk."""
         assert self.server.loop is not None
 
+        def _do_save() -> None:
+            assert self.server.loop is not None
+            self.server.loop.create_task(self.async_save())
+
         if self._timer_handle is not None:
             self._timer_handle.cancel()
             self._timer_handle = None
 
         if immediate:
-            self.server.loop.create_task(self.async_save())
+            _do_save()
+
         else:
             # schedule the save for later
             self._timer_handle = self.server.loop.call_later(
-                DEFAULT_SAVE_DELAY, self.server.loop.create_task, self.async_save()
+                DEFAULT_SAVE_DELAY, _do_save
             )
 
     async def async_save(self) -> None:
         """Save persistent data to disk."""
         assert self.server.loop is not None
 
         def do_save() -> None:
```

### Comparing `python-matter-server-3.5.2/matter_server/server/vendor_info.py` & `python-matter-server-3.6.0/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.2/pyproject.toml` & `python-matter-server-3.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools~=62.3",
     "wheel~=0.37.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.5.2"
+version = "3.6.0"
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "The Home Assistant Authors", email = "hello@home-assistant.io" },
 ]
 classifiers = [
@@ -40,17 +40,17 @@
     "cryptography==41.0.1",
 ]
 test = [
     "black==23.3.0",
     "flake8==6.0.0",
     "flake8-docstrings==1.7.0",
     "isort==5.12.0",
-    "mypy==1.3.0",
+    "mypy==1.4.1",
     "pylint==2.17.4",
-    "pytest==7.3.2",
+    "pytest==7.4.0",
     "pytest-aiohttp==1.0.4",
     "pytest-cov==4.1.0",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
```

### Comparing `python-matter-server-3.5.2/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-3.6.0/python_matter_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.5.2
+Version: 3.6.0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -59,25 +59,25 @@
 relies on the networking managed by your operating system.
 
 ### Requirements to communicate with Wi-Fi/Ethernet based Thread devices
 
 Make sure your you run the container on the host network. The host network
 interface needs to be in the same network as the Android/iPhone device
 you are using for commissioning. Matter uses link-local multicast protocols
-which do not work accross different LANs or VLANs.
+which do not work across different LANs or VLANs.
 
 The host network interface needs IPv6 support enabled.
 
 ### Requirements to communicate with Thread devices through Thread border routers
 
 For communication through Thread border routers which are not running on the same
 host as the Matter Controller server to work, IPv6 routing needs to be properly
 working. IPv6 routing is largely setup automatically through the IPv6 Neighbor
 Discovery Protocol, specifically the Route Information Options (RIO). However,
-if IPv6 ND RIO's are processed, and processed correctly depends on the network
+if IPv6 Neighbor Discovery RIO's are processed, and processed correctly depends on the network
 management software your system is using. There may be bugs and cavats in
 processing this Route Information Options.
 
 In general, make sure the kernel option `CONFIG_IPV6_ROUTER_PREF` is enabled and
 that IPv6 forwarding is disabled (sysctl variable `net.ipv6.conf.all.forwarding`).
 If IPv6 forwarding is enabled, the Linux kernel doesn't employ reachability
 probing (RFC 4191), which can lead to longer outages (up to 30min) until
```

### Comparing `python-matter-server-3.5.2/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.6.0/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

