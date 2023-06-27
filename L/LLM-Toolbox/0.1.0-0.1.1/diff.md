# Comparing `tmp/LLM-Toolbox-0.1.0.tar.gz` & `tmp/LLM-Toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM-Toolbox-0.1.0.tar", last modified: Sat Jun 24 03:24:00 2023, max compression
+gzip compressed data, was "LLM-Toolbox-0.1.1.tar", last modified: Tue Jun 27 01:28:33 2023, max compression
```

## Comparing `LLM-Toolbox-0.1.0.tar` & `LLM-Toolbox-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 03:24:00.386939 LLM-Toolbox-0.1.0/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.0/LICENSE
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 03:24:00.376939 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15779 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      875 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      674 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       88 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15779 2023-06-24 03:24:00.386939 LLM-Toolbox-0.1.0/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15241 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 03:24:00.376939 LLM-Toolbox-0.1.0/llm_toolbox/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.0/llm_toolbox/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    12492 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 03:24:00.376939 LLM-Toolbox-0.1.0/llm_toolbox/tools/
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 03:24:00.386939 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/cheermeup.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/codereview.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/commitgen.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/critique.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/define.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/explain.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/lessonize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/pathlearner.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/proofread.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/study.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      424 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/summarize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/teachlib.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/thesaurus.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/translate.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-24 03:24:00.386939 LLM-Toolbox-0.1.0/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2915 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.1/LICENSE
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16781 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      875 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      674 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       88 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-27 01:28:33.000000 LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16781 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16243 2023-06-26 21:11:54.000000 LLM-Toolbox-0.1.1/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/llm_toolbox/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.1/llm_toolbox/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    12595 2023-06-26 23:19:47.000000 LLM-Toolbox-0.1.1/llm_toolbox/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/llm_toolbox/tools/
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/cheermeup.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/codereview.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/commitgen.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/critique.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/define.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/explain.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/lessonize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/pathlearner.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/proofread.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/study.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      424 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/summarize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/teachlib.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/thesaurus.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/translate.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-27 01:28:33.600817 LLM-Toolbox-0.1.1/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2915 2023-06-27 01:27:52.000000 LLM-Toolbox-0.1.1/setup.py
```

### Comparing `LLM-Toolbox-0.1.0/LICENSE` & `LLM-Toolbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/PKG-INFO` & `LLM-Toolbox-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,16 @@
-Metadata-Version: 2.1
-Name: LLM-Toolbox
-Version: 0.1.0
-Summary: A versatile collection of CLI tools leveraging large language models
-Home-page: https://github.com/sderev/llm-toolbox
-Author: Sébastien De Revière
-License: Apache Licence, Version 2.0
-Project-URL: Documentation, https://github.com/sderev/llm-toolbox
-Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
-Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # LLM-Toolbox
 
 **Development Status**: 
 
 LLM-Toolbox is currently under active development. Your feedback is crucial for this ongoing journey of refinement. Please share your thoughts, experiences, and suggestions. If you find this project beneficial, consider expression your support by giving it a star ⭐😊.
 
 ---
 
