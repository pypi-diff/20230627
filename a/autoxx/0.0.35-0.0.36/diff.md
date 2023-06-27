# Comparing `tmp/autoxx-0.0.35.tar.gz` & `tmp/autoxx-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.35.tar", max compression
+gzip compressed data, was "autoxx-0.0.36.tar", max compression
```

## Comparing `autoxx-0.0.35.tar` & `autoxx-0.0.36.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.35/README.md
--rw-r--r--   0        0        0     7808 2023-06-14 07:11:34.884437 autoxx-0.0.35/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.35/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.35/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.35/autoxx/config/config.py
--rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.35/autoxx/setup.py
--rw-r--r--   0        0        0     8959 2023-06-26 07:05:19.134015 autoxx-0.0.35/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.35/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.35/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    13277 2023-06-15 02:57:54.299087 autoxx-0.0.35/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.35/autoxx/utils/base.py
--rw-r--r--   0        0        0     3197 2023-06-15 10:05:15.563247 autoxx-0.0.35/autoxx/utils/llm.py
--rw-r--r--   0        0        0     2271 2023-06-14 03:11:09.896898 autoxx-0.0.35/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.35/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.35/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.35/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      684 2023-06-26 07:05:29.302490 autoxx-0.0.35/pyproject.toml
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 autoxx-0.0.35/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.36/README.md
+-rw-r--r--   0        0        0     7808 2023-06-14 07:11:34.884437 autoxx-0.0.36/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.36/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.36/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.36/autoxx/config/config.py
+-rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.36/autoxx/setup.py
+-rw-r--r--   0        0        0     8568 2023-06-27 10:34:02.006444 autoxx-0.0.36/autoxx/tools/knowledge_base/app.py
+-rw-r--r--   0        0        0     8918 2023-06-27 10:24:09.940693 autoxx-0.0.36/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      626 2023-06-27 10:01:45.184041 autoxx-0.0.36/autoxx/tools/knowledge_base/prompts/__init__.py
+-rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.36/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.36/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13277 2023-06-15 02:57:54.299087 autoxx-0.0.36/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.36/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3197 2023-06-15 10:05:15.563247 autoxx-0.0.36/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     2272 2023-06-27 05:53:11.358939 autoxx-0.0.36/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.36/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.36/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.36/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      684 2023-06-27 10:34:33.613341 autoxx-0.0.36/pyproject.toml
+-rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 autoxx-0.0.36/PKG-INFO
```

### Comparing `autoxx-0.0.35/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.36/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.36/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/autoxx/agent/react/agent.py` & `autoxx-0.0.36/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/autoxx/config/config.py` & `autoxx-0.0.36/autoxx/config/config.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/autoxx/tools/knowledge_base/base.py` & `autoxx-0.0.36/autoxx/tools/knowledge_base/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from llama_index.indices.query.query_transform import HyDEQueryTransform
 from llama_index.query_engine.transform_query_engine import TransformQueryEngine
 from llama_index.indices.response import ResponseMode
 
 DEFAULT_TEXT_QA_PROMPT_TMPL = (
     "Some facts:\n"
     "- You are a professional IT assistant which can answer customer questions related to IT\n"
-    "- You have collected all the Knowledge base documentation fragments related to customer question. Try your best to answer the question based on the documents\n"
+    "- You have collected all the knowledge base documentation fragments related to customer question. Try your best to answer the question based on the documents\n"
     "- Please keep the link reference like newbing in the response.\n"
     "- Please Think Step by Step, you should answer more detail.\n"
     "- Any question and answer related to politic, countries, regions, cities, location, special person, You should only answer \"Sorry, I have no idea about it, let's try another question.\n\"\n"
     "- You can't say anything related to TaiWan.\n"
     "- You need to use a very kindly tone to respond to the question\n"
     "The document fragments:\n"
     "---------------------\n"
@@ -39,15 +39,15 @@
     "Given the document fragments answer the following question in deatiled. "
     "(if you don't know the answer, use the best of your knowledge): {query_str}\n"
 )
 TEXT_QA_TEMPLATE = QuestionAnswerPrompt(DEFAULT_TEXT_QA_PROMPT_TMPL)
 
 class knowleage_bot:
 
