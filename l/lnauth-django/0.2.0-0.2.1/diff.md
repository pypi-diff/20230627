# Comparing `tmp/lnauth_django-0.2.0.tar.gz` & `tmp/lnauth_django-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnauth_django-0.2.0.tar", max compression
+gzip compressed data, was "lnauth_django-0.2.1.tar", max compression
```

## Comparing `lnauth_django-0.2.0.tar` & `lnauth_django-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-06-24 22:25:50.420220 lnauth_django-0.2.0/LICENSE
--rw-r--r--   0        0        0     1424 2023-06-24 23:03:45.863381 lnauth_django-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-24 22:25:50.380220 lnauth_django-0.2.0/lnauth_django/__init__.py
--rw-r--r--   0        0        0      148 2023-06-24 22:34:51.066120 lnauth_django-0.2.0/lnauth_django/apps.py
--rw-r--r--   0        0        0      929 2023-06-24 23:33:54.636101 lnauth_django-0.2.0/lnauth_django/django.py
--rw-r--r--   0        0        0      141 2023-06-24 23:33:50.028248 lnauth_django-0.2.0/lnauth_django/exceptions.py
--rw-r--r--   0        0        0     1382 2023-06-24 22:50:06.437211 lnauth_django-0.2.0/lnauth_django/lnauth.py
--rw-r--r--   0        0        0      786 2023-06-26 23:23:58.916632 lnauth_django-0.2.0/lnauth_django/migrations/0000_initial.py
--rw-r--r--   0        0        0        0 2023-06-26 23:21:16.365884 lnauth_django-0.2.0/lnauth_django/migrations/__init__.py
--rw-r--r--   0        0        0      266 2023-06-24 23:33:50.044247 lnauth_django-0.2.0/lnauth_django/models.py
--rw-r--r--   0        0        0        0 2023-06-24 22:31:09.280965 lnauth_django-0.2.0/lnauth_django/tests/__init__.py
--rw-r--r--   0        0        0     1522 2023-06-24 23:33:21.865177 lnauth_django-0.2.0/lnauth_django/tests/test_service.py
--rw-r--r--   0        0        0      297 2023-06-24 22:33:44.897736 lnauth_django-0.2.0/lnauth_django/urls.py
--rw-r--r--   0        0        0     2293 2023-06-24 23:33:54.644101 lnauth_django-0.2.0/lnauth_django/views.py
--rw-r--r--   0        0        0      437 2023-06-26 23:26:47.988309 lnauth_django-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 lnauth_django-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-24 22:25:50.420220 lnauth_django-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1424 2023-06-24 23:03:45.863381 lnauth_django-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 22:25:50.380220 lnauth_django-0.2.1/lnauth_django/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-24 22:34:51.066120 lnauth_django-0.2.1/lnauth_django/apps.py
+-rw-r--r--   0        0        0      923 2023-06-26 23:43:59.700290 lnauth_django-0.2.1/lnauth_django/django_auth.py
+-rw-r--r--   0        0        0      141 2023-06-24 23:33:50.028248 lnauth_django-0.2.1/lnauth_django/exceptions.py
+-rw-r--r--   0        0        0     1382 2023-06-24 22:50:06.437211 lnauth_django-0.2.1/lnauth_django/lnauth.py
+-rw-r--r--   0        0        0      786 2023-06-26 23:23:58.916632 lnauth_django-0.2.1/lnauth_django/migrations/0000_initial.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:21:16.365884 lnauth_django-0.2.1/lnauth_django/migrations/__init__.py
+-rw-r--r--   0        0        0      266 2023-06-24 23:33:50.044247 lnauth_django-0.2.1/lnauth_django/models.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:31:09.280965 lnauth_django-0.2.1/lnauth_django/tests/__init__.py
+-rw-r--r--   0        0        0     1522 2023-06-24 23:33:21.865177 lnauth_django-0.2.1/lnauth_django/tests/test_service.py
+-rw-r--r--   0        0        0      297 2023-06-24 22:33:44.897736 lnauth_django-0.2.1/lnauth_django/urls.py
+-rw-r--r--   0        0        0     2316 2023-06-26 23:43:50.079648 lnauth_django-0.2.1/lnauth_django/views.py
+-rw-r--r--   0        0        0      437 2023-06-26 23:44:31.494358 lnauth_django-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 lnauth_django-0.2.1/PKG-INFO
```

### Comparing `lnauth_django-0.2.0/README.md` & `lnauth_django-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.2.0/lnauth_django/django.py` & `lnauth_django-0.2.1/lnauth_django/django_auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.conf import settings
 from django.contrib.auth import login
 from django.db import transaction
 
 from . import exceptions, models
 
 
-def django_register(request):
+def app_register(request):
     try:
         with transaction.atomic():
 
             user = settings.AUTH_USER_MODEL.objects.create_user(
                 username=request.GET["key"], password=request.GET["key"]
             )
             user.lnauthkey.linking_key = request.GET["key"]
@@ -17,15 +17,15 @@
             user.save()
     except models.LnAuthKey.IntegrityError:
         raise exceptions.DjangoAuthException("User already registered.")
 
     login(request, user)
 
 
-def django_login(request):
+def app_login(request):
     try:
         user = settings.AUTH_USER_MODEL.objects.get(
             lnauthkey__linking_key=request.GET["key"]
         )
     except settings.AUTH_USER_MODEL.DoesNotExist:
         raise exceptions.DjangoAuthException("User not registered.")
```

### Comparing `lnauth_django-0.2.0/lnauth_django/lnauth.py` & `lnauth_django-0.2.1/lnauth_django/lnauth.py`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.2.0/lnauth_django/migrations/0000_initial.py` & `lnauth_django-0.2.1/lnauth_django/migrations/0000_initial.py`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.2.0/lnauth_django/tests/test_service.py` & `lnauth_django-0.2.1/lnauth_django/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.2.0/lnauth_django/views.py` & `lnauth_django-0.2.1/lnauth_django/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from django.http import JsonResponse
 from django.views import generic
 
-from . import django, exceptions, lnauth
+from . import django_auth, exceptions, lnauth
 
 logger = logging.getLogger(__name__)
 
 
 class AuthURLProviderView(generic.View):
     def get(self, request):
         if request.GET and "action" in request.GET:
@@ -43,23 +43,23 @@
             return JsonResponse(
                 {"status": "ERROR", "reason": f"Invalid request. {e}"}, status=400
             )
 
         if request.GET["action"] == "login":
 
             try:
-                django.login(request)
+                django_auth.app_login(request)
             except exceptions.DjangoAuthException as e:
                 return JsonResponse(
                     {"status": "ERROR", "reason": f"Unauthorized. {e}"}, status=401
                 )
 
         elif request.GET["action"] == "register":
             try:
-                django.register(request)
+                django_auth.app_register(request)
             except exceptions.DjangoAuthException as e:
                 return JsonResponse(
                     {"status": "ERROR", "reason": f"Unauthorized. {e}"}, status=401
                 )
         else:
             return JsonResponse(
                 {"status": "ERROR", "reason": "Invalid request. Invalid action."},
```

### Comparing `lnauth_django-0.2.0/PKG-INFO` & `lnauth_django-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnauth-django
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: zwx00
 Author-email: blaz@bolt.observer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

