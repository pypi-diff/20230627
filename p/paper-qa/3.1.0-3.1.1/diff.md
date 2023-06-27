# Comparing `tmp/paper-qa-3.1.0.tar.gz` & `tmp/paper-qa-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.1.0.tar", last modified: Fri Jun 16 15:34:54 2023, max compression
+gzip compressed data, was "paper-qa-3.1.1.tar", last modified: Tue Jun 27 01:29:07 2023, max compression
```

## Comparing `paper-qa-3.1.0.tar` & `paper-qa-3.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:34:54.380644 paper-qa-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 15:34:17.000000 paper-qa-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-16 15:34:54.380644 paper-qa-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-16 15:34:17.000000 paper-qa-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:34:54.376644 paper-qa-3.1.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-16 15:34:54.000000 paper-qa-3.1.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 15:34:54.000000 paper-qa-3.1.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:34:54.000000 paper-qa-3.1.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 15:34:54.000000 paper-qa-3.1.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 15:34:54.000000 paper-qa-3.1.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:34:54.376644 paper-qa-3.1.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:34:54.380644 paper-qa-3.1.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22435 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 15:34:17.000000 paper-qa-3.1.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:34:54.380644 paper-qa-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-16 15:34:17.000000 paper-qa-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:34:54.380644 paper-qa-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20285 2023-06-16 15:34:17.000000 paper-qa-3.1.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:29:07.568499 paper-qa-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 01:28:22.000000 paper-qa-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-27 01:29:07.568499 paper-qa-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-27 01:28:22.000000 paper-qa-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:29:07.564499 paper-qa-3.1.1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-27 01:29:07.000000 paper-qa-3.1.1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 01:29:07.000000 paper-qa-3.1.1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 01:29:07.000000 paper-qa-3.1.1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 01:29:07.000000 paper-qa-3.1.1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 01:29:07.000000 paper-qa-3.1.1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:29:07.568499 paper-qa-3.1.1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:29:07.568499 paper-qa-3.1.1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22564 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 01:28:22.000000 paper-qa-3.1.1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 01:29:07.568499 paper-qa-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-27 01:28:22.000000 paper-qa-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:29:07.568499 paper-qa-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-06-27 01:28:22.000000 paper-qa-3.1.1/tests/test_paperqa.py
```

### Comparing `paper-qa-3.1.0/LICENSE` & `paper-qa-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.0/PKG-INFO` & `paper-qa-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.1.0
+Version: 3.1.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.1.0/README.md` & `paper-qa-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.1.1/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.1.0
+Version: 3.1.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.1.0/paperqa/chains.py` & `paper-qa-3.1.1/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.0/paperqa/contrib/zotero.py` & `paper-qa-3.1.1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.0/paperqa/docs.py` & `paper-qa-3.1.1/paperqa/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,19 +242,21 @@
             text_embeddings = self.embeddings.embed_documents([t.text for t in texts])
             for i, t in enumerate(texts):
                 t.embeddings = text_embeddings[i]
         else:
             text_embeddings = cast(List[List[float]], [t.embeddings for t in texts])
         if self.texts_index is not None:
             try:
+                # TODO: Simplify - super weird
+                vec_store_text_and_embeddings = list(
+                    map(lambda x: (x.text, x.embeddings), texts)
+                )
                 self.texts_index.add_embeddings(  # type: ignore
-                    list(zip(texts, text_embeddings)),
-                    metadatas=[
-                        t.dict(exclude={"embeddings", "text"}) for t in self.texts
-                    ],
+                    vec_store_text_and_embeddings,
+                    metadatas=[t.dict(exclude={"embeddings", "text"}) for t in texts],
                 )
             except AttributeError:
                 raise ValueError("Need a vector store that supports adding embeddings.")
         if self.doc_index is not None:
             self.doc_index.add_texts([doc.citation], metadatas=[{"dockey": doc.dockey}])
         self.docs[doc.dockey] = doc
         self.texts += texts
