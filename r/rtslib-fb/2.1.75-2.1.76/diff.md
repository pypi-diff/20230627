# Comparing `tmp/rtslib-fb-2.1.75.tar.gz` & `tmp/rtslib-fb-2.1.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rtslib-fb-2.1.75.tar", last modified: Wed May 11 08:35:10 2022, max compression
+gzip compressed data, was "rtslib-fb-2.1.76.tar", last modified: Tue Jun 27 14:59:18 2023, max compression
```

## Comparing `rtslib-fb-2.1.75.tar` & `rtslib-fb-2.1.76.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 mlombard  (1000) mlombard  (1000)        0 2022-05-11 08:35:10.000000 rtslib-fb-2.1.75/
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)       38 2022-05-11 08:35:10.000000 rtslib-fb-2.1.75/setup.cfg
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)      430 2022-05-11 08:35:10.000000 rtslib-fb-2.1.75/PKG-INFO
--rwxrwxr-x   0 mlombard  (1000) mlombard  (1000)     1656 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/setup.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     1648 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/README.md
-drwxrwxr-x   0 mlombard  (1000) mlombard  (1000)        0 2022-05-11 08:35:10.000000 rtslib-fb-2.1.75/scripts/
--rwxrwxr-x   0 mlombard  (1000) mlombard  (1000)     2137 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/scripts/targetctl
-drwxrwxr-x   0 mlombard  (1000) mlombard  (1000)        0 2022-05-11 08:35:10.000000 rtslib-fb-2.1.75/rtslib_fb.egg-info/
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)       17 2022-05-11 08:35:09.000000 rtslib-fb-2.1.75/rtslib_fb.egg-info/top_level.txt
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)       19 2022-05-11 08:35:09.000000 rtslib-fb-2.1.75/rtslib_fb.egg-info/requires.txt
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)        1 2022-05-11 08:35:09.000000 rtslib-fb-2.1.75/rtslib_fb.egg-info/dependency_links.txt
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)      480 2022-05-11 08:35:09.000000 rtslib-fb-2.1.75/rtslib_fb.egg-info/SOURCES.txt
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)      430 2022-05-11 08:35:09.000000 rtslib-fb-2.1.75/rtslib_fb.egg-info/PKG-INFO
-drwxrwxr-x   0 mlombard  (1000) mlombard  (1000)        0 2022-05-11 08:35:10.000000 rtslib-fb-2.1.75/rtslib_fb/
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    16169 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib_fb/utils.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    38260 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib_fb/tcm.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    55507 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib_fb/target.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    20962 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib_fb/root.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     9630 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib_fb/node.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    18729 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib_fb/fabric.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    15637 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib_fb/alua.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     1585 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib_fb/__init__.py
-drwxrwxr-x   0 mlombard  (1000) mlombard  (1000)        0 2022-05-11 08:35:10.000000 rtslib-fb-2.1.75/rtslib/
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    16169 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib/utils.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    38260 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib/tcm.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    55507 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib/target.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    20962 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib/root.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     9630 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib/node.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    18729 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib/fabric.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)    15637 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib/alua.py
--rw-rw-r--   0 mlombard  (1000) mlombard  (1000)     1585 2022-05-11 08:33:52.000000 rtslib-fb-2.1.75/rtslib/__init__.py
+drwxr-xr-x   0 mlombard  (1000) mlombard  (1000)        0 2023-06-27 14:59:18.795119 rtslib-fb-2.1.76/
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    10143 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/COPYING
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)      452 2023-06-27 14:59:18.794119 rtslib-fb-2.1.76/PKG-INFO
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     1648 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/README.md
+drwxr-xr-x   0 mlombard  (1000) mlombard  (1000)        0 2023-06-27 14:59:18.791119 rtslib-fb-2.1.76/rtslib/
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     1585 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib/__init__.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    15637 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib/alua.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    18729 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib/fabric.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     9630 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib/node.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    20962 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib/root.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    55434 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib/target.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    38292 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib/tcm.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    16175 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib/utils.py
+drwxr-xr-x   0 mlombard  (1000) mlombard  (1000)        0 2023-06-27 14:59:18.793119 rtslib-fb-2.1.76/rtslib_fb/
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     1585 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib_fb/__init__.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    15637 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib_fb/alua.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    18729 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib_fb/fabric.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)     9630 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib_fb/node.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    20962 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib_fb/root.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    55434 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib_fb/target.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    38292 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib_fb/tcm.py
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)    16175 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/rtslib_fb/utils.py
+drwxr-xr-x   0 mlombard  (1000) mlombard  (1000)        0 2023-06-27 14:59:18.794119 rtslib-fb-2.1.76/rtslib_fb.egg-info/
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)      452 2023-06-27 14:59:18.000000 rtslib-fb-2.1.76/rtslib_fb.egg-info/PKG-INFO
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)      488 2023-06-27 14:59:18.000000 rtslib-fb-2.1.76/rtslib_fb.egg-info/SOURCES.txt
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)        1 2023-06-27 14:59:18.000000 rtslib-fb-2.1.76/rtslib_fb.egg-info/dependency_links.txt
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)       19 2023-06-27 14:59:18.000000 rtslib-fb-2.1.76/rtslib_fb.egg-info/requires.txt
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)       17 2023-06-27 14:59:18.000000 rtslib-fb-2.1.76/rtslib_fb.egg-info/top_level.txt
+drwxr-xr-x   0 mlombard  (1000) mlombard  (1000)        0 2023-06-27 14:59:18.794119 rtslib-fb-2.1.76/scripts/
+-rwxr-xr-x   0 mlombard  (1000) mlombard  (1000)     2137 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/scripts/targetctl
+-rw-r--r--   0 mlombard  (1000) mlombard  (1000)       38 2023-06-27 14:59:18.795119 rtslib-fb-2.1.76/setup.cfg
+-rwxr-xr-x   0 mlombard  (1000) mlombard  (1000)     1671 2023-06-27 14:56:59.000000 rtslib-fb-2.1.76/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rtslib-fb-2.1.75/setup.py` & `rtslib-fb-2.1.76/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools import setup
 
 # Get version without importing.
 init_file_path = os.path.join(os.path.dirname(__file__), 'rtslib/__init__.py')
 
 with open(init_file_path) as f:
     for line in f:
