# Comparing `tmp/jinaai-0.1.3.tar.gz` & `tmp/jinaai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinaai-0.1.3.tar", last modified: Mon Jun 26 06:15:55 2023, max compression
+gzip compressed data, was "jinaai-0.2.0.tar", last modified: Tue Jun 27 13:44:34 2023, max compression
```

## Comparing `jinaai-0.1.3.tar` & `jinaai-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-26 06:15:55.262952 jinaai-0.1.3/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.1.3/LICENSE
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12903 2023-06-26 06:15:55.262670 jinaai-0.1.3/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12653 2023-06-21 05:42:42.000000 jinaai-0.1.3/README.md
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-26 06:15:55.260595 jinaai-0.1.3/jinaai/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2617 2023-06-26 05:41:46.000000 jinaai-0.1.3/jinaai/__init__.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-26 06:15:55.262505 jinaai-0.1.3/jinaai/clients/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1866 2023-06-26 05:41:25.000000 jinaai-0.1.3/jinaai/clients/ChatCatClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1082 2023-06-19 03:53:55.000000 jinaai-0.1.3/jinaai/clients/HTTPClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2110 2023-06-19 04:25:56.000000 jinaai-0.1.3/jinaai/clients/PromptPerfectClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1934 2023-06-19 08:21:16.000000 jinaai-0.1.3/jinaai/clients/RationaleClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1686 2023-06-19 03:26:43.000000 jinaai-0.1.3/jinaai/clients/SceneXClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.1.3/jinaai/clients/__init__.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.1.3/jinaai/utils.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-26 06:15:55.261208 jinaai-0.1.3/jinaai.egg-info/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12903 2023-06-26 06:15:55.000000 jinaai-0.1.3/jinaai.egg-info/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      372 2023-06-26 06:15:55.000000 jinaai-0.1.3/jinaai.egg-info/SOURCES.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-06-26 06:15:55.000000 jinaai-0.1.3/jinaai.egg-info/dependency_links.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-06-26 06:15:55.000000 jinaai-0.1.3/jinaai.egg-info/top_level.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-06-26 06:15:55.262997 jinaai-0.1.3/setup.cfg
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      483 2023-06-26 06:14:56.000000 jinaai-0.1.3/setup.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-27 13:44:34.098364 jinaai-0.2.0/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.2.0/LICENSE
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13476 2023-06-27 13:44:34.098042 jinaai-0.2.0/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13227 2023-06-27 13:38:12.000000 jinaai-0.2.0/README.md
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-27 13:44:34.096825 jinaai-0.2.0/jinaai/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2642 2023-06-27 13:33:29.000000 jinaai-0.2.0/jinaai/__init__.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-27 13:44:34.097886 jinaai-0.2.0/jinaai/clients/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1082 2023-06-19 03:53:55.000000 jinaai-0.2.0/jinaai/clients/HTTPClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1867 2023-06-27 13:25:15.000000 jinaai-0.2.0/jinaai/clients/JinaChatClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2110 2023-06-19 04:25:56.000000 jinaai-0.2.0/jinaai/clients/PromptPerfectClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1934 2023-06-19 08:21:16.000000 jinaai-0.2.0/jinaai/clients/RationaleClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1686 2023-06-19 03:26:43.000000 jinaai-0.2.0/jinaai/clients/SceneXClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.2.0/jinaai/clients/__init__.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.2.0/jinaai/utils.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-27 13:44:34.097234 jinaai-0.2.0/jinaai.egg-info/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13476 2023-06-27 13:44:34.000000 jinaai-0.2.0/jinaai.egg-info/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      373 2023-06-27 13:44:34.000000 jinaai-0.2.0/jinaai.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-06-27 13:44:34.000000 jinaai-0.2.0/jinaai.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-06-27 13:44:34.000000 jinaai-0.2.0/jinaai.egg-info/top_level.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-06-27 13:44:34.098409 jinaai-0.2.0/setup.cfg
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      483 2023-06-27 13:44:25.000000 jinaai-0.2.0/setup.py
```

### Comparing `jinaai-0.1.3/LICENSE` & `jinaai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.3/PKG-INFO` & `jinaai-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,44 @@
-Metadata-Version: 2.1
-Name: jinaai
-Version: 0.1.3
-Summary: Jina AI Python SDK
-Home-page: https://github.com/jina-ai/jinaai-py.git
-Author: Jina AI
-Author-email: guillaume.roncari@jina.ai
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# JinaAI Python SDK
 
