# Comparing `tmp/tencentcloud-sdk-python-tdid-3.0.921.tar.gz` & `tmp/tencentcloud-sdk-python-tdid-3.0.922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdid-3.0.921.tar", last modified: Mon Jun 26 00:34:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdid-3.0.922.tar", last modified: Tue Jun 27 00:34:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdid-3.0.921.tar` & `tencentcloud-sdk-python-tdid-3.0.922.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45275 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/models.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    18789 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/tdid_client.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/README.rst
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-26 00:34:02.000000 tencentcloud-sdk-python-tdid-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud_sdk_python_tdid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud_sdk_python_tdid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud_sdk_python_tdid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud_sdk_python_tdid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/tdid/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/tdid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/tdid/v20210519/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/tdid/v20210519/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39876 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/tdid/v20210519/models.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/tdid/v20210519/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    17289 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/tdid/v20210519/tdid_client.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-27 00:34:19.000000 tencentcloud-sdk-python-tdid-3.0.922/setup.py
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.921/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdid-3.0.922/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdid
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Tdid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/models.py` & `tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/tdid/v20210519/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -590,98 +590,14 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DidCluster(AbstractModel):
-    """did区块链网络信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ChainId: 链ID
-        :type ChainId: int
-        :param ChainName: 链名称
-        :type ChainName: str
-        :param AgencyCount: 组织数量
-        :type AgencyCount: int
-        :param ConsortiumId: 联盟ID
-        :type ConsortiumId: int
-        :param CreateTime: 创建时间
-        :type CreateTime: str
-        :param ExpireTime: 过期时间
-        :type ExpireTime: str
-        :param ChainStatus: 网络状态
-        :type ChainStatus: int
-        :param ResourceId: 资源ID
-        :type ResourceId: str
-        :param ClusterId: 网络ID
-        :type ClusterId: str
-        :param ConsortiumName: 联盟名称
-        :type ConsortiumName: str
-        :param AgencyId: 组织ID
-        :type AgencyId: int
-        :param AutoRenewFlag: 自动续费
-        :type AutoRenewFlag: int
-        :param TotalNetworkNode: 网络节点总数
-        :type TotalNetworkNode: int
-        :param TotalCreateNode: 本机构节点数
-        :type TotalCreateNode: int
-        :param TotalGroups: 总群组数
-        :type TotalGroups: int
-        :param DidCount: DID总数
-        :type DidCount: int
-        """
-        self.ChainId = None
-        self.ChainName = None
-        self.AgencyCount = None
-        self.ConsortiumId = None
-        self.CreateTime = None
-        self.ExpireTime = None
-        self.ChainStatus = None
-        self.ResourceId = None
-        self.ClusterId = None
-        self.ConsortiumName = None
-        self.AgencyId = None
-        self.AutoRenewFlag = None
-        self.TotalNetworkNode = None
-        self.TotalCreateNode = None
-        self.TotalGroups = None
-        self.DidCount = None
-
-
-    def _deserialize(self, params):
-        self.ChainId = params.get("ChainId")
-        self.ChainName = params.get("ChainName")
-        self.AgencyCount = params.get("AgencyCount")
-        self.ConsortiumId = params.get("ConsortiumId")
-        self.CreateTime = params.get("CreateTime")
-        self.ExpireTime = params.get("ExpireTime")
-        self.ChainStatus = params.get("ChainStatus")
-        self.ResourceId = params.get("ResourceId")
-        self.ClusterId = params.get("ClusterId")
-        self.ConsortiumName = params.get("ConsortiumName")
-        self.AgencyId = params.get("AgencyId")
-        self.AutoRenewFlag = params.get("AutoRenewFlag")
-        self.TotalNetworkNode = params.get("TotalNetworkNode")
-        self.TotalCreateNode = params.get("TotalCreateNode")
-        self.TotalGroups = params.get("TotalGroups")
-        self.DidCount = params.get("DidCount")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class FunctionArg(AbstractModel):
     """创建凭证入参的FunctionArg
 
     """
 
     def __init__(self):
         r"""
@@ -1065,99 +981,14 @@
     def _deserialize(self, params):
         if params.get("CredentialStatus") is not None:
             self.CredentialStatus = CredentialStatus()
             self.CredentialStatus._deserialize(params.get("CredentialStatus"))
         self.RequestId = params.get("RequestId")
 
 
-class GetDidClusterDetailRequest(AbstractModel):
-    """GetDidClusterDetail请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ClusterId: DID网络ID
-        :type ClusterId: str
-        """
-        self.ClusterId = None
-
-
-    def _deserialize(self, params):
-        self.ClusterId = params.get("ClusterId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class GetDidClusterDetailResponse(AbstractModel):
-    """GetDidClusterDetail返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ClusterId: 网络ID
-        :type ClusterId: str
-        :param ConsortiumName: 组织名称
-        :type ConsortiumName: str
-        :param ChainAgency: 区块链组织名称
-        :type ChainAgency: str
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.ClusterId = None
-        self.ConsortiumName = None
-        self.ChainAgency = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.ClusterId = params.get("ClusterId")
-        self.ConsortiumName = params.get("ConsortiumName")
-        self.ChainAgency = params.get("ChainAgency")
-        self.RequestId = params.get("RequestId")
-
-
-class GetDidClusterListRequest(AbstractModel):
-    """GetDidClusterList请求参数结构体
-
-    """
-
-
-class GetDidClusterListResponse(AbstractModel):
-    """GetDidClusterList返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param DidClusterList: DID网络列表
-        :type DidClusterList: list of DidCluster
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.DidClusterList = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        if params.get("DidClusterList") is not None:
-            self.DidClusterList = []
-            for item in params.get("DidClusterList"):
-                obj = DidCluster()
-                obj._deserialize(item)
-                self.DidClusterList.append(obj)
-        self.RequestId = params.get("RequestId")
-
-
 class GetDidDocumentRequest(AbstractModel):
     """GetDidDocument请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/errorcodes.py` & `tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/tdid/v20210519/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdid-3.0.921/tencentcloud/tdid/v20210519/tdid_client.py` & `tencentcloud-sdk-python-tdid-3.0.922/tencentcloud/tdid/v20210519/tdid_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CheckChain(self, request):
