# Comparing `tmp/tencentcloud-sdk-python-nlp-3.0.921.tar.gz` & `tmp/tencentcloud-sdk-python-nlp-3.0.922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.921.tar", last modified: Mon Jun 26 00:29:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.922.tar", last modified: Tue Jun 27 00:29:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-nlp-3.0.921.tar` & `tencentcloud-sdk-python-nlp-3.0.922.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/nlp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/nlp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/nlp/v20190408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/nlp/v20190408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44601 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/nlp/v20190408/nlp_client.py
--rw-r--r--   0 root         (0) root         (0)    81020 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/nlp/v20190408/models.py
--rw-r--r--   0 root         (0) root         (0)     5906 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/nlp/v20190408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud_sdk_python_nlp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-26 00:29:18.000000 tencentcloud-sdk-python-nlp-3.0.921/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/nlp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/nlp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/nlp/v20190408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/nlp/v20190408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49107 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/nlp/v20190408/nlp_client.py
+-rw-r--r--   0 root         (0) root         (0)    90360 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/nlp/v20190408/models.py
+-rw-r--r--   0 root         (0) root         (0)     6090 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/nlp/v20190408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud_sdk_python_nlp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-27 00:29:37.000000 tencentcloud-sdk-python-nlp-3.0.922/setup.py
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/__init__.py` & `tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/nlp/v20190408/nlp_client.py` & `tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/nlp/v20190408/nlp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,37 @@
 
 class NlpClient(AbstractClient):
     _apiVersion = '2019-04-08'
     _endpoint = 'nlp.tencentcloudapi.com'
     _service = 'nlp'
 
 