-LLM-Toolbox is an ensemble of AI-powered command-line tools designed to modernize your workflow in the terminal. Built using OpenAI's ChatGPT, the tools in this toolbox can generate automatic commit messages, perform dictionary and thesaurus quesries, translate text, proofread content, enrich language learning, and automate shell commands, among others.
+LLM-Toolbox is an ensemble of AI-powered command-line tools designed to modernize your workflow in the terminal. Built using OpenAI's ChatGPT, the tools in this toolbox can generate automatic commit messages, perform dictionary and thesaurus queries, translate text, proofread content, enrich language learning, and automate shell commands, among others.
 
 Additionally, the toolbox provides an array of [prompt templates](#prompt-templates) that can serve as a valuable resource, whether you're new to using languages models or you're an experienced user.
 
 I've created video demos to help you see the LLM-Toolbox in action and understand its wide-ranging capabilities. Therefore, I strongly recommend you check out the video demos of the tools to gain a hands-on understanding of their potential. After watching the demos, you can return here for a deeper dive into the specific applications and benefits. So, go ahead, watch the demos! 😊
 
 <!-- TOC -->
 ## Table of Contents
@@ -60,19 +46,19 @@
     1. [Summarize](#summarize)
     1. [Teachlib](#teachlib)
 1. [License](#license)
 <!-- /TOC -->
 
 ## Prompt Templates 
 
-If you're less familiar with terminal interfaces, or if you simply prefer the convenience of a web interface, you'll find our [ChatGPT web interface templates](https://github.com/sderev/llm-toolbox/prompt-templates) quite helpful. Particularly for longer chat interactions with GPT-4, the web interface is advantageous, although it does necessitate a ChatGPT Plus subscription.
+For those less experienced with terminal interfaces or those preferring the convenience of a web interface, the [ChatGPT web interface templates](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) in the LLM-Toolbox can prove incredibly useful. These templates offer a broad spectrum of pre-structured prompts designed to enhance your engagement with ChatGPT, particularly in the context of longer chat interactions with GPT-4 in order to avoid expensive API costs.
 
-The LLM-Toolbox goes beyond just tools; it also offers a comprehensive collection of prompt templates located in the [`prompt-templates/`](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) directory. These templates cater to a broad range of situations and are crafted to enhance your engagement with language models. If you're unsure about prompt structuring or want to boost the efficacy of your existing prompts, these templates serve as a great starting point.
+These templates, found in the [`prompt-templates/`](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) directory, cater to various situations and are an excellent resource if you're uncertain about structuring prompts or seek to improve the effectiveness of your existing ones.
 
-You're encouraged to browse these templates and modify them to fit your unique requirements.
+Feel free to explore these templates and adjust them to better suit your individual needs.
 
 ## Isn't the OpenAI API expensive?
 
 A lot of people are afraid that these tools will cost them too much. But the truth is, as long as you're not sending too many requests to GPT-4, you won't have exorbitant bills. On the contrary, this may surprise you, but I'm pretty confident that the majority of people won't exceed a cost of $3 to $5 per month, as long as they continue to use GPT-3.5, even if they use these tools more than a hundred times a day.
 
 Also, there's a safeguard: **you can configure a soft and a hard usage limit on your OpenAI account**. This ensures that you won't ever be taken by surprise.
 
@@ -204,122 +190,125 @@
 
 * **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
 
 * **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
 
 Here's a brief overview of the tools:
 
-### LMT
+### [LMT](https://github.com/sderev/lmt)
 
 [LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
 
-### ShellGenius
+### [ShellGenius](https://github.com/sderev/shellgenius)
 
 [ShellGenius](https://github.com/sderev/shellgenius) is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands. Check out the project on [its dedicated repository](https://github.com/sderev/shellgenius).
 
 ![shellgenius](https://github.com/sderev/llm-toolbox/assets/24412384/688d9a1a-f351-42d0-9f4d-06a9a6d1909a)
 
-### Commitgen
+### [Commitgen](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen)
 
 The [`commitgen`](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen) tool is designed to streamline your `git` workflow by automatically generating meaningful commit messages for your code changes.
 
 ![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/d41985d5-d8a2-4622-9ef7-643176cdc741)
 ___
 
-### Codereview
+### [Codereview](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview)
 
 The [`Codereview`](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview) tool accepts a file or a piece of text as input and provides an in-depth analysis of the code. It can identify potential issues, suggest improvements, and even detect security vulnerabilities. The Codereview tool is capable of handling a variety of programming languages, and its feedback can serve as an invaluable resource for developers seeking to enhance the quality of their code. 
 
 ___
 
-### VocabMaster
+### [VocabMaster](https://github.com/sderev/vocabmaster)
 
 Master new languages with [VocabMaster](https://github.com/sderev/vocabmaster), a CLI tool designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience. Check out the project on [its dedicated repository](https://github.com/sderev/vocabmaster).
 
 ![vocabmaster_translate_japanese](https://github.com/sderev/llm-toolbox/assets/24412384/5f5612fe-f1fb-4d4c-bb25-68f07961e66b)
 
 ___
 
-### Thesaurus
+### [Thesaurus](https://github.com/sderev/llm-toolbox/tree/main/tools/thesaurus)
 
 The [`thesaurus`](https://github.com/sderev/llm-toolbox/tree/main/tools/thesaurus) tool takes a word or a phrase as input and provides a list of synonyms and antonyms.
 
 ![thesaurus](https://github.com/sderev/llm-toolbox/assets/24412384/dca6bf42-2545-4b56-bb20-4c8e6c872529)
 
 ___
 
-### Define
+### [Define](https://github.com/sderev/llm-toolbox/tree/main/tools/define)
 
 The [`define`](https://github.com/sderev/llm-toolbox/tree/main/tools/define) tool takes a word as input and provides its definition along with an example sentence using the word.
 
 ![define](https://github.com/sderev/llm-toolbox/assets/24412384/1e813b80-6896-483b-b31a-65ad7cb81173)
 
 ___
 
-### Proofread
+### [Proofread](https://github.com/sderev/llm-toolbox/tree/main/tools/proofread)
 
 The [`proofread`](https://github.com/sderev/llm-toolbox/tree/main/tools/proofread) tool takes a sentence as input and provides a corrected version of it, if needed, along with an explanation of the corrections.
 
 ![proofread_english](https://github.com/sderev/llm-toolbox/assets/24412384/e84ce7cd-68e9-4d6d-8c56-55b93c7e4fee)
 
 ___
 
-### Translate
+### [Translate](https://github.com/sderev/llm-toolbox/tree/main/tools/translate)
 
 The [`translate`](https://github.com/sderev/llm-toolbox/tree/main/tools/translate) tool takes a sentence and a target language as input and provides the translated sentence in the target language.
 
 ![translate](https://github.com/sderev/llm-toolbox/assets/24412384/505237c9-7735-4db6-aa4a-63c3ed2867a7)
 
 ___
 
-### Cheermeup
+### [Cheermeup](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup)
 
 The [`cheermeup`](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup) tool is designed to uplift your spirits based on your current mood. Whether you're feeling down or just need a little pick-me-up, this tool uses a variety of methods to bring a smile to your face and brighten your day.
 
 ___
 
-### Critique
+### [Critique](https://github.com/sderev/llm-toolbox/tree/main/tools/critique)
 
 The [`critique`](https://github.com/sderev/llm-toolbox/tree/main/tools/critique) tool is your personal constructive text critic, designed to analyze a given piece of text and provide detailed, insightful feedback. It enables users to enhance their writing by addressing potential shortcomings and improving the overall quality.
 
 ___
 
-### Explain
+### [Explain](https://github.com/sderev/llm-toolbox/tree/main/tools/explain)
 
 The [`explain`](https://github.com/sderev/llm-toolbox/tree/main/tools/explain) tool helps to clarify complex concepts. When given a concept, it presents a comprehensive and straightforward explanation, aiding in understanding and knowledge retention.
 
 ___
 
-### Lessonize
+### [Lessonize](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize)
 
 The [`lessonize`](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize) tool transforms any piece of text into an informative lesson. Whether you're a teacher looking for instructional material or a student looking to further understand a subject, this tool makes learning more accessible.
 
 ___
 
-### Pathlearner
+### [Pathlearner](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner)
 
 The [`pathlearner`](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner) tool provides a comprehensive study plan for a given topic. Whether you're studying for an exam or learning a new subject, this tool creates a structured, step-by-step plan that aids in understanding and mastering the material.
 
 ___
 
-### Study
+### [Study](https://github.com/sderev/llm-toolbox/tree/main/tools/study)
 
 The [`study`](https://github.com/sderev/llm-toolbox/tree/main/tools/study) tool is a comprehensive guide that generates study material for a particular topic or content. It helps students to better prepare for exams, giving them access to tailored study material designed to enhance their learning experience.
 
 ___
 
-### Summarize
+### [Summarize](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize)
 
 The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
 
 ___
 
-### Teachlib
+### [Teachlib](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib)
 
 The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
 
 ___
 
 ## License
 
 This project is licensed under the terms of the Apache License 2.0.
 
+___
+
+<https://github.com/sderev/llm-toolbox>
```

### Comparing `LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/SOURCES.txt` & `LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/entry_points.txt` & `LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.0/PKG-INFO` & `LLM-Toolbox-0.1.1/LLM_Toolbox.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
@@ -16,15 +16,15 @@
 
 **Development Status**: 
 
 LLM-Toolbox is currently under active development. Your feedback is crucial for this ongoing journey of refinement. Please share your thoughts, experiences, and suggestions. If you find this project beneficial, consider expression your support by giving it a star ⭐😊.
 
 ---
 
-LLM-Toolbox is an ensemble of AI-powered command-line tools designed to modernize your workflow in the terminal. Built using OpenAI's ChatGPT, the tools in this toolbox can generate automatic commit messages, perform dictionary and thesaurus quesries, translate text, proofread content, enrich language learning, and automate shell commands, among others.
+LLM-Toolbox is an ensemble of AI-powered command-line tools designed to modernize your workflow in the terminal. Built using OpenAI's ChatGPT, the tools in this toolbox can generate automatic commit messages, perform dictionary and thesaurus queries, translate text, proofread content, enrich language learning, and automate shell commands, among others.
 
 Additionally, the toolbox provides an array of [prompt templates](#prompt-templates) that can serve as a valuable resource, whether you're new to using languages models or you're an experienced user.
 
 I've created video demos to help you see the LLM-Toolbox in action and understand its wide-ranging capabilities. Therefore, I strongly recommend you check out the video demos of the tools to gain a hands-on understanding of their potential. After watching the demos, you can return here for a deeper dive into the specific applications and benefits. So, go ahead, watch the demos! 😊
 
 <!-- TOC -->
 ## Table of Contents
@@ -60,19 +60,19 @@
     1. [Summarize](#summarize)
     1. [Teachlib](#teachlib)
 1. [License](#license)
 <!-- /TOC -->
 
 ## Prompt Templates 
 
-If you're less familiar with terminal interfaces, or if you simply prefer the convenience of a web interface, you'll find our [ChatGPT web interface templates](https://github.com/sderev/llm-toolbox/prompt-templates) quite helpful. Particularly for longer chat interactions with GPT-4, the web interface is advantageous, although it does necessitate a ChatGPT Plus subscription.
+For those less experienced with terminal interfaces or those preferring the convenience of a web interface, the [ChatGPT web interface templates](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) in the LLM-Toolbox can prove incredibly useful. These templates offer a broad spectrum of pre-structured prompts designed to enhance your engagement with ChatGPT, particularly in the context of longer chat interactions with GPT-4 in order to avoid expensive API costs.
 
-The LLM-Toolbox goes beyond just tools; it also offers a comprehensive collection of prompt templates located in the [`prompt-templates/`](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) directory. These templates cater to a broad range of situations and are crafted to enhance your engagement with language models. If you're unsure about prompt structuring or want to boost the efficacy of your existing prompts, these templates serve as a great starting point.
+These templates, found in the [`prompt-templates/`](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) directory, cater to various situations and are an excellent resource if you're uncertain about structuring prompts or seek to improve the effectiveness of your existing ones.
 
-You're encouraged to browse these templates and modify them to fit your unique requirements.
+Feel free to explore these templates and adjust them to better suit your individual needs.
 
 ## Isn't the OpenAI API expensive?
 
 A lot of people are afraid that these tools will cost them too much. But the truth is, as long as you're not sending too many requests to GPT-4, you won't have exorbitant bills. On the contrary, this may surprise you, but I'm pretty confident that the majority of people won't exceed a cost of $3 to $5 per month, as long as they continue to use GPT-3.5, even if they use these tools more than a hundred times a day.
 
 Also, there's a safeguard: **you can configure a soft and a hard usage limit on your OpenAI account**. This ensures that you won't ever be taken by surprise.
 
@@ -204,122 +204,125 @@
 
 * **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
 
 * **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
 
 Here's a brief overview of the tools:
 
-### LMT
+### [LMT](https://github.com/sderev/lmt)
 
 [LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
 
-### ShellGenius
+### [ShellGenius](https://github.com/sderev/shellgenius)
 
 [ShellGenius](https://github.com/sderev/shellgenius) is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands. Check out the project on [its dedicated repository](https://github.com/sderev/shellgenius).
 
 ![shellgenius](https://github.com/sderev/llm-toolbox/assets/24412384/688d9a1a-f351-42d0-9f4d-06a9a6d1909a)
 
-### Commitgen
+### [Commitgen](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen)
 
 The [`commitgen`](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen) tool is designed to streamline your `git` workflow by automatically generating meaningful commit messages for your code changes.
 
 ![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/d41985d5-d8a2-4622-9ef7-643176cdc741)
 ___
 
-### Codereview
+### [Codereview](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview)
 
 The [`Codereview`](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview) tool accepts a file or a piece of text as input and provides an in-depth analysis of the code. It can identify potential issues, suggest improvements, and even detect security vulnerabilities. The Codereview tool is capable of handling a variety of programming languages, and its feedback can serve as an invaluable resource for developers seeking to enhance the quality of their code. 
 
 ___
 
-### VocabMaster
+### [VocabMaster](https://github.com/sderev/vocabmaster)
 
 Master new languages with [VocabMaster](https://github.com/sderev/vocabmaster), a CLI tool designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience. Check out the project on [its dedicated repository](https://github.com/sderev/vocabmaster).
 
 ![vocabmaster_translate_japanese](https://github.com/sderev/llm-toolbox/assets/24412384/5f5612fe-f1fb-4d4c-bb25-68f07961e66b)
 
 ___
 
-### Thesaurus
+### [Thesaurus](https://github.com/sderev/llm-toolbox/tree/main/tools/thesaurus)
 
 The [`thesaurus`](https://github.com/sderev/llm-toolbox/tree/main/tools/thesaurus) tool takes a word or a phrase as input and provides a list of synonyms and antonyms.
 
 ![thesaurus](https://github.com/sderev/llm-toolbox/assets/24412384/dca6bf42-2545-4b56-bb20-4c8e6c872529)
 
 ___
 
-### Define
+### [Define](https://github.com/sderev/llm-toolbox/tree/main/tools/define)
 
 The [`define`](https://github.com/sderev/llm-toolbox/tree/main/tools/define) tool takes a word as input and provides its definition along with an example sentence using the word.
 
 ![define](https://github.com/sderev/llm-toolbox/assets/24412384/1e813b80-6896-483b-b31a-65ad7cb81173)
 
 ___
 
-### Proofread
+### [Proofread](https://github.com/sderev/llm-toolbox/tree/main/tools/proofread)
 
 The [`proofread`](https://github.com/sderev/llm-toolbox/tree/main/tools/proofread) tool takes a sentence as input and provides a corrected version of it, if needed, along with an explanation of the corrections.
 
 ![proofread_english](https://github.com/sderev/llm-toolbox/assets/24412384/e84ce7cd-68e9-4d6d-8c56-55b93c7e4fee)
 
 ___
 
-### Translate
+### [Translate](https://github.com/sderev/llm-toolbox/tree/main/tools/translate)
 
 The [`translate`](https://github.com/sderev/llm-toolbox/tree/main/tools/translate) tool takes a sentence and a target language as input and provides the translated sentence in the target language.
 
 ![translate](https://github.com/sderev/llm-toolbox/assets/24412384/505237c9-7735-4db6-aa4a-63c3ed2867a7)
 
 ___
 
-### Cheermeup
+### [Cheermeup](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup)
 
 The [`cheermeup`](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup) tool is designed to uplift your spirits based on your current mood. Whether you're feeling down or just need a little pick-me-up, this tool uses a variety of methods to bring a smile to your face and brighten your day.
 
 ___
 
-### Critique
+### [Critique](https://github.com/sderev/llm-toolbox/tree/main/tools/critique)
 
 The [`critique`](https://github.com/sderev/llm-toolbox/tree/main/tools/critique) tool is your personal constructive text critic, designed to analyze a given piece of text and provide detailed, insightful feedback. It enables users to enhance their writing by addressing potential shortcomings and improving the overall quality.
 
 ___
 
-### Explain
+### [Explain](https://github.com/sderev/llm-toolbox/tree/main/tools/explain)
 
 The [`explain`](https://github.com/sderev/llm-toolbox/tree/main/tools/explain) tool helps to clarify complex concepts. When given a concept, it presents a comprehensive and straightforward explanation, aiding in understanding and knowledge retention.
 
 ___
 
-### Lessonize
+### [Lessonize](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize)
 
 The [`lessonize`](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize) tool transforms any piece of text into an informative lesson. Whether you're a teacher looking for instructional material or a student looking to further understand a subject, this tool makes learning more accessible.
 
 ___
 
-### Pathlearner
+### [Pathlearner](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner)
 
 The [`pathlearner`](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner) tool provides a comprehensive study plan for a given topic. Whether you're studying for an exam or learning a new subject, this tool creates a structured, step-by-step plan that aids in understanding and mastering the material.
 
 ___
 
-### Study
+### [Study](https://github.com/sderev/llm-toolbox/tree/main/tools/study)
 
 The [`study`](https://github.com/sderev/llm-toolbox/tree/main/tools/study) tool is a comprehensive guide that generates study material for a particular topic or content. It helps students to better prepare for exams, giving them access to tailored study material designed to enhance their learning experience.
 
 ___
 
-### Summarize
+### [Summarize](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize)
 
 The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
 
 ___
 
-### Teachlib
+### [Teachlib](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib)
 
 The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
 
 ___
 
 ## License
 
 This project is licensed under the terms of the Apache License 2.0.
 
+___
+
+<https://github.com/sderev/llm-toolbox>
```

### Comparing `LLM-Toolbox-0.1.0/README.md` & `LLM-Toolbox-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,30 @@
+Metadata-Version: 2.1
+Name: LLM-Toolbox
+Version: 0.1.1
+Summary: A versatile collection of CLI tools leveraging large language models
+Home-page: https://github.com/sderev/llm-toolbox
+Author: Sébastien De Revière
+License: Apache Licence, Version 2.0
+Project-URL: Documentation, https://github.com/sderev/llm-toolbox
+Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
+Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # LLM-Toolbox
 
 **Development Status**: 
 
 LLM-Toolbox is currently under active development. Your feedback is crucial for this ongoing journey of refinement. Please share your thoughts, experiences, and suggestions. If you find this project beneficial, consider expression your support by giving it a star ⭐😊.
 
 ---
 
-LLM-Toolbox is an ensemble of AI-powered command-line tools designed to modernize your workflow in the terminal. Built using OpenAI's ChatGPT, the tools in this toolbox can generate automatic commit messages, perform dictionary and thesaurus quesries, translate text, proofread content, enrich language learning, and automate shell commands, among others.
+LLM-Toolbox is an ensemble of AI-powered command-line tools designed to modernize your workflow in the terminal. Built using OpenAI's ChatGPT, the tools in this toolbox can generate automatic commit messages, perform dictionary and thesaurus queries, translate text, proofread content, enrich language learning, and automate shell commands, among others.
 
 Additionally, the toolbox provides an array of [prompt templates](#prompt-templates) that can serve as a valuable resource, whether you're new to using languages models or you're an experienced user.
 
 I've created video demos to help you see the LLM-Toolbox in action and understand its wide-ranging capabilities. Therefore, I strongly recommend you check out the video demos of the tools to gain a hands-on understanding of their potential. After watching the demos, you can return here for a deeper dive into the specific applications and benefits. So, go ahead, watch the demos! 😊
 
 <!-- TOC -->
 ## Table of Contents
@@ -46,19 +60,19 @@
     1. [Summarize](#summarize)
     1. [Teachlib](#teachlib)
 1. [License](#license)
 <!-- /TOC -->
 
 ## Prompt Templates 
 
-If you're less familiar with terminal interfaces, or if you simply prefer the convenience of a web interface, you'll find our [ChatGPT web interface templates](https://github.com/sderev/llm-toolbox/prompt-templates) quite helpful. Particularly for longer chat interactions with GPT-4, the web interface is advantageous, although it does necessitate a ChatGPT Plus subscription.
+For those less experienced with terminal interfaces or those preferring the convenience of a web interface, the [ChatGPT web interface templates](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) in the LLM-Toolbox can prove incredibly useful. These templates offer a broad spectrum of pre-structured prompts designed to enhance your engagement with ChatGPT, particularly in the context of longer chat interactions with GPT-4 in order to avoid expensive API costs.
 
-The LLM-Toolbox goes beyond just tools; it also offers a comprehensive collection of prompt templates located in the [`prompt-templates/`](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) directory. These templates cater to a broad range of situations and are crafted to enhance your engagement with language models. If you're unsure about prompt structuring or want to boost the efficacy of your existing prompts, these templates serve as a great starting point.
+These templates, found in the [`prompt-templates/`](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) directory, cater to various situations and are an excellent resource if you're uncertain about structuring prompts or seek to improve the effectiveness of your existing ones.
 
-You're encouraged to browse these templates and modify them to fit your unique requirements.
+Feel free to explore these templates and adjust them to better suit your individual needs.
 
 ## Isn't the OpenAI API expensive?
 
 A lot of people are afraid that these tools will cost them too much. But the truth is, as long as you're not sending too many requests to GPT-4, you won't have exorbitant bills. On the contrary, this may surprise you, but I'm pretty confident that the majority of people won't exceed a cost of $3 to $5 per month, as long as they continue to use GPT-3.5, even if they use these tools more than a hundred times a day.
 
 Also, there's a safeguard: **you can configure a soft and a hard usage limit on your OpenAI account**. This ensures that you won't ever be taken by surprise.
 
@@ -190,122 +204,125 @@
 
 * **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
 
 * **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
 
 Here's a brief overview of the tools:
 
-### LMT
+### [LMT](https://github.com/sderev/lmt)
 
 [LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
 
-### ShellGenius
+### [ShellGenius](https://github.com/sderev/shellgenius)
 
 [ShellGenius](https://github.com/sderev/shellgenius) is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands. Check out the project on [its dedicated repository](https://github.com/sderev/shellgenius).
 
 ![shellgenius](https://github.com/sderev/llm-toolbox/assets/24412384/688d9a1a-f351-42d0-9f4d-06a9a6d1909a)
 
-### Commitgen
+### [Commitgen](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen)
 
 The [`commitgen`](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen) tool is designed to streamline your `git` workflow by automatically generating meaningful commit messages for your code changes.
 
 ![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/d41985d5-d8a2-4622-9ef7-643176cdc741)
 ___
 
-### Codereview
+### [Codereview](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview)
 
 The [`Codereview`](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview) tool accepts a file or a piece of text as input and provides an in-depth analysis of the code. It can identify potential issues, suggest improvements, and even detect security vulnerabilities. The Codereview tool is capable of handling a variety of programming languages, and its feedback can serve as an invaluable resource for developers seeking to enhance the quality of their code. 
 
 ___
 
-### VocabMaster
+### [VocabMaster](https://github.com/sderev/vocabmaster)
 
 Master new languages with [VocabMaster](https://github.com/sderev/vocabmaster), a CLI tool designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience. Check out the project on [its dedicated repository](https://github.com/sderev/vocabmaster).
 
 ![vocabmaster_translate_japanese](https://github.com/sderev/llm-toolbox/assets/24412384/5f5612fe-f1fb-4d4c-bb25-68f07961e66b)
 
 ___
 
-### Thesaurus
+### [Thesaurus](https://github.com/sderev/llm-toolbox/tree/main/tools/thesaurus)
 
 The [`thesaurus`](https://github.com/sderev/llm-toolbox/tree/main/tools/thesaurus) tool takes a word or a phrase as input and provides a list of synonyms and antonyms.
 
 ![thesaurus](https://github.com/sderev/llm-toolbox/assets/24412384/dca6bf42-2545-4b56-bb20-4c8e6c872529)
 
 ___
 
-### Define
+### [Define](https://github.com/sderev/llm-toolbox/tree/main/tools/define)
 
 The [`define`](https://github.com/sderev/llm-toolbox/tree/main/tools/define) tool takes a word as input and provides its definition along with an example sentence using the word.
 
 ![define](https://github.com/sderev/llm-toolbox/assets/24412384/1e813b80-6896-483b-b31a-65ad7cb81173)
 
 ___
 
-### Proofread
+### [Proofread](https://github.com/sderev/llm-toolbox/tree/main/tools/proofread)
 
 The [`proofread`](https://github.com/sderev/llm-toolbox/tree/main/tools/proofread) tool takes a sentence as input and provides a corrected version of it, if needed, along with an explanation of the corrections.
 
 ![proofread_english](https://github.com/sderev/llm-toolbox/assets/24412384/e84ce7cd-68e9-4d6d-8c56-55b93c7e4fee)
 
 ___
 
-### Translate
+### [Translate](https://github.com/sderev/llm-toolbox/tree/main/tools/translate)
 
 The [`translate`](https://github.com/sderev/llm-toolbox/tree/main/tools/translate) tool takes a sentence and a target language as input and provides the translated sentence in the target language.
 
 ![translate](https://github.com/sderev/llm-toolbox/assets/24412384/505237c9-7735-4db6-aa4a-63c3ed2867a7)
 
 ___
 
-### Cheermeup
+### [Cheermeup](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup)
 
 The [`cheermeup`](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup) tool is designed to uplift your spirits based on your current mood. Whether you're feeling down or just need a little pick-me-up, this tool uses a variety of methods to bring a smile to your face and brighten your day.
 
 ___
 
-### Critique
+### [Critique](https://github.com/sderev/llm-toolbox/tree/main/tools/critique)
 
 The [`critique`](https://github.com/sderev/llm-toolbox/tree/main/tools/critique) tool is your personal constructive text critic, designed to analyze a given piece of text and provide detailed, insightful feedback. It enables users to enhance their writing by addressing potential shortcomings and improving the overall quality.
 
 ___
 
-### Explain
+### [Explain](https://github.com/sderev/llm-toolbox/tree/main/tools/explain)
 
 The [`explain`](https://github.com/sderev/llm-toolbox/tree/main/tools/explain) tool helps to clarify complex concepts. When given a concept, it presents a comprehensive and straightforward explanation, aiding in understanding and knowledge retention.
 
 ___
 
-### Lessonize
+### [Lessonize](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize)
 
 The [`lessonize`](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize) tool transforms any piece of text into an informative lesson. Whether you're a teacher looking for instructional material or a student looking to further understand a subject, this tool makes learning more accessible.
 
 ___
 
-### Pathlearner
+### [Pathlearner](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner)
 
 The [`pathlearner`](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner) tool provides a comprehensive study plan for a given topic. Whether you're studying for an exam or learning a new subject, this tool creates a structured, step-by-step plan that aids in understanding and mastering the material.
 
 ___
 
-### Study
+### [Study](https://github.com/sderev/llm-toolbox/tree/main/tools/study)
 
 The [`study`](https://github.com/sderev/llm-toolbox/tree/main/tools/study) tool is a comprehensive guide that generates study material for a particular topic or content. It helps students to better prepare for exams, giving them access to tailored study material designed to enhance their learning experience.
 
 ___
 
-### Summarize
+### [Summarize](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize)
 
 The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
 
 ___
 
-### Teachlib
+### [Teachlib](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib)
 
 The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
 
 ___
 
 ## License
 
 This project is licensed under the terms of the Apache License 2.0.
 
+___
+
+<https://github.com/sderev/llm-toolbox>
```

### Comparing `LLM-Toolbox-0.1.0/llm_toolbox/cli.py` & `LLM-Toolbox-0.1.1/llm_toolbox/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from functools import wraps
-from pathlib import Path
 import os
 import re
 import requests
 import subprocess
 import sys
 import tempfile
+from functools import wraps
+from pathlib import Path
 
 import click
 import validators
 from strip_tags.lib import strip_tags
 
 from lmt_cli.lib import *
 from lmt_cli.cli import VALID_MODELS
@@ -42,14 +42,17 @@
 @click.pass_context
 @click.version_option()
 def cli():
     pass
 
 
 def common_options(f):
+    """
+    Common options for all commands.
+    """
     @wraps(f)
     @click.option("--emoji", is_flag=True, help="Add emotions and emojis.")
     @click.option(
         "-m",
         "--model",
         default="gpt-3.5-turbo",
         help="The model to use for the requests.",
@@ -319,15 +322,15 @@
     """
     Summarize the text, the content of a given file, or a webpage (provided as URL).
     """
     source_str = " ".join(source)
 
     prompt_input = ""
 
-    if is_valid_url(source_str):
+    if validators.url(source_str):
         source_content = requests.get(source_str).text
         prompt_input = strip_tags(input=source_content, minify=True)
     else:
         if source:
             content = "".join(source)
             prompt_input += content
 
@@ -493,23 +496,26 @@
         if not sys.stdin.isatty():
             prompt_input = sys.stdin.read()
         elif sys.stdin.isatty():
             click.echo(
                 click.style(
                     (
                         "You can paste your prompt below. Press <Enter> to"
-                        " validate.\nOnce you've done, press Ctrl+D to send it."
+                        " skip a line.\nOnce you've done, press Ctrl+D to send it."
                     ),
                     fg="yellow",
                 )
                 + "\n---"
             )
             prompt_input = sys.stdin.read()
             click.echo()
-    prompt_input = "".join(prompt_input).rstrip()
+    if template == "summarize":
+        prompt_input = "".join(prompt_input).rstrip()
+    else:
+        prompt_input = " ".join(prompt_input).rstrip()
 
     return prepare_and_generate_response(
         system=None,
         template=template,
         model=model,
         prompt_input=prompt_input,
         emoji=emoji,
@@ -517,13 +523,9 @@
         tokens=tokens,
         no_stream=no_stream,
         raw=raw,
         debug=debug,
     )
 
 
-def is_valid_url(url):
-    return validators.url(url)
-
-
 if __name__ == "__main__":
     cli()
```

### Comparing `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/codereview.yaml` & `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/codereview.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/commitgen.yaml` & `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/commitgen.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/critique.yaml` & `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/critique.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/lessonize.yaml` & `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/lessonize.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/pathlearner.yaml` & `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/pathlearner.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/teachlib.yaml` & `LLM-Toolbox-0.1.1/llm_toolbox/tools/templates/teachlib.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.0/setup.py` & `LLM-Toolbox-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 from pathlib import Path
 import shutil
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 
 class PostDevelopCommand(develop):
     """Post-installation for development mode."""
 
     def run(self):
         develop.run(self)
```

