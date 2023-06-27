# Comparing `tmp/django_descope-1.1.0.tar.gz` & `tmp/django_descope-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_descope-1.1.0.tar", max compression
+gzip compressed data, was "django_descope-1.2.0.tar", max compression
```

## Comparing `django_descope-1.1.0.tar` & `django_descope-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-05-17 07:33:56.354577 django_descope-1.1.0/LICENSE
--rw-r--r--   0        0        0     1715 2023-05-17 07:33:56.354577 django_descope-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/__init__.py
--rw-r--r--   0        0        0       96 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/apps.py
--rw-r--r--   0        0        0     1910 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/authentication.py
--rw-r--r--   0        0        0      544 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/middleware.py
--rw-r--r--   0        0        0      666 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/migrations/__init__.py
--rw-r--r--   0        0        0     1367 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/models.py
--rw-r--r--   0        0        0      576 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/settings.py
--rw-r--r--   0        0        0        0 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/templatetags/__init__.py
--rw-r--r--   0        0        0     1619 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/templatetags/descope.py
--rw-r--r--   0        0        0      165 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/urls.py
--rw-r--r--   0        0        0     1045 2023-05-17 07:33:56.354577 django_descope-1.1.0/django_descope/views.py
--rw-r--r--   0        0        0     2512 2023-05-17 07:34:30.222324 django_descope-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 django_descope-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-27 11:03:29.218118 django_descope-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1855 2023-06-27 11:03:29.218118 django_descope-1.2.0/README.md
+-rw-r--r--   0        0        0      194 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/__init__.py
+-rw-r--r--   0        0        0       96 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/apps.py
+-rw-r--r--   0        0        0     1949 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/authentication.py
+-rw-r--r--   0        0        0      544 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/middleware.py
+-rw-r--r--   0        0        0      666 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/migrations/__init__.py
+-rw-r--r--   0        0        0     1293 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/models.py
+-rw-r--r--   0        0        0      643 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/settings.py
+-rw-r--r--   0        0        0      498 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/templates/admin/descope_login.html
+-rw-r--r--   0        0        0        0 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/templatetags/__init__.py
+-rw-r--r--   0        0        0     1619 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/templatetags/descope.py
+-rw-r--r--   0        0        0      165 2023-06-27 11:03:29.218118 django_descope-1.2.0/django_descope/urls.py
+-rw-r--r--   0        0        0      942 2023-06-27 11:03:29.222118 django_descope-1.2.0/django_descope/views.py
+-rw-r--r--   0        0        0     2535 2023-06-27 11:04:02.509620 django_descope-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3261 1970-01-01 00:00:00.000000 django_descope-1.2.0/PKG-INFO
```

### Comparing `django_descope-1.1.0/LICENSE` & `django_descope-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_descope-1.1.0/README.md` & `django_descope-1.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,20 +26,21 @@
 ```
    INSTALLED_APPS = [
    ...
    'django_descope',
    ]
 ```
 
-3. Add Descope Middleware **after** the SessionMiddleware
+3. Add Descope Middleware **after** the AuthenticationMiddleware and SessionMiddleware
 
 ```
    MIDDLEWARE = [
    ...
    'django.contrib.sessions.middleware.SessionMiddleware',
+   'django.contrib.auth.middleware.AuthenticationMiddleware',
    ...
    'django_descope.middleware.DescopeMiddleware',
    ]
 ```
 
 4. Include descope URLconf in your project urls.py like this:
 
@@ -63,12 +64,20 @@
 
 6. Start the development server and visit the newly created view
 
 ## Settings
 
 The following settings are available to configure in your project `settings.py`
 
+#### Required
+
+```
+DESCOPE_PROJECT_ID
+```
+
+#### Optional
+
 ```
-DESCOPE_PROJECT_ID **Required**
+DESCOPE_MANAGEMENT_KEY
 DESCOPE_IS_STAFF_ROLE
 DESCOPE_IS_SUPERUSER_ROLE
 ```
```

#### html2text {}

```diff
@@ -3,21 +3,22 @@
 for Descope and set admin roles - Get your project id - Create two roles in
 Descope, that will be mapped to Django permissions - is_staff - is_superuser
 Map these roles to any user you would like to make a staff or superuser in your
 Django app. _The names of these roles can be customized in the settings below._
 2. Install "django-descope" and add to your INSTALLED_APPS setting like this:
 ```bash poetry add django-descope OR pip install django-descope ``` ```
 INSTALLED_APPS = [ ... 'django_descope', ] ``` 3. Add Descope Middleware
