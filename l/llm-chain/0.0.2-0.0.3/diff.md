# Comparing `tmp/llm-chain-0.0.2.tar.gz` & `tmp/llm-chain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-chain-0.0.2.tar", last modified: Mon Jun 26 21:19:21 2023, max compression
+gzip compressed data, was "llm-chain-0.0.3.tar", last modified: Tue Jun 27 00:17:02 2023, max compression
```

## Comparing `llm-chain-0.0.2.tar` & `llm-chain-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:19:21.561850 llm-chain-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-02-25 17:02:25.000000 llm-chain-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7647 2023-06-26 21:19:21.562898 llm-chain-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7119 2023-06-26 21:13:57.000000 llm-chain-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:19:21.504820 llm-chain-0.0.2/llm_chain/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-09 17:08:19.000000 llm-chain-0.0.2/llm_chain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13569 2023-06-26 17:26:17.000000 llm-chain-0.0.2/llm_chain/base.py
--rw-r--r--   0 root         (0) root         (0)     2577 2023-06-26 01:19:40.000000 llm-chain-0.0.2/llm_chain/indexes.py
--rw-r--r--   0 root         (0) root         (0)     1253 2023-06-26 16:49:38.000000 llm-chain-0.0.2/llm_chain/memory.py
--rw-r--r--   0 root         (0) root         (0)     6458 2023-06-24 02:02:59.000000 llm-chain-0.0.2/llm_chain/models.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-06-26 01:19:59.000000 llm-chain-0.0.2/llm_chain/prompt_templates.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-14 02:06:25.000000 llm-chain-0.0.2/llm_chain/resources.py
--rw-r--r--   0 root         (0) root         (0)     2714 2023-06-26 00:25:02.000000 llm-chain-0.0.2/llm_chain/tools.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-06-23 02:34:10.000000 llm-chain-0.0.2/llm_chain/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:19:21.524264 llm-chain-0.0.2/llm_chain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7647 2023-06-26 21:19:21.000000 llm-chain-0.0.2/llm_chain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-06-26 21:19:21.000000 llm-chain-0.0.2/llm_chain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 21:19:21.000000 llm-chain-0.0.2/llm_chain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-26 21:19:21.000000 llm-chain-0.0.2/llm_chain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-26 21:19:21.000000 llm-chain-0.0.2/llm_chain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-25 17:02:25.000000 llm-chain-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-26 21:19:21.565098 llm-chain-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:19:21.559354 llm-chain-0.0.2/tests/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-10 00:17:26.000000 llm-chain-0.0.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4281 2023-06-24 02:22:45.000000 llm-chain-0.0.2/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)    23562 2023-06-26 01:05:52.000000 llm-chain-0.0.2/tests/test_chains.py
--rw-r--r--   0 root         (0) root         (0)    11370 2023-06-26 17:14:59.000000 llm-chain-0.0.2/tests/test_indexes.py
--rw-r--r--   0 root         (0) root         (0)    13991 2023-06-26 16:57:51.000000 llm-chain-0.0.2/tests/test_memory.py
--rw-r--r--   0 root         (0) root         (0)    26878 2023-06-26 17:13:47.000000 llm-chain-0.0.2/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-06-23 05:43:22.000000 llm-chain-0.0.2/tests/test_prompt_templates.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-06-14 02:16:47.000000 llm-chain-0.0.2/tests/test_records.py
--rw-r--r--   0 root         (0) root         (0)    13510 2023-06-26 00:34:09.000000 llm-chain-0.0.2/tests/test_tools.py
--rw-r--r--   0 root         (0) root         (0)     3408 2023-06-26 17:18:37.000000 llm-chain-0.0.2/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:17:02.446094 llm-chain-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-02-25 17:02:25.000000 llm-chain-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10350 2023-06-27 00:17:02.447234 llm-chain-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9822 2023-06-26 22:06:13.000000 llm-chain-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:17:02.386967 llm-chain-0.0.3/llm_chain/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-09 17:08:19.000000 llm-chain-0.0.3/llm_chain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15474 2023-06-27 00:14:54.000000 llm-chain-0.0.3/llm_chain/base.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-06-26 01:19:40.000000 llm-chain-0.0.3/llm_chain/indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-06-26 16:49:38.000000 llm-chain-0.0.3/llm_chain/memory.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2023-06-26 22:47:09.000000 llm-chain-0.0.3/llm_chain/models.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-06-26 23:23:59.000000 llm-chain-0.0.3/llm_chain/prompt_templates.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-14 02:06:25.000000 llm-chain-0.0.3/llm_chain/resources.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2023-06-26 00:25:02.000000 llm-chain-0.0.3/llm_chain/tools.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-06-23 02:34:10.000000 llm-chain-0.0.3/llm_chain/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:17:02.405178 llm-chain-0.0.3/llm_chain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10350 2023-06-27 00:17:02.000000 llm-chain-0.0.3/llm_chain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      642 2023-06-27 00:17:02.000000 llm-chain-0.0.3/llm_chain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 00:17:02.000000 llm-chain-0.0.3/llm_chain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-27 00:17:02.000000 llm-chain-0.0.3/llm_chain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-27 00:17:02.000000 llm-chain-0.0.3/llm_chain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-02-25 17:02:25.000000 llm-chain-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-27 00:17:02.449079 llm-chain-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 00:17:02.443968 llm-chain-0.0.3/tests/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-10 00:17:26.000000 llm-chain-0.0.3/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4281 2023-06-24 02:22:45.000000 llm-chain-0.0.3/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    23550 2023-06-26 23:23:05.000000 llm-chain-0.0.3/tests/test_chains.py
+-rw-r--r--   0 root         (0) root         (0)    11370 2023-06-26 17:14:59.000000 llm-chain-0.0.3/tests/test_indexes.py
+-rw-r--r--   0 root         (0) root         (0)    13991 2023-06-26 16:57:51.000000 llm-chain-0.0.3/tests/test_memory.py
+-rw-r--r--   0 root         (0) root         (0)    26878 2023-06-26 17:13:47.000000 llm-chain-0.0.3/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-06-23 05:43:22.000000 llm-chain-0.0.3/tests/test_prompt_templates.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-06-14 02:16:47.000000 llm-chain-0.0.3/tests/test_records.py
+-rw-r--r--   0 root         (0) root         (0)     5349 2023-06-27 00:13:32.000000 llm-chain-0.0.3/tests/test_session.py
+-rw-r--r--   0 root         (0) root         (0)    13510 2023-06-26 00:34:09.000000 llm-chain-0.0.3/tests/test_tools.py
+-rw-r--r--   0 root         (0) root         (0)     3408 2023-06-26 17:18:37.000000 llm-chain-0.0.3/tests/test_utilities.py
```

### Comparing `llm-chain-0.0.2/LICENSE` & `llm-chain-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/PKG-INFO` & `llm-chain-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-chain
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple and extensible LLM Chaining
 Home-page: https://github.com/shane-kercheval/llm-chain
 Author: Shane Kercheval
 Author-email: shane.kercheval@gmail.com
 Project-URL: Bug Tracker, https://github.com/shane-kercheval/llm-chain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,20 +15,80 @@
 
 # `llm-chain`: simple and extensible LLM chaining
 
 A `chain` consists of `links`. Each link in the chain is a callable, which can be either a function or an object that implements the `__call__` method. **The output of one link serves as the input to the next link in the chain.** Pretty simple.
 
 Additionally, each link can track its own history, including messages sent/received and token usage/costs, through a `history` property that returns a list of `Record` objects. A `chain` aggregates and propagates the history of any link that has a `history` property, making it convenient to analyze costs or explore intermediate steps in the chain.
 
