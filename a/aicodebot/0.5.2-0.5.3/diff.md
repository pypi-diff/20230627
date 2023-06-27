# Comparing `tmp/aicodebot-0.5.2.tar.gz` & `tmp/aicodebot-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.5.2.tar", last modified: Tue Jun 27 05:09:21 2023, max compression
+gzip compressed data, was "aicodebot-0.5.3.tar", last modified: Tue Jun 27 05:35:57 2023, max compression
```

## Comparing `aicodebot-0.5.2.tar` & `aicodebot-0.5.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:21.727999 aicodebot-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 05:08:57.000000 aicodebot-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-27 05:09:21.727999 aicodebot-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-27 05:08:57.000000 aicodebot-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:21.727999 aicodebot-0.5.2/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:21.727999 aicodebot-0.5.2/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/fun_fact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/review.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:21.727999 aicodebot-0.5.2/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-27 05:08:57.000000 aicodebot-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:09:21.727999 aicodebot-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-27 05:08:57.000000 aicodebot-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:35:57.833034 aicodebot-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 05:35:35.000000 aicodebot-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-27 05:35:57.833034 aicodebot-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-06-27 05:35:35.000000 aicodebot-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:35:57.833034 aicodebot-0.5.3/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:35:57.833034 aicodebot-0.5.3/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/fun_fact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/review.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:35:57.833034 aicodebot-0.5.3/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-27 05:35:35.000000 aicodebot-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:35:57.833034 aicodebot-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-27 05:35:35.000000 aicodebot-0.5.3/setup.py
```

### Comparing `aicodebot-0.5.2/LICENSE` & `aicodebot-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.2/PKG-INFO` & `aicodebot-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.5.2
+Version: 0.5.3
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 
 ⚠️ It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
 
 We're working on it and it's getting better all the time.
 
 ### What it's not
 
-`aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the [Alignment](#alignment) section below for more on that.
+`aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
 It's also not a "build a website for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, it's built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it
 
 ### AI-Assisted Git Commit
```

### Comparing `aicodebot-0.5.2/README.md` & `aicodebot-0.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ⚠️ It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
 
 We're working on it and it's getting better all the time.
 
 ### What it's not
 
-`aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the [Alignment](#alignment) section below for more on that.
+`aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
 It's also not a "build a website for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, it's built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it
 
 ### AI-Assisted Git Commit
```

### Comparing `aicodebot-0.5.2/aicodebot/cli.py` & `aicodebot-0.5.3/aicodebot/cli.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.2/aicodebot/helpers.py` & `aicodebot-0.5.3/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.2/aicodebot/prompts/alignment.yaml` & `aicodebot-0.5.3/aicodebot/prompts/alignment.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.2/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.5.3/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.2/aicodebot/prompts/review.yaml` & `aicodebot-0.5.3/aicodebot/prompts/review.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.2/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.5.3/aicodebot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.5.2
+Version: 0.5.3
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 
 ⚠️ It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
 
 We're working on it and it's getting better all the time.
 
 ### What it's not
 
-`aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the [Alignment](#alignment) section below for more on that.
+`aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
 It's also not a "build a website for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, it's built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it
 
 ### AI-Assisted Git Commit
```

### Comparing `aicodebot-0.5.2/aicodebot.egg-info/SOURCES.txt` & `aicodebot-0.5.3/aicodebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.2/pyproject.toml` & `aicodebot-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.2/setup.py` & `aicodebot-0.5.3/setup.py`

 * *Files identical despite different names*

