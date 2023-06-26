# Comparing `tmp/aicodebot-0.4.1.tar.gz` & `tmp/aicodebot-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.4.1.tar", last modified: Sat Jun 24 21:38:04 2023, max compression
+gzip compressed data, was "aicodebot-0.5.0.tar", last modified: Mon Jun 26 23:11:22 2023, max compression
```

## Comparing `aicodebot-0.4.1.tar` & `aicodebot-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:38:04.231264 aicodebot-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-24 21:37:41.000000 aicodebot-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-24 21:38:04.231264 aicodebot-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-24 21:37:41.000000 aicodebot-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:38:04.227265 aicodebot-0.4.1/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:38:04.231264 aicodebot-0.4.1/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-24 21:37:41.000000 aicodebot-0.4.1/aicodebot/prompts/fun_fact.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:38:04.227265 aicodebot-0.4.1/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-24 21:38:04.000000 aicodebot-0.4.1/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-24 21:37:41.000000 aicodebot-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:38:04.231264 aicodebot-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-24 21:37:41.000000 aicodebot-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:11:22.388131 aicodebot-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 23:11:02.000000 aicodebot-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-26 23:11:22.388131 aicodebot-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-26 23:11:02.000000 aicodebot-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:11:22.388131 aicodebot-0.5.0/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 23:11:02.000000 aicodebot-0.5.0/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 23:11:02.000000 aicodebot-0.5.0/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-06-26 23:11:02.000000 aicodebot-0.5.0/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-26 23:11:02.000000 aicodebot-0.5.0/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:11:22.388131 aicodebot-0.5.0/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:11:02.000000 aicodebot-0.5.0/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 23:11:02.000000 aicodebot-0.5.0/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-26 23:11:02.000000 aicodebot-0.5.0/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 23:11:02.000000 aicodebot-0.5.0/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 23:11:02.000000 aicodebot-0.5.0/aicodebot/prompts/fun_fact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-26 23:11:02.000000 aicodebot-0.5.0/aicodebot/prompts/review.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:11:22.388131 aicodebot-0.5.0/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-26 23:11:22.000000 aicodebot-0.5.0/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 23:11:22.000000 aicodebot-0.5.0/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 23:11:22.000000 aicodebot-0.5.0/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 23:11:22.000000 aicodebot-0.5.0/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 23:11:22.000000 aicodebot-0.5.0/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 23:11:22.000000 aicodebot-0.5.0/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-26 23:11:02.000000 aicodebot-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 23:11:22.388131 aicodebot-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-26 23:11:02.000000 aicodebot-0.5.0/setup.py
```

### Comparing `aicodebot-0.4.1/LICENSE` & `aicodebot-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.4.1/PKG-INFO` & `aicodebot-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.4.1
+Version: 0.5.0
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aicodebot-0.4.1/README.md` & `aicodebot-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aicodebot-0.4.1/aicodebot/prompts/alignment.yaml` & `aicodebot-0.5.0/aicodebot/prompts/alignment.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.4.1/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.5.0/aicodebot/prompts/commit_message.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 _type: prompt
 template_format: f-string
-input_variables: ["diff"]
+input_variables: ["diff_context"]
 template: |
-    I have a diff of a code change that I need to commit to a git repository. The diff is as follows:
+    I have a diff of a code change that I need to commit to a git repository. The relevant diff context is as follows,
+    between the BEGIN DIFF and END DIFF markers:
 
     BEGIN DIFF
-    {diff}
+    {diff_context}
     END DIFF
 
     Generate a commit message for me. The commit message should follow best practices,
     which means it should have a short, single-line summary, followed by a blank line, and then a more
     detailed explanatory text, but only if necessary.
     Avoid redundancy between the summary line and the explanatory text. Don't repeat yourself.
     If the detailed explanatory text is not necessary, then omit it and just do the summary
+    Use imperative mood for the commit message, e.g. "Add feature" instead of "Added feature".
 
     The text can be in GitHub-flavored markdown format.
 
     Contextually appropriate emojis are encouraged, but not required.
 
     Important - the summary line should not be longer than 72 characters.
```

### Comparing `aicodebot-0.4.1/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.5.0/aicodebot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.4.1
+Version: 0.5.0
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aicodebot-0.4.1/pyproject.toml` & `aicodebot-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.4.1/setup.py` & `aicodebot-0.5.0/setup.py`

 * *Files identical despite different names*