-**Note: This package is tested on Python versions 3.10 and 3.11**
+Here's a simple example:
+
+- Ask the chat model a question ("What is the meaning of life?")
+- The model responds, and the response is sent to the next link, which creates and returns a new prompt indicating that the link's input (which is the output from the last link; i.e. the model's response) should be summarized in two sentences.
+- The new prompt is sent to the next link, which is the chat model, and the response is returned.
+
+```python
+from llm_chain.base import Chain
+from llm_chain.models import OpenAIChat
+
+chat_model = OpenAIChat(model_name='gpt-3.5-turbo')
+chain = Chain(links=[
+    chat_model,
+    lambda x: f"Summarize the following in two sentences: ```{x}```",
+    chat_model,
+])
+chain("What is the meaning of life?")
+```
+
+Response:
+
+```
+The meaning of life is a philosophical question that has been debated for centuries with no definitive answer. It varies depending on one's beliefs, values, and experiences and is ultimately a personal and subjective concept."
+```
+
+Total costs/tokens for all activity in the chain:
+
+```python
+print(f"Cost:   ${chain.cost:.4f}")
+print(f"Tokens: {chain.total_tokens:,}")
+```
+
+Output:
+
+```
+Cost:   $0.0007
+Tokens: 395
+```
+
+Message History:
+
+```python
+print(chain.message_history[0].prompt)
+print(chain.message_history[0].response)
+print(chain.message_history[1].prompt)
+print(chain.message_history[1].response)
+```
+
+Output:
+
+```
+What is the meaning of life?
+
+The meaning of life is a philosophical question that has been debated by scholars, theologians, and philosophers for centuries. There is no one definitive answer to this question, as it can vary depending on one's beliefs, values, and experiences. Some people believe that the meaning of life is to seek happiness, while others believe it is to fulfill a specific purpose or destiny. Ultimately, the meaning of life is a personal and subjective concept that each individual must determine for themselves.
+
+Summarize the following in two sentences: ```The meaning of life is a philosophical question that has been debated by scholars, theologians, and philosophers for centuries. There is no one definitive answer to this question, as it can vary depending on one's beliefs, values, and experiences. Some people believe that the meaning of life is to seek happiness, while others believe it is to fulfill a specific purpose or destiny. Ultimately, the meaning of life is a personal and subjective concept that each individual must determine for themselves.```
+
+The meaning of life is a philosophical question that has been debated for centuries with no definitive answer. It varies depending on one's beliefs, values, and experiences and is ultimately a personal and subjective concept.
+```
 
 ---
 
 # Installing
 
+**Note: This package is tested on Python versions 3.10 and 3.11**
+
 ```commandline
 pip install llm-chain
 ```
 
 ---
 
 # Examples
```

