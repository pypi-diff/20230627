# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.921.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.921.tar", last modified: Mon Jun 26 00:20:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.922.tar", last modified: Tue Jun 27 00:20:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.921.tar` & `tencentcloud-sdk-python-ckafka-3.0.922.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   486111 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    71620 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/README.rst
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-26 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   486738 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    71620 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-27 00:20:38.000000 tencentcloud-sdk-python-ckafka-3.0.922/setup.py
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2306,15 +2306,15 @@
         :type SubnetId: str
         :param InstanceType: 实例规格。当创建标准版实例时必填，创建专业版实例时不需要填写。1：入门型；2：标准型；3：进阶型；4：容量型；5：高阶型1；6：高阶性2；7：高阶型3；8：高阶型4；9 ：独占型
         :type InstanceType: int
         :param MsgRetentionTime: 实例日志的默认最长保留时间，单位分钟。不传入该参数时默认为 1440 分钟（1天），最大30天。当 topic 显式设置消息保留时间时，以 topic 保留时间为准
         :type MsgRetentionTime: int
         :param ClusterId: 创建实例时可以选择集群Id, 该入参表示集群Id。不指定实例所在集群则不传入该参数
         :type ClusterId: int
-        :param KafkaVersion: 实例版本。目前支持 "0.10.2","1.1.1","2.4.2","2.8.1"
+        :param KafkaVersion: 实例版本。目前支持 "0.10.2","1.1.1","2.4.1","2.4.2","2.8.1"。"2.4.1" 与 "2.4.2" 属于同一个版本，传任意一个均可。
         :type KafkaVersion: str
         :param SpecificationsType: 实例类型。"standard"：标准版，"profession"：专业版
         :type SpecificationsType: str
         :param DiskType: 实例硬盘类型，"CLOUD_BASIC"：云硬盘，"CLOUD_SSD"：高速云硬盘。不传默认为 "CLOUD_BASIC"
         :type DiskType: str
         :param DiskSize: 实例硬盘大小，需要满足当前实例的计费规格
         :type DiskSize: int
@@ -2326,15 +2326,15 @@
         :type ZoneId: int
         :param MultiZoneFlag: 当前实例是否为多可用区实例。
         :type MultiZoneFlag: bool
         :param ZoneIds: 当实例为多可用区实例时，多可用区 id 列表。注意参数 ZoneId 对应的多可用区需要包含在该参数数组中
         :type ZoneIds: list of int
         :param InstanceNum: 购买实例数量。非必填，默认值为 1。当传入该参数时，会创建多个 instanceName 加后缀区分的实例
         :type InstanceNum: int
-        :param PublicNetworkMonthly: 公网带宽大小，单位 Mbps。默认是没有加上免费 3Mbps 带宽。例如总共需要 3Mbps 公网带宽，此处传 0；总共需要 4Mbps 公网带宽，此处传 1
+        :param PublicNetworkMonthly: 公网带宽大小，单位 Mbps。默认是没有加上免费 3Mbps 带宽。例如总共需要 3Mbps 公网带宽，此处传 0；总共需要 6Mbps 公网带宽，此处传 3。需要保证传入参数为 3 的整数倍
         :type PublicNetworkMonthly: int
         """
         self.InstanceName = None
         self.BandWidth = None
         self.VpcId = None
         self.SubnetId = None
         self.InstanceType = None
@@ -2496,25 +2496,25 @@
         :param ZoneId: 可用区，购买多可用区实例时，填写ZoneIds.N字段中的任意一个值
         :type ZoneId: int
         :param Period: 预付费购买时长，例如 "1m",就是一个月
         :type Period: str
         :param InstanceType: 实例规格说明 专业版实例[所有规格]填写1.
 标准版实例 ([入门型(general)]填写1，[标准型(standard)]填写2，[进阶型(advanced)]填写3，[容量型(capacity)]填写4，[高阶型1(specialized-1)]填写5，[高阶性2(specialized-2)]填写6,[高阶型3(specialized-3)]填写7,[高阶型4(specialized-4)]填写8，[独占型(exclusive)]填写9。
         :type InstanceType: int
-        :param VpcId: vpcId，不填默认基础网络
+        :param VpcId: vpcId必填
         :type VpcId: str
         :param SubnetId: 子网id，vpc网络需要传该参数，基础网络可以不传
         :type SubnetId: str
         :param MsgRetentionTime: 可选。实例日志的最长保留时间，单位分钟，默认为10080（7天），最大30天，不填默认0，代表不开启日志保留时间回收策略
         :type MsgRetentionTime: int
         :param ClusterId: 创建实例时可以选择集群Id, 该入参表示集群Id
         :type ClusterId: int
         :param RenewFlag: 预付费自动续费标记，0表示默认状态(用户未设置，即初始状态)， 1表示自动续费，2表示明确不自动续费(用户设置)
         :type RenewFlag: int
-        :param KafkaVersion: CKafka版本号[0.10.2、1.1.1、2.4.1], 默认是1.1.1
+        :param KafkaVersion: CKafka版本号[0.10.2、1.1.1、2.4.1、2.4.2、2.8.1], 默认是1.1.1。2.4.1 与 2.4.2 属于同一个版本，传任意一个均可。
         :type KafkaVersion: str
         :param SpecificationsType: 实例类型: [标准版实例]填写 standard(默认), [专业版实例]填写 profession
         :type SpecificationsType: str
         :param DiskSize: 磁盘大小，专业版不填写默认最小磁盘，如果跟控制台规格配比不相符，则无法创建成功
         :type DiskSize: int
         :param BandWidth: 带宽，专业版不填写默认最小带宽，如果跟控制台规格配比不相符，则无法创建成功
         :type BandWidth: int
@@ -2524,16 +2524,18 @@
         :type Tags: list of Tag
         :param DiskType: 磁盘类型（ssd填写CLOUD_SSD，sata填写CLOUD_BASIC）
         :type DiskType: str
         :param MultiZoneFlag: 跨可用区，zoneIds必填
         :type MultiZoneFlag: bool
         :param ZoneIds: 可用区列表，购买多可用区实例时为必填项
         :type ZoneIds: list of int
-        :param PublicNetworkMonthly: 公网带宽大小，单位 Mbps。默认是没有加上免费 3Mbps 带宽。例如总共需要 3Mbps 公网带宽，此处传 0；总共需要 4Mbps 公网带宽，此处传 1。默认值为 0
+        :param PublicNetworkMonthly: 公网带宽大小，单位 Mbps。默认是没有加上免费 3Mbps 带宽。例如总共需要 3Mbps 公网带宽，此处传 0；总共需要 6Mbps 公网带宽，此处传 3。默认值为 0。需要保证传入参数为 3 的整数倍
         :type PublicNetworkMonthly: int
+        :param InstanceNum: 购买实例数量。非必填，默认值为 1。当传入该参数时，会创建多个 instanceName 加后缀区分的实例
+        :type InstanceNum: int
         """
         self.InstanceName = None
         self.ZoneId = None
         self.Period = None
         self.InstanceType = None
         self.VpcId = None
         self.SubnetId = None