+    def AnalyzeSentiment(self, request):
+        """情感分析接口能够对带有情感色彩的主观性文本进行分析、处理、归纳和推理，识别出用户的情感倾向，是积极、中性还是消极，并且提供各自概率。
+
+        :param request: Request instance for AnalyzeSentiment.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.AnalyzeSentimentRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.AnalyzeSentimentResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("AnalyzeSentiment", params, headers=headers)
+            response = json.loads(body)
+            model = models.AnalyzeSentimentResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def AutoSummarization(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         利用人工智能算法，自动抽取文本中的关键信息并生成指定长度的文本摘要。可用于新闻标题生成、科技文献摘要生成和商品评论摘要等。
 
         :param request: Request instance for AutoSummarization.
         :type request: :class:`tencentcloud.nlp.v20190408.models.AutoSummarizationRequest`
@@ -71,14 +94,83 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ClassifyContent(self, request):
+        """文本分类接口能够对用户输入的文章进行自动分类，将其映射到具体的类目上，用户只需要提供待分类的文本，而无需关注具体实现。该功能定义了一套较为完备的[三级分类体系](https://cloud.tencent.com/document/product/271/94286)，积累了数百万的语料，经过多轮迭代优化打造了较先进的深度学习模型，以保证效果不断提升。
+
+        :param request: Request instance for ClassifyContent.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.ClassifyContentRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.ClassifyContentResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ClassifyContent", params, headers=headers)
+            response = json.loads(body)
+            model = models.ClassifyContentResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ComposeCouplet(self, request):
+        """对联生成接口根据用户输入的命题关键词，智能生成一副完整的春联，包括上联、下联和横批。该接口利用先进的自然语言处理技术，确保生成的春联既符合传统对仗、对韵、对义的要求，又具有新意和创意，为用户提供独特的春节祝福。
+
+        :param request: Request instance for ComposeCouplet.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.ComposeCoupletRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.ComposeCoupletResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ComposeCouplet", params, headers=headers)
+            response = json.loads(body)
+            model = models.ComposeCoupletResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ComposePoetry(self, request):
+        """诗词生成接口利用现代的自然语言处理和深度学习技术，模仿了古代著名诗人的风格，为用户产生独特的诗词。用户只需输入的命题关键词，接口就能自动生成一首七言律诗或五言律诗。
+
+        :param request: Request instance for ComposePoetry.
+        :type request: :class:`tencentcloud.nlp.v20190408.models.ComposePoetryRequest`
+        :rtype: :class:`tencentcloud.nlp.v20190408.models.ComposePoetryResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ComposePoetry", params, headers=headers)
+            response = json.loads(body)
+            model = models.ComposePoetryResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateDict(self, request):
         """因业务调整该接口将于北京时间2023年8月1日0点下线，届时该产品功能将无法正常使用，为了避免对您的业务造成影响，请您尽快做好相关业务调整。详见：https://cloud.tencent.com/document/product/271/90711
 
         根据指定的名称、描述创建自定义词库。
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/nlp/v20190408/models.py` & `tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/nlp/v20190408/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,74 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class AnalyzeSentimentRequest(AbstractModel):
+    """AnalyzeSentiment请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Text: 待分析的文本（仅支持UTF-8格式，不超过200字）。
+        :type Text: str
+        """
+        self.Text = None
+
+
+    def _deserialize(self, params):
+        self.Text = params.get("Text")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AnalyzeSentimentResponse(AbstractModel):
+    """AnalyzeSentiment返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Positive: 正面情感概率。
+        :type Positive: float
+        :param Neutral: 中性情感概率。
+        :type Neutral: float
+        :param Negative: 负面情感概率。
+        :type Negative: float
+        :param Sentiment: 情感分类结果：
+positive：正面情感
+negative：负面情感
+neutral：中性、无情感
+        :type Sentiment: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Positive = None
+        self.Neutral = None
+        self.Negative = None
+        self.Sentiment = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Positive = params.get("Positive")
+        self.Neutral = params.get("Neutral")
+        self.Negative = params.get("Negative")
+        self.Sentiment = params.get("Sentiment")
+        self.RequestId = params.get("RequestId")
+
+
 class AutoSummarizationRequest(AbstractModel):
     """AutoSummarization请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -132,14 +192,54 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class Category(AbstractModel):
+    """分类详细信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: 分类id。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: int
+        :param Label: 分类英文名。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Label: str
+        :param Name: 分类中文名。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param Score: 分类置信度。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Score: float
+        """
+        self.Id = None
+        self.Label = None
+        self.Name = None
+        self.Score = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.Label = params.get("Label")
+        self.Name = params.get("Name")
+        self.Score = params.get("Score")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ChatBotRequest(AbstractModel):
     """ChatBot请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -249,14 +349,192 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ClassifyContentRequest(AbstractModel):
+    """ClassifyContent请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 待分类的文章的标题（仅支持UTF-8格式，不超过100字符）。
+        :type Title: str
+        :param Content: 待分类文章的内容, 每个元素对应一个段落。（仅支持UTF-8格式，文章内容长度总和不超过2000字符）
+        :type Content: list of str
+        """
+        self.Title = None
+        self.Content = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Content = params.get("Content")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ClassifyContentResponse(AbstractModel):
+    """ClassifyContent返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FirstClassification: 一级分类。分类详情见附录-三级分类体系表。
+        :type FirstClassification: :class:`tencentcloud.nlp.v20190408.models.Category`
+        :param SecondClassification: 二级分类。分类详情见附录-三级分类体系表。
+        :type SecondClassification: :class:`tencentcloud.nlp.v20190408.models.Category`
+        :param ThirdClassification: 三级分类。分类详情见附录-三级分类体系表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ThirdClassification: :class:`tencentcloud.nlp.v20190408.models.Category`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FirstClassification = None
+        self.SecondClassification = None
+        self.ThirdClassification = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("FirstClassification") is not None:
+            self.FirstClassification = Category()
+            self.FirstClassification._deserialize(params.get("FirstClassification"))
+        if params.get("SecondClassification") is not None:
+            self.SecondClassification = Category()
+            self.SecondClassification._deserialize(params.get("SecondClassification"))
+        if params.get("ThirdClassification") is not None:
+            self.ThirdClassification = Category()
+            self.ThirdClassification._deserialize(params.get("ThirdClassification"))
+        self.RequestId = params.get("RequestId")
+
+
+class ComposeCoupletRequest(AbstractModel):
+    """ComposeCouplet请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Text: 生成对联的关键词。长度需>=2，当长度>2时，自动截取前两个字作为关键字。内容需为常用汉字（不含有数字、英文、韩语、日语、符号等等其他）。
+        :type Text: str
+        :param TargetType: 返回的文本结果为繁体还是简体。0：简体；1：繁体。默认为0。
+        :type TargetType: int
+        """
+        self.Text = None
+        self.TargetType = None
+
+
+    def _deserialize(self, params):
+        self.Text = params.get("Text")
+        self.TargetType = params.get("TargetType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ComposeCoupletResponse(AbstractModel):
+    """ComposeCouplet返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TopScroll: 横批。
+        :type TopScroll: str
+        :param Content: 上联与下联。
+        :type Content: list of str
+        :param RandomCause: 当对联随机生成时，展示随机生成原因。
+        :type RandomCause: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TopScroll = None
+        self.Content = None
+        self.RandomCause = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TopScroll = params.get("TopScroll")
+        self.Content = params.get("Content")
+        self.RandomCause = params.get("RandomCause")
+        self.RequestId = params.get("RequestId")
+
+
+class ComposePoetryRequest(AbstractModel):
+    """ComposePoetry请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Text: 生成诗词的关键词。
+        :type Text: str
+        :param PoetryType: 生成诗词的类型。0：藏头或藏身；1：藏头；2：藏身。默认为0。
+        :type PoetryType: int
+        :param Genre: 诗的体裁。0：五言律诗或七言律诗；5：五言律诗；7：七言律诗。默认为0。
+        :type Genre: int
+        """
+        self.Text = None
+        self.PoetryType = None
+        self.Genre = None
+
+
+    def _deserialize(self, params):
+        self.Text = params.get("Text")
+        self.PoetryType = params.get("PoetryType")
+        self.Genre = params.get("Genre")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ComposePoetryResponse(AbstractModel):
+    """ComposePoetry返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 诗题，即输入的生成诗词的关键词。
+        :type Title: str
+        :param Content: 诗的内容。
+        :type Content: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Title = None
+        self.Content = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Content = params.get("Content")
+        self.RequestId = params.get("RequestId")
+
+
 class CompoundParticiple(AbstractModel):
     """复合粒度分词和词性标注的结果。
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.921/tencentcloud/nlp/v20190408/errorcodes.py` & `tencentcloud-sdk-python-nlp-3.0.922/tencentcloud/nlp/v20190408/errorcodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,20 @@
 
 # 内部服务调用错误。
 INTERNALERROR_SERVICECALLERROR = 'InternalError.ServiceCallError'
 
 # 内部服务调用失败。
 INTERNALERROR_SERVICEERROR = 'InternalError.ServiceError'
 
+# 文本分类异常。
+INTERNALERROR_TEXTCLASSIFYERROR = 'InternalError.TextClassifyError'
+
+# 文本解析异常。
+INTERNALERROR_TEXTPARSINGERROR = 'InternalError.TextParsingError'
+
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 服务调用失败。
 INVALIDPARAMETER_SERVICEERROR = 'InvalidParameter.ServiceError'
 
 # 文本长度超过限制。
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.921/README.rst` & `tencentcloud-sdk-python-nlp-3.0.922/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.921/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.922/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.921/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.922/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.921
+Version: 3.0.922
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.921/setup.py` & `tencentcloud-sdk-python-nlp-3.0.922/setup.py`

 * *Files identical despite different names*