-**after** the SessionMiddleware ``` MIDDLEWARE = [ ...
-'django.contrib.sessions.middleware.SessionMiddleware', ...
+**after** the AuthenticationMiddleware and SessionMiddleware ``` MIDDLEWARE =
+[ ... 'django.contrib.sessions.middleware.SessionMiddleware',
+'django.contrib.auth.middleware.AuthenticationMiddleware', ...
 'django_descope.middleware.DescopeMiddleware', ] ``` 4. Include descope URLconf
 in your project urls.py like this: ``` path('auth/', include
 ('django_descope.urls')), ``` 5. In your site templates, insert the
 `descope_flow` tag where you want to place your flow ```html {% load descope %}
 {% if user.is_authenticated %}
 ****** Welcome {{ user.email }} you are logged in! ******
 Log_Out
 {% else %} {% descope_flow "sign-up-or-in" "/" %}  {% endif %} ``` 6. Start the
 development server and visit the newly created view ## Settings The following
-settings are available to configure in your project `settings.py` ```
-DESCOPE_PROJECT_ID **Required** DESCOPE_IS_STAFF_ROLE DESCOPE_IS_SUPERUSER_ROLE
-```
+settings are available to configure in your project `settings.py` #### Required
+``` DESCOPE_PROJECT_ID ``` #### Optional ``` DESCOPE_MANAGEMENT_KEY
+DESCOPE_IS_STAFF_ROLE DESCOPE_IS_SUPERUSER_ROLE ```
```

### Comparing `django_descope-1.1.0/django_descope/middleware.py` & `django_descope-1.2.0/django_descope/middleware.py`

 * *Files identical despite different names*

### Comparing `django_descope-1.1.0/django_descope/migrations/0001_initial.py` & `django_descope-1.2.0/django_descope/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_descope-1.1.0/django_descope/models.py` & `django_descope-1.2.0/django_descope/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 import logging
 
-from descope import DescopeClient
+from descope import SESSION_TOKEN_NAME
 from django.contrib.auth import models as auth_models
 from django.core.cache import cache
-from django.utils.functional import cached_property
 
-from .settings import IS_STAFF_ROLE, IS_SUPERUSER_ROLE, PROJECT_ID
+from . import descope_client
+from .settings import IS_STAFF_ROLE, IS_SUPERUSER_ROLE
 
 logger = logging.getLogger(__name__)
 
 
 class DescopeUser(auth_models.User):
     class Meta:
         proxy = True
 
-    # User is always active since Descioe will never issue a token for an
+    # User is always active since Descope will never issue a token for an
     # inactive user
     is_active = True
-    _descope = DescopeClient(PROJECT_ID)
 
     def sync(self, session, refresh):
-        self.token = session
-        self.session = session.get("jwt")
-        self.refresh = refresh
-        self.user = session.get("user")
-        self.firstSeen = session.get("firstSeen")
+        self.session_token = session[SESSION_TOKEN_NAME]  # this should always exist
+        self.refresh_token = refresh
         self.username = self._me.get("userId")
+        self.user = self.username
         self.email = self._me.get("email")
-        self.is_staff = IS_STAFF_ROLE in self._roles
-        self.is_superuser = IS_SUPERUSER_ROLE in self._roles
+        self.is_staff = descope_client.validate_roles(
+            self.session_token, [IS_STAFF_ROLE]
+        )
+        self.is_superuser = descope_client.validate_roles(
+            self.session_token, [IS_SUPERUSER_ROLE]
+        )
         self.save()
 
     def __str__(self):
         return f"DescopeUser {self.username}"
 
-    @cached_property
+    @property
     def _me(self):
         return cache.get_or_set(
-            f"descope_me:{self.username}", lambda: self._descope.me(self.refresh)
+            f"descope_me:{self.username}", lambda: descope_client.me(self.refresh_token)
         )
 
-    @cached_property
-    def _roles(self):
-        return self.token.get("roles", [])
-
     def get_username(self):
         return self.username