-        match = re.match(r"__version__.*'([0-9.]+)'", line)
+        match = re.match(r"__version__.*'([0-9.]+)(\.g[0-9a-f]+)?'", line)
         if match:
             version = match.group(1)
             break
     else:
         raise Exception("Couldn't find version in setup.py")
 
 setup (
```

### Comparing `rtslib-fb-2.1.75/README.md` & `rtslib-fb-2.1.76/README.md`

 * *Files identical despite different names*

### Comparing `rtslib-fb-2.1.75/scripts/targetctl` & `rtslib-fb-2.1.76/scripts/targetctl`

 * *Files identical despite different names*

### Comparing `rtslib-fb-2.1.75/rtslib_fb/utils.py` & `rtslib-fb-2.1.76/rtslib/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
     '''
     wwn_test = {
     'free': lambda wwn: True,
     'iqn': lambda wwn: \
         re.match(r"iqn\.[0-9]{4}-[0-1][0-9]\..*\..*", wwn) \
         and not re.search(' ', wwn) \
         and not re.search('_', wwn),
-    'naa': lambda wwn: re.match(r"naa\.[125][0-9a-fA-F]{15}$", wwn),
+    'naa': lambda wwn: re.match(r"naa\.[125c-fC-F][0-9a-fA-F]{15}$", wwn),
     'eui': lambda wwn: re.match(r"eui\.[0-9a-f]{16}$", wwn),
     'ib': lambda wwn: re.match(r"ib\.[0-9a-f]{32}$", wwn),
     'unit_serial': lambda wwn: \
         re.match("[0-9A-Fa-f]{8}(-[0-9A-Fa-f]{4}){3}-[0-9A-Fa-f]{12}$", wwn),
     }
 
     for wwn_type in wwn_types:
```

### Comparing `rtslib-fb-2.1.75/rtslib_fb/tcm.py` & `rtslib-fb-2.1.76/rtslib/tcm.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,14 @@
 from .node import CFSNode
 from .utils import fread, fwrite, generate_wwn, RTSLibError, RTSLibNotInCFS
 from .utils import convert_scsi_path_to_hctl, convert_scsi_hctl_to_path
 from .utils import is_dev_in_use, get_blockdev_type
 from .utils import get_size_for_blk_dev, get_size_for_disk_name
 
 lock_file = '/var/run/rtslib_backstore.lock'
-if not os.path.exists('/var/run'):
-    os.makedirs('/var/run')
 
 def storage_object_get_alua_support_attr(so):
     '''
     Helper function that can be called by passthrough type of backends.
     '''
     try:
         if int(so.get_attribute("alua_support")) == 1:
@@ -997,14 +995,16 @@
 
         if self._index == None:
             if mode == 'lookup':
                 raise RTSLibNotInCFS("Storage object %s/%s not found" %
                                      (self._plugin, name))
             else:
                 # Allocate new index value
+                if not os.path.exists('/var/run'):
+                    os.makedirs('/var/run')
                 lkfd = open(lock_file, 'w+')
                 fcntl.flock(lkfd, fcntl.LOCK_EX)
                 indexes = set(bs_cache.values())
                 for index in range(1048576):
                     if index not in indexes:
                         self._index = index
                         bs_cache[self._lookup_key] = self._index
```

### Comparing `rtslib-fb-2.1.75/rtslib_fb/target.py` & `rtslib-fb-2.1.76/rtslib/target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1056,16 +1056,14 @@
     This is an interface to RTS Target Mapped LUNs.
     A MappedLUN is a mapping of a TPG LUN to a specific initiator node, and is
     part of a NodeACL. It allows the initiator to actually access the TPG LUN
     if ACLs are enabled for the TPG. The initial TPG LUN will then be seen by
     the initiator node as the MappedLUN.
     '''
 
-    MAX_LUN = 255
-
     # MappedLUN private stuff
 
     def __repr__(self):
         return "<MappedLUN %s lun %d -> tpg%d lun %d>" % \
             (self.parent_nodeacl.node_wwn, self.mapped_lun,
              self.parent_nodeacl.parent_tpg.tag, self.tpg_lun.lun)
 
@@ -1104,17 +1102,16 @@
                 raise RTSLibError("The parent_nodeacl does not exist")
 
         try:
             self._mapped_lun = int(mapped_lun)
         except ValueError:
             raise RTSLibError("The mapped_lun parameter must be an " \
                               + "integer value")
-
-        if self._mapped_lun < 0 or self._mapped_lun > self.MAX_LUN:
-            raise RTSLibError("Mapped LUN must be 0 to %d" % self.MAX_LUN)
+        if self._mapped_lun < 0:
+            raise RTSLibError("Mapped LUN must be >= 0")
 
         self._path = "%s/lun_%d" % (self.parent_nodeacl.path, self.mapped_lun)
 
         if tpg_lun is None and write_protect is not None:
             raise RTSLibError("The write_protect parameter has no " \
                               + "meaning without the tpg_lun parameter")
```

### Comparing `rtslib-fb-2.1.75/rtslib_fb/root.py` & `rtslib-fb-2.1.76/rtslib/root.py`

 * *Files identical despite different names*

### Comparing `rtslib-fb-2.1.75/rtslib_fb/node.py` & `rtslib-fb-2.1.76/rtslib/node.py`

 * *Files identical despite different names*

### Comparing `rtslib-fb-2.1.75/rtslib_fb/fabric.py` & `rtslib-fb-2.1.76/rtslib/fabric.py`

 * *Files identical despite different names*

### Comparing `rtslib-fb-2.1.75/rtslib_fb/alua.py` & `rtslib-fb-2.1.76/rtslib/alua.py`

 * *Files identical despite different names*

### Comparing `rtslib-fb-2.1.75/rtslib_fb/__init__.py` & `rtslib-fb-2.1.76/rtslib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,12 +32,12 @@
 
 from .tcm import FileIOStorageObject, BlockStorageObject
 from .tcm import PSCSIStorageObject, RDMCPStorageObject, UserBackedStorageObject
 from .tcm import StorageObjectFactory
 
 from .alua import ALUATargetPortGroup
 
-__version__ = '2.1.75'
+__version__ = '2.1.76'
 __author__ = "Jerome Martin <jxm@risingtidesystems.com>"
 __url__ = 'http://github.com/open-iscsi/rtslib-fb'
 __description__ = 'API for Linux kernel SCSI target (aka LIO)'
 __license__ = 'Apache 2.0'
```

### Comparing `rtslib-fb-2.1.75/rtslib/utils.py` & `rtslib-fb-2.1.76/rtslib_fb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
     '''
     wwn_test = {
     'free': lambda wwn: True,
     'iqn': lambda wwn: \
         re.match(r"iqn\.[0-9]{4}-[0-1][0-9]\..*\..*", wwn) \
         and not re.search(' ', wwn) \
         and not re.search('_', wwn),
-    'naa': lambda wwn: re.match(r"naa\.[125][0-9a-fA-F]{15}$", wwn),
+    'naa': lambda wwn: re.match(r"naa\.[125c-fC-F][0-9a-fA-F]{15}$", wwn),
     'eui': lambda wwn: re.match(r"eui\.[0-9a-f]{16}$", wwn),
     'ib': lambda wwn: re.match(r"ib\.[0-9a-f]{32}$", wwn),
     'unit_serial': lambda wwn: \
         re.match("[0-9A-Fa-f]{8}(-[0-9A-Fa-f]{4}){3}-[0-9A-Fa-f]{12}$", wwn),
     }
 
     for wwn_type in wwn_types:
```

### Comparing `rtslib-fb-2.1.75/rtslib/tcm.py` & `rtslib-fb-2.1.76/rtslib_fb/tcm.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,14 @@
 from .node import CFSNode
 from .utils import fread, fwrite, generate_wwn, RTSLibError, RTSLibNotInCFS
 from .utils import convert_scsi_path_to_hctl, convert_scsi_hctl_to_path
 from .utils import is_dev_in_use, get_blockdev_type
 from .utils import get_size_for_blk_dev, get_size_for_disk_name
 
 lock_file = '/var/run/rtslib_backstore.lock'
-if not os.path.exists('/var/run'):
-    os.makedirs('/var/run')
 
 def storage_object_get_alua_support_attr(so):
     '''
     Helper function that can be called by passthrough type of backends.
     '''
     try:
         if int(so.get_attribute("alua_support")) == 1:
@@ -997,14 +995,16 @@
 
         if self._index == None:
             if mode == 'lookup':
                 raise RTSLibNotInCFS("Storage object %s/%s not found" %
                                      (self._plugin, name))
             else:
                 # Allocate new index value
+                if not os.path.exists('/var/run'):
+                    os.makedirs('/var/run')
                 lkfd = open(lock_file, 'w+')
                 fcntl.flock(lkfd, fcntl.LOCK_EX)
                 indexes = set(bs_cache.values())
                 for index in range(1048576):
                     if index not in indexes:
                         self._index = index
                         bs_cache[self._lookup_key] = self._index
```

### Comparing `rtslib-fb-2.1.75/rtslib/target.py` & `rtslib-fb-2.1.76/rtslib_fb/target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1056,16 +1056,14 @@
     This is an interface to RTS Target Mapped LUNs.
     A MappedLUN is a mapping of a TPG LUN to a specific initiator node, and is
     part of a NodeACL. It allows the initiator to actually access the TPG LUN
     if ACLs are enabled for the TPG. The initial TPG LUN will then be seen by
     the initiator node as the MappedLUN.
     '''
 
-    MAX_LUN = 255
-
     # MappedLUN private stuff
 
     def __repr__(self):
         return "<MappedLUN %s lun %d -> tpg%d lun %d>" % \
             (self.parent_nodeacl.node_wwn, self.mapped_lun,
              self.parent_nodeacl.parent_tpg.tag, self.tpg_lun.lun)
 
@@ -1104,17 +1102,16 @@
                 raise RTSLibError("The parent_nodeacl does not exist")
 
         try:
             self._mapped_lun = int(mapped_lun)
         except ValueError:
             raise RTSLibError("The mapped_lun parameter must be an " \
                               + "integer value")
-
-        if self._mapped_lun < 0 or self._mapped_lun > self.MAX_LUN:
-            raise RTSLibError("Mapped LUN must be 0 to %d" % self.MAX_LUN)
+        if self._mapped_lun < 0:
+            raise RTSLibError("Mapped LUN must be >= 0")
 
         self._path = "%s/lun_%d" % (self.parent_nodeacl.path, self.mapped_lun)
 
         if tpg_lun is None and write_protect is not None:
             raise RTSLibError("The write_protect parameter has no " \
                               + "meaning without the tpg_lun parameter")
```

### Comparing `rtslib-fb-2.1.75/rtslib/root.py` & `rtslib-fb-2.1.76/rtslib_fb/root.py`

 * *Files identical despite different names*

### Comparing `rtslib-fb-2.1.75/rtslib/node.py` & `rtslib-fb-2.1.76/rtslib_fb/node.py`

 * *Files identical despite different names*

### Comparing `rtslib-fb-2.1.75/rtslib/fabric.py` & `rtslib-fb-2.1.76/rtslib_fb/fabric.py`

 * *Files identical despite different names*

### Comparing `rtslib-fb-2.1.75/rtslib/alua.py` & `rtslib-fb-2.1.76/rtslib_fb/alua.py`

 * *Files identical despite different names*

### Comparing `rtslib-fb-2.1.75/rtslib/__init__.py` & `rtslib-fb-2.1.76/rtslib_fb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,12 +32,12 @@
 
 from .tcm import FileIOStorageObject, BlockStorageObject
 from .tcm import PSCSIStorageObject, RDMCPStorageObject, UserBackedStorageObject
 from .tcm import StorageObjectFactory
 
 from .alua import ALUATargetPortGroup
 
-__version__ = '2.1.75'
+__version__ = '2.1.76'
 __author__ = "Jerome Martin <jxm@risingtidesystems.com>"
 __url__ = 'http://github.com/open-iscsi/rtslib-fb'
 __description__ = 'API for Linux kernel SCSI target (aka LIO)'
 __license__ = 'Apache 2.0'
```