@@ -2546,14 +2548,15 @@
         self.BandWidth = None
         self.Partition = None
         self.Tags = None
         self.DiskType = None
         self.MultiZoneFlag = None
         self.ZoneIds = None
         self.PublicNetworkMonthly = None
+        self.InstanceNum = None
 
 
     def _deserialize(self, params):
         self.InstanceName = params.get("InstanceName")
         self.ZoneId = params.get("ZoneId")
         self.Period = params.get("Period")
         self.InstanceType = params.get("InstanceType")
@@ -2573,14 +2576,15 @@
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.DiskType = params.get("DiskType")
         self.MultiZoneFlag = params.get("MultiZoneFlag")
         self.ZoneIds = params.get("ZoneIds")
         self.PublicNetworkMonthly = params.get("PublicNetworkMonthly")
+        self.InstanceNum = params.get("InstanceNum")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2719,15 +2723,15 @@
         :type SubnetId: str
         :param InstanceType: 实例规格。当创建标准版实例时必填，创建专业版实例时不需要填写。1：入门型；2：标准型；3：进阶型；4：容量型；5：高阶型1；6：高阶性2；7：高阶型3；8：高阶型4；9 ：独占型
         :type InstanceType: int
         :param MsgRetentionTime: 实例日志的默认最长保留时间，单位分钟。不传入该参数时默认为 1440 分钟（1天），最大30天。当 topic 显式设置消息保留时间时，以 topic 保留时间为准
         :type MsgRetentionTime: int
         :param ClusterId: 创建实例时可以选择集群Id, 该入参表示集群Id。不指定实例所在集群则不传入该参数
         :type ClusterId: int
-        :param KafkaVersion: 实例版本。目前支持 "0.10.2","1.1.1","2.4.2","2.8.1"
+        :param KafkaVersion: 实例版本。目前支持 "0.10.2","1.1.1","2.4.1","2.4.2","2.8.1"。"2.4.1" 与 "2.4.2" 属于同一个版本，传任意一个均可。
         :type KafkaVersion: str
         :param SpecificationsType: 实例类型。"standard"：标准版，"profession"：专业版
         :type SpecificationsType: str
         :param DiskType: 实例硬盘类型，"CLOUD_BASIC"：云硬盘，"CLOUD_SSD"：高速云硬盘。不传默认为 "CLOUD_BASIC"
         :type DiskType: str
         :param BandWidth: 实例内网峰值带宽。单位 MB/s。标准版需传入当前实例规格所对应的峰值带宽。注意如果创建的实例为专业版实例，峰值带宽，分区数等参数配置需要满足专业版的计费规格。
         :type BandWidth: int
@@ -2741,15 +2745,15 @@
         :type ZoneId: int
         :param MultiZoneFlag: 当前实例是否为多可用区实例。
         :type MultiZoneFlag: bool
         :param ZoneIds: 当实例为多可用区实例时，多可用区 id 列表。注意参数 ZoneId 对应的多可用区需要包含在该参数数组中
         :type ZoneIds: list of int
         :param InstanceNum: 购买实例数量。非必填，默认值为 1。当传入该参数时，会创建多个 instanceName 加后缀区分的实例
         :type InstanceNum: int
-        :param PublicNetworkMonthly: 公网带宽大小，单位 Mbps。默认是没有加上免费 3Mbps 带宽。例如总共需要 3Mbps 公网带宽，此处传 0；总共需要 4Mbps 公网带宽，此处传 1
+        :param PublicNetworkMonthly: 公网带宽大小，单位 Mbps。默认是没有加上免费 3Mbps 带宽。例如总共需要 3Mbps 公网带宽，此处传 0；总共需要 6Mbps 公网带宽，此处传 3。需要保证传入参数为 3 的整数倍
         :type PublicNetworkMonthly: int
         """
         self.InstanceName = None
         self.VpcId = None
         self.SubnetId = None
         self.InstanceType = None
         self.MsgRetentionTime = None
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.921/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.922/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.921/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.922/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.921/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.922/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.921/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.922/setup.py`

 * *Files identical despite different names*