### Comparing `llm-chain-0.0.2/README.md` & `llm-chain-0.0.3/llm_chain.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,94 @@
+Metadata-Version: 2.1
+Name: llm-chain
+Version: 0.0.3
+Summary: Simple and extensible LLM Chaining
+Home-page: https://github.com/shane-kercheval/llm-chain
+Author: Shane Kercheval
+Author-email: shane.kercheval@gmail.com
+Project-URL: Bug Tracker, https://github.com/shane-kercheval/llm-chain/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # `llm-chain`: simple and extensible LLM chaining
 
 A `chain` consists of `links`. Each link in the chain is a callable, which can be either a function or an object that implements the `__call__` method. **The output of one link serves as the input to the next link in the chain.** Pretty simple.
 
 Additionally, each link can track its own history, including messages sent/received and token usage/costs, through a `history` property that returns a list of `Record` objects. A `chain` aggregates and propagates the history of any link that has a `history` property, making it convenient to analyze costs or explore intermediate steps in the chain.
 
-**Note: This package is tested on Python versions 3.10 and 3.11**
+Here's a simple example:
+
+- Ask the chat model a question ("What is the meaning of life?")
+- The model responds, and the response is sent to the next link, which creates and returns a new prompt indicating that the link's input (which is the output from the last link; i.e. the model's response) should be summarized in two sentences.
+- The new prompt is sent to the next link, which is the chat model, and the response is returned.
+
+```python
+from llm_chain.base import Chain
+from llm_chain.models import OpenAIChat
+
+chat_model = OpenAIChat(model_name='gpt-3.5-turbo')
+chain = Chain(links=[
+    chat_model,
+    lambda x: f"Summarize the following in two sentences: ```{x}```",
+    chat_model,
+])
+chain("What is the meaning of life?")
+```
+
+Response:
+
+```
+The meaning of life is a philosophical question that has been debated for centuries with no definitive answer. It varies depending on one's beliefs, values, and experiences and is ultimately a personal and subjective concept."
+```
+
+Total costs/tokens for all activity in the chain:
+
+```python
+print(f"Cost:   ${chain.cost:.4f}")
+print(f"Tokens: {chain.total_tokens:,}")
+```
+
+Output:
+
+```
+Cost:   $0.0007
+Tokens: 395
+```
+
+Message History:
+
+```python
+print(chain.message_history[0].prompt)
+print(chain.message_history[0].response)
+print(chain.message_history[1].prompt)
+print(chain.message_history[1].response)
+```
+
+Output:
+
+```
+What is the meaning of life?
+
+The meaning of life is a philosophical question that has been debated by scholars, theologians, and philosophers for centuries. There is no one definitive answer to this question, as it can vary depending on one's beliefs, values, and experiences. Some people believe that the meaning of life is to seek happiness, while others believe it is to fulfill a specific purpose or destiny. Ultimately, the meaning of life is a personal and subjective concept that each individual must determine for themselves.
+
+Summarize the following in two sentences: ```The meaning of life is a philosophical question that has been debated by scholars, theologians, and philosophers for centuries. There is no one definitive answer to this question, as it can vary depending on one's beliefs, values, and experiences. Some people believe that the meaning of life is to seek happiness, while others believe it is to fulfill a specific purpose or destiny. Ultimately, the meaning of life is a personal and subjective concept that each individual must determine for themselves.```
+
+The meaning of life is a philosophical question that has been debated for centuries with no definitive answer. It varies depending on one's beliefs, values, and experiences and is ultimately a personal and subjective concept.
+```
 
 ---
 
 # Installing
 
+**Note: This package is tested on Python versions 3.10 and 3.11**
+
 ```commandline
 pip install llm-chain
 ```
 
 ---
 
 # Examples
```