-        """检查区块链信息
+        """该接口不再使用
+
+        检查区块链信息
 
         :param request: Request instance for CheckChain.
         :type request: :class:`tencentcloud.tdid.v20210519.models.CheckChainRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.CheckChainResponse`
 
         """
         try:
@@ -71,15 +73,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateCredential(self, request):
-        """创建凭证
+        """该接口不再使用
+
+        创建凭证
 
         :param request: Request instance for CreateCredential.
         :type request: :class:`tencentcloud.tdid.v20210519.models.CreateCredentialRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.CreateCredentialResponse`
 
         """
         try:
@@ -94,15 +98,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateSelectiveCredential(self, request):
-        """创建选择性批露凭证
+        """该接口不再使用
+
+        创建选择性批露凭证
 
         :param request: Request instance for CreateSelectiveCredential.
         :type request: :class:`tencentcloud.tdid.v20210519.models.CreateSelectiveCredentialRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.CreateSelectiveCredentialResponse`
 
         """
         try:
@@ -117,15 +123,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateTDid(self, request):
-        """创建机构DID
+        """该接口不再使用
+
+        创建机构DID
 
         :param request: Request instance for CreateTDid.
         :type request: :class:`tencentcloud.tdid.v20210519.models.CreateTDidRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.CreateTDidResponse`
 
         """
         try:
@@ -140,15 +148,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateTDidByPrivateKey(self, request):
-        """新建DID根据私钥生成Tdid
+        """该接口不再使用
+
+        新建DID根据私钥生成Tdid
 
         :param request: Request instance for CreateTDidByPrivateKey.
         :type request: :class:`tencentcloud.tdid.v20210519.models.CreateTDidByPrivateKeyRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.CreateTDidByPrivateKeyResponse`
 
         """
         try:
@@ -163,15 +173,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateTDidByPublicKey(self, request):
-        """新建DID根据公钥生成Tdid
+        """该接口不再使用
+
+         新建DID根据公钥生成Tdid
 
         :param request: Request instance for CreateTDidByPublicKey.
         :type request: :class:`tencentcloud.tdid.v20210519.models.CreateTDidByPublicKeyRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.CreateTDidByPublicKeyResponse`
 
         """
         try:
