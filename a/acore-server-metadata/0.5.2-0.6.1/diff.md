# Comparing `tmp/acore_server_metadata-0.5.2.tar.gz` & `tmp/acore_server_metadata-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.5.2.tar", last modified: Mon Jun 26 05:28:01 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.6.1.tar", last modified: Tue Jun 27 20:24:04 2023, max compression
```

## Comparing `acore_server_metadata-0.5.2.tar` & `acore_server_metadata-0.6.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.087415 acore_server_metadata-0.5.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     7052 2023-06-26 05:28:01.087251 acore_server_metadata-0.5.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5903 2023-06-26 05:13:50.000000 acore_server_metadata-0.5.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.081349 acore_server_metadata-0.5.2/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.5.2/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-26 05:13:00.000000 acore_server_metadata-0.5.2/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      105 2023-06-22 16:18:25.000000 acore_server_metadata-0.5.2/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.082321 acore_server_metadata-0.5.2/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.5.2/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.083968 acore_server_metadata-0.5.2/acore_server_metadata/server/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-22 14:16:00.000000 acore_server_metadata-0.5.2/acore_server_metadata/server/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-22 15:54:39.000000 acore_server_metadata-0.5.2/acore_server_metadata/server/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12104 2023-06-26 05:15:51.000000 acore_server_metadata-0.5.2/acore_server_metadata/server/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17223 2023-06-26 05:15:47.000000 acore_server_metadata-0.5.2/acore_server_metadata/server/server_operation.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1665 2023-06-22 15:56:21.000000 acore_server_metadata-0.5.2/acore_server_metadata/server/server_status.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      270 2023-06-26 05:12:13.000000 acore_server_metadata-0.5.2/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.084709 acore_server_metadata-0.5.2/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.5.2/acore_server_metadata/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      479 2023-06-22 15:28:39.000000 acore_server_metadata-0.5.2/acore_server_metadata/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.085964 acore_server_metadata-0.5.2/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.5.2/acore_server_metadata/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.082191 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     7052 2023-06-26 05:28:01.000000 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1187 2023-06-26 05:28:01.000000 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-26 05:28:01.000000 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      272 2023-06-26 05:28:01.000000 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-26 05:28:01.000000 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     4747 2023-06-26 05:15:20.000000 acore_server_metadata-0.5.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.5.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      118 2023-06-26 05:08:10.000000 acore_server_metadata-0.5.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-26 05:28:01.087469 acore_server_metadata-0.5.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.086785 acore_server_metadata-0.5.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.5.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     8043 2023-06-26 05:11:16.000000 acore_server_metadata-0.5.2/tests/test_server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-06-22 15:33:22.000000 acore_server_metadata-0.5.2/tests/test_utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 20:24:04.254797 acore_server_metadata-0.6.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7052 2023-06-27 20:24:04.254652 acore_server_metadata-0.6.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5903 2023-06-26 05:13:50.000000 acore_server_metadata-0.6.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 20:24:04.249852 acore_server_metadata-0.6.1/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.6.1/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-27 20:15:54.000000 acore_server_metadata-0.6.1/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      153 2023-06-27 20:14:17.000000 acore_server_metadata-0.6.1/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 20:24:04.250919 acore_server_metadata-0.6.1/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.6.1/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/acore_server_metadata/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 20:24:04.252369 acore_server_metadata-0.6.1/acore_server_metadata/server/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-22 14:16:00.000000 acore_server_metadata-0.6.1/acore_server_metadata/server/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-22 15:54:39.000000 acore_server_metadata-0.6.1/acore_server_metadata/server/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13373 2023-06-27 20:14:01.000000 acore_server_metadata-0.6.1/acore_server_metadata/server/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17223 2023-06-26 05:15:47.000000 acore_server_metadata-0.6.1/acore_server_metadata/server/server_operation.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1665 2023-06-22 15:56:21.000000 acore_server_metadata-0.6.1/acore_server_metadata/server/server_status.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      270 2023-06-26 05:12:13.000000 acore_server_metadata-0.6.1/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 20:24:04.253041 acore_server_metadata-0.6.1/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.6.1/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      745 2023-06-27 20:10:16.000000 acore_server_metadata-0.6.1/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 20:24:04.253679 acore_server_metadata-0.6.1/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.6.1/acore_server_metadata/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 20:24:04.250786 acore_server_metadata-0.6.1/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7052 2023-06-27 20:24:04.000000 acore_server_metadata-0.6.1/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1187 2023-06-27 20:24:04.000000 acore_server_metadata-0.6.1/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-27 20:24:04.000000 acore_server_metadata-0.6.1/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      272 2023-06-27 20:24:04.000000 acore_server_metadata-0.6.1/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-27 20:24:04.000000 acore_server_metadata-0.6.1/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4894 2023-06-27 20:19:56.000000 acore_server_metadata-0.6.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.6.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      118 2023-06-27 20:06:13.000000 acore_server_metadata-0.6.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-27 20:24:04.254848 acore_server_metadata-0.6.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.6.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 20:24:04.254214 acore_server_metadata-0.6.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1233 2023-06-27 20:14:43.000000 acore_server_metadata-0.6.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8043 2023-06-26 05:11:16.000000 acore_server_metadata-0.6.1/tests/test_server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-06-22 15:33:22.000000 acore_server_metadata-0.6.1/tests/test_utils.py
```

### Comparing `acore_server_metadata-0.5.2/AUTHORS.rst` & `acore_server_metadata-0.6.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/LICENSE.txt` & `acore_server_metadata-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/PKG-INFO` & `acore_server_metadata-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_metadata
-Version: 0.5.2
+Version: 0.6.1
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.5.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.6.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.5.2/README.rst` & `acore_server_metadata-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/acore_server_metadata/paths.py` & `acore_server_metadata-0.6.1/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/acore_server_metadata/server/server.py` & `acore_server_metadata-0.6.1/acore_server_metadata/server/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import typing as T
 import dataclasses
 
 from simple_aws_ec2.api import Ec2Instance, EC2InstanceStatusEnum
 from simple_aws_rds.api import RDSDBInstance, RDSDBInstanceStatusEnum
 from acore_constants.api import TagKey
 
