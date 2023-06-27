# Comparing `tmp/ai-coach-xblock-1.0.2.tar.gz` & `tmp/ai-coach-xblock-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-coach-xblock-1.0.2.tar", last modified: Mon Jun 12 13:47:17 2023, max compression
+gzip compressed data, was "ai-coach-xblock-1.0.3.tar", last modified: Tue Jun 27 09:30:27 2023, max compression
```

## Comparing `ai-coach-xblock-1.0.2.tar` & `ai-coach-xblock-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.791727 ai-coach-xblock-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-06-12 13:47:17.791727 ai-coach-xblock-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.787727 ai-coach-xblock-1.0.2/ai_coach/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5909 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/ai_coach.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.787727 ai-coach-xblock-1.0.2/ai_coach/static/
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/static/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.787727 ai-coach-xblock-1.0.2/ai_coach/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/static/css/ai_coach.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.787727 ai-coach-xblock-1.0.2/ai_coach/static/html/
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/static/html/ai_coach.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.783727 ai-coach-xblock-1.0.2/ai_coach/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.787727 ai-coach-xblock-1.0.2/ai_coach/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/ai_coach/static/js/src/ai_coach.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:47:17.791727 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-12 13:47:17.000000 ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-12 13:47:17.791727 ai-coach-xblock-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-12 13:47:14.000000 ai-coach-xblock-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:30:27.660857 ai-coach-xblock-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-06-27 09:30:19.000000 ai-coach-xblock-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-06-27 09:30:27.656857 ai-coach-xblock-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-06-27 09:30:19.000000 ai-coach-xblock-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:30:27.656857 ai-coach-xblock-1.0.3/ai_coach/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-27 09:30:19.000000 ai-coach-xblock-1.0.3/ai_coach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8038 2023-06-27 09:30:19.000000 ai-coach-xblock-1.0.3/ai_coach/ai_coach.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:30:27.656857 ai-coach-xblock-1.0.3/ai_coach/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-27 09:30:19.000000 ai-coach-xblock-1.0.3/ai_coach/static/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:30:27.656857 ai-coach-xblock-1.0.3/ai_coach/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     6225 2023-06-27 09:30:19.000000 ai-coach-xblock-1.0.3/ai_coach/static/css/ai_coach.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:30:27.656857 ai-coach-xblock-1.0.3/ai_coach/static/html/
+-rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-06-27 09:30:19.000000 ai-coach-xblock-1.0.3/ai_coach/static/html/ai_coach.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:30:27.656857 ai-coach-xblock-1.0.3/ai_coach/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:30:27.656857 ai-coach-xblock-1.0.3/ai_coach/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     3645 2023-06-27 09:30:19.000000 ai-coach-xblock-1.0.3/ai_coach/static/js/src/ai_coach.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:30:27.656857 ai-coach-xblock-1.0.3/ai_coach_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-06-27 09:30:27.000000 ai-coach-xblock-1.0.3/ai_coach_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-06-27 09:30:27.000000 ai-coach-xblock-1.0.3/ai_coach_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 09:30:27.000000 ai-coach-xblock-1.0.3/ai_coach_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-27 09:30:27.000000 ai-coach-xblock-1.0.3/ai_coach_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-27 09:30:27.000000 ai-coach-xblock-1.0.3/ai_coach_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-27 09:30:27.000000 ai-coach-xblock-1.0.3/ai_coach_xblock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 09:30:27.660857 ai-coach-xblock-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-27 09:30:19.000000 ai-coach-xblock-1.0.3/setup.py
```

### Comparing `ai-coach-xblock-1.0.2/LICENSE` & `ai-coach-xblock-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.2/PKG-INFO` & `ai-coach-xblock-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-coach-xblock
-Version: 1.0.2
+Version: 1.0.3
 Summary: AI Coach Xblock evaluates open response answer of a question using Open AI
 Home-page: https://github.com/edly-io/ai-feedback-xblock
 Author: edly
 License: AGPL v3
 Description: # **AI Coach XBlock**
         
         AI Coach Xblock helps learner in improving their answers by levering power of AI. It evaluates open response answer of a question using Open AI and provides feedback to learner.
```

### Comparing `ai-coach-xblock-1.0.2/README.md` & `ai-coach-xblock-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.2/ai_coach/static/README.txt` & `ai-coach-xblock-1.0.3/ai_coach/static/README.txt`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.2/ai_coach_xblock.egg-info/PKG-INFO` & `ai-coach-xblock-1.0.3/ai_coach_xblock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-coach-xblock
-Version: 1.0.2
+Version: 1.0.3
 Summary: AI Coach Xblock evaluates open response answer of a question using Open AI
 Home-page: https://github.com/edly-io/ai-feedback-xblock
 Author: edly
 License: AGPL v3
 Description: # **AI Coach XBlock**
         
         AI Coach Xblock helps learner in improving their answers by levering power of AI. It evaluates open response answer of a question using Open AI and provides feedback to learner.
```

### Comparing `ai-coach-xblock-1.0.2/setup.py` & `ai-coach-xblock-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 data.append(os.path.relpath(os.path.join(dirname, fname), pkg))
 
     return {pkg: data}
 
 
 setup(
     name='ai-coach-xblock',
-    version='1.0.2',
+    version='1.0.3',
     description="AI Coach Xblock evaluates open response answer of a question using Open AI",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/edly-io/ai-feedback-xblock',
     license='AGPL v3',
     author='edly',
     packages=[
```

