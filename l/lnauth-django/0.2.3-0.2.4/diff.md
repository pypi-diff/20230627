# Comparing `tmp/lnauth_django-0.2.3.tar.gz` & `tmp/lnauth_django-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnauth_django-0.2.3.tar", max compression
+gzip compressed data, was "lnauth_django-0.2.4.tar", max compression
```

## Comparing `lnauth_django-0.2.3.tar` & `lnauth_django-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-06-24 22:25:50.420220 lnauth_django-0.2.3/LICENSE
--rw-r--r--   0        0        0     1424 2023-06-24 23:03:45.863381 lnauth_django-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-06-24 22:25:50.380220 lnauth_django-0.2.3/lnauth_django/__init__.py
--rw-r--r--   0        0        0      148 2023-06-24 22:34:51.066120 lnauth_django-0.2.3/lnauth_django/apps.py
--rw-r--r--   0        0        0      840 2023-06-27 00:12:04.407930 lnauth_django-0.2.3/lnauth_django/django_auth.py
--rw-r--r--   0        0        0      141 2023-06-24 23:33:50.028248 lnauth_django-0.2.3/lnauth_django/exceptions.py
--rw-r--r--   0        0        0     1382 2023-06-24 22:50:06.437211 lnauth_django-0.2.3/lnauth_django/lnauth.py
--rw-r--r--   0        0        0      786 2023-06-26 23:23:58.916632 lnauth_django-0.2.3/lnauth_django/migrations/0000_initial.py
--rw-r--r--   0        0        0        0 2023-06-26 23:21:16.365884 lnauth_django-0.2.3/lnauth_django/migrations/__init__.py
--rw-r--r--   0        0        0      266 2023-06-24 23:33:50.044247 lnauth_django-0.2.3/lnauth_django/models.py
--rw-r--r--   0        0        0        0 2023-06-24 22:31:09.280965 lnauth_django-0.2.3/lnauth_django/tests/__init__.py
--rw-r--r--   0        0        0     1522 2023-06-24 23:33:21.865177 lnauth_django-0.2.3/lnauth_django/tests/test_service.py
--rw-r--r--   0        0        0      297 2023-06-24 22:33:44.897736 lnauth_django-0.2.3/lnauth_django/urls.py
--rw-r--r--   0        0        0     2316 2023-06-26 23:43:50.079648 lnauth_django-0.2.3/lnauth_django/views.py
--rw-r--r--   0        0        0      437 2023-06-27 00:11:39.759332 lnauth_django-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 lnauth_django-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-24 22:25:50.420220 lnauth_django-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1424 2023-06-24 23:03:45.863381 lnauth_django-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 22:25:50.380220 lnauth_django-0.2.4/lnauth_django/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-24 22:34:51.066120 lnauth_django-0.2.4/lnauth_django/apps.py
+-rw-r--r--   0        0        0      912 2023-06-27 00:25:35.417368 lnauth_django-0.2.4/lnauth_django/django_auth.py
+-rw-r--r--   0        0        0      141 2023-06-24 23:33:50.028248 lnauth_django-0.2.4/lnauth_django/exceptions.py
+-rw-r--r--   0        0        0     1382 2023-06-24 22:50:06.437211 lnauth_django-0.2.4/lnauth_django/lnauth.py
+-rw-r--r--   0        0        0      786 2023-06-26 23:23:58.916632 lnauth_django-0.2.4/lnauth_django/migrations/0000_initial.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:21:16.365884 lnauth_django-0.2.4/lnauth_django/migrations/__init__.py
+-rw-r--r--   0        0        0      266 2023-06-24 23:33:50.044247 lnauth_django-0.2.4/lnauth_django/models.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:31:09.280965 lnauth_django-0.2.4/lnauth_django/tests/__init__.py
+-rw-r--r--   0        0        0     1522 2023-06-24 23:33:21.865177 lnauth_django-0.2.4/lnauth_django/tests/test_service.py
+-rw-r--r--   0        0        0      297 2023-06-24 22:33:44.897736 lnauth_django-0.2.4/lnauth_django/urls.py
+-rw-r--r--   0        0        0     2316 2023-06-26 23:43:50.079648 lnauth_django-0.2.4/lnauth_django/views.py
+-rw-r--r--   0        0        0      437 2023-06-27 00:25:14.490423 lnauth_django-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 lnauth_django-0.2.4/PKG-INFO
```

### Comparing `lnauth_django-0.2.3/README.md` & `lnauth_django-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.2.3/lnauth_django/django_auth.py` & `lnauth_django-0.2.4/lnauth_django/django_auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from django.contrib.auth import get_user_model, login
 from django.db import IntegrityError, transaction
 
-from . import exceptions
+from . import exceptions, models
 
 User = get_user_model()
 
 
 def app_register(request):
     try:
         with transaction.atomic():
 
             user = User.objects.create_user(
                 username=request.GET["key"], password=request.GET["key"]
             )
-            user.lnauthkey.linking_key = request.GET["key"]
-            user.lnauthkey.save()
+            lnauthkey = models.LnAuthKey.objects.create(
+                user=user, linking_key=request.GET["key"]
+            )
+            lnauthkey.save()
             user.save()
     except IntegrityError:
         raise exceptions.DjangoAuthException("User already registered.")
 
     login(request, user)
```

### Comparing `lnauth_django-0.2.3/lnauth_django/lnauth.py` & `lnauth_django-0.2.4/lnauth_django/lnauth.py`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.2.3/lnauth_django/migrations/0000_initial.py` & `lnauth_django-0.2.4/lnauth_django/migrations/0000_initial.py`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.2.3/lnauth_django/tests/test_service.py` & `lnauth_django-0.2.4/lnauth_django/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.2.3/lnauth_django/views.py` & `lnauth_django-0.2.4/lnauth_django/views.py`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.2.3/PKG-INFO` & `lnauth_django-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnauth-django
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: zwx00
 Author-email: blaz@bolt.observer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

