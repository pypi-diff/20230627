# Comparing `tmp/gspot_django_auth-0.0.1.tar.gz` & `tmp/gspot_django_auth-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspot_django_auth-0.0.1.tar", last modified: Tue Jun 27 13:53:48 2023, max compression
+gzip compressed data, was "gspot_django_auth-0.0.2.tar", last modified: Tue Jun 27 14:00:24 2023, max compression
```

## Comparing `gspot_django_auth-0.0.1.tar` & `gspot_django_auth-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 13:53:48.928213 gspot_django_auth-0.0.1/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.1/LICENSE
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.1/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)     1068 2023-06-27 13:53:48.928289 gspot_django_auth-0.0.1/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      472 2023-06-27 13:53:48.000000 gspot_django_auth-0.0.1/README.md
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 13:53:48.927213 gspot_django_auth-0.0.1/gspot-django-auth/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.1/gspot-django-auth/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1294 2023-06-27 12:37:46.000000 gspot_django_auth-0.0.1/gspot-django-auth/authentication.py
--rw-r--r--   0 vitya      (501) staff       (20)      229 2023-06-27 13:40:12.000000 gspot_django_auth-0.0.1/gspot-django-auth/exceptions.py
--rw-r--r--   0 vitya      (501) staff       (20)     1535 2023-06-27 12:19:26.000000 gspot_django_auth-0.0.1/gspot-django-auth/models.py
--rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.1/gspot-django-auth/redis_client.py
--rw-r--r--   0 vitya      (501) staff       (20)      711 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.1/gspot-django-auth/token.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 13:53:48.928058 gspot_django_auth-0.0.1/gspot_django_auth.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)     1068 2023-06-27 13:53:48.000000 gspot_django_auth-0.0.1/gspot_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      454 2023-06-27 13:53:48.000000 gspot_django_auth-0.0.1/gspot_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-27 13:53:48.000000 gspot_django_auth-0.0.1/gspot_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-27 13:53:48.000000 gspot_django_auth-0.0.1/gspot_django_auth.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-27 13:53:48.000000 gspot_django_auth-0.0.1/gspot_django_auth.egg-info/top_level.txt
--rw-r--r--   0 vitya      (501) staff       (20)      988 2023-06-27 13:53:48.000000 gspot_django_auth-0.0.1/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-27 13:53:48.928590 gspot_django_auth-0.0.1/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)       37 2023-06-24 17:48:18.000000 gspot_django_auth-0.0.1/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:00:24.436073 gspot_django_auth-0.0.2/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.2/LICENSE
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.2/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)     1068 2023-06-27 14:00:24.436170 gspot_django_auth-0.0.2/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      472 2023-06-27 13:53:48.000000 gspot_django_auth-0.0.2/README.md
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:00:24.435026 gspot_django_auth-0.0.2/gspot_django_auth/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.2/gspot_django_auth/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1294 2023-06-27 12:37:46.000000 gspot_django_auth-0.0.2/gspot_django_auth/authentication.py
+-rw-r--r--   0 vitya      (501) staff       (20)      229 2023-06-27 13:40:12.000000 gspot_django_auth-0.0.2/gspot_django_auth/exceptions.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1535 2023-06-27 12:19:26.000000 gspot_django_auth-0.0.2/gspot_django_auth/models.py
+-rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.2/gspot_django_auth/redis_client.py
+-rw-r--r--   0 vitya      (501) staff       (20)      711 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.2/gspot_django_auth/token.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:00:24.435918 gspot_django_auth-0.0.2/gspot_django_auth.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)     1068 2023-06-27 14:00:24.000000 gspot_django_auth-0.0.2/gspot_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      454 2023-06-27 14:00:24.000000 gspot_django_auth-0.0.2/gspot_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-27 14:00:24.000000 gspot_django_auth-0.0.2/gspot_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-27 14:00:24.000000 gspot_django_auth-0.0.2/gspot_django_auth.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-27 14:00:24.000000 gspot_django_auth-0.0.2/gspot_django_auth.egg-info/top_level.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      988 2023-06-27 14:00:23.000000 gspot_django_auth-0.0.2/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-27 14:00:24.436497 gspot_django_auth-0.0.2/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)       37 2023-06-24 17:48:18.000000 gspot_django_auth-0.0.2/setup.py
```

### Comparing `gspot_django_auth-0.0.1/LICENSE` & `gspot_django_auth-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.1/PKG-INFO` & `gspot_django_auth-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot_django_auth
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
```

### Comparing `gspot_django_auth-0.0.1/gspot-django-auth/authentication.py` & `gspot_django_auth-0.0.2/gspot_django_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.1/gspot-django-auth/models.py` & `gspot_django_auth-0.0.2/gspot_django_auth/models.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.1/gspot-django-auth/redis_client.py` & `gspot_django_auth-0.0.2/gspot_django_auth/redis_client.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.1/gspot-django-auth/token.py` & `gspot_django_auth-0.0.2/gspot_django_auth/token.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.1/gspot_django_auth.egg-info/PKG-INFO` & `gspot_django_auth-0.0.2/gspot_django_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot-django-auth
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
```

### Comparing `gspot_django_auth-0.0.1/pyproject.toml` & `gspot_django_auth-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_django_auth"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = "A Django app for auth."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_django_auth-0.0.1/setup.cfg` & `gspot_django_auth-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gspot_django_auth
-version = 0.1
+version = 0.2
 description = A Django app for auth.
 long_description = file: README.md
 url = https://github.com/DJWOMS/GSpot
 author = Kosenko Viktor
 author_email = kosenkoviktor11@gmail.com
 license = MIT License
 classifiers =
```

