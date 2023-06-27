# Comparing `tmp/auto-eval-0.2.6.tar.gz` & `tmp/auto-eval-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.2.6.tar", last modified: Tue Jun 13 07:08:03 2023, max compression
+gzip compressed data, was "auto-eval-0.2.7.tar", last modified: Tue Jun 27 06:40:23 2023, max compression
```

## Comparing `auto-eval-0.2.6.tar` & `auto-eval-0.2.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-13 07:08:03.663618 auto-eval-0.2.6/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.6/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-13 07:08:03.663381 auto-eval-0.2.6/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.2.6/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-13 07:08:03.660444 auto-eval-0.2.6/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-13 07:08:03.000000 auto-eval-0.2.6/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-06-13 07:08:03.000000 auto-eval-0.2.6/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-13 07:08:03.000000 auto-eval-0.2.6/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-06-13 07:08:03.000000 auto-eval-0.2.6/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-06-13 07:08:03.000000 auto-eval-0.2.6/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-06-13 07:08:03.000000 auto-eval-0.2.6/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-13 07:08:03.660884 auto-eval-0.2.6/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.6/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    10360 2023-06-06 12:00:40.000000 auto-eval-0.2.6/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-13 07:08:03.661321 auto-eval-0.2.6/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.6/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6088 2023-06-06 11:35:46.000000 auto-eval-0.2.6/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-13 07:08:03.662400 auto-eval-0.2.6/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.6/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3090 2023-06-13 06:40:19.000000 auto-eval-0.2.6/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2026 2023-06-06 12:13:28.000000 auto-eval-0.2.6/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-13 07:08:03.662995 auto-eval-0.2.6/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.6/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     4152 2023-06-13 06:59:50.000000 auto-eval-0.2.6/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-13 07:08:03.663667 auto-eval-0.2.6/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-06-13 06:57:04.000000 auto-eval-0.2.6/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.955586 auto-eval-0.2.7/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.7/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-27 06:40:23.955322 auto-eval-0.2.7/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.2.7/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.952563 auto-eval-0.2.7/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-06-27 06:40:23.000000 auto-eval-0.2.7/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.953132 auto-eval-0.2.7/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.7/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    10360 2023-06-06 12:00:40.000000 auto-eval-0.2.7/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.953606 auto-eval-0.2.7/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.7/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6088 2023-06-06 11:35:46.000000 auto-eval-0.2.7/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.954511 auto-eval-0.2.7/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.7/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.2.7/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2418 2023-06-27 06:37:14.000000 auto-eval-0.2.7/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-27 06:40:23.954962 auto-eval-0.2.7/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.7/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4152 2023-06-13 06:59:50.000000 auto-eval-0.2.7/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-27 06:40:23.955629 auto-eval-0.2.7/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-06-27 06:40:14.000000 auto-eval-0.2.7/setup.py
```

### Comparing `auto-eval-0.2.6/LICENSE` & `auto-eval-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.6/PKG-INFO` & `auto-eval-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.6
+Version: 0.2.7
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.2.6/README.md` & `auto-eval-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.6/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.2.7/auto_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.6
+Version: 0.2.7
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.2.6/eval/auto_llms_eval.py` & `auto-eval-0.2.7/eval/auto_llms_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.6/eval/commands/auto_eval.py` & `auto-eval-0.2.7/eval/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.6/eval/prompt_template/prompter.py` & `auto-eval-0.2.7/eval/prompt_template/prompter.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def generate_prompt(self, question: str, target: str,
                         candidate_answers: List[str]) -> str:
         """
         Generate a prompt based on the given question, target, and candidate answers.
         """
         candidate_answer_numbers = generate_letters(len(candidate_answers))
         format_option_data = '\n\n'.join([
-            f'{candidate_answer_numbers[i]}. {candidate_answers[i]}'
+            f'**{candidate_answer_numbers[i]}**. {candidate_answers[i]}'
             for i in range(len(candidate_answers))
         ])
 
         if target:
             eval_prompt = self.eval_with_target_template.format(
                 question=question, target=target, answers=format_option_data)
         else:
```

### Comparing `auto-eval-0.2.6/eval/utils/data_utils.py` & `auto-eval-0.2.7/eval/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.6/setup.py` & `auto-eval-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.2.6",
+    version="0.2.7",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

