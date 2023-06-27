# Comparing `tmp/nso-oc-2.70.0.tar.gz` & `tmp/nso-oc-2.71.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.70.0.tar", last modified: Wed Jun 21 17:50:06 2023, max compression
+gzip compressed data, was "nso-oc-2.71.0.tar", last modified: Tue Jun 27 10:50:11 2023, max compression
```

## Comparing `nso-oc-2.70.0.tar` & `nso-oc-2.71.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:50:06.067971 nso-oc-2.70.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-21 17:49:35.000000 nso-oc-2.70.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 17:49:35.000000 nso-oc-2.70.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-21 17:50:06.067971 nso-oc-2.70.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-21 17:49:35.000000 nso-oc-2.70.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:50:06.063971 nso-oc-2.70.0/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-21 17:50:06.000000 nso-oc-2.70.0/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-21 17:50:06.000000 nso-oc-2.70.0/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:50:06.000000 nso-oc-2.70.0/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 17:50:06.000000 nso-oc-2.70.0/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 17:50:06.000000 nso-oc-2.70.0/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 17:50:06.000000 nso-oc-2.70.0/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:50:06.063971 nso-oc-2.70.0/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:50:06.063971 nso-oc-2.70.0/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_mpls.py
--rw-r--r--   0 runner    (1001) docker     (123)    42337 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:50:06.067971 nso-oc-2.70.0/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-21 17:49:35.000000 nso-oc-2.70.0/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 17:49:35.000000 nso-oc-2.70.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 17:50:06.067971 nso-oc-2.70.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-21 17:49:35.000000 nso-oc-2.70.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:50:11.725886 nso-oc-2.71.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-27 10:49:32.000000 nso-oc-2.71.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-27 10:49:32.000000 nso-oc-2.71.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-27 10:50:11.725886 nso-oc-2.71.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-27 10:49:32.000000 nso-oc-2.71.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:50:11.721886 nso-oc-2.71.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-27 10:50:11.000000 nso-oc-2.71.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-27 10:50:11.000000 nso-oc-2.71.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:50:11.000000 nso-oc-2.71.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 10:50:11.000000 nso-oc-2.71.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 10:50:11.000000 nso-oc-2.71.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 10:50:11.000000 nso-oc-2.71.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:50:11.721886 nso-oc-2.71.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:50:11.725886 nso-oc-2.71.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32603 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_mpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42337 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:50:11.725886 nso-oc-2.71.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-27 10:49:32.000000 nso-oc-2.71.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-27 10:49:32.000000 nso-oc-2.71.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 10:50:11.725886 nso-oc-2.71.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-27 10:49:32.000000 nso-oc-2.71.0/setup.py
```

### Comparing `nso-oc-2.70.0/LICENSE` & `nso-oc-2.71.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/PKG-INFO` & `nso-oc-2.71.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.70.0
+Version: 2.71.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.70.0/README.md` & `nso-oc-2.71.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.71.0/nso_oc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.70.0
+Version: 2.71.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.70.0/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.71.0/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/README.md` & `nso-oc-2.71.0/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/common.py` & `nso-oc-2.71.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/main.py` & `nso-oc-2.71.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,48 @@
     "tcp": "IP_TCP",
     "udp": "IP_UDP",
     "gre": "IP_GRE",
     "ahp": "IP_AUTH",
     "esp": "IP_ESP",
     "pim": "IP_PIM"
 }
+icmp_names_to_types = {
+    'administratively-prohibited': (3, 13),
+    'alternate-address': (6, 0),
+    'dod-host-prohibited': (3, 10),
+    'dod-net-prohibited': (3, 9),
+    'echo': (8, 0),
+    'echo-reply': (0, 0),
+    'general-parameter-problem': (12, 0),
+    'host-redirect': (5, 1),
+    'host-tos-redirect': (5, 3),
+    'host-tos-unreachable': (3, 12),
+    'host-unknown': (3, 7),
+    'host-unreachable': (3, 1),
+    'information-reply': (16, 0),
+    'information-request': (15, 0),
+    'mask-reply': (18, 0),
+    'mask-request': (17, 0),
+    'net-redirect': (5, 0),
+    'net-tos-redirect': (5, 2),
+    'net-tos-unreachable': (3, 11),
+    'net-unreachable': (3, 0),
+    'network-unknown': (3, 6),
+    'no-room-for-option': (12, 2),
+    'option-missing': (12, 1),
+    'packet-too-big': (3, 4),
+    'port-unreachable': (3, 3),
+    'protocol-unreachable': (3, 2),
+    'reassembly-timeout': (11, 1),
+    'source-quench': (4, 0),
+    'source-route-failed': (3, 5),
+    'time-exceeded': (11, 0),
+    'timestamp-reply': (14, 0),
+    'timestamp-request': (13, 0),
+    'unreachable': (3, 0)}
 # OC has an additional forwarding action, "DROP", which also translates to "deny" in XE.
 actions_xe_to_oc = {
     "permit": "ACCEPT",
     "deny": "REJECT",
 }
 port_operators = ["range", "eq", "lt", "gt", "neq"]
 ACL_STD_TYPE = "ACL_IPV4_STANDARD"
