# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.921.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.921.tar", last modified: Mon Jun 26 00:16:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.922.tar", last modified: Tue Jun 27 00:17:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.921.tar` & `tencentcloud-sdk-python-asr-3.0.922.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:16:24.000000 tencentcloud-sdk-python-asr-3.0.921/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:16:24.000000 tencentcloud-sdk-python-asr-3.0.921/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:16:24.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:16:24.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud/asr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud/asr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:16:24.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64128 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)    25038 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     6520 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:16:24.000000 tencentcloud-sdk-python-asr-3.0.921/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:16:24.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-26 00:16:24.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/tencentcloud_sdk_python_asr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-26 00:16:23.000000 tencentcloud-sdk-python-asr-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud/asr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:17:05.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud/asr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:17:05.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64222 2023-06-27 00:17:05.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)    24910 2023-06-27 00:17:05.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-06-27 00:17:05.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-27 00:17:05.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-27 00:17:05.000000 tencentcloud-sdk-python-asr-3.0.922/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 00:17:06.000000 tencentcloud-sdk-python-asr-3.0.922/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-27 00:17:05.000000 tencentcloud-sdk-python-asr-3.0.922/setup.py
```

### Comparing `tencentcloud-sdk-python-asr-3.0.921/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.922/tencentcloud/asr/v20190614/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,16 +363,16 @@
         :type EngineModelType: str
         :param ChannelNum: 识别声道数。1：单声道（非电话场景，直接选择单声道即可，忽略音频声道数）；2：双声道（仅支持8k_zh电话场景，双声道应分别对应通话双方）。注意：双声道的电话音频已物理分离说话人，无需再开启说话人分离功能。
         :type ChannelNum: int
         :param ResTextFormat: 识别结果返回形式。0： 识别结果文本(含分段时间戳)； 1：词级别粒度的[详细识别结果](https://cloud.tencent.com/document/api/1093/37824#SentenceDetail)(不含标点，含语速值)；2：词级别粒度的详细识别结果（包含标点、语速值）；3: 标点符号分段，包含每段时间戳，特别适用于字幕场景（包含词级时间、标点、语速值）。
         :type ResTextFormat: int
         :param SourceType: 语音数据来源。0：语音 URL；1：语音数据（post body）。
         :type SourceType: int
-        :param SpeakerDiarization: 是否开启说话人分离，0：不开启，1：开启(仅支持8k_zh，16k_zh，16k_zh_video，单声道音频)，默认值为 0。
-注意：8k电话场景建议使用双声道来区分通话双方，设置ChannelNum=2即可，不用开启说话人分离。
+        :param SpeakerDiarization: 是否开启说话人分离，0：不开启，1：开启(仅支持8k_zh/16k_zh，ChannelNum=1时可用)，默认值为 0。
+注意：8k电话场景建议使用双声道来区分通话双方，设置ChannelNum=2即可，不用开启说话人分离，如果设置了ChannelNum=1，后台会先转码成单声道，说话人分离结果可能产生偏差。
         :type SpeakerDiarization: int
         :param SpeakerNumber: 说话人分离人数（需配合开启说话人分离使用），取值范围：0-10，0代表自动分离（目前仅支持≤6个人），1-10代表指定说话人数分离。默认值为 0。
 注：此功能结果仅供参考，请根据您的需要谨慎使用。
         :type SpeakerNumber: int
         :param CallbackUrl: 回调 URL，用户自行搭建的用于接收识别结果的服务URL。如果用户使用轮询方式获取识别结果，则无需提交该参数。回调格式&内容详见：[录音识别回调说明](https://cloud.tencent.com/document/product/1093/52632)
         :type CallbackUrl: str
         :param Url: 语音的URL地址，需要公网环境浏览器可下载。当 SourceType 值为 0 时须填写该字段，为 1 时不需要填写。注意：请确保录音文件时长在5个小时之内，否则可能识别失败。请保证文件的下载速度，否则可能下载失败。
```

### Comparing `tencentcloud-sdk-python-asr-3.0.921/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.922/tencentcloud/asr/v20190614/asr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         • 支持中文普通话、英语、粤语、日语、越南语、马来语、印度尼西亚语、菲律宾语、葡萄牙语、土耳其语、上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话。
         • 支持wav、mp3、m4a、flv、mp4、wma、3gp、amr、aac、ogg-opus、flac格式。
         • 支持语音 URL 和本地语音文件两种请求方式。语音 URL 的音频时长不能长于5小时，文件大小不超过1GB。本地语音文件调用不能大于5MB。推荐使用 [ 腾讯云COS](https://cloud.tencent.com/document/product/436/38484) 来存储&生成URL提交任务，无外网&流量下行费用，节约成本、提升任务速度。(COS桶权限需要设置公有读私有写，或URL设置外部可访问)
         • 提交录音文件识别请求后，在3小时内完成识别（大多数情况下1小时音频约3分钟以内完成识别，半小时内发送超过1000小时录音或者2万条识别任务的除外），识别结果在服务端可保存7天。
         • 支持回调或轮询的方式获取结果，结果获取请参考[ 录音文件识别结果查询](https://cloud.tencent.com/document/product/1093/37822)。
         •   生成字幕场景可设置参数ResTextFormat为3，解析ResultDetail结构生成字幕，可参考 [生成字幕最佳实践](https://cloud.tencent.com/document/product/1093/84291)。
         •   签名方法参考 [公共参数](https://cloud.tencent.com/document/api/1093/35640) 中签名方法v3。
-        • 默认接口请求频率限制：20次/秒，如您有提高请求频率限制的需求，请提[工单](https://console.cloud.tencent.com/workorder/category)进行咨询。
+        • 默认接口请求频率限制：20次/秒。
 
         :param request: Request instance for CreateRecTask.
         :type request: :class:`tencentcloud.asr.v20190614.models.CreateRecTaskRequest`
         :rtype: :class:`tencentcloud.asr.v20190614.models.CreateRecTaskResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-asr-3.0.921/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.922/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.921/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.922/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.921/README.rst` & `tencentcloud-sdk-python-asr-3.0.922/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.921/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.922/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.921/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.922/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.921/setup.py` & `tencentcloud-sdk-python-asr-3.0.922/setup.py`

 * *Files identical despite different names*

