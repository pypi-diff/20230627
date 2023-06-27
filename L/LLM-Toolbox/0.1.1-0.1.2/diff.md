# Comparing `tmp/LLM-Toolbox-0.1.1.tar.gz` & `tmp/LLM-Toolbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM-Toolbox-0.1.1.tar", last modified: Tue Jun 27 01:28:33 2023, max compression
+gzip compressed data, was "LLM-Toolbox-0.1.2.tar", last modified: Tue Jun 27 02:46:03 2023, max compression
```

## Comparing `LLM-Toolbox-0.1.1.tar` & `LLM-Toolbox-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.1/LICENSE
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16781 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      875 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      674 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       88 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16781 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16243 2023-06-26 21:11:54.000000 LLM-Toolbox-0.1.1/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/llm_toolbox/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.1/llm_toolbox/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    12595 2023-06-26 23:19:47.000000 LLM-Toolbox-0.1.1/llm_toolbox/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/llm_toolbox/tools/
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/cheermeup.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/codereview.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/commitgen.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/critique.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/define.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/explain.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/lessonize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/pathlearner.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/proofread.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/study.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      424 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/summarize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/teachlib.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/thesaurus.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/translate.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2915 2023-06-27 01:27:52.000000 LLM-Toolbox-0.1.1/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 02:46:03.540809 LLM-Toolbox-0.1.2/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.2/LICENSE
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 02:46:03.540809 LLM-Toolbox-0.1.2/LLM_Toolbox.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17821 2023-06-27 02:46:03.000000 LLM-Toolbox-0.1.2/LLM_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      875 2023-06-27 02:46:03.000000 LLM-Toolbox-0.1.2/LLM_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-27 02:46:03.000000 LLM-Toolbox-0.1.2/LLM_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      674 2023-06-27 02:46:03.000000 LLM-Toolbox-0.1.2/LLM_Toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       88 2023-06-27 02:46:03.000000 LLM-Toolbox-0.1.2/LLM_Toolbox.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-27 02:46:03.000000 LLM-Toolbox-0.1.2/LLM_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17821 2023-06-27 02:46:03.540809 LLM-Toolbox-0.1.2/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17283 2023-06-27 02:43:22.000000 LLM-Toolbox-0.1.2/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 02:46:03.540809 LLM-Toolbox-0.1.2/llm_toolbox/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.2/llm_toolbox/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    12595 2023-06-26 23:19:47.000000 LLM-Toolbox-0.1.2/llm_toolbox/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 02:46:03.540809 LLM-Toolbox-0.1.2/llm_toolbox/tools/
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 02:46:03.540809 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/cheermeup.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/codereview.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/commitgen.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/critique.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/define.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/explain.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/lessonize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/pathlearner.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/proofread.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/study.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      424 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/summarize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/teachlib.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/thesaurus.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/translate.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-27 02:46:03.540809 LLM-Toolbox-0.1.2/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2915 2023-06-27 02:45:26.000000 LLM-Toolbox-0.1.2/setup.py
```

### Comparing `LLM-Toolbox-0.1.1/LICENSE` & `LLM-Toolbox-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/PKG-INFO` & `LLM-Toolbox-0.1.2/LLM_Toolbox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
@@ -200,39 +200,48 @@
 
 Instructions on how to use each of the tools are included in the individual directories under [tools/](https://github.com/sderev/llm-toolbox/tree/main/tools). This is also where I give some tricks and tips on their usage 💡👀💭.
 
 Note that LMT is the main tool in the LLM-Toolbox. All of its options apply to (almost) all of the other tools. For instance, you change the model to GPT-4 with `-m 4` or add emojis with `--emoji`. Refer to the [LMT's documentation](https://github.com/sderev/lmt) for more information. 
 
 * **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
 
-* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
+* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique > critique_of_my_text.md`
 
 Here's a brief overview of the tools:
 
 ### [LMT](https://github.com/sderev/lmt)
 
 [LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
 
+![cioran](https://github.com/sderev/llm-toolbox/assets/24412384/c1a7d7f2-1edb-425d-bd8c-2a813be9d088)
+
+___
+
 ### [ShellGenius](https://github.com/sderev/shellgenius)
 
 [ShellGenius](https://github.com/sderev/shellgenius) is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands. Check out the project on [its dedicated repository](https://github.com/sderev/shellgenius).
 
 ![shellgenius](https://github.com/sderev/llm-toolbox/assets/24412384/688d9a1a-f351-42d0-9f4d-06a9a6d1909a)
 
+___
+
 ### [Commitgen](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen)
 
 The [`commitgen`](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen) tool is designed to streamline your `git` workflow by automatically generating meaningful commit messages for your code changes.
 
-![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/d41985d5-d8a2-4622-9ef7-643176cdc741)
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/37103ef6-7078-4b38-bdb6-bb4c9880ad3f)
+
 ___
 
 ### [Codereview](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview)
 
 The [`Codereview`](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview) tool accepts a file or a piece of text as input and provides an in-depth analysis of the code. It can identify potential issues, suggest improvements, and even detect security vulnerabilities. The Codereview tool is capable of handling a variety of programming languages, and its feedback can serve as an invaluable resource for developers seeking to enhance the quality of their code. 
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/6ee649e5-4e0f-4e59-8a36-a13080a2aa52)
+
 ___
 
 ### [VocabMaster](https://github.com/sderev/vocabmaster)
 
 Master new languages with [VocabMaster](https://github.com/sderev/vocabmaster), a CLI tool designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience. Check out the project on [its dedicated repository](https://github.com/sderev/vocabmaster).
 
 ![vocabmaster_translate_japanese](https://github.com/sderev/llm-toolbox/assets/24412384/5f5612fe-f1fb-4d4c-bb25-68f07961e66b)
@@ -271,56 +280,72 @@
 
 ___
 
 ### [Cheermeup](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup)
 
 The [`cheermeup`](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup) tool is designed to uplift your spirits based on your current mood. Whether you're feeling down or just need a little pick-me-up, this tool uses a variety of methods to bring a smile to your face and brighten your day.
 
+![ice_cream](https://github.com/sderev/llm-toolbox/assets/24412384/d9928f50-19fd-40a1-a862-697606a1c7c5)
+
 ___
 
 ### [Critique](https://github.com/sderev/llm-toolbox/tree/main/tools/critique)
 
 The [`critique`](https://github.com/sderev/llm-toolbox/tree/main/tools/critique) tool is your personal constructive text critic, designed to analyze a given piece of text and provide detailed, insightful feedback. It enables users to enhance their writing by addressing potential shortcomings and improving the overall quality.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/e63186fe-ad22-400c-b98a-24ba9417a332)
+
 ___
 
 ### [Explain](https://github.com/sderev/llm-toolbox/tree/main/tools/explain)
 
 The [`explain`](https://github.com/sderev/llm-toolbox/tree/main/tools/explain) tool helps to clarify complex concepts. When given a concept, it presents a comprehensive and straightforward explanation, aiding in understanding and knowledge retention.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/86c7d6b0-3ab3-4021-9355-638bd1eee956)
+
 ___
 
 ### [Lessonize](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize)
 
 The [`lessonize`](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize) tool transforms any piece of text into an informative lesson. Whether you're a teacher looking for instructional material or a student looking to further understand a subject, this tool makes learning more accessible.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/c9945c67-a561-4666-9c74-a714a1d69b78)
+
 ___
 
 ### [Pathlearner](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner)
 
 The [`pathlearner`](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner) tool provides a comprehensive study plan for a given topic. Whether you're studying for an exam or learning a new subject, this tool creates a structured, step-by-step plan that aids in understanding and mastering the material.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/8e743ab9-ddff-4d77-bcac-b22afec40c79)
+
 ___
 
 ### [Study](https://github.com/sderev/llm-toolbox/tree/main/tools/study)
 
 The [`study`](https://github.com/sderev/llm-toolbox/tree/main/tools/study) tool is a comprehensive guide that generates study material for a particular topic or content. It helps students to better prepare for exams, giving them access to tailored study material designed to enhance their learning experience.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/07192886-7203-4cf5-ae68-86783116fe3d)
+
 ___
 
 ### [Summarize](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize)
 
 The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
 
+![wikipedia](https://github.com/sderev/llm-toolbox/assets/24412384/655e34aa-07d9-4f3c-97e9-36fd319126ce)
+
 ___
 
 ### [Teachlib](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib)
 
 The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
 
+![numpy](https://github.com/sderev/llm-toolbox/assets/24412384/a85721e2-0be4-4b81-bfe3-8db5af560456)
+
 ___
 
 ## License
 
 This project is licensed under the terms of the Apache License 2.0.
 
 ___
```

### Comparing `LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/SOURCES.txt` & `LLM-Toolbox-0.1.2/LLM_Toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/entry_points.txt` & `LLM-Toolbox-0.1.2/LLM_Toolbox.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.1/PKG-INFO` & `LLM-Toolbox-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
@@ -200,39 +200,48 @@
 
 Instructions on how to use each of the tools are included in the individual directories under [tools/](https://github.com/sderev/llm-toolbox/tree/main/tools). This is also where I give some tricks and tips on their usage 💡👀💭.
 
 Note that LMT is the main tool in the LLM-Toolbox. All of its options apply to (almost) all of the other tools. For instance, you change the model to GPT-4 with `-m 4` or add emojis with `--emoji`. Refer to the [LMT's documentation](https://github.com/sderev/lmt) for more information. 
 
 * **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
 
-* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
+* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique > critique_of_my_text.md`
 
 Here's a brief overview of the tools:
 
 ### [LMT](https://github.com/sderev/lmt)
 
 [LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
 
+![cioran](https://github.com/sderev/llm-toolbox/assets/24412384/c1a7d7f2-1edb-425d-bd8c-2a813be9d088)
+
+___
+
 ### [ShellGenius](https://github.com/sderev/shellgenius)
 
 [ShellGenius](https://github.com/sderev/shellgenius) is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands. Check out the project on [its dedicated repository](https://github.com/sderev/shellgenius).
 
 ![shellgenius](https://github.com/sderev/llm-toolbox/assets/24412384/688d9a1a-f351-42d0-9f4d-06a9a6d1909a)
 
+___
+
 ### [Commitgen](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen)
 
 The [`commitgen`](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen) tool is designed to streamline your `git` workflow by automatically generating meaningful commit messages for your code changes.
 
-![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/d41985d5-d8a2-4622-9ef7-643176cdc741)
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/37103ef6-7078-4b38-bdb6-bb4c9880ad3f)
+
 ___
 
 ### [Codereview](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview)
 
 The [`Codereview`](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview) tool accepts a file or a piece of text as input and provides an in-depth analysis of the code. It can identify potential issues, suggest improvements, and even detect security vulnerabilities. The Codereview tool is capable of handling a variety of programming languages, and its feedback can serve as an invaluable resource for developers seeking to enhance the quality of their code. 
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/6ee649e5-4e0f-4e59-8a36-a13080a2aa52)
+
 ___
 
 ### [VocabMaster](https://github.com/sderev/vocabmaster)
 
 Master new languages with [VocabMaster](https://github.com/sderev/vocabmaster), a CLI tool designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience. Check out the project on [its dedicated repository](https://github.com/sderev/vocabmaster).
 
 ![vocabmaster_translate_japanese](https://github.com/sderev/llm-toolbox/assets/24412384/5f5612fe-f1fb-4d4c-bb25-68f07961e66b)
@@ -271,56 +280,72 @@
 
 ___
 
 ### [Cheermeup](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup)
 
 The [`cheermeup`](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup) tool is designed to uplift your spirits based on your current mood. Whether you're feeling down or just need a little pick-me-up, this tool uses a variety of methods to bring a smile to your face and brighten your day.
 
+![ice_cream](https://github.com/sderev/llm-toolbox/assets/24412384/d9928f50-19fd-40a1-a862-697606a1c7c5)
+
 ___
 
 ### [Critique](https://github.com/sderev/llm-toolbox/tree/main/tools/critique)
 
 The [`critique`](https://github.com/sderev/llm-toolbox/tree/main/tools/critique) tool is your personal constructive text critic, designed to analyze a given piece of text and provide detailed, insightful feedback. It enables users to enhance their writing by addressing potential shortcomings and improving the overall quality.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/e63186fe-ad22-400c-b98a-24ba9417a332)
+
 ___
 
 ### [Explain](https://github.com/sderev/llm-toolbox/tree/main/tools/explain)
 
 The [`explain`](https://github.com/sderev/llm-toolbox/tree/main/tools/explain) tool helps to clarify complex concepts. When given a concept, it presents a comprehensive and straightforward explanation, aiding in understanding and knowledge retention.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/86c7d6b0-3ab3-4021-9355-638bd1eee956)
+
 ___
 
 ### [Lessonize](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize)
 
 The [`lessonize`](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize) tool transforms any piece of text into an informative lesson. Whether you're a teacher looking for instructional material or a student looking to further understand a subject, this tool makes learning more accessible.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/c9945c67-a561-4666-9c74-a714a1d69b78)
+
 ___
 
 ### [Pathlearner](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner)
 
 The [`pathlearner`](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner) tool provides a comprehensive study plan for a given topic. Whether you're studying for an exam or learning a new subject, this tool creates a structured, step-by-step plan that aids in understanding and mastering the material.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/8e743ab9-ddff-4d77-bcac-b22afec40c79)
+
 ___
 
 ### [Study](https://github.com/sderev/llm-toolbox/tree/main/tools/study)
 
 The [`study`](https://github.com/sderev/llm-toolbox/tree/main/tools/study) tool is a comprehensive guide that generates study material for a particular topic or content. It helps students to better prepare for exams, giving them access to tailored study material designed to enhance their learning experience.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/07192886-7203-4cf5-ae68-86783116fe3d)
+
 ___
 
 ### [Summarize](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize)
 
 The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
 
+![wikipedia](https://github.com/sderev/llm-toolbox/assets/24412384/655e34aa-07d9-4f3c-97e9-36fd319126ce)
+
 ___
 
 ### [Teachlib](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib)
 
 The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
 
+![numpy](https://github.com/sderev/llm-toolbox/assets/24412384/a85721e2-0be4-4b81-bfe3-8db5af560456)
+
 ___
 
 ## License
 
 This project is licensed under the terms of the Apache License 2.0.
 
 ___
```

### Comparing `LLM-Toolbox-0.1.1/README.md` & `LLM-Toolbox-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -186,39 +186,48 @@
 
 Instructions on how to use each of the tools are included in the individual directories under [tools/](https://github.com/sderev/llm-toolbox/tree/main/tools). This is also where I give some tricks and tips on their usage 💡👀💭.
 
 Note that LMT is the main tool in the LLM-Toolbox. All of its options apply to (almost) all of the other tools. For instance, you change the model to GPT-4 with `-m 4` or add emojis with `--emoji`. Refer to the [LMT's documentation](https://github.com/sderev/lmt) for more information. 
 
 * **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
 
-* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
+* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique > critique_of_my_text.md`
 
 Here's a brief overview of the tools:
 
 ### [LMT](https://github.com/sderev/lmt)
 
 [LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
 
+![cioran](https://github.com/sderev/llm-toolbox/assets/24412384/c1a7d7f2-1edb-425d-bd8c-2a813be9d088)
+
+___
+
 ### [ShellGenius](https://github.com/sderev/shellgenius)
 
 [ShellGenius](https://github.com/sderev/shellgenius) is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands. Check out the project on [its dedicated repository](https://github.com/sderev/shellgenius).
 
 ![shellgenius](https://github.com/sderev/llm-toolbox/assets/24412384/688d9a1a-f351-42d0-9f4d-06a9a6d1909a)
 
+___
+
 ### [Commitgen](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen)
 
 The [`commitgen`](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen) tool is designed to streamline your `git` workflow by automatically generating meaningful commit messages for your code changes.
 
-![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/d41985d5-d8a2-4622-9ef7-643176cdc741)
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/37103ef6-7078-4b38-bdb6-bb4c9880ad3f)
+
 ___
 
 ### [Codereview](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview)
 
 The [`Codereview`](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview) tool accepts a file or a piece of text as input and provides an in-depth analysis of the code. It can identify potential issues, suggest improvements, and even detect security vulnerabilities. The Codereview tool is capable of handling a variety of programming languages, and its feedback can serve as an invaluable resource for developers seeking to enhance the quality of their code. 
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/6ee649e5-4e0f-4e59-8a36-a13080a2aa52)
+
 ___
 
 ### [VocabMaster](https://github.com/sderev/vocabmaster)
 
 Master new languages with [VocabMaster](https://github.com/sderev/vocabmaster), a CLI tool designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience. Check out the project on [its dedicated repository](https://github.com/sderev/vocabmaster).
 
 ![vocabmaster_translate_japanese](https://github.com/sderev/llm-toolbox/assets/24412384/5f5612fe-f1fb-4d4c-bb25-68f07961e66b)
@@ -257,56 +266,72 @@
 
 ___
 
 ### [Cheermeup](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup)
 
 The [`cheermeup`](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup) tool is designed to uplift your spirits based on your current mood. Whether you're feeling down or just need a little pick-me-up, this tool uses a variety of methods to bring a smile to your face and brighten your day.
 
+![ice_cream](https://github.com/sderev/llm-toolbox/assets/24412384/d9928f50-19fd-40a1-a862-697606a1c7c5)
+
 ___
 
 ### [Critique](https://github.com/sderev/llm-toolbox/tree/main/tools/critique)
 
 The [`critique`](https://github.com/sderev/llm-toolbox/tree/main/tools/critique) tool is your personal constructive text critic, designed to analyze a given piece of text and provide detailed, insightful feedback. It enables users to enhance their writing by addressing potential shortcomings and improving the overall quality.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/e63186fe-ad22-400c-b98a-24ba9417a332)
+
 ___
 
 ### [Explain](https://github.com/sderev/llm-toolbox/tree/main/tools/explain)
 
 The [`explain`](https://github.com/sderev/llm-toolbox/tree/main/tools/explain) tool helps to clarify complex concepts. When given a concept, it presents a comprehensive and straightforward explanation, aiding in understanding and knowledge retention.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/86c7d6b0-3ab3-4021-9355-638bd1eee956)
+
 ___
 
 ### [Lessonize](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize)
 
 The [`lessonize`](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize) tool transforms any piece of text into an informative lesson. Whether you're a teacher looking for instructional material or a student looking to further understand a subject, this tool makes learning more accessible.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/c9945c67-a561-4666-9c74-a714a1d69b78)
+
 ___
 
 ### [Pathlearner](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner)
 
 The [`pathlearner`](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner) tool provides a comprehensive study plan for a given topic. Whether you're studying for an exam or learning a new subject, this tool creates a structured, step-by-step plan that aids in understanding and mastering the material.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/8e743ab9-ddff-4d77-bcac-b22afec40c79)
+
 ___
 
 ### [Study](https://github.com/sderev/llm-toolbox/tree/main/tools/study)
 
 The [`study`](https://github.com/sderev/llm-toolbox/tree/main/tools/study) tool is a comprehensive guide that generates study material for a particular topic or content. It helps students to better prepare for exams, giving them access to tailored study material designed to enhance their learning experience.
 
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/07192886-7203-4cf5-ae68-86783116fe3d)
+
 ___
 
 ### [Summarize](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize)
 
 The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
 
+![wikipedia](https://github.com/sderev/llm-toolbox/assets/24412384/655e34aa-07d9-4f3c-97e9-36fd319126ce)
+
 ___
 
 ### [Teachlib](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib)
 
 The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
 
+![numpy](https://github.com/sderev/llm-toolbox/assets/24412384/a85721e2-0be4-4b81-bfe3-8db5af560456)
+
 ___
 
 ## License
 
 This project is licensed under the terms of the Apache License 2.0.
 
 ___
```

### Comparing `LLM-Toolbox-0.1.1/llm_toolbox/cli.py` & `LLM-Toolbox-0.1.2/llm_toolbox/cli.py`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/codereview.yaml` & `LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/codereview.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/commitgen.yaml` & `LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/commitgen.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/critique.yaml` & `LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/critique.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/lessonize.yaml` & `LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/lessonize.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/pathlearner.yaml` & `LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/pathlearner.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/teachlib.yaml` & `LLM-Toolbox-0.1.2/llm_toolbox/tools/templates/teachlib.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.1/setup.py` & `LLM-Toolbox-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 from pathlib import Path
 import shutil
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 
 
 class PostDevelopCommand(develop):
     """Post-installation for development mode."""
 
     def run(self):
         develop.run(self)
```