-from ..utils import group_by
+from ..utils import group_by, get_boto_ses_from_ec2_inside
 from ..exc import (
     ServerNotUniqueError,
 )
 
 from .server_status import ServerStatusMixin
 from .server_operation import ServerOperationMixin
 
@@ -197,20 +197,52 @@
             raise ServerNotUniqueError(f"Found multiple RDS instance with id {id}")
         elif len(rds_inst_list) == 0:
             return None
         else:
             return rds_inst_list[0]
 
     @classmethod
+    def from_ec2_inside(
+        cls,
+        ec2_client = None,
+        rds_client = None,
+    ) -> "Server":  # pragma: no cover
+        """
+        用 "自省" 的方式, 从 EC2 实例内部通过 metadata API 获得自己的 instance id,
+        进而获得 Server 的 metadata. 如果这台 EC2 不是一个魔兽世界服务器, 那么将会抛出异常.
+
+        :param ec2_client: optional EC2 client, if not given, will automatically
+            create on using EC2 IAM role.
+        :param rds_client: optional RDS client, if not given, will automatically
+            create on using EC2 IAM role.
+        """
+        boto_ses = None
+        if ec2_client is None:
+            boto_ses = get_boto_ses_from_ec2_inside()
+            ec2_client = boto_ses.client("ec2")
+        if rds_client is None:
+            if boto_ses is None:
+                boto_ses = get_boto_ses_from_ec2_inside()
+            rds_client = boto_ses.client("rds")
+        ec2_inst = Ec2Instance.from_ec2_inside(ec2_client)
+        server_id = ec2_inst.tags[TagKey.SERVER_ID]
+        rds_inst = cls.get_rds(rds_client, server_id)
+        return cls(
+            id=server_id,
+            ec2_inst=ec2_inst,
+            rds_inst=rds_inst,
+        )
+
+    @classmethod
     def get_server(
         cls,
         id: str,
         ec2_client,
         rds_client,
-    ) -> T.Optional["Server"]:
+    ) -> "Server":
         """
         尝试获得某个 Server 的 EC2 和 RDS 信息. 这个方法会同时调用 :meth:`Server.get_ec2`
         和 :meth:`Server.get_rds`. 无论 EC2 还是 RDS 存不存在, 它都会返回一个 :class:`Server`
         对象. 如果 EC2 或 RDS 不存在, 那么 ``.ec2_inst`` 或 ``.rds_inst`` 属性的值可能是 None.
         关于 "不存在" 的定义请参考 :meth:`Server.get_ec2` 和 :meth:`Server.get_rds`.
 
         该方法是本模块最常用的方法之一. 用例如下:
```

### Comparing `acore_server_metadata-0.5.2/acore_server_metadata/server/server_operation.py` & `acore_server_metadata-0.6.1/acore_server_metadata/server/server_operation.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/acore_server_metadata/server/server_status.py` & `acore_server_metadata-0.6.1/acore_server_metadata/server/server_status.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.6.1/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/acore_server_metadata/vendor/hashes.py` & `acore_server_metadata-0.6.1/acore_server_metadata/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.6.1/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.6.1/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-metadata
-Version: 0.5.2
+Version: 0.6.1
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.5.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.6.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.5.2/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.6.1/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/release-history.rst` & `acore_server_metadata-0.6.1/release-history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
-x.y.z (Backlog)
+0.6.1 (2023-06-27)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
-**Minor Improvements**
-
-**Bugfixes**
+- add the following public API:
+    - ``acore_server_metadata.api.Server.from_ec2_inside``
+    - ``acore_server_metadata.api.get_boto_ses_from_ec2_inside``
 
 **Miscellaneous**
 
+- upgrade dependencies.
+
 
 0.5.2 (2023-06-26)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - ``acore_server_metadata.settings`` module is not in used anymore. It is kept for backward compatibility. Now we use `acore_constants <https://github.com/MacHu-GWU/acore_constants-project>`_ library to define constants.
```

### Comparing `acore_server_metadata-0.5.2/requirements-doc.txt` & `acore_server_metadata-0.6.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/setup.py` & `acore_server_metadata-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/tests/test_api.py` & `acore_server_metadata-0.6.1/tests/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 
 def test():
     _ = api
 
     # top level API
     _ = api.exc
+    _ = api.get_boto_ses_from_ec2_inside
     _ = api.settings
     _ = api.Server
 
     # attribute and method
     _ = api.exc.ServerNotFoundError
     _ = api.exc.ServerNotUniqueError
 
     _ = api.Server.get_ec2
     _ = api.Server.get_rds
+    _ = api.Server.from_ec2_inside
     _ = api.Server.get_server
     _ = api.Server.batch_get_server
     _ = api.Server.is_exists
     _ = api.Server.is_running
     _ = api.Server.is_ec2_exists
     _ = api.Server.is_ec2_running
     _ = api.Server.is_rds_exists
```

### Comparing `acore_server_metadata-0.5.2/tests/test_server.py` & `acore_server_metadata-0.6.1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.2/tests/test_utils.py` & `acore_server_metadata-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