@@ -262,14 +296,16 @@
         if len(rule_parts) <= current_index:
             return current_index
 
         current_index = self.__set_ip_and_network(rule_parts, current_index, entry, is_source)
 
         if rule_parts[index + 1] == "tcp" or rule_parts[index + 1] == "udp":
             current_index = self.__set_port(rule_parts, current_index, entry, is_source)
+        elif rule_parts[index + 1] == "icmp" and not is_source:
+            current_index = self.__set_icmp(rule_parts, current_index, entry)
 
         return current_index
 
     def __set_ip_and_network(self, rule_parts, current_index, entry, is_source):
         ip = rule_parts[current_index]
 
         if ip == "any":
@@ -281,15 +317,14 @@
             return current_index + 1
         elif ip == "host":
             if is_source:
                 self.__get_ipv4_config(entry)[self._src_addr_key] = f"{rule_parts[current_index + 1]}/32"
             else:
                 self.__get_ipv4_config(entry)[
                     "openconfig-acl:destination-address"] = f"{rule_parts[current_index + 1]}/32"
-
             return current_index + 2
         elif (rule_parts[0].isdigit() and len(rule_parts) == 3) \
                 or (rule_parts[0].isdigit() and len(rule_parts) == 4 and rule_parts[-1] == "log") \
                 or (rule_parts[0].isdigit() and len(rule_parts) == 4 and rule_parts[-1] == "log-input") \
                 or len(rule_parts) == 2 \
                 or (len(rule_parts) == 3 and rule_parts[-1] == "log") \
                 or (len(rule_parts) == 3 and rule_parts[-1] == "log-input"):
@@ -319,15 +354,14 @@
         else:
             prefixlen =temp_ip.prefixlen
 
         if is_source:
             self.__get_ipv4_config(entry)[self._src_addr_key] = f"{ip}/{prefixlen}"
         else:
             self.__get_ipv4_config(entry)["openconfig-acl:destination-address"] = f"{ip}/{prefixlen}"
-
         return current_index + 2
 
     def __set_port(self, rule_parts, current_index, entry, is_source):
         if len(rule_parts) <= current_index or not rule_parts[current_index] in port_operators:
             # We've either reached the end of the rule or there's no specified port
             if is_source:
                 self.__get_transport_config(entry)["openconfig-acl:source-port"] = "ANY"
@@ -383,14 +417,36 @@
             raise ValueError
 
         if not is_source:
             current_index = self.__set_tcp_flags(rule_parts, current_index + 2, entry)
 
         return current_index + 2
 
+    def __set_icmp(self, rule_parts, current_index, entry):
+        if len(rule_parts) <= current_index:
+            # end of the rule or there's messages specified
+            return current_index
+        elif rule_parts[current_index] in icmp_names_to_types:
+            msg, code = icmp_names_to_types[rule_parts[current_index]]
+            entry['openconfig-acl-ext:icmp-v4'] = {'openconfig-acl-ext:config':
+                                                       {'openconfig-acl-ext:type': msg,
+                                                        'openconfig-acl-ext:code': code}}
+            return current_index + 1
+        elif rule_parts[current_index].isdigit():
+            entry['openconfig-acl-ext:icmp-v4'] = {'openconfig-acl-ext:config':
+                                                       {'openconfig-acl-ext:type': rule_parts[current_index],
+                                                        'openconfig-acl-ext:code': 0}}
+            if current_index + 1 < len(rule_parts) and rule_parts[current_index + 1].isdigit():
+                entry['openconfig-acl-ext:icmp-v4']['openconfig-acl-ext:config']['openconfig-acl-ext:code'] = rule_parts[current_index + 1]
+                return current_index + 2
+            return current_index + 1
+        else:
+            return current_index
+
+
     def __set_tcp_flags(self, rule_parts, current_index, entry):
         if len(rule_parts) <= current_index or not rule_parts[current_index] in ["ack", "rst", "established"]:
             return current_index
 
         if rule_parts[current_index] == "ack":
             self.__get_transport_config(entry)["openconfig-acl:tcp-flags"] = ["TCP_ACK"]
         if rule_parts[current_index] == "rst":
```

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_mpls.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_mpls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.71.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.71.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.71.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.71.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.71.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.71.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.70.0/setup.py` & `nso-oc-2.71.0/setup.py`

 * *Files identical despite different names*