-# jinaai-py
+The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products—SceneXplain, PromptPerfect, Rationale, and JinaChat—into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK enables users to effortlessly formulate and fine-tune prompts, thus streamlining application development.
 
-The JinaAI Python SDK is a powerful tool that seamlessly integrates the capabilities of JinaAI's products, including SceneXplain, PromptPerfect, Rationale and JinaChat into Python applications. This SDK acts as a robust wrapper around JinaAI's APIs, empowering users to create and optimize prompts effectively.
 
 ## Installing
 
 ### Package Manager
 
 Using pip:
 ```bash
 $ pip install jinaai
 ```
-## API Tokens
 
-Authenticate on each platforms and go on the API tab to generate an API token:
-- https://scenex.jina.ai
-- https://promptperfect.jina.ai
-- https://rationale.jina.ai
-- https://chat.jina.ai
+## API Secrets
+
+To generate an API secret, you need to authenticate on each respective platform and navigate to the API tab:
+
+- [SceneXplain API](https://scenex.jina.ai/api)
+- [PromptPerfect API](https://promptperfect.jina.ai/api)
+- [Rationale API](https://rationale.jina.ai/api)
+- [JinaChat API](https://chat.jina.ai/api)
+
+> **Note:** Each secret is product-specific and cannot be interchanged. If you're planning to use multiple products, you'll need to generate a separate secret for each.
 
 ## Example Usage
 
-Import the SDK and instantiate a new client with your authentication tokens:
+Import the SDK and instantiate a new client with your authentication secrets:
 ```python
 from jinaai import JinaAI
 
 jinaai = new JinaAI(
-    tokens = {
-        'promptperfect-token': 'XXXXXX',
-        'scenex-token': 'XXXXXX',
-        'rationale-token': 'XXXXXX',
-        'chatcat-token': 'XXXXXX',
+    secrets = {
+        'promptperfect-secret': 'XXXXXX',
+        'scenex-secret': 'XXXXXX',
+        'rationale-secret': 'XXXXXX',
+        'jinachat-secret': 'XXXXXX',
     }
 )
 ```
 
 Describe images:
 ```python
 descriptions = jinaai.describe(
@@ -102,14 +97,27 @@
 
 swot = jinaai.decide(
     recommendation['output'],
     { 'analysis': 'swot' }
 )
 ```
 
+## Raw Output
+
+You can retrieve the raw output of each APIs by passing `raw: True` in the options:
+
+```python
+descriptions = jinaai.describe(
+    'https://picsum.photos/200',
+    { 'raw': True }
+)
+
+print(descriptions['raw'])
+```
+
 ## API Documentation
 
 <br/>
 
 ### JinaAi.describe
 
 ```python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jinaai-0.1.3/README.md` & `jinaai-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,54 @@
-# jinaai-py
+Metadata-Version: 2.1
+Name: jinaai
+Version: 0.2.0
+Summary: Jina AI Python SDK
+Home-page: https://github.com/jina-ai/jinaai-py.git
+Author: Jina AI
+Author-email: guillaume.roncari@jina.ai
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# JinaAI Python SDK
+
+The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products—SceneXplain, PromptPerfect, Rationale, and JinaChat—into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK enables users to effortlessly formulate and fine-tune prompts, thus streamlining application development.
 
-The JinaAI Python SDK is a powerful tool that seamlessly integrates the capabilities of JinaAI's products, including SceneXplain, PromptPerfect, Rationale and JinaChat into Python applications. This SDK acts as a robust wrapper around JinaAI's APIs, empowering users to create and optimize prompts effectively.
 
 ## Installing
 
 ### Package Manager
 
 Using pip:
 ```bash
 $ pip install jinaai
 ```
-## API Tokens
 
-Authenticate on each platforms and go on the API tab to generate an API token:
-- https://scenex.jina.ai
-- https://promptperfect.jina.ai
-- https://rationale.jina.ai
-- https://chat.jina.ai
+## API Secrets
+
+To generate an API secret, you need to authenticate on each respective platform and navigate to the API tab:
+
+- [SceneXplain API](https://scenex.jina.ai/api)
+- [PromptPerfect API](https://promptperfect.jina.ai/api)
+- [Rationale API](https://rationale.jina.ai/api)
+- [JinaChat API](https://chat.jina.ai/api)
+
+> **Note:** Each secret is product-specific and cannot be interchanged. If you're planning to use multiple products, you'll need to generate a separate secret for each.
 
 ## Example Usage
 
-Import the SDK and instantiate a new client with your authentication tokens:
+Import the SDK and instantiate a new client with your authentication secrets:
 ```python
 from jinaai import JinaAI
 
 jinaai = new JinaAI(
-    tokens = {
-        'promptperfect-token': 'XXXXXX',
-        'scenex-token': 'XXXXXX',
-        'rationale-token': 'XXXXXX',
-        'chatcat-token': 'XXXXXX',
+    secrets = {
+        'promptperfect-secret': 'XXXXXX',
+        'scenex-secret': 'XXXXXX',
+        'rationale-secret': 'XXXXXX',
+        'jinachat-secret': 'XXXXXX',
     }
 )
 ```
 
 Describe images:
 ```python
 descriptions = jinaai.describe(
@@ -92,14 +107,27 @@
 
 swot = jinaai.decide(
     recommendation['output'],
     { 'analysis': 'swot' }
 )
 ```
 
+## Raw Output
+
+You can retrieve the raw output of each APIs by passing `raw: True` in the options:
+
+```python
+descriptions = jinaai.describe(
+    'https://picsum.photos/200',
+    { 'raw': True }
+)
+
+print(descriptions['raw'])
+```
+
 ## API Documentation
 
 <br/>
 
 ### JinaAi.describe
 
 ```python
@@ -295,8 +323,8 @@
 ```python
 outout = JinaAI.utils.is_base64(input)
 ```
 
 >| VARIABLE                              | TYPE              | VALUE 
 >|---------------------------------------|-------------------|----------
 >| input                                 | str               | 
->| output                                | boolean           | 
+>| output                                | boolean           |
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jinaai-0.1.3/jinaai/__init__.py` & `jinaai-0.2.0/jinaai/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from .clients.SceneXClient import SceneXClient
 from .clients.PromptPerfectClient import PromptPerfectClient
 from .clients.RationaleClient import RationaleClient
-from .clients.ChatCatClient import ChatCatClient
+from .clients.JinaChatClient import JinaChatClient
 from .utils import is_url, is_base64, image_to_base64
 
 class JinaAI:
-    def __init__(self, tokens={}):
-        PPToken = f"token {tokens['promptperfect-token']}" if tokens else ''
-        SXToken = f"token {tokens['scenex-token']}" if tokens else ''
-        RAToken = f"token {tokens['rationale-token']}" if tokens else ''
-        CCToken = f"Bearer {tokens['chatcat-token']}" if tokens else ''
-        self.PPClient = PromptPerfectClient(headers = { "x-api-key": PPToken })
-        self.SXClient = SceneXClient(headers = { "x-api-key": SXToken })
-        self.RAClient = RationaleClient(headers = { "x-api-key": RAToken })
-        self.CCClient = ChatCatClient(headers = { "authorization": CCToken })
+    def __init__(self, secrets={}):
+        PPSecret = f"token {secrets['promptperfect-secret']}" if secrets else ''
+        SXSecret = f"token {secrets['scenex-secret']}" if secrets else ''
+        RASecret = f"token {secrets['rationale-secret']}" if secrets else ''
+        CCSecret = f"Bearer {secrets['jinachat-secret']}" if secrets else ''
+        self.PPClient = PromptPerfectClient(headers = { "x-api-key": PPSecret })
+        self.SXClient = SceneXClient(headers = { "x-api-key": SXSecret })
+        self.RAClient = RationaleClient(headers = { "x-api-key": RASecret })
+        self.CCClient = JinaChatClient(headers = { "authorization": CCSecret })
 
     def decide(self, input, options=None):
         if isinstance(input, list):
             data = self.RAClient.from_array(input, options)
         elif isinstance(input, str):
             data = self.RAClient.from_string(input, options)
         else:
```

### Comparing `jinaai-0.1.3/jinaai/clients/ChatCatClient.py` & `jinaai-0.2.0/jinaai/clients/JinaChatClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .HTTPClient import HTTPClient
 from ..utils import is_base64, is_url
 
 
-class ChatCatClient(HTTPClient):
+class JinaChatClient(HTTPClient):
     def __init__(self, headers=None):
         baseUrl = 'https://api-dyzugixgtq-uc.a.run.app/v1/chat'
         defaultHeaders = { 
             'Content-Type': 'application/json',
         }
         mergedHeaders = defaultHeaders.update(headers)
         super().__init__(baseUrl=baseUrl, headers=defaultHeaders)
```

### Comparing `jinaai-0.1.3/jinaai/clients/HTTPClient.py` & `jinaai-0.2.0/jinaai/clients/HTTPClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.3/jinaai/clients/PromptPerfectClient.py` & `jinaai-0.2.0/jinaai/clients/PromptPerfectClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.3/jinaai/clients/RationaleClient.py` & `jinaai-0.2.0/jinaai/clients/RationaleClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.3/jinaai/clients/SceneXClient.py` & `jinaai-0.2.0/jinaai/clients/SceneXClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.3/jinaai/utils.py` & `jinaai-0.2.0/jinaai/utils.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.3/jinaai.egg-info/PKG-INFO` & `jinaai-0.2.0/jinaai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 Metadata-Version: 2.1
 Name: jinaai
-Version: 0.1.3
+Version: 0.2.0
 Summary: Jina AI Python SDK
 Home-page: https://github.com/jina-ai/jinaai-py.git
 Author: Jina AI
 Author-email: guillaume.roncari@jina.ai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# jinaai-py
+# JinaAI Python SDK
+
+The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products—SceneXplain, PromptPerfect, Rationale, and JinaChat—into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK enables users to effortlessly formulate and fine-tune prompts, thus streamlining application development.
 
-The JinaAI Python SDK is a powerful tool that seamlessly integrates the capabilities of JinaAI's products, including SceneXplain, PromptPerfect, Rationale and JinaChat into Python applications. This SDK acts as a robust wrapper around JinaAI's APIs, empowering users to create and optimize prompts effectively.
 
 ## Installing
 
 ### Package Manager
 
 Using pip:
 ```bash
 $ pip install jinaai
 ```
-## API Tokens
 
-Authenticate on each platforms and go on the API tab to generate an API token:
-- https://scenex.jina.ai
-- https://promptperfect.jina.ai
-- https://rationale.jina.ai
-- https://chat.jina.ai
+## API Secrets
+
+To generate an API secret, you need to authenticate on each respective platform and navigate to the API tab:
+
+- [SceneXplain API](https://scenex.jina.ai/api)
+- [PromptPerfect API](https://promptperfect.jina.ai/api)
+- [Rationale API](https://rationale.jina.ai/api)
+- [JinaChat API](https://chat.jina.ai/api)
+
+> **Note:** Each secret is product-specific and cannot be interchanged. If you're planning to use multiple products, you'll need to generate a separate secret for each.
 
 ## Example Usage
 
-Import the SDK and instantiate a new client with your authentication tokens:
+Import the SDK and instantiate a new client with your authentication secrets:
 ```python
 from jinaai import JinaAI
 
 jinaai = new JinaAI(
-    tokens = {
-        'promptperfect-token': 'XXXXXX',
-        'scenex-token': 'XXXXXX',
-        'rationale-token': 'XXXXXX',
-        'chatcat-token': 'XXXXXX',
+    secrets = {
+        'promptperfect-secret': 'XXXXXX',
+        'scenex-secret': 'XXXXXX',
+        'rationale-secret': 'XXXXXX',
+        'jinachat-secret': 'XXXXXX',
     }
 )
 ```
 
 Describe images:
 ```python
 descriptions = jinaai.describe(
@@ -102,14 +107,27 @@
 
 swot = jinaai.decide(
     recommendation['output'],
     { 'analysis': 'swot' }
 )
 ```
 
+## Raw Output
+
+You can retrieve the raw output of each APIs by passing `raw: True` in the options:
+
+```python
+descriptions = jinaai.describe(
+    'https://picsum.photos/200',
+    { 'raw': True }
+)
+
+print(descriptions['raw'])
+```
+
 ## API Documentation
 
 <br/>
 
 ### JinaAi.describe
 
 ```python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

