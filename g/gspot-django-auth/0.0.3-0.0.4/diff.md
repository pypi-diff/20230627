# Comparing `tmp/gspot_django_auth-0.0.3.tar.gz` & `tmp/gspot_django_auth-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspot_django_auth-0.0.3.tar", last modified: Tue Jun 27 14:04:31 2023, max compression
+gzip compressed data, was "gspot_django_auth-0.0.4.tar", last modified: Tue Jun 27 14:48:19 2023, max compression
```

## Comparing `gspot_django_auth-0.0.3.tar` & `gspot_django_auth-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:04:31.709888 gspot_django_auth-0.0.3/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.3/LICENSE
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.3/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)     1068 2023-06-27 14:04:31.709980 gspot_django_auth-0.0.3/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      472 2023-06-27 13:53:48.000000 gspot_django_auth-0.0.3/README.md
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:04:31.708876 gspot_django_auth-0.0.3/gspot_django_auth/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.3/gspot_django_auth/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1294 2023-06-27 12:37:46.000000 gspot_django_auth-0.0.3/gspot_django_auth/authentication.py
--rw-r--r--   0 vitya      (501) staff       (20)      282 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.3/gspot_django_auth/exceptions.py
--rw-r--r--   0 vitya      (501) staff       (20)     1535 2023-06-27 12:19:26.000000 gspot_django_auth-0.0.3/gspot_django_auth/models.py
--rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.3/gspot_django_auth/redis_client.py
--rw-r--r--   0 vitya      (501) staff       (20)      712 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.3/gspot_django_auth/token.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:04:31.709745 gspot_django_auth-0.0.3/gspot_django_auth.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)     1068 2023-06-27 14:04:31.000000 gspot_django_auth-0.0.3/gspot_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      454 2023-06-27 14:04:31.000000 gspot_django_auth-0.0.3/gspot_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-27 14:04:31.000000 gspot_django_auth-0.0.3/gspot_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-27 14:04:31.000000 gspot_django_auth-0.0.3/gspot_django_auth.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-27 14:04:31.000000 gspot_django_auth-0.0.3/gspot_django_auth.egg-info/top_level.txt
--rw-r--r--   0 vitya      (501) staff       (20)      988 2023-06-27 14:04:27.000000 gspot_django_auth-0.0.3/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-27 14:04:31.710313 gspot_django_auth-0.0.3/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)       37 2023-06-24 17:48:18.000000 gspot_django_auth-0.0.3/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:48:19.402037 gspot_django_auth-0.0.4/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.4/LICENSE
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.4/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)     1226 2023-06-27 14:48:19.402146 gspot_django_auth-0.0.4/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      631 2023-06-27 14:47:21.000000 gspot_django_auth-0.0.4/README.md
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:48:19.400570 gspot_django_auth-0.0.4/gspot_django_auth/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.4/gspot_django_auth/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1294 2023-06-27 12:37:46.000000 gspot_django_auth-0.0.4/gspot_django_auth/authentication.py
+-rw-r--r--   0 vitya      (501) staff       (20)      282 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.4/gspot_django_auth/exceptions.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1535 2023-06-27 12:19:26.000000 gspot_django_auth-0.0.4/gspot_django_auth/models.py
+-rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.4/gspot_django_auth/redis_client.py
+-rw-r--r--   0 vitya      (501) staff       (20)      712 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.4/gspot_django_auth/token.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:48:19.401812 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)     1226 2023-06-27 14:48:19.000000 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      454 2023-06-27 14:48:19.000000 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-27 14:48:19.000000 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-27 14:48:19.000000 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-27 14:48:19.000000 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/top_level.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      989 2023-06-27 14:48:11.000000 gspot_django_auth-0.0.4/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-27 14:48:19.402517 gspot_django_auth-0.0.4/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)       37 2023-06-24 17:48:18.000000 gspot_django_auth-0.0.4/setup.py
```

### Comparing `gspot_django_auth-0.0.3/LICENSE` & `gspot_django_auth-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.3/PKG-INFO` & `gspot_django_auth-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot_django_auth
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
@@ -27,14 +27,23 @@
 ```
 INSTALLED_APPS = [
     ...
     'gspot_django_auth',
 ]
 ```
 
+2. Define these parameters in `settings.py`
+
+- `REDIS_ACCESS_PREFIX`
+- `REDIS_ACCESS_DB`
+- `REDIS_HOST`
+- `REDIS_PORT`
+- `REDIS_PASSWORD`
+- `GET_TOKEN_FROM`
+
 2. Add CustomJWTAuthentication to DEFAULT_AUTHENTICATION_CLASSES in settings.py
 
 ```
 REST_FRAMEWORK = {
     ...
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'gspot_django_auth.authentication.CustomJWTAuthentication'
```

### Comparing `gspot_django_auth-0.0.3/gspot_django_auth/authentication.py` & `gspot_django_auth-0.0.4/gspot_django_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.3/gspot_django_auth/models.py` & `gspot_django_auth-0.0.4/gspot_django_auth/models.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.3/gspot_django_auth/redis_client.py` & `gspot_django_auth-0.0.4/gspot_django_auth/redis_client.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.3/gspot_django_auth/token.py` & `gspot_django_auth-0.0.4/gspot_django_auth/token.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.3/gspot_django_auth.egg-info/PKG-INFO` & `gspot_django_auth-0.0.4/gspot_django_auth.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot-django-auth
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
@@ -27,14 +27,23 @@
 ```
 INSTALLED_APPS = [
     ...
     'gspot_django_auth',
 ]
 ```
 
+2. Define these parameters in `settings.py`
+
+- `REDIS_ACCESS_PREFIX`
+- `REDIS_ACCESS_DB`
+- `REDIS_HOST`
+- `REDIS_PORT`
+- `REDIS_PASSWORD`
+- `GET_TOKEN_FROM`
+
 2. Add CustomJWTAuthentication to DEFAULT_AUTHENTICATION_CLASSES in settings.py
 
 ```
 REST_FRAMEWORK = {
     ...
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'gspot_django_auth.authentication.CustomJWTAuthentication'
```

### Comparing `gspot_django_auth-0.0.3/pyproject.toml` & `gspot_django_auth-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_django_auth"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = "A Django app for auth."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -42,8 +42,8 @@
     | \.tox
     | \.venv
     | _build
     | buck-out
     | build
     | dist
 )/
-'''
+'''
```

### Comparing `gspot_django_auth-0.0.3/setup.cfg` & `gspot_django_auth-0.0.4/setup.cfg`

 * *Files identical despite different names*

