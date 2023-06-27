# Comparing `tmp/gspot_django_auth-0.0.4.tar.gz` & `tmp/gspot_django_auth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspot_django_auth-0.0.4.tar", last modified: Tue Jun 27 14:48:19 2023, max compression
+gzip compressed data, was "gspot_django_auth-0.0.5.tar", last modified: Tue Jun 27 14:56:22 2023, max compression
```

## Comparing `gspot_django_auth-0.0.4.tar` & `gspot_django_auth-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:48:19.402037 gspot_django_auth-0.0.4/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.4/LICENSE
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.4/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)     1226 2023-06-27 14:48:19.402146 gspot_django_auth-0.0.4/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      631 2023-06-27 14:47:21.000000 gspot_django_auth-0.0.4/README.md
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:48:19.400570 gspot_django_auth-0.0.4/gspot_django_auth/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.4/gspot_django_auth/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1294 2023-06-27 12:37:46.000000 gspot_django_auth-0.0.4/gspot_django_auth/authentication.py
--rw-r--r--   0 vitya      (501) staff       (20)      282 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.4/gspot_django_auth/exceptions.py
--rw-r--r--   0 vitya      (501) staff       (20)     1535 2023-06-27 12:19:26.000000 gspot_django_auth-0.0.4/gspot_django_auth/models.py
--rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.4/gspot_django_auth/redis_client.py
--rw-r--r--   0 vitya      (501) staff       (20)      712 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.4/gspot_django_auth/token.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:48:19.401812 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)     1226 2023-06-27 14:48:19.000000 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      454 2023-06-27 14:48:19.000000 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-27 14:48:19.000000 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-27 14:48:19.000000 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-27 14:48:19.000000 gspot_django_auth-0.0.4/gspot_django_auth.egg-info/top_level.txt
--rw-r--r--   0 vitya      (501) staff       (20)      989 2023-06-27 14:48:11.000000 gspot_django_auth-0.0.4/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-27 14:48:19.402517 gspot_django_auth-0.0.4/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)       37 2023-06-24 17:48:18.000000 gspot_django_auth-0.0.4/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:56:22.055378 gspot_django_auth-0.0.5/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.5/LICENSE
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.5/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)     1226 2023-06-27 14:56:22.055479 gspot_django_auth-0.0.5/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      631 2023-06-27 14:47:21.000000 gspot_django_auth-0.0.5/README.md
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:56:22.054037 gspot_django_auth-0.0.5/gspot_django_auth/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.5/gspot_django_auth/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1209 2023-06-27 14:56:06.000000 gspot_django_auth-0.0.5/gspot_django_auth/authentication.py
+-rw-r--r--   0 vitya      (501) staff       (20)      282 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.5/gspot_django_auth/exceptions.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1535 2023-06-27 12:19:26.000000 gspot_django_auth-0.0.5/gspot_django_auth/models.py
+-rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.5/gspot_django_auth/redis_client.py
+-rw-r--r--   0 vitya      (501) staff       (20)      712 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.5/gspot_django_auth/token.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 14:56:22.055171 gspot_django_auth-0.0.5/gspot_django_auth.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)     1226 2023-06-27 14:56:21.000000 gspot_django_auth-0.0.5/gspot_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      454 2023-06-27 14:56:22.000000 gspot_django_auth-0.0.5/gspot_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-27 14:56:21.000000 gspot_django_auth-0.0.5/gspot_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-27 14:56:21.000000 gspot_django_auth-0.0.5/gspot_django_auth.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-27 14:56:21.000000 gspot_django_auth-0.0.5/gspot_django_auth.egg-info/top_level.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      989 2023-06-27 14:56:19.000000 gspot_django_auth-0.0.5/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-27 14:56:22.055834 gspot_django_auth-0.0.5/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)       37 2023-06-24 17:48:18.000000 gspot_django_auth-0.0.5/setup.py
```

### Comparing `gspot_django_auth-0.0.4/LICENSE` & `gspot_django_auth-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.4/PKG-INFO` & `gspot_django_auth-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot_django_auth
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
```

### Comparing `gspot_django_auth-0.0.4/README.md` & `gspot_django_auth-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.4/gspot_django_auth/authentication.py` & `gspot_django_auth-0.0.5/gspot_django_auth/authentication.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,20 @@
 from .models import UserFactory
 from .exceptions import AuthenticationFailed
 from .token import Token
 
 
 class CustomJWTAuthentication(BaseAuthentication):
     def authenticate(self, request):
-        try:
-            jwt_token = self.get_token(request)
-        except AuthenticationFailed:
-            return None
-
+        jwt_token = self.get_token(request)
         token = Token()
 
         data = token.get_token_data(jwt_token)
         if not data:
-            raise AuthenticationFailed('Empty Payload')
+            raise AuthenticationFailed('No data')
         user_class = UserFactory().get_user(data.pop('role'))
         return user_class(**data)
 
     def get_token(self, request) -> str:
         if settings.GET_TOKEN_FROM == 'header':
             token = self._get_token_from_header(request)
         else:
```

### Comparing `gspot_django_auth-0.0.4/gspot_django_auth/models.py` & `gspot_django_auth-0.0.5/gspot_django_auth/models.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.4/gspot_django_auth/redis_client.py` & `gspot_django_auth-0.0.5/gspot_django_auth/redis_client.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.4/gspot_django_auth/token.py` & `gspot_django_auth-0.0.5/gspot_django_auth/token.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.4/gspot_django_auth.egg-info/PKG-INFO` & `gspot_django_auth-0.0.5/gspot_django_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot-django-auth
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
```

### Comparing `gspot_django_auth-0.0.4/pyproject.toml` & `gspot_django_auth-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_django_auth"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = "A Django app for auth."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_django_auth-0.0.4/setup.cfg` & `gspot_django_auth-0.0.5/setup.cfg`

 * *Files identical despite different names*

