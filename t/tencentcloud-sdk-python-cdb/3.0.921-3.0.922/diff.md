# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.921.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.921.tar", last modified: Mon Jun 26 00:18:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.922.tar", last modified: Tue Jun 27 00:19:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.921.tar` & `tencentcloud-sdk-python-cdb-3.0.922.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/cdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/cdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   151510 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)   528803 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)    18943 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-26 00:18:50.000000 tencentcloud-sdk-python-cdb-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/cdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/cdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   151510 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)   528885 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)    19040 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-27 00:19:21.000000 tencentcloud-sdk-python-cdb-3.0.922/setup.py
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.921/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.922/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.921'
+__version__ = '3.0.922'
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -11797,17 +11797,17 @@
         r"""
         :param InstanceId: 实例ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceId: str
         :param InstanceName: 实例名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceName: str
-        :param InstanceType: 实例类型
+        :param InstanceType: 实例类型：1 master 主实例; 2 ro 只读实例; 3 dr 灾备实例; 4 sdr 小灾备实例
 注意：此字段可能返回 null，表示取不到有效值。
-        :type InstanceType: str
+        :type InstanceType: int
         :param Status: 实例状态，可能的返回值：0-创建中；1-运行中；4-隔离中；5-已隔离
 注意：此字段可能返回 null，表示取不到有效值。
         :type Status: int
         :param Weight: 只读权重,如果权重为系统自动分配，改值不生效，只代表是否启用该实例
 注意：此字段可能返回 null，表示取不到有效值。
         :type Weight: int
         :param Region: 实例所属地域
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.921/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.922/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,14 +463,17 @@
 
 # 基础版实例不支持当前操作（功能）。
 OPERATIONDENIED_NOTSUPPORTBASIC = 'OperationDenied.NotSupportBasic'
 
 # 不支持修改本地root账号host信息。
 OPERATIONDENIED_NOTSUPPORTMODIFYLOCALROOTHOSTERROR = 'OperationDenied.NotSupportModifyLocalRootHostError'
 
+# 操作拒绝。
+OPERATIONDENIED_OPERATIONDENIEDERROR = 'OperationDenied.OperationDeniedError'
+
 # 当前有其他订单正在处于下单过程中，请稍后重试。
 OPERATIONDENIED_OTHERODERINPROCESS = 'OperationDenied.OtherOderInProcess'
 
 # 资源配额超限。
 OPERATIONDENIED_OVERQUOTA = 'OperationDenied.OverQuota'
 
 # 代理地址超限。
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.921/README.rst` & `tencentcloud-sdk-python-cdb-3.0.922/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.921/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.922/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.921/setup.py` & `tencentcloud-sdk-python-cdb-3.0.922/setup.py`

 * *Files identical despite different names*

