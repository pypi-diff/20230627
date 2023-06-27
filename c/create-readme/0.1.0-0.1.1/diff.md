# Comparing `tmp/create_readme-0.1.0.tar.gz` & `tmp/create_readme-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_readme-0.1.0.tar", max compression
+gzip compressed data, was "create_readme-0.1.1.tar", max compression
```

## Comparing `create_readme-0.1.0.tar` & `create_readme-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1160 2023-06-27 18:51:32.773059 create_readme-0.1.0/README.md
--rw-r--r--   0        0        0       82 2023-06-27 18:43:26.598266 create_readme-0.1.0/create_readme/__init__.py
--rw-r--r--   0        0        0     5932 2023-06-27 18:44:51.614706 create_readme-0.1.0/create_readme/generator.py
--rw-r--r--   0        0        0      508 2023-06-27 18:29:28.541772 create_readme-0.1.0/create_readme/multiline_input.py
--rw-r--r--   0        0        0     1964 2023-06-27 18:34:21.129856 create_readme-0.1.0/create_readme/prompts.py
--rw-r--r--   0        0        0     1592 2023-06-27 18:09:25.112583 create_readme-0.1.0/create_readme/run.py
--rw-r--r--   0        0        0      444 2023-06-27 18:33:13.131302 create_readme-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 create_readme-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1160 2023-06-27 18:51:32.773059 create_readme-0.1.1/README.md
+-rw-r--r--   0        0        0       82 2023-06-27 18:43:26.598266 create_readme-0.1.1/create_readme/__init__.py
+-rw-r--r--   0        0        0     5932 2023-06-27 18:44:51.614706 create_readme-0.1.1/create_readme/generator.py
+-rw-r--r--   0        0        0      508 2023-06-27 18:29:28.541772 create_readme-0.1.1/create_readme/multiline_input.py
+-rw-r--r--   0        0        0     1964 2023-06-27 18:34:21.129856 create_readme-0.1.1/create_readme/prompts.py
+-rw-r--r--   0        0        0     1592 2023-06-27 18:09:25.112583 create_readme-0.1.1/create_readme/run.py
+-rw-r--r--   0        0        0      432 2023-06-27 18:58:43.675214 create_readme-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1550 1970-01-01 00:00:00.000000 create_readme-0.1.1/PKG-INFO
```

### Comparing `create_readme-0.1.0/README.md` & `create_readme-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `create_readme-0.1.0/create_readme/generator.py` & `create_readme-0.1.1/create_readme/generator.py`

 * *Files identical despite different names*

### Comparing `create_readme-0.1.0/create_readme/prompts.py` & `create_readme-0.1.1/create_readme/prompts.py`

 * *Files identical despite different names*

### Comparing `create_readme-0.1.0/create_readme/run.py` & `create_readme-0.1.1/create_readme/run.py`

 * *Files identical despite different names*

### Comparing `create_readme-0.1.0/PKG-INFO` & `create_readme-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: create-readme
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click-config-file (>=0.6.0,<0.7.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Description-Content-Type: text/markdown
 
 # create-readme
 
 create-readme is a tool that allows users to quickly and easily create README files with ChatGPT. By asking users a set of questions, create-readme generates a README based on the answers, eliminating the need to manually open OpenAI's website and type the prompt.
```

