# Comparing `tmp/tencentcloud-sdk-python-antiddos-3.0.921.tar.gz` & `tmp/tencentcloud-sdk-python-antiddos-3.0.922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.921.tar", last modified: Mon Jun 26 00:15:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.922.tar", last modified: Tue Jun 27 00:16:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-antiddos-3.0.921.tar` & `tencentcloud-sdk-python-antiddos-3.0.922.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/antiddos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/antiddos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/antiddos/v20200309/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/antiddos/v20200309/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316964 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/antiddos/v20200309/models.py
--rw-r--r--   0 root         (0) root         (0)    88167 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/antiddos/v20200309/antiddos_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/antiddos/v20200309/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/README.rst
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud_sdk_python_antiddos.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-26 00:15:49.000000 tencentcloud-sdk-python-antiddos-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/antiddos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/antiddos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/antiddos/v20200309/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/antiddos/v20200309/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   317473 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/antiddos/v20200309/models.py
+-rw-r--r--   0 root         (0) root         (0)    88167 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/antiddos/v20200309/antiddos_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/antiddos/v20200309/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud_sdk_python_antiddos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-27 00:16:31.000000 tencentcloud-sdk-python-antiddos-3.0.922/setup.py
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/__init__.py` & `tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/antiddos/v20200309/models.py` & `tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/antiddos/v20200309/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,14 +573,17 @@
         :param ElasticServiceBandwidth: 弹性业务带宽开关
         :type ElasticServiceBandwidth: int
         :param GiftServiceBandWidth: 赠送的业务带宽
         :type GiftServiceBandWidth: int
         :param ModifyTime: 修改时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type ModifyTime: str
+        :param BasicPlusFlag: 是否是基础防护加强版 0: 不是 1: 是
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BasicPlusFlag: int
         """
         self.InstanceDetail = None
         self.SpecificationLimit = None
         self.Usage = None
         self.Region = None
         self.Status = None
         self.CreatedTime = None
@@ -594,14 +597,15 @@
         self.TagInfoList = None
         self.IpCountNewFlag = None
         self.VitalityVersion = None
         self.Line = None
         self.ElasticServiceBandwidth = None
         self.GiftServiceBandWidth = None
         self.ModifyTime = None
+        self.BasicPlusFlag = None
 
 
     def _deserialize(self, params):
         if params.get("InstanceDetail") is not None:
             self.InstanceDetail = InstanceRelation()
             self.InstanceDetail._deserialize(params.get("InstanceDetail"))
         if params.get("SpecificationLimit") is not None:
@@ -637,14 +641,15 @@
                 self.TagInfoList.append(obj)
         self.IpCountNewFlag = params.get("IpCountNewFlag")
         self.VitalityVersion = params.get("VitalityVersion")
         self.Line = params.get("Line")
         self.ElasticServiceBandwidth = params.get("ElasticServiceBandwidth")
         self.GiftServiceBandWidth = params.get("GiftServiceBandWidth")
         self.ModifyTime = params.get("ModifyTime")
+        self.BasicPlusFlag = params.get("BasicPlusFlag")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4945,14 +4950,16 @@
         :type FilterTrialFlag: int
         :param FilterConvoy: 重保护航搜索
         :type FilterConvoy: int
         :param ExcludeAdvancedInfo: 默认false；接口传true，返回数据中不包含高级信息，高级信息包含：InstanceList[0].Usage。
         :type ExcludeAdvancedInfo: bool
         :param FilterAssetIpList: 资产IP数组
         :type FilterAssetIpList: list of str
+        :param FilterBasicPlusFlag: 是否包含基础防护增强版 0: 不包含 1: 包含
+        :type FilterBasicPlusFlag: int
         """
         self.Offset = None
         self.Limit = None
         self.FilterIp = None
         self.FilterInstanceId = None
         self.FilterRegion = None
         self.FilterName = None
@@ -4964,14 +4971,15 @@
         self.FilterLightFlag = None
         self.FilterChannelFlag = None
         self.FilterTag = None
         self.FilterTrialFlag = None
         self.FilterConvoy = None
         self.ExcludeAdvancedInfo = None
         self.FilterAssetIpList = None
+        self.FilterBasicPlusFlag = None
 
 
     def _deserialize(self, params):
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
         self.FilterIp = params.get("FilterIp")
         self.FilterInstanceId = params.get("FilterInstanceId")
@@ -4987,14 +4995,15 @@
         if params.get("FilterTag") is not None:
             self.FilterTag = TagFilter()
             self.FilterTag._deserialize(params.get("FilterTag"))
         self.FilterTrialFlag = params.get("FilterTrialFlag")
         self.FilterConvoy = params.get("FilterConvoy")
         self.ExcludeAdvancedInfo = params.get("ExcludeAdvancedInfo")
         self.FilterAssetIpList = params.get("FilterAssetIpList")
+        self.FilterBasicPlusFlag = params.get("FilterBasicPlusFlag")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/antiddos/v20200309/antiddos_client.py` & `tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/antiddos/v20200309/antiddos_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud/antiddos/v20200309/errorcodes.py` & `tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud/antiddos/v20200309/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.921/README.rst` & `tencentcloud-sdk-python-antiddos-3.0.922/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.921/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.922/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.921/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.922/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.921/setup.py` & `tencentcloud-sdk-python-antiddos-3.0.922/setup.py`

 * *Files identical despite different names*

