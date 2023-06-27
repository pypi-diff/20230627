# Comparing `tmp/LLM-Toolbox-0.1.5.tar.gz` & `tmp/LLM-Toolbox-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM-Toolbox-0.1.5.tar", last modified: Tue Jun 27 10:23:46 2023, max compression
+gzip compressed data, was "LLM-Toolbox-0.1.6.tar", last modified: Tue Jun 27 10:29:22 2023, max compression
```

## Comparing `LLM-Toolbox-0.1.5.tar` & `LLM-Toolbox-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.5/LICENSE
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17827 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      913 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      702 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       96 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17827 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17289 2023-06-27 04:18:20.000000 LLM-Toolbox-0.1.5/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/llm_toolbox/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.5/llm_toolbox/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15872 2023-06-27 10:19:56.000000 LLM-Toolbox-0.1.5/llm_toolbox/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/llm_toolbox/tools/
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/cheermeup.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/codereview.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/commitgen.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/critique.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/define.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/explain.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/lessonize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      818 2023-06-27 10:12:29.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/life.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/pathlearner.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/proofread.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/study.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      411 2023-06-27 04:12:58.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/summarize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/teachlib.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/thesaurus.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/translate.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2173 2023-06-27 10:20:58.000000 LLM-Toolbox-0.1.5/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:29:22.030678 LLM-Toolbox-0.1.6/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.6/LICENSE
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:29:22.030678 LLM-Toolbox-0.1.6/LLM_Toolbox.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17827 2023-06-27 10:29:22.000000 LLM-Toolbox-0.1.6/LLM_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      913 2023-06-27 10:29:22.000000 LLM-Toolbox-0.1.6/LLM_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-27 10:29:22.000000 LLM-Toolbox-0.1.6/LLM_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      702 2023-06-27 10:29:22.000000 LLM-Toolbox-0.1.6/LLM_Toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       96 2023-06-27 10:29:22.000000 LLM-Toolbox-0.1.6/LLM_Toolbox.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-27 10:29:22.000000 LLM-Toolbox-0.1.6/LLM_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17827 2023-06-27 10:29:22.030678 LLM-Toolbox-0.1.6/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17289 2023-06-27 04:18:20.000000 LLM-Toolbox-0.1.6/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:29:22.030678 LLM-Toolbox-0.1.6/llm_toolbox/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.6/llm_toolbox/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15872 2023-06-27 10:19:56.000000 LLM-Toolbox-0.1.6/llm_toolbox/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:29:22.020678 LLM-Toolbox-0.1.6/llm_toolbox/tools/
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:29:22.030678 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/cheermeup.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/codereview.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/commitgen.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/critique.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/define.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/explain.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/lessonize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      831 2023-06-27 10:28:40.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/life.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/pathlearner.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/proofread.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/study.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      411 2023-06-27 04:12:58.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/summarize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/teachlib.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/thesaurus.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/translate.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-27 10:29:22.030678 LLM-Toolbox-0.1.6/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2173 2023-06-27 10:29:03.000000 LLM-Toolbox-0.1.6/setup.py
```

### Comparing `LLM-Toolbox-0.1.5/LICENSE` & `LLM-Toolbox-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/PKG-INFO` & `LLM-Toolbox-0.1.6/LLM_Toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.5
+Version: 0.1.6
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
```

### Comparing `LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/SOURCES.txt` & `LLM-Toolbox-0.1.6/LLM_Toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/entry_points.txt` & `LLM-Toolbox-0.1.6/LLM_Toolbox.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/PKG-INFO` & `LLM-Toolbox-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.5
+Version: 0.1.6
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
```

### Comparing `LLM-Toolbox-0.1.5/README.md` & `LLM-Toolbox-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/llm_toolbox/cli.py` & `LLM-Toolbox-0.1.6/llm_toolbox/cli.py`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/codereview.yaml` & `LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/codereview.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/commitgen.yaml` & `LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/commitgen.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/critique.yaml` & `LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/critique.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/lessonize.yaml` & `LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/lessonize.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/life.yaml` & `LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/life.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 user_info:
   name:
   date_of_birth:
   life_expectancy: 28470 # Average life expectancy in days, approximately 78 years
 
 system: >
-  Write a thoughtful, genuine message for {user_name},
+  As a friend, write a thoughtful, genuine message for {user_name},
   who has about {remaining_days} days ahead of them,
   which represents approximately {percentage}% of their expected life span.
   Based on this percentage, provide a unique perspective
   on how {user_name} might view their future.
   Keep in mind that these are statistical estimations
   and the uncertainty of life is what makes it precious.
   Make sure to reference these numbers in your message,
```

### Comparing `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/pathlearner.yaml` & `LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/pathlearner.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/teachlib.yaml` & `LLM-Toolbox-0.1.6/llm_toolbox/tools/templates/teachlib.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.5/setup.py` & `LLM-Toolbox-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 from pathlib import Path
 import shutil
 
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