### Comparing `llm-chain-0.0.2/llm_chain/base.py` & `llm-chain-0.0.3/llm_chain/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,15 +333,62 @@
     def __call__(self, value: object | None = None) -> object:
         """TODO."""
         if value:
             self.value = value
         return self.value
 
 
-class Chain:
+class LinkAggregator(ABC):
+    """TODO."""
+
+    @property
+    @abstractmethod
+    def history(self) -> list[Record]:
+        """TODO."""
+
+    @property
+    def usage_history(self) -> list[UsageRecord]:
+        """TODO."""
+        return [x for x in self.history if isinstance(x, UsageRecord)]
+
+    @property
+    def message_history(self) -> list[UsageRecord]:
+        """TODO."""
+        return [x for x in self.history if isinstance(x, MessageRecord)]
+
+    @property
+    def total_tokens(self) -> int | None:
+        """
+        Returns the total number of tokens used by the all models during the chain/object's
+        lifetime.
+
+        Returns `None` if none of the models knows how to count tokens.
+        """
+        records = self.usage_history
+        totals = [x.total_tokens for x in records if x.total_tokens]
+        if not totals:
+            return None
+        return sum(totals)
+
+    @property
+    def cost(self) -> float | None:
+        """
+        Returns the total number of cost used by the all models during the chain/object's
+        lifetime.
+
+        Returns `None` if none of the models knows how to count cost.
+        """
+        records = self.usage_history
+        totals = [x.cost for x in records if x.cost]
+        if not totals:
+            return None
+        return sum(totals)
+
+
+class Chain(LinkAggregator):
     """TODO."""
 
     def __init__(self, links: list[Callable[[Any], Any]]):
         self._links = links
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:  # noqa: ANN401
         """TODO."""
@@ -373,51 +420,57 @@
         for history in histories:
             for record in history:
                 if record.uuid not in unique_uuids:
                     unique_records.append(record)
                     unique_uuids |= {record.uuid}
         return sorted(unique_records, key=lambda x: x.timestamp)
 
-    @property
-    def usage_history(self) -> list[UsageRecord]:
-        """TODO."""
-        return [x for x in self.history if isinstance(x, UsageRecord)]
 
-    @property
-    def message_history(self) -> list[UsageRecord]:
+class Session(LinkAggregator):
+    """
+    TODO: A session is a way to aggregate the history of chains, calling a session will call
+    the last chain added to the session.
+    """
+
+    def __init__(self, chains: list[Chain] | None = None):
+        self._chains = chains or []
+
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:  # noqa: ANN401
         """TODO."""
-        return [x for x in self.history if isinstance(x, MessageRecord)]
+        if self._chains:
+            return self._chains[-1](*args, **kwargs)
+        raise ValueError()
 
-    @property
-    def total_tokens(self) -> int | None:
-        """
-        Returns the total number of tokens used by the all models during the chain/object's
-        lifetime.
+    def append(self, chain: Chain) -> None:
+        """TODO."""
+        self._chains.append(chain)
 
-        Returns `None` if none of the models knows how to count tokens.
-        """
-        records = self.usage_history
-        totals = [x.total_tokens for x in records if x.total_tokens]
-        if not totals:
-            return None
-        return sum(totals)
+    def __len__(self) -> int:
+        return len(self._chains)
 
     @property