@@ -211,15 +223,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetAuthorityIssuer(self, request):
-        """获取权威机构信息
+        """该接口不再使用
+
+        获取权威机构信息
 
         :param request: Request instance for GetAuthorityIssuer.
         :type request: :class:`tencentcloud.tdid.v20210519.models.GetAuthorityIssuerRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.GetAuthorityIssuerResponse`
 
         """
         try:
@@ -284,15 +298,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetCptInfo(self, request):
-        """凭证模版详情
+        """该接口不再使用
+
+        凭证模版详情
 
         :param request: Request instance for GetCptInfo.
         :type request: :class:`tencentcloud.tdid.v20210519.models.GetCptInfoRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.GetCptInfoResponse`
 
         """
         try:
@@ -332,15 +348,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetCredentialStatus(self, request):
-        """获取凭证链上状态信息
+        """该接口不再使用
+
+        获取凭证链上状态信息
 
         :param request: Request instance for GetCredentialStatus.
         :type request: :class:`tencentcloud.tdid.v20210519.models.GetCredentialStatusRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.GetCredentialStatusResponse`
 
         """
         try:
@@ -354,66 +372,18 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def GetDidClusterDetail(self, request):
-        """下线已有内测接口，待上线正式版本的接口
-
-        获取DID区块链网络详情
-
-        :param request: Request instance for GetDidClusterDetail.
-        :type request: :class:`tencentcloud.tdid.v20210519.models.GetDidClusterDetailRequest`
-        :rtype: :class:`tencentcloud.tdid.v20210519.models.GetDidClusterDetailResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GetDidClusterDetail", params, headers=headers)
-            response = json.loads(body)
-            model = models.GetDidClusterDetailResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def GetDidClusterList(self, request):
-        """下线已有内测接口，待上线正式版本的接口
-
-        获取用户的DID网络列表
-
-        :param request: Request instance for GetDidClusterList.
-        :type request: :class:`tencentcloud.tdid.v20210519.models.GetDidClusterListRequest`
-        :rtype: :class:`tencentcloud.tdid.v20210519.models.GetDidClusterListResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GetDidClusterList", params, headers=headers)
-            response = json.loads(body)
-            model = models.GetDidClusterListResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def GetDidDocument(self, request):
-        """查看DID文档
+        """该接口不再使用
+
+        查看DID文档
 
         :param request: Request instance for GetDidDocument.
         :type request: :class:`tencentcloud.tdid.v20210519.models.GetDidDocumentRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.GetDidDocumentResponse`
 
         """
         try:
@@ -428,15 +398,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RegisterCpt(self, request):
-        """凭证模版新建
+        """该接口不再使用
+
+        凭证模版新建
 
         :param request: Request instance for RegisterCpt.
         :type request: :class:`tencentcloud.tdid.v20210519.models.RegisterCptRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.RegisterCptResponse`
 
         """
         try:
@@ -451,15 +423,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def SetCredentialStatus(self, request):
-        """设置凭证链上状态
+        """该接口不再使用
+
+        设置凭证链上状态
 
         :param request: Request instance for SetCredentialStatus.
         :type request: :class:`tencentcloud.tdid.v20210519.models.SetCredentialStatusRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.SetCredentialStatusResponse`
 
         """
         try:
@@ -474,15 +448,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def VerifyCredential(self, request):
-        """验证凭证
+        """该接口不再使用
+
+        验证凭证
 
         :param request: Request instance for VerifyCredential.
         :type request: :class:`tencentcloud.tdid.v20210519.models.VerifyCredentialRequest`
         :rtype: :class:`tencentcloud.tdid.v20210519.models.VerifyCredentialResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.921/README.rst` & `tencentcloud-sdk-python-tdid-3.0.922/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdid-3.0.921/PKG-INFO` & `tencentcloud-sdk-python-tdid-3.0.922/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdid
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Tdid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.921/setup.py` & `tencentcloud-sdk-python-tdid-3.0.922/setup.py`

 * *Files identical despite different names*

