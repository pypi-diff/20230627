# Comparing `tmp/ailingbot-0.0.3.tar.gz` & `tmp/ailingbot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailingbot-0.0.3.tar", max compression
+gzip compressed data, was "ailingbot-0.0.4.tar", max compression
```

## Comparing `ailingbot-0.0.3.tar` & `ailingbot-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,34 @@
--rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.3/LICENSE
--rw-r--r--   0        0        0     4761 2023-06-26 06:59:47.356194 ailingbot-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.3/ailingbot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.3/ailingbot/channels/__init__.py
--rw-r--r--   0        0        0     2387 2023-06-26 06:57:43.397704 ailingbot-0.0.3/ailingbot/channels/channel.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.3/ailingbot/channels/dingtalk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.3/ailingbot/channels/feishu/__init__.py
--rw-r--r--   0        0        0     5760 2023-06-26 06:57:43.398602 ailingbot-0.0.3/ailingbot/channels/feishu/agent.py
--rw-r--r--   0        0        0      736 2023-06-19 04:32:16.486131 ailingbot-0.0.3/ailingbot/channels/feishu/render.py
--rw-r--r--   0        0        0     6793 2023-06-26 06:57:43.399534 ailingbot-0.0.3/ailingbot/channels/feishu/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.3/ailingbot/channels/slack/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.3/ailingbot/channels/wechatwork/__init__.py
--rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.3/ailingbot/channels/wechatwork/agent.py
--rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.3/ailingbot/channels/wechatwork/encrypt.py
--rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.3/ailingbot/channels/wechatwork/render.py
--rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.3/ailingbot/channels/wechatwork/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.3/ailingbot/chat/__init__.py
--rw-r--r--   0        0        0     2076 2023-06-26 06:57:43.401435 ailingbot-0.0.3/ailingbot/chat/chatbot.py
--rw-r--r--   0        0        0     3487 2023-06-25 06:38:56.364334 ailingbot-0.0.3/ailingbot/chat/messages.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.3/ailingbot/chat/policies/__init__.py
--rw-r--r--   0        0        0     5759 2023-06-25 09:11:14.559103 ailingbot-0.0.3/ailingbot/chat/policies/langchain.py
--rw-r--r--   0        0        0     1678 2023-06-25 07:39:16.611374 ailingbot-0.0.3/ailingbot/chat/policy.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.3/ailingbot/cli/__init__.py
--rw-r--r--   0        0        0     8659 2023-06-26 06:57:43.402052 ailingbot-0.0.3/ailingbot/cli/cli.py
--rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.3/ailingbot/cli/options.py
--rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.3/ailingbot/cli/render.py
--rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.3/ailingbot/config.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.3/ailingbot/endpoint/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033407 ailingbot-0.0.3/ailingbot/repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033650 ailingbot-0.0.3/ailingbot/repositories/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.3/ailingbot/shared/__init__.py
--rw-r--r--   0        0        0     3953 2023-06-13 06:48:58.034885 ailingbot-0.0.3/ailingbot/shared/abc.py
--rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.3/ailingbot/shared/errors.py
--rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.3/ailingbot/shared/misc.py
--rw-r--r--   0        0        0     1071 2023-06-26 06:58:18.165938 ailingbot-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6243 1970-01-01 00:00:00.000000 ailingbot-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.4/LICENSE
+-rw-r--r--   0        0        0    19304 2023-06-27 07:53:22.469092 ailingbot-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.4/ailingbot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.4/ailingbot/channels/__init__.py
+-rw-r--r--   0        0        0     2444 2023-06-27 07:20:37.148547 ailingbot-0.0.4/ailingbot/channels/channel.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.4/ailingbot/channels/dingtalk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.4/ailingbot/channels/feishu/__init__.py
+-rw-r--r--   0        0        0     5760 2023-06-26 06:57:43.398602 ailingbot-0.0.4/ailingbot/channels/feishu/agent.py
+-rw-r--r--   0        0        0     1398 2023-06-27 07:03:48.368295 ailingbot-0.0.4/ailingbot/channels/feishu/render.py
+-rw-r--r--   0        0        0     7122 2023-06-27 07:22:31.063828 ailingbot-0.0.4/ailingbot/channels/feishu/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.4/ailingbot/channels/slack/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.4/ailingbot/channels/wechatwork/__init__.py
+-rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.4/ailingbot/channels/wechatwork/agent.py
+-rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.4/ailingbot/channels/wechatwork/encrypt.py
+-rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.4/ailingbot/channels/wechatwork/render.py
+-rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.4/ailingbot/channels/wechatwork/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.4/ailingbot/chat/__init__.py
+-rw-r--r--   0        0        0     2076 2023-06-26 06:57:43.401435 ailingbot-0.0.4/ailingbot/chat/chatbot.py
+-rw-r--r--   0        0        0     3487 2023-06-25 06:38:56.364334 ailingbot-0.0.4/ailingbot/chat/messages.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.4/ailingbot/chat/policies/__init__.py
+-rw-r--r--   0        0        0     5850 2023-06-27 07:20:37.223615 ailingbot-0.0.4/ailingbot/chat/policies/langchain.py
+-rw-r--r--   0        0        0     1678 2023-06-25 07:39:16.611374 ailingbot-0.0.4/ailingbot/chat/policy.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.4/ailingbot/cli/__init__.py
+-rw-r--r--   0        0        0     9231 2023-06-27 07:20:37.309101 ailingbot-0.0.4/ailingbot/cli/cli.py
+-rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.4/ailingbot/cli/options.py
+-rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.4/ailingbot/cli/render.py
+-rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.4/ailingbot/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.4/ailingbot/endpoint/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.4/ailingbot/shared/__init__.py
+-rw-r--r--   0        0        0     3953 2023-06-27 05:30:31.536603 ailingbot-0.0.4/ailingbot/shared/abc.py
+-rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.4/ailingbot/shared/errors.py
+-rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.4/ailingbot/shared/misc.py
+-rw-r--r--   0        0        0     1115 2023-06-27 08:59:52.998949 ailingbot-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    20872 1970-01-01 00:00:00.000000 ailingbot-0.0.4/PKG-INFO
```

### Comparing `ailingbot-0.0.3/LICENSE` & `ailingbot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/channels/channel.py` & `ailingbot-0.0.4/ailingbot/channels/channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,31 +49,33 @@
 
         :return: ASGI application.
         :rtype: typing.Union[ASGIApplication, typing.Callable]
         """
         raise NotImplementedError
 
     @staticmethod
-    async def get_webhook(name: str) -> ASGIApplication | typing.Callable:
+    async def get_webhook(
+        name: str, debug: bool = False
+    ) -> ASGIApplication | typing.Callable:
         """Gets channel webhook ASGI application instance.
 
         :param name: Built-in channel name or full path of webhook factory class.
         :type name: str
         :return: Webhook ASGI application.
         :rtype: typing.Union[ASGIApplication, typing.Callable]
         """
         if name.lower() == 'wechatwork':
             from ailingbot.channels.wechatwork.webhook import (
                 WechatworkWebhookFactory,
             )
 
-            factory = WechatworkWebhookFactory()
+            factory = WechatworkWebhookFactory(debug=debug)
         elif name.lower() == 'feishu':
             from ailingbot.channels.feishu.webhook import (
                 FeishuWebhookFactory,
             )
 
-            factory = FeishuWebhookFactory()
+            factory = FeishuWebhookFactory(debug=debug)
         else:
             factory = get_class_dynamically(name)()
 
         return await factory.create_webhook_app()
```

### Comparing `ailingbot-0.0.3/ailingbot/channels/feishu/agent.py` & `ailingbot-0.0.4/ailingbot/channels/feishu/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/channels/feishu/webhook.py` & `ailingbot-0.0.4/ailingbot/channels/feishu/webhook.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import json
 import typing
 
 from asgiref.typing import ASGIApplication
+from cachetools import LRUCache
 from fastapi import FastAPI, status, HTTPException
 from pydantic import BaseModel
 from starlette.background import BackgroundTasks
 
 from ailingbot.channels.channel import ChannelWebhookFactory
 from ailingbot.channels.feishu.agent import FeishuAgent
 from ailingbot.chat.chatbot import ChatBot
@@ -59,32 +60,38 @@
     header: typing.Optional[FeishuEventBodyHeader]
     event: typing.Optional[FeishuEventBodyEvent]
 
 
 class FeishuWebhookFactory(ChannelWebhookFactory):
     """Factory that creates Feishu webhook ASGI application."""
 
-    def __init__(self):
-        super(FeishuWebhookFactory, self).__init__()
+    def __init__(self, *, debug: bool = False):
+        super(FeishuWebhookFactory, self).__init__(debug=debug)
 
         self.verification_token = settings.channel.verification_token
 
         self.app: typing.Optional[ASGIApplication | typing.Callable] = None
         self.agent: typing.Optional[FeishuAgent] = None
         self.bot: typing.Optional[ChatBot] = None
+        self.event_id_cache: typing.Optional[LRUCache] = None
 
     async def create_webhook_app(self) -> ASGIApplication | typing.Callable:
         self.app = FastAPI()
         self.agent = FeishuAgent()
         self.bot = ChatBot(debug=self.debug)
+        self.event_id_cache = LRUCache(maxsize=1024)
 
         async def _chat_task(
             conversation_id: str, event: FeishuEventBody
         ) -> None:
             """Send a request message to the bot, receive a response message, and send it back to the user."""
+            if event.header.event_id in self.event_id_cache:
+                return
+            self.event_id_cache[event.header.event_id] = True
+
             if event.event.message.message_type == 'text':
                 req_msg = _create_text_request_message(event)
             elif event.event.message.message_type == 'file':
                 req_msg = await _create_file_request_message(event)
             else:
                 return
```

### Comparing `ailingbot-0.0.3/ailingbot/channels/wechatwork/agent.py` & `ailingbot-0.0.4/ailingbot/channels/wechatwork/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/channels/wechatwork/encrypt.py` & `ailingbot-0.0.4/ailingbot/channels/wechatwork/encrypt.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/channels/wechatwork/render.py` & `ailingbot-0.0.4/ailingbot/channels/wechatwork/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/channels/wechatwork/webhook.py` & `ailingbot-0.0.4/ailingbot/channels/wechatwork/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/chat/chatbot.py` & `ailingbot-0.0.4/ailingbot/chat/chatbot.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/chat/messages.py` & `ailingbot-0.0.4/ailingbot/chat/messages.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/chat/policies/langchain.py` & `ailingbot-0.0.4/ailingbot/chat/policies/langchain.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         return self.memories[conversation_id]
 
     async def respond(
         self, *, conversation_id: str, message: RequestMessage
     ) -> ResponseMessage:
         if not isinstance(message, TextRequestMessage):
             response = FallbackResponseMessage()
-            response.reason = 'LCConversationChatPolicy can only handle messages of type TextRequestMessage.'
+            response.reason = '不支持的消息类型'
         else:
             if conversation_id not in self.chain:
                 self.chain.memory = await self._load_memory(
                     conversation_id=conversation_id
                 )
             response = TextResponseMessage()
             response.text = await self.chain.arun(message.text)
@@ -93,33 +93,35 @@
         super(LCDocumentQAPolicy, self).__init__(
             debug=debug,
         )
 
         llm_config = copy.deepcopy(settings.policy.llm)
         self.llm = load_llm_from_config(llm_config)
         self.chains: dict[str, Chain] = {}
-        self.trunk_size = settings.policy.trunk_size or 1000
-        self.trunk_overlap = settings.policy.trunk_overlap or 0
+        self.chunk_size = settings.policy.chunk_size or 1000
+        self.chunk_overlap = settings.policy.chunk_overlap or 0
 
-    @staticmethod
     def _build_documents_index(
-        *, content: bytes, file_type: str
+        self, *, content: bytes, file_type: str
     ) -> VectorStoreRetriever:
         """Load document and build index."""
         if file_type.lower() != 'pdf':
             raise ailingbot.shared.errors.ChatPolicyError(
-                reason='Currently only PDF file are supported.',
+                reason='目前只支持PDF文档',
+                suggestion='请上传PDF文档',
             )
 
         with tempfile.NamedTemporaryFile(delete=True) as tf:
             tf.write(content)
             loader = PyPDFLoader(file_path=tf.name)
             documents = loader.load()
 
-        text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
+        text_splitter = CharacterTextSplitter(
+            chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
+        )
         texts = text_splitter.split_documents(documents)
 
         embeddings = OpenAIEmbeddings(
             openai_api_key=settings.policy.llm.openai_api_key,
         )
         docsearch = Chroma.from_documents(texts, embeddings)
 
@@ -127,34 +129,36 @@
 
     async def respond(
         self, *, conversation_id: str, message: RequestMessage
     ) -> ResponseMessage:
         if isinstance(message, TextRequestMessage):
             if conversation_id not in self.chains:
                 response = FallbackResponseMessage()
-                response.reason = 'Please upload the document first.'
+                response.reason = '还没有上传文档'
+                response.suggestion = '请先上传文档'
             else:
                 response = TextResponseMessage()
                 response.text = await self.chains[conversation_id].arun(
                     message.text
                 )
         elif isinstance(message, FileRequestMessage):
             self.chains[conversation_id] = RetrievalQA.from_chain_type(
                 llm=self.llm,
                 chain_type='stuff',
                 retriever=self._build_documents_index(
                     content=message.content, file_type=message.file_type
                 ),
                 return_source_documents=False,
+                verbose=self.debug,
             )
             response = TextResponseMessage()
-            response.text = f'I am ready! Please ask questions regarding the content of {message.file_name}.'
+            response.text = f'我已完成学习，现在可以针对 {message.file_name} 进行提问了'
         else:
             response = FallbackResponseMessage()
-            response.reason = 'Unsupported Request message type.'
+            response.reason = '不支持的消息类型'
 
         response.uuid = str(uuid.uuid4())
         response.ack_uuid = message.uuid
         response.receiver_id = message.sender_id
         response.scope = message.scope
         response.echo = message.echo
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ailingbot-0.0.3/ailingbot/chat/policy.py` & `ailingbot-0.0.4/ailingbot/chat/policy.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/cli/cli.py` & `ailingbot-0.0.4/ailingbot/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,22 +162,26 @@
 
 
 @command_line_tools.command(
     name='serve', help='Run webhook server to receive events.'
 )
 @options.log_level_option
 @options.log_file_option
+@click.option('--debug', is_flag=True, help='Enable debug mode.')
 @_coro_cmd
 async def serve(
     log_level: str,
     log_file: str,
+    debug: bool,
 ):
     _set_logger(sink=log_file, level=log_level)
 
-    webhook = await ChannelWebhookFactory.get_webhook(settings.channel.name)
+    webhook = await ChannelWebhookFactory.get_webhook(
+        settings.channel.name, debug=debug
+    )
 
     config = uvicorn.Config(app=webhook, **settings.uvicorn)
     server = uvicorn.Server(config)
     await server.serve()
 
 
 @command_line_tools.command(
@@ -259,26 +263,39 @@
     else:
         policy = await display_radio_prompt(
             title='Select chat policy:',
             values=[
                 (x, x)
                 for x in [
                     'lc_conversation',
+                    'lc_document_qa',
                     'Configure Later',
                 ]
             ],
             cancel_value='Configure Later',
         )
         if policy == 'lc_conversation':
             config['policy'] = {
                 'name': 'lc_conversation',
                 'history_size': 5,
                 'llm': {
                     '_type': 'openai',
-                    'model_name': 'gpt-3.5-turbo',
+                    'model_name': 'gpt-3.5-turbo-16k',
+                    'openai_api_key': '',
+                    'temperature': 0,
+                },
+            }
+        elif policy == 'lc_document_qa':
+            config['policy'] = {
+                'name': 'lc_document_qa',
+                'chunk_size': 1000,
+                'chunk_overlap': 0,
+                'llm': {
+                    '_type': 'openai',
+                    'model_name': 'gpt-3.5-turbo-16k',
                     'openai_api_key': '',
                     'temperature': 0,
                 },
             }
 
         channel = await display_radio_prompt(
             title='Select channel:',
```

### Comparing `ailingbot-0.0.3/ailingbot/cli/options.py` & `ailingbot-0.0.4/ailingbot/cli/options.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/cli/render.py` & `ailingbot-0.0.4/ailingbot/cli/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/config.py` & `ailingbot-0.0.4/ailingbot/config.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/shared/abc.py` & `ailingbot-0.0.4/ailingbot/shared/abc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/shared/errors.py` & `ailingbot-0.0.4/ailingbot/shared/errors.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/ailingbot/shared/misc.py` & `ailingbot-0.0.4/ailingbot/shared/misc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.3/pyproject.toml` & `ailingbot-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "ailingbot"
-version = "0.0.3"
-description = "An all-in-one solution to empower your IM bot with LLM."
+version = "0.0.4"
+description = "An all-in-one solution to empower your IM bot with AI."
 authors = ["ericzhang-cn <ericzhang.buaa@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 pydantic = "^1.10.2"
@@ -27,14 +27,16 @@
 langchain = "^0.0.214"
 openai = "^0.27.8"
 rich = "^13.4.2"
 tomlkit = "^0.11.8"
 chromadb = "^0.3.26"
 pypdf = "^3.11.0"
 tiktoken = "^0.4.0"
+sqlalchemy = "^2.0.17"
+cachetools = "^5.3.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 sphinx = "^5.3.0"
 pytest-asyncio = "^0.20.1"
 blue = "^0.9.1"
```

