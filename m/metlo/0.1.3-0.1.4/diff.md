# Comparing `tmp/metlo-0.1.3.tar.gz` & `tmp/metlo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/akshay/code/metlo-enterprise/ingestors/python/dist/.tmp-tjmjvnxw/metlo-0.1.3.tar", last modified: Thu Jun 22 22:40:23 2023, max compression
+gzip compressed data, was "/Users/akshay/code/metlo-enterprise/ingestors/python/dist/.tmp-33bxv6nz/metlo-0.1.4.tar", last modified: Tue Jun 27 19:26:58 2023, max compression
```

## Comparing `metlo-0.1.3.tar` & `metlo-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-22 22:40:23.000000 metlo-0.1.3/
--rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-22 22:40:23.000000 metlo-0.1.3/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)     1513 2022-10-31 23:50:46.000000 metlo-0.1.3/README.md
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo/
--rw-r--r--   0 akshay     (501) staff       (20)        0 2022-10-31 23:50:46.000000 metlo-0.1.3/metlo/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)     7795 2023-06-21 05:25:41.000000 metlo-0.1.3/metlo/django.py
--rw-r--r--   0 akshay     (501) staff       (20)    22277 2023-06-22 22:39:55.000000 metlo-0.1.3/metlo/fastapi.py
--rw-r--r--   0 akshay     (501) staff       (20)     7380 2023-06-21 05:25:41.000000 metlo-0.1.3/metlo/flask.py
--rw-r--r--   0 akshay     (501) staff       (20)      382 2023-06-21 05:25:41.000000 metlo-0.1.3/metlo/utils.py
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/
--rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      259 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (501) staff       (20)        1 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (501) staff       (20)       42 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/requires.txt
--rw-r--r--   0 akshay     (501) staff       (20)        6 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/top_level.txt
--rw-r--r--   0 akshay     (501) staff       (20)       80 2022-10-31 23:50:46.000000 metlo-0.1.3/pyproject.toml
--rw-r--r--   0 akshay     (501) staff       (20)     1175 2023-06-22 22:40:23.000000 metlo-0.1.3/setup.cfg
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-27 19:26:58.000000 metlo-0.1.4/
+-rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-27 19:26:58.000000 metlo-0.1.4/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)     1513 2022-10-31 23:50:46.000000 metlo-0.1.4/README.md
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-27 19:26:58.000000 metlo-0.1.4/metlo/
+-rw-r--r--   0 akshay     (501) staff       (20)        0 2022-10-31 23:50:46.000000 metlo-0.1.4/metlo/__init__.py
+-rw-r--r--   0 akshay     (501) staff       (20)     7795 2023-06-21 05:25:41.000000 metlo-0.1.4/metlo/django.py
+-rw-r--r--   0 akshay     (501) staff       (20)    22737 2023-06-27 19:26:33.000000 metlo-0.1.4/metlo/fastapi.py
+-rw-r--r--   0 akshay     (501) staff       (20)     7380 2023-06-21 05:25:41.000000 metlo-0.1.4/metlo/flask.py
+-rw-r--r--   0 akshay     (501) staff       (20)      382 2023-06-21 05:25:41.000000 metlo-0.1.4/metlo/utils.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-27 19:26:58.000000 metlo-0.1.4/metlo.egg-info/
+-rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-27 19:26:58.000000 metlo-0.1.4/metlo.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      259 2023-06-27 19:26:58.000000 metlo-0.1.4/metlo.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        1 2023-06-27 19:26:58.000000 metlo-0.1.4/metlo.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       42 2023-06-27 19:26:58.000000 metlo-0.1.4/metlo.egg-info/requires.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        6 2023-06-27 19:26:58.000000 metlo-0.1.4/metlo.egg-info/top_level.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       80 2022-10-31 23:50:46.000000 metlo-0.1.4/pyproject.toml
+-rw-r--r--   0 akshay     (501) staff       (20)     1175 2023-06-27 19:26:58.000000 metlo-0.1.4/setup.cfg
```

### Comparing `metlo-0.1.3/PKG-INFO` & `metlo-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metlo
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Python Agent for Metlo
 Home-page: https://www.metlo.com
 License: MIT
 Project-URL: Documentation, https://docs.metlo.com/docs/python
 Project-URL: Source Code, https://github.com/metlo-labs/metlo/
 Project-URL: Issue Tracker, https://github.com/metlo-labs/metlo/issues/
 Project-URL: Twitter, https://mobile.twitter.com/metlohq
```

### Comparing `metlo-0.1.3/README.md` & `metlo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `metlo-0.1.3/metlo/django.py` & `metlo-0.1.4/metlo/django.py`

 * *Files identical despite different names*

### Comparing `metlo-0.1.3/metlo/fastapi.py` & `metlo-0.1.4/metlo/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,28 @@
         return default
 
 
 def set_value_in_state(key: str, data: typing.Any, scope: Scope):
     scope["state"][get_key(key)] = data
 
 
-class ASGIMiddleware:
+class ASGIMiddleware(object):
+    instance = None
+
+    def __init__(self, app, host, api_key, **kwargs):
+        if ASGIMiddleware.instance is None:
+            ASGIMiddleware.instance = MetaASGIMiddleware(app, host, api_key, **kwargs)
+        else:
+            ASGIMiddleware.instance.logger.debug("Attempted multiple init")
+
+    async def __call__(self, scope, receive, send):
+        return await ASGIMiddleware.instance(scope, receive, send)
+
+
+class MetaASGIMiddleware(object):
     def compile_request(self, scope: Scope):
         user = None
         req_body = ""
         try:
             user = self.get_user(scope) if self.get_user is not None else None
         except Exception as e:
             self.logger.error("Error obtaining user info from function")
```

### Comparing `metlo-0.1.3/metlo/flask.py` & `metlo-0.1.4/metlo/flask.py`

 * *Files identical despite different names*

### Comparing `metlo-0.1.3/metlo.egg-info/PKG-INFO` & `metlo-0.1.4/metlo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metlo
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Python Agent for Metlo
 Home-page: https://www.metlo.com
 License: MIT
 Project-URL: Documentation, https://docs.metlo.com/docs/python
 Project-URL: Source Code, https://github.com/metlo-labs/metlo/
 Project-URL: Issue Tracker, https://github.com/metlo-labs/metlo/issues/
 Project-URL: Twitter, https://mobile.twitter.com/metlohq
```

### Comparing `metlo-0.1.3/setup.cfg` & `metlo-0.1.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = metlo
-version = 0.1.3
+version = 0.1.4
 description = The Python Agent for Metlo
 long_description = file: README.md
 long_description_content_type = text/markdown
 repository = https://github.com/metlo-labs/metlo
 url = https://www.metlo.com
 license = MIT
 project_urls =
```