```

### Comparing `django_descope-1.1.0/django_descope/templatetags/descope.py` & `django_descope-1.2.0/django_descope/templatetags/descope.py`

 * *Files identical despite different names*

### Comparing `django_descope-1.1.0/django_descope/views.py` & `django_descope-1.2.0/django_descope/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import logging
 
-from descope import REFRESH_SESSION_COOKIE_NAME, SESSION_COOKIE_NAME, DescopeClient
+from descope import REFRESH_SESSION_COOKIE_NAME, SESSION_COOKIE_NAME
 from django.http import HttpRequest, HttpResponseBadRequest, JsonResponse
 from django.utils.decorators import method_decorator
 from django.views import View
 from django.views.decorators.cache import never_cache
 
-from . import settings
-
 # User = get_user_model()
 logger = logging.getLogger(__name__)
 
-descope_client = DescopeClient(project_id=settings.PROJECT_ID)
-
 
 @method_decorator([never_cache], name="dispatch")
 class StoreJwt(View):
     def post(self, request: HttpRequest):
         session = request.POST.get(SESSION_COOKIE_NAME)
         refresh = request.COOKIES.get(REFRESH_SESSION_COOKIE_NAME)
         if not refresh:
```

### Comparing `django_descope-1.1.0/pyproject.toml` & `django_descope-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1,<2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django_descope"
-version = "v1.1.0"
+version = "v1.2.0"
 description = "Descope plugin for Django"
 readme = "README.md"
 authors = ["Descope <info@descope.com>"]
 repository = "https://github.com/descope/django-descope"
 documentation = "https://docs.descope.com"
 keywords = ["descope", "jwt", "authentication", "django"]
 license = "MIT"
@@ -37,25 +37,26 @@
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 Django = ">=3.2.19,<4.3"
-descope = "^1.0.0"
+descope = "^1.5.1"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "6.0.0"
 black = "23.3.0"
-pre-commit = "3.3.1"
-liccheck = "0.9.0"
+pre-commit = "3.3.2"
+liccheck = "0.9.1"
 isort = "5.12.0"
 python-dotenv = "1.0.0"