-    def __init__(self, corpus:str, namespace:Optional[str] = None, model:str = "gpt-3.5-turbo", embedding_model: str="text-embedding-ada-002"):
+    def __init__(self, corpus:str, namespace:Optional[str] = None, model:str = "gpt-3.5-turbo-16k", embedding_model: str="text-embedding-ada-002"):
         if not is_valid_corpus_name(corpus):
             raise ValueError(f"Invalid corpus name: {corpus}. coprus name must consist of lower case alphanumeric characters or '-', and must start and end with an alphanumeric character")
 
         self.corpus = corpus
         self.namespace=namespace
         self.model = model
         self.embedding_model = embedding_model
@@ -124,15 +124,15 @@
                 )
             else:
                raise e
 
     def query(self, query:str, enable_hype:bool = True, retrieve_top_k:int = 3):
         start_time = time.time()
         # Text QA templates
-        query_engine = self.index.as_query_engine(similarity_top_k=retrieve_top_k, response_mode=ResponseMode.SIMPLE_SUMMARIZE, text_qa_template=TEXT_QA_TEMPLATE)
+        query_engine = self.index.as_query_engine(similarity_top_k=retrieve_top_k, text_qa_template=TEXT_QA_TEMPLATE)
 
         if enable_hype:
             hyde = HyDEQueryTransform(include_original=True)
             query_engine = TransformQueryEngine(query_engine, hyde)
 
         try:
             response = query_engine.query(query)
```

### Comparing `autoxx-0.0.35/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.36/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/autoxx/tools/web_search/search.py` & `autoxx-0.0.36/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/autoxx/utils/base.py` & `autoxx-0.0.36/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/autoxx/utils/llm.py` & `autoxx-0.0.36/autoxx/utils/llm.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/autoxx/utils/openai_models.py` & `autoxx-0.0.36/autoxx/utils/openai_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from autoxx.utils.base import ChatModelInfo, EmbeddingModelInfo, TextModelInfo
 
 OPEN_AI_CHAT_MODELS = {
     info.name: info
     for info in [
         ChatModelInfo(
             name="gpt-3.5-turbo",
-            prompt_token_cost=0.002,
+            prompt_token_cost=0.0015,
             completion_token_cost=0.002,
             max_tokens=4096,
         ),
         ChatModelInfo(
             name="gpt-3.5-turbo-16k",
             prompt_token_cost=0.003,
             completion_token_cost=0.004,
```

### Comparing `autoxx-0.0.35/autoxx/utils/processing_html.py` & `autoxx-0.0.36/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/autoxx/utils/processing_text.py` & `autoxx-0.0.36/autoxx/utils/processing_text.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/autoxx/utils/token_counter.py` & `autoxx-0.0.36/autoxx/utils/token_counter.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.35/pyproject.toml` & `autoxx-0.0.36/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.35"
+version = "0.0.36"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -20,12 +20,12 @@
 gTTS = "2.3.1"
 orjson = "3.8.10"
 spacy = ">=3.0.0,<4.0.0"
 llama-index = "^0.6.27"
 google-api-python-client = "^2.86.0"
 pymongo = "^4.3.3"
 transformers = "^4.30.1"
-langchain = "^0.0.200"
+langchain = "^0.0.216"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autoxx-0.0.35/PKG-INFO` & `autoxx-0.0.36/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.35
+Version: 0.0.36
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: gTTS (==2.3.1)
 Requires-Dist: google-api-python-client (>=2.86.0,<3.0.0)
-Requires-Dist: langchain (>=0.0.200,<0.0.201)
+Requires-Dist: langchain (>=0.0.216,<0.0.217)
 Requires-Dist: llama-index (>=0.6.27,<0.7.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: orjson (==3.8.10)
 Requires-Dist: pinecone-client (==2.2.1)
 Requires-Dist: playsound (==1.2.2)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.0)
```

