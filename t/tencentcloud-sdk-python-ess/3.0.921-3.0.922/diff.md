# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.921.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.921.tar", last modified: Mon Jun 26 00:24:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.922.tar", last modified: Tue Jun 27 00:24:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.921.tar` & `tencentcloud-sdk-python-ess-3.0.922.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   258602 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)    59451 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24756 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-26 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   258602 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)    59451 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24834 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-27 00:24:35.000000 tencentcloud-sdk-python-ess-3.0.922/setup.py
```

### Comparing `tencentcloud-sdk-python-ess-3.0.921/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.922/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.922/tencentcloud/ess/v20201111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.922/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.921/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.922/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,14 +457,17 @@
 
 # 签署人年龄限制无法使用电子签服务。
 OPERATIONDENIED_INVALIDAPPROVERAGE = 'OperationDenied.InvalidApproverAge'
 
 # 资源id超过使用上限限制，请联系客服了解规则，并在修改后重试。
 OPERATIONDENIED_MANYRESOURCEID = 'OperationDenied.ManyResourceId'
 
+# 没有API权限。
+OPERATIONDENIED_NOAPIAUTH = 'OperationDenied.NoApiAuth'
+
 # 无权限操作签署流程，请联系客服了解权限，并在修改后重试。
 OPERATIONDENIED_NOFLOWPERMISSION = 'OperationDenied.NoFlowPermission'
 
 # 未通过个人实名认证。
 OPERATIONDENIED_NOIDENTITYVERIFY = 'OperationDenied.NoIdentityVerify'
 
 # 用户未登录,请先登录后再操作。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.921/README.rst` & `tencentcloud-sdk-python-ess-3.0.922/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.921/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.922/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.921/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.922/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.921/setup.py` & `tencentcloud-sdk-python-ess-3.0.922/setup.py`

 * *Files identical despite different names*