-tox = "4.4.8"
-django-debug-toolbar = "3.8.1"
+tox = "4.5.1"
+django-debug-toolbar = "4.1.0"
+django-stubs = "4.2.1"
 
 # Authorized and unauthorized licenses in LOWER CASE
 [tool.liccheck]
 authorized_licenses= [
         "bsd",
         "new bsd",
         "bsd license",
```

### Comparing `django_descope-1.1.0/PKG-INFO` & `django_descope-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-descope
-Version: 1.1.0
+Version: 1.2.0
 Summary: Descope plugin for Django
 Home-page: https://github.com/descope/django-descope
 License: MIT
 Keywords: descope,jwt,authentication,django
 Author: Descope
 Author-email: info@descope.com
 Requires-Python: >=3.8.1,<4.0
@@ -17,24 +17,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: Django (>=3.2.19,<4.3)
-Requires-Dist: descope (>=1.0.0,<2.0.0)
+Requires-Dist: descope (>=1.5.1,<2.0.0)
 Project-URL: Documentation, https://docs.descope.com
 Project-URL: Repository, https://github.com/descope/django-descope
 Description-Content-Type: text/markdown
 
 # Descope Django App
 
 Descope is a user management and authentication platform.
@@ -63,20 +61,21 @@
 ```
    INSTALLED_APPS = [
    ...
    'django_descope',
    ]
 ```
 
-3. Add Descope Middleware **after** the SessionMiddleware
+3. Add Descope Middleware **after** the AuthenticationMiddleware and SessionMiddleware
 
 ```
    MIDDLEWARE = [
    ...
    'django.contrib.sessions.middleware.SessionMiddleware',
+   'django.contrib.auth.middleware.AuthenticationMiddleware',
    ...
    'django_descope.middleware.DescopeMiddleware',
    ]
 ```
 
 4. Include descope URLconf in your project urls.py like this:
 
@@ -100,13 +99,21 @@
 
 6. Start the development server and visit the newly created view
 
 ## Settings
 
 The following settings are available to configure in your project `settings.py`
 
+#### Required
+
+```
+DESCOPE_PROJECT_ID
+```
+
+#### Optional
+
 ```
-DESCOPE_PROJECT_ID **Required**
+DESCOPE_MANAGEMENT_KEY
 DESCOPE_IS_STAFF_ROLE
 DESCOPE_IS_SUPERUSER_ROLE
 ```
```

#### html2text {}

```diff
@@ -1,42 +1,43 @@
-Metadata-Version: 2.1 Name: django-descope Version: 1.1.0 Summary: Descope
+Metadata-Version: 2.1 Name: django-descope Version: 1.2.0 Summary: Descope
 plugin for Django Home-page: https://github.com/descope/django-descope License:
 MIT Keywords: descope,jwt,authentication,django Author: Descope Author-email:
 info@descope.com Requires-Python: >=3.8.1,<4.0 Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework :: Django ::
 4.1 Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
-Internet :: WWW/HTTP :: Dynamic Content Requires-Dist: Django (>=3.2.19,<4.3)
-Requires-Dist: descope (>=1.0.0,<2.0.0) Project-URL: Documentation, https://
-docs.descope.com Project-URL: Repository, https://github.com/descope/django-
-descope Description-Content-Type: text/markdown # Descope Django App Descope is
-a user management and authentication platform. This plugin integrates Descope
-with your Django app. ## Quick start 1. Sign up for Descope and set admin roles
-- Get your project id - Create two roles in Descope, that will be mapped to
-Django permissions - is_staff - is_superuser Map these roles to any user you
-would like to make a staff or superuser in your Django app. _The names of these
-roles can be customized in the settings below._ 2. Install "django-descope" and
-add to your INSTALLED_APPS setting like this: ```bash poetry add django-descope
-OR pip install django-descope ``` ``` INSTALLED_APPS = [ ... 'django_descope',
-] ``` 3. Add Descope Middleware **after** the SessionMiddleware ``` MIDDLEWARE
-= [ ... 'django.contrib.sessions.middleware.SessionMiddleware', ...
+Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
+HTTP :: Dynamic Content Requires-Dist: Django (>=3.2.19,<4.3) Requires-Dist:
+descope (>=1.5.1,<2.0.0) Project-URL: Documentation, https://docs.descope.com
+Project-URL: Repository, https://github.com/descope/django-descope Description-
+Content-Type: text/markdown # Descope Django App Descope is a user management
+and authentication platform. This plugin integrates Descope with your Django
+app. ## Quick start 1. Sign up for Descope and set admin roles - Get your
+project id - Create two roles in Descope, that will be mapped to Django
+permissions - is_staff - is_superuser Map these roles to any user you would
+like to make a staff or superuser in your Django app. _The names of these roles
+can be customized in the settings below._ 2. Install "django-descope" and add
+to your INSTALLED_APPS setting like this: ```bash poetry add django-descope OR
+pip install django-descope ``` ``` INSTALLED_APPS = [ ... 'django_descope', ]
+``` 3. Add Descope Middleware **after** the AuthenticationMiddleware and
+SessionMiddleware ``` MIDDLEWARE = [ ...
+'django.contrib.sessions.middleware.SessionMiddleware',
+'django.contrib.auth.middleware.AuthenticationMiddleware', ...
 'django_descope.middleware.DescopeMiddleware', ] ``` 4. Include descope URLconf
 in your project urls.py like this: ``` path('auth/', include
 ('django_descope.urls')), ``` 5. In your site templates, insert the
 `descope_flow` tag where you want to place your flow ```html {% load descope %}
 {% if user.is_authenticated %}
 ****** Welcome {{ user.email }} you are logged in! ******
 Log_Out
 {% else %} {% descope_flow "sign-up-or-in" "/" %}  {% endif %} ``` 6. Start the
 development server and visit the newly created view ## Settings The following
-settings are available to configure in your project `settings.py` ```
-DESCOPE_PROJECT_ID **Required** DESCOPE_IS_STAFF_ROLE DESCOPE_IS_SUPERUSER_ROLE
-```
+settings are available to configure in your project `settings.py` #### Required
+``` DESCOPE_PROJECT_ID ``` #### Optional ``` DESCOPE_MANAGEMENT_KEY
+DESCOPE_IS_STAFF_ROLE DESCOPE_IS_SUPERUSER_ROLE ```
```

