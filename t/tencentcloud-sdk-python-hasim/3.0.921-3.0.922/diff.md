# Comparing `tmp/tencentcloud-sdk-python-hasim-3.0.921.tar.gz` & `tmp/tencentcloud-sdk-python-hasim-3.0.922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hasim-3.0.921.tar", last modified: Mon Jun 26 00:25:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hasim-3.0.922.tar", last modified: Tue Jun 27 00:25:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-hasim-3.0.921.tar` & `tencentcloud-sdk-python-hasim-3.0.922.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/hasim/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/hasim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/hasim/v20210716/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/hasim/v20210716/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76088 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/hasim/v20210716/models.py
--rw-r--r--   0 root         (0) root         (0)    19634 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/hasim/v20210716/hasim_client.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/hasim/v20210716/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/README.rst
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud_sdk_python_hasim.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud_sdk_python_hasim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud_sdk_python_hasim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud_sdk_python_hasim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:25:30.000000 tencentcloud-sdk-python-hasim-3.0.921/tencentcloud_sdk_python_hasim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/hasim/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/hasim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/hasim/v20210716/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/hasim/v20210716/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76088 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/hasim/v20210716/models.py
+-rw-r--r--   0 root         (0) root         (0)    19634 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/hasim/v20210716/hasim_client.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/hasim/v20210716/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud_sdk_python_hasim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud_sdk_python_hasim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud_sdk_python_hasim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud_sdk_python_hasim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 00:25:57.000000 tencentcloud-sdk-python-hasim-3.0.922/tencentcloud_sdk_python_hasim.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/hasim/v20210716/models.py` & `tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/hasim/v20210716/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/hasim/v20210716/hasim_client.py` & `tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/hasim/v20210716/hasim_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hasim-3.0.921/tencentcloud/hasim/v20210716/errorcodes.py` & `tencentcloud-sdk-python-hasim-3.0.922/tencentcloud/hasim/v20210716/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hasim-3.0.921/README.rst` & `tencentcloud-sdk-python-hasim-3.0.922/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hasim-3.0.921/PKG-INFO` & `tencentcloud-sdk-python-hasim-3.0.922/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hasim
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Hasim SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hasim-3.0.921/setup.py` & `tencentcloud-sdk-python-hasim-3.0.922/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hasim-3.0.921/tencentcloud_sdk_python_hasim.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hasim-3.0.922/tencentcloud_sdk_python_hasim.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hasim
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Hasim SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

