# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.921.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.921.tar", last modified: Mon Jun 26 00:21:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.922.tar", last modified: Tue Jun 27 00:22:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.921.tar` & `tencentcloud-sdk-python-cynosdb-3.0.922.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   415832 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)   118494 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)    11095 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-26 00:21:54.000000 tencentcloud-sdk-python-cynosdb-3.0.921/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-26 00:21:53.000000 tencentcloud-sdk-python-cynosdb-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   415832 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)   118494 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    11292 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-27 00:22:18.000000 tencentcloud-sdk-python-cynosdb-3.0.922/setup.py
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/cynosdb/v20190107/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 # 创建资源包失败
 FAILEDOPERATION_CREATESOURCEPACKAGEERROR = 'FailedOperation.CreateSourcePackageError'
 
 # 数据库访问失败，请稍后重试。如果持续不成功，请联系客服进行处理。
 FAILEDOPERATION_DATABASEACCESSERROR = 'FailedOperation.DatabaseAccessError'
 
+# 修改账号权限失败。
+FAILEDOPERATION_DESCRIBEACCOUNTPRIVILEGESERROR = 'FailedOperation.DescribeAccountPrivilegesError'
+
 # 创建流程失败，请稍后重试。如果持续不成功，请联系客服进行处理。
 FAILEDOPERATION_FLOWCREATEERROR = 'FailedOperation.FlowCreateError'
 
 # Flow不存在。
 FAILEDOPERATION_FLOWNOTFOUNDERROR = 'FailedOperation.FlowNotFoundError'
 
 # 获取备份策略失败，请稍后重试。如果持续不成功，请联系客服进行处理。
@@ -91,14 +94,17 @@
 
 # 获取子网失败。
 INTERNALERROR_GETSUBNETFAILED = 'InternalError.GetSubnetFailed'
 
 # 获取VPC失败。
 INTERNALERROR_GETVPCFAILED = 'InternalError.GetVpcFailed'
 
+# 网络错误
+INTERNALERROR_HTTPERROR = 'InternalError.HttpError'
+
 # http请求执行异常。
 INTERNALERROR_INTERNALHTTPSERVERERROR = 'InternalError.InternalHttpServerError'
 
 # 安全组查询实例失败。
 INTERNALERROR_LISTINSTANCEFAILED = 'InternalError.ListInstanceFailed'
 
 # 操作外网失败。
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.921/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.922/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.921/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.922/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.921/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.922/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.921/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.922/setup.py`

 * *Files identical despite different names*

