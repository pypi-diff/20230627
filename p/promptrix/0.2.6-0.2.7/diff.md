# Comparing `tmp/promptrix-0.2.6.tar.gz` & `tmp/promptrix-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptrix-0.2.6.tar", last modified: Tue Jun 20 03:27:33 2023, max compression
+gzip compressed data, was "promptrix-0.2.7.tar", last modified: Tue Jun 27 16:38:57 2023, max compression
```

## Comparing `promptrix-0.2.6.tar` & `promptrix-0.2.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:27:33.940387 promptrix-0.2.6/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.6/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-06-20 03:27:33.940387 promptrix-0.2.6/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1607 2023-06-15 20:10:06.000000 promptrix-0.2.6/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      833 2023-06-20 03:24:19.000000 promptrix-0.2.6/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-20 03:27:33.940387 promptrix-0.2.6/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:27:33.936387 promptrix-0.2.6/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:27:33.940387 promptrix-0.2.6/src/promptrix/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      763 2023-06-12 20:40:27.000000 promptrix-0.2.6/src/promptrix/AssistantMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2580 2023-06-19 22:45:55.000000 promptrix-0.2.6/src/promptrix/ConversationHistory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.6/src/promptrix/FunctionRegistry.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      607 2023-06-14 17:33:19.000000 promptrix-0.2.6/src/promptrix/GPT3Tokenizer.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1187 2023-06-15 17:06:46.000000 promptrix-0.2.6/src/promptrix/GroupSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-15 17:06:10.000000 promptrix-0.2.6/src/promptrix/LayoutEngine.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.6/src/promptrix/Prompt.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2445 2023-06-15 17:06:28.000000 promptrix-0.2.6/src/promptrix/PromptSectionBase.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.6/src/promptrix/SystemMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5738 2023-06-14 19:26:14.000000 promptrix-0.2.6/src/promptrix/TemplateSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.6/src/promptrix/TextSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.2.6/src/promptrix/UserMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-14 19:25:22.000000 promptrix-0.2.6/src/promptrix/Utilities.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-19 22:47:47.000000 promptrix-0.2.6/src/promptrix/VolatileMemory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.6/src/promptrix/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.6/src/promptrix/promptrixTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:27:33.940387 promptrix-0.2.6/src/promptrix.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-06-20 03:27:33.000000 promptrix-0.2.6/src/promptrix.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-06-20 03:27:33.000000 promptrix-0.2.6/src/promptrix.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-20 03:27:33.000000 promptrix-0.2.6/src/promptrix.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-20 03:27:33.000000 promptrix-0.2.6/src/promptrix.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-20 03:27:33.000000 promptrix-0.2.6/src/promptrix.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-27 16:38:57.227686 promptrix-0.2.7/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.7/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-06-27 16:38:57.227686 promptrix-0.2.7/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1607 2023-06-15 20:10:06.000000 promptrix-0.2.7/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      833 2023-06-27 16:38:48.000000 promptrix-0.2.7/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-27 16:38:57.227686 promptrix-0.2.7/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-27 16:38:57.223686 promptrix-0.2.7/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-27 16:38:57.223686 promptrix-0.2.7/src/promptrix/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      759 2023-06-27 16:18:19.000000 promptrix-0.2.7/src/promptrix/AssistantMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2576 2023-06-27 16:18:52.000000 promptrix-0.2.7/src/promptrix/ConversationHistory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.7/src/promptrix/FunctionRegistry.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      607 2023-06-14 17:33:19.000000 promptrix-0.2.7/src/promptrix/GPT3Tokenizer.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1187 2023-06-15 17:06:46.000000 promptrix-0.2.7/src/promptrix/GroupSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-15 17:06:10.000000 promptrix-0.2.7/src/promptrix/LayoutEngine.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.7/src/promptrix/Prompt.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2445 2023-06-15 17:06:28.000000 promptrix-0.2.7/src/promptrix/PromptSectionBase.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.7/src/promptrix/SystemMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5738 2023-06-14 19:26:14.000000 promptrix-0.2.7/src/promptrix/TemplateSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.7/src/promptrix/TextSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.2.7/src/promptrix/UserMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-14 19:25:22.000000 promptrix-0.2.7/src/promptrix/Utilities.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-19 22:47:47.000000 promptrix-0.2.7/src/promptrix/VolatileMemory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.7/src/promptrix/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.7/src/promptrix/promptrixTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-27 16:38:57.227686 promptrix-0.2.7/src/promptrix.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-06-27 16:38:57.000000 promptrix-0.2.7/src/promptrix.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-06-27 16:38:57.000000 promptrix-0.2.7/src/promptrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-27 16:38:57.000000 promptrix-0.2.7/src/promptrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-27 16:38:57.000000 promptrix-0.2.7/src/promptrix.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-27 16:38:57.000000 promptrix-0.2.7/src/promptrix.egg-info/top_level.txt
```

### Comparing `promptrix-0.2.6/LICENSE` & `promptrix-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/PKG-INFO` & `promptrix-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.6
+Version: 0.2.7
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/promptrix
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.2.6/README.md` & `promptrix-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/pyproject.toml` & `promptrix-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptrix"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "Promptrix. A prompt layout manager for LLMs"
 #documentation = "https://github.com/Stevenic/promptrix-py/README.md"