-    def cost(self) -> float | None:
-        """
-        Returns the total number of cost used by the all models during the chain/object's
-        lifetime.
-
-        Returns `None` if none of the models knows how to count cost.
-        """
-        records = self.usage_history
-        totals = [x.cost for x in records if x.cost]
-        if not totals:
-            return None
-        return sum(totals)
+    def history(self) -> list[Record]:
+        """TODO."""
+        # for each history in chain, cycle through each link's history and add to the list of
+        # records if it hasn't already been added.
+        chains = [chain for chain in self._chains if chain.history]
+        # Edge-case: if the same model is used multiple times in the same chain or across different
+        # links (e.g. embedding
+        # model to embed documents and then embed query to search documents) then we can't loop
+        # through the chains because we'd be double-counting the history from those objects.
+        # we have to build up a history and include the objects if they aren't already
+        # to do this we'll use the uuid, and then sort by timestamp
+        unique_records = []
+        unique_uuids = set()
+        for chain in chains:
+            for record in chain.history:
+                if record.uuid not in unique_uuids:
+                    unique_records.append(record)
+                    unique_uuids |= {record.uuid}
+        return sorted(unique_records, key=lambda x: x.timestamp)
 
 
 def _has_history(obj: object) -> bool:
     """TODO."""
     return _has_property(obj, property_name='history') and \
         isinstance(obj.history, list) and \
         len(obj.history) > 0 and \
```

### Comparing `llm-chain-0.0.2/llm_chain/indexes.py` & `llm-chain-0.0.3/llm_chain/indexes.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/llm_chain/memory.py` & `llm-chain-0.0.3/llm_chain/memory.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/llm_chain/models.py` & `llm-chain-0.0.3/llm_chain/models.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/llm_chain/prompt_templates.py` & `llm-chain-0.0.3/llm_chain/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/llm_chain/resources.py` & `llm-chain-0.0.3/llm_chain/resources.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/llm_chain/tools.py` & `llm-chain-0.0.3/llm_chain/tools.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/llm_chain/utilities.py` & `llm-chain-0.0.3/llm_chain/utilities.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/llm_chain.egg-info/SOURCES.txt` & `llm-chain-0.0.3/llm_chain.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 tests/conftest.py
 tests/test_chains.py
 tests/test_indexes.py
 tests/test_memory.py
 tests/test_models.py
 tests/test_prompt_templates.py
 tests/test_records.py
+tests/test_session.py
 tests/test_tools.py
 tests/test_utilities.py
```

### Comparing `llm-chain-0.0.2/setup.cfg` & `llm-chain-0.0.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = llm-chain
-version = 0.0.2
+version = 0.0.3
 author = Shane Kercheval
 author_email = shane.kercheval@gmail.com
 description = Simple and extensible LLM Chaining
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shane-kercheval/llm-chain
 project_urls =
```

### Comparing `llm-chain-0.0.2/tests/conftest.py` & `llm-chain-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/tests/test_chains.py` & `llm-chain-0.0.3/tests/test_chains.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
         mock_records.record_b.total_tokens + \
         mock_records.record_c.total_tokens
     assert chain.cost == mock_records.record_a.cost + \
         mock_records.record_b.cost + \
         mock_records.record_c.cost
 
 def test_usage_history_no_usage():  # noqa
-    sum([])
     mock_records = MockNoUsageRecords()
     mock_wrapper = MockHistoryWrapper(hist_obj=mock_records)
     # make sure historical records are only counted once
     chain = Chain(links=[mock_records, mock_wrapper, mock_records])
     records = chain.usage_history
     assert len(records) == 3
     assert records[0] == mock_records.record_a
```

### Comparing `llm-chain-0.0.2/tests/test_indexes.py` & `llm-chain-0.0.3/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/tests/test_memory.py` & `llm-chain-0.0.3/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/tests/test_models.py` & `llm-chain-0.0.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/tests/test_prompt_templates.py` & `llm-chain-0.0.3/tests/test_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/tests/test_records.py` & `llm-chain-0.0.3/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/tests/test_tools.py` & `llm-chain-0.0.3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.2/tests/test_utilities.py` & `llm-chain-0.0.3/tests/test_utilities.py`

 * *Files identical despite different names*