```

### Comparing `paper-qa-3.1.0/paperqa/prompts.py` & `paper-qa-3.1.1/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.0/paperqa/readers.py` & `paper-qa-3.1.1/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.0/paperqa/types.py` & `paper-qa-3.1.1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.0/paperqa/utils.py` & `paper-qa-3.1.1/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.1.0/setup.py` & `paper-qa-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,7 @@
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
-
```

### Comparing `paper-qa-3.1.0/tests/test_paperqa.py` & `paper-qa-3.1.1/tests/test_paperqa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import pickle
 from io import BytesIO
 from typing import Any
 from unittest import IsolatedAsyncioTestCase
 
+import numpy as np
 import requests
 from langchain.callbacks.base import AsyncCallbackHandler
 from langchain.llms import OpenAI
 from langchain.llms.fake import FakeListLLM
 from langchain.prompts import PromptTemplate
 
-from paperqa import Answer, Docs, PromptCollection
+from paperqa import Answer, Docs, PromptCollection, Text
 from paperqa.readers import read_doc
 from paperqa.types import Doc
 from paperqa.utils import maybe_is_html, maybe_is_text, name_in_text, strings_similarity
 
 
 class TestHandler(AsyncCallbackHandler):
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
@@ -404,23 +405,24 @@
     docs = Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     # add with new dockey
     with open("example.txt", "w", encoding="utf-8") as f:
         f.write(r.text)
         f.write("\n\nBates could be from Angola")  # so we don't have same hash
     docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", dockey="test")
-    answer = Answer(question="What country is Bates from?")
+    answer = Answer(question="What country was Bates born in?")
     answer = docs.get_evidence(answer, marginal_relevance=False)
+    print(answer)
     keys = set([c.text.doc.dockey for c in answer.contexts])
     assert len(keys) == 2
     assert len(docs.docs) == 2
 
     docs.delete(dockey="test")
     assert len(docs.docs) == 1
-    answer = Answer(question="What country is Bates from?")
+    answer = Answer(question="What country was Bates born in?")
     answer = docs.get_evidence(answer, marginal_relevance=False)
     keys = set([c.text.doc.dockey for c in answer.contexts])
     assert len(keys) == 1
 
 
 def test_query_filter():
     """Test that we can filter evidence with in query"""
@@ -502,15 +504,15 @@
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     answer = docs.query("What country is Bates from?")
     print(answer.answer)
-    assert "United States" == answer.answer
+    assert "United States" in answer.answer
 
 
 def test_pre_prompt():
     pre = PromptTemplate(
         input_variables=["question"],
         template="Provide context you have memorized "
         "that could help answer '{question}'. ",
@@ -571,7 +573,44 @@
     answer3 = docs.query("When was the conflict resolved?")
     assert answer3.memory is not None
     assert (
         "I cannot answer" in answer3.answer
         or "insufficient" in answer3.answer
         or "does not provide" in answer3.answer
     )
+
+
+def test_add_texts():
+    llm = OpenAI(client=None, temperature=0.1, model="text-ada-001")
+    docs = Docs(llm=llm)
+    docs.add_url(
+        "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test",
+    )
+
+    docs2 = Docs(llm=llm)
+    texts = [Text(**dict(t)) for t in docs.texts]
+    for t in texts:
+        t.embeddings = None
+    docs2.add_texts(texts, list(docs.docs.values())[0])
+
+    for t1, t2 in zip(docs2.texts, docs.texts):
+        assert t1.text == t2.text
+        assert np.allclose(t1.embeddings, t2.embeddings, atol=1e-3)
+
+    docs2._build_texts_index()
+    print("BUILT NOW")
+    # now do it again to test after text index is already built
+    llm = OpenAI(client=None, temperature=0.1, model="text-ada-001")
+    docs = Docs(llm=llm)
+    docs.add_url(
+        "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test3",
+    )
+
+    texts = [Text(**dict(t)) for t in docs.texts]
+    for t in texts:
+        t.embeddings = None
+    docs2.add_texts(texts, list(docs.docs.values())[0])
+    assert len(docs2.docs) == 2
```