```

### Comparing `promptrix-0.2.6/src/promptrix/AssistantMessage.py` & `promptrix-0.2.7/src/promptrix/AssistantMessage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional
 import promptrix.TemplateSection as TemplateSection
 
 class AssistantMessage(TemplateSection.TemplateSection):
     """
     A message sent by the assistant.
     """
-    def __init__(self, template: str, tokens: Optional[int] = -1, assistant_prefix: Optional[str] = 'assistant: '):
+    def __init__(self, template: str, tokens: Optional[int] = -1, assistant_prefix: Optional[str] = 'assistant'):
         """
         Creates a new 'AssistantMessage' instance.
         :param template: Template to use for this section.
         :param tokens: Optional. Sizing strategy for this section. Defaults to `auto`.
-        :param assistant_prefix: Optional. Prefix to use for assistant messages when rendering as text. Defaults to `assistant: `.
+        :param assistant_prefix: Optional. Prefix to use for assistant messages when rendering as text. Defaults to `assistant`.
         """
         super().__init__(template, assistant_prefix, tokens, True, '\n', text_prefix=assistant_prefix)
```

### Comparing `promptrix-0.2.6/src/promptrix/ConversationHistory.py` & `promptrix-0.2.7/src/promptrix/ConversationHistory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from promptrix.promptrixTypes import Message, PromptFunctions, PromptMemory, RenderedPromptSection, Tokenizer
 from promptrix.PromptSectionBase import PromptSectionBase
 from promptrix.Utilities import Utilities
 
 class ConversationHistory(PromptSectionBase):
-    def __init__(self, variable, tokens=1.0, required=False, userPrefix='user: ', assistantPrefix='assistant: ', separator='\n'):
+    def __init__(self, variable, tokens=1.0, required=False, userPrefix='user', assistantPrefix='assistant', separator='\n'):
         super().__init__(tokens, required, separator)
         self.variable = variable
         self.userPrefix = userPrefix
         self.assistantPrefix = assistantPrefix
 
     async def renderAsText(self, memory, functions, tokenizer, maxTokens):
         history = memory.get(self.variable)
```

### Comparing `promptrix-0.2.6/src/promptrix/FunctionRegistry.py` & `promptrix-0.2.7/src/promptrix/FunctionRegistry.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix/GPT3Tokenizer.py` & `promptrix-0.2.7/src/promptrix/GPT3Tokenizer.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix/GroupSection.py` & `promptrix-0.2.7/src/promptrix/GroupSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix/LayoutEngine.py` & `promptrix-0.2.7/src/promptrix/LayoutEngine.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix/PromptSectionBase.py` & `promptrix-0.2.7/src/promptrix/PromptSectionBase.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix/TemplateSection.py` & `promptrix-0.2.7/src/promptrix/TemplateSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix/TextSection.py` & `promptrix-0.2.7/src/promptrix/TextSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix/UserMessage.py` & `promptrix-0.2.7/src/promptrix/UserMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix/Utilities.py` & `promptrix-0.2.7/src/promptrix/Utilities.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix/VolatileMemory.py` & `promptrix-0.2.7/src/promptrix/VolatileMemory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix/promptrixTypes.py` & `promptrix-0.2.7/src/promptrix/promptrixTypes.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.6/src/promptrix.egg-info/PKG-INFO` & `promptrix-0.2.7/src/promptrix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.6
+Version: 0.2.7
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/promptrix
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.2.6/src/promptrix.egg-info/SOURCES.txt` & `promptrix-0.2.7/src/promptrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

