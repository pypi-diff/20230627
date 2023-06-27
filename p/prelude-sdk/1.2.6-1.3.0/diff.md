# Comparing `tmp/prelude-sdk-1.2.6.tar.gz` & `tmp/prelude-sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.2.6.tar", last modified: Wed Jun 21 21:00:59 2023, max compression
+gzip compressed data, was "prelude-sdk-1.3.0.tar", last modified: Tue Jun 27 14:54:28 2023, max compression
```

## Comparing `prelude-sdk-1.2.6.tar` & `prelude-sdk-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:00:59.510915 prelude-sdk-1.2.6/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.2.6/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-21 21:00:59.510960 prelude-sdk-1.2.6/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.2.6/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:00:59.507082 prelude-sdk-1.2.6/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.6/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:00:59.508911 prelude-sdk-1.2.6/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.6/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2248 2023-06-06 22:22:58.000000 prelude-sdk-1.2.6/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5438 2023-06-06 22:22:58.000000 prelude-sdk-1.2.6/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3711 2023-06-08 13:35:49.000000 prelude-sdk-1.2.6/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     2057 2023-05-23 21:42:11.000000 prelude-sdk-1.2.6/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.2.6/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:00:59.509565 prelude-sdk-1.2.6/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.6/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.2.6/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2964 2023-06-21 16:09:59.000000 prelude-sdk-1.2.6/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:00:59.507613 prelude-sdk-1.2.6/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-21 21:00:59.000000 prelude-sdk-1.2.6/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      773 2023-06-21 21:00:59.000000 prelude-sdk-1.2.6/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-21 21:00:59.000000 prelude-sdk-1.2.6/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-06-21 21:00:59.000000 prelude-sdk-1.2.6/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-06-21 21:00:59.000000 prelude-sdk-1.2.6/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.2.6/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2023-06-21 21:00:59.511160 prelude-sdk-1.2.6/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:00:59.510605 prelude-sdk-1.2.6/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.6/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.2.6/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:00:59.510823 prelude-sdk-1.2.6/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.6/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.2.6/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.2.6/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.2.6/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.2.6/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.307729 prelude-sdk-1.3.0/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.3.0/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-27 14:54:28.307780 prelude-sdk-1.3.0/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.3.0/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.303319 prelude-sdk-1.3.0/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.0/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.305134 prelude-sdk-1.3.0/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2416 2023-06-23 19:11:07.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5438 2023-06-06 22:22:58.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3711 2023-06-08 13:35:49.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     2057 2023-05-23 21:42:11.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.3.0/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.305841 prelude-sdk-1.3.0/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.0/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.3.0/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     2964 2023-06-21 16:09:59.000000 prelude-sdk-1.3.0/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.303859 prelude-sdk-1.3.0/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-27 14:54:28.000000 prelude-sdk-1.3.0/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      773 2023-06-27 14:54:28.000000 prelude-sdk-1.3.0/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-27 14:54:28.000000 prelude-sdk-1.3.0/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-06-27 14:54:28.000000 prelude-sdk-1.3.0/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-06-27 14:54:28.000000 prelude-sdk-1.3.0/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.3.0/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-06-27 14:54:28.307986 prelude-sdk-1.3.0/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.307430 prelude-sdk-1.3.0/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.0/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.3.0/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:54:28.307643 prelude-sdk-1.3.0/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.0/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.3.0/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.3.0/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.3.0/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.3.0/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-1.2.6/LICENSE` & `prelude-sdk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/PKG-INFO` & `prelude-sdk-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.2.6
+Version: 1.3.0
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.2.6/README.md` & `prelude-sdk-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.3.0/prelude_sdk/controllers/build_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 class BuildController:
 
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
-    def create_test(self, name, unit, advisory=None, test_id=None):
+    def create_test(self, name, unit, techniques=None, advisory=None, test_id=None):
         """ Create or update a test """
         body = dict(name=name, unit=unit)
+        if techniques:
+            body['techniques'] = techniques
         if advisory:
             body['advisory'] = advisory
         if test_id:
             body['id'] = test_id
 
         res = requests.post(
             f'{self.account.hq}/build/tests',
@@ -24,21 +26,23 @@
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
-    def update_test(self, test_id, name=None, unit=None, advisory=None):
+    def update_test(self, test_id, name=None, unit=None, techniques=None, advisory=None):
         """ Update a test """
         body = dict()
         if name:
             body['name'] = name
         if unit:
             body['unit'] = unit
+        if techniques:
+            body['techniques'] = techniques
         if advisory:
             body['advisory'] = advisory
 
         res = requests.post(
             f'{self.account.hq}/build/tests/{test_id}',
             json=body,
             headers=self.account.headers,
```

### Comparing `prelude-sdk-1.2.6/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.3.0/prelude_sdk/controllers/detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.3.0/prelude_sdk/controllers/iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/prelude_sdk/controllers/partner_controller.py` & `prelude-sdk-1.3.0/prelude_sdk/controllers/partner_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/prelude_sdk/models/account.py` & `prelude-sdk-1.3.0/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/prelude_sdk/models/codes.py` & `prelude-sdk-1.3.0/prelude_sdk/models/codes.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.3.0/prelude_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.2.6
+Version: 1.3.0
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.2.6/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.3.0/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/setup.cfg` & `prelude-sdk-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.2.6
+version = 1.3.0
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.2.6/tests/conftest.py` & `prelude-sdk-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/tests/test_build_controller.py` & `prelude-sdk-1.3.0/tests/test_build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/tests/test_detect_controller.py` & `prelude-sdk-1.3.0/tests/test_detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/tests/test_iam_controller.py` & `prelude-sdk-1.3.0/tests/test_iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.6/tests/test_probe_controller.py` & `prelude-sdk-1.3.0/tests/test_probe_controller.py`

 * *Files identical despite different names*

