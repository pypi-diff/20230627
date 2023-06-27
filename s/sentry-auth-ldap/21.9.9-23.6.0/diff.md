# Comparing `tmp/sentry-auth-ldap-21.9.9.tar.gz` & `tmp/sentry-auth-ldap-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-auth-ldap-21.9.9.tar", last modified: Thu Mar 16 10:48:40 2023, max compression
+gzip compressed data, was "sentry-auth-ldap-23.6.0.tar", last modified: Tue Jun 27 11:44:09 2023, max compression
```

## Comparing `sentry-auth-ldap-21.9.9.tar` & `sentry-auth-ldap-23.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:48:40.478174 sentry-auth-ldap-21.9.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-16 10:48:27.000000 sentry-auth-ldap-21.9.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-16 10:48:40.478174 sentry-auth-ldap-21.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-03-16 10:48:27.000000 sentry-auth-ldap-21.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:48:40.474174 sentry-auth-ldap-21.9.9/sentry_auth_ldap/
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-03-16 10:48:27.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:48:40.478174 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-16 10:48:40.000000 sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-16 10:48:40.478174 sentry-auth-ldap-21.9.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-03-16 10:48:27.000000 sentry-auth-ldap-21.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:44:09.320958 sentry-auth-ldap-23.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-27 11:43:57.000000 sentry-auth-ldap-23.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-27 11:44:09.320958 sentry-auth-ldap-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-27 11:43:57.000000 sentry-auth-ldap-23.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:44:09.320958 sentry-auth-ldap-23.6.0/sentry_auth_ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-27 11:43:57.000000 sentry-auth-ldap-23.6.0/sentry_auth_ldap/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:44:09.320958 sentry-auth-ldap-23.6.0/sentry_auth_ldap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-27 11:44:09.000000 sentry-auth-ldap-23.6.0/sentry_auth_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-27 11:44:09.000000 sentry-auth-ldap-23.6.0/sentry_auth_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:44:09.000000 sentry-auth-ldap-23.6.0/sentry_auth_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:44:09.000000 sentry-auth-ldap-23.6.0/sentry_auth_ldap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 11:44:09.000000 sentry-auth-ldap-23.6.0/sentry_auth_ldap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 11:44:09.000000 sentry-auth-ldap-23.6.0/sentry_auth_ldap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-27 11:44:09.320958 sentry-auth-ldap-23.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-06-27 11:43:57.000000 sentry-auth-ldap-23.6.0/setup.py
```

### Comparing `sentry-auth-ldap-21.9.9/LICENSE.txt` & `sentry-auth-ldap-23.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sentry-auth-ldap-21.9.9/PKG-INFO` & `sentry-auth-ldap-23.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-auth-ldap
-Version: 21.9.9
+Version: 23.6.0
 Summary: A Sentry extension to add an LDAP server as an authentication source.
 Home-page: https://github.com/PMExtra/sentry-auth-ldap
 Download-URL: https://github.com/PMExtra/sentry-auth-ldap
 Author: Chad Killingsworth <chad.killingsworth@banno.com>, Barron Hagerman <barron.hagerman@banno.com>, PM Extra <pm@jubeat.net>
 Author-email: pm@jubeat.net
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/PMExtra/sentry-auth-ldap/issues
@@ -28,15 +28,17 @@
 A Django custom authentication backend for [Sentry](https://github.com/getsentry/sentry). This module extends the functionality of [django-auth-ldap](https://github.com/django-auth-ldap/django-auth-ldap) with Sentry specific features.
 
 ## Features
 * Users created by this backend are managed users. Managed fields are not editable through the Sentry account page.
 * Users may be auto-added to an Organization upon creation.
 
 ## Prerequisites
-Plugin 21.9.x support Sentry 21.9.0 or higher. For legacy Sentry support, you can use another project [sentry-ldap-auth](https://github.com/Banno/getsentry-ldap-auth)
+* Sentry < 21.9.0 should work with [sentry-ldap-auth==2.9.0](https://github.com/Banno/getsentry-ldap-auth) (which is another project for legacy support)
+* Sentry >= 21.9.0 and Sentry < 23.6.0 should work with sentry-auth-ldap==21.9.11
+* Sentry >= 23.6.0 should work with sentry-auth-ldap==23.6.0
 
 ## Installation
 To install, simply add `sentry-auth-ldap` to your *requirements.txt* for your Sentry environment (or `pip install sentry-auth-ldap`).
 
 For container environment, because of the minimal base image, it may miss some dependencies.
 
 You can easily enhance the image by `sentry/enhance-image.sh` script (need [getsentry/self-hosted](https://github.com/getsentry/self-hosted) 22.6.0 or higher):
@@ -164,15 +166,15 @@
 AUTH_LDAP_SENTRY_ORGANIZATION_GLOBAL_ACCESS = True
 
 AUTHENTICATION_BACKENDS = AUTHENTICATION_BACKENDS + (
     'sentry_auth_ldap.backend.SentryLdapBackend',
 )
 
 # Optional logging for diagnostics.
-# Make sure LOGGING.disable_existing_loggers is set to False (in sentry/conf/server.py)
+LOGGING['disable_existing_loggers'] = False
 import logging
 logger = logging.getLogger('django_auth_ldap')
 logger.setLevel(logging.DEBUG)
 ```
 
 ### Troubleshooting
```

### Comparing `sentry-auth-ldap-21.9.9/README.md` & `sentry-auth-ldap-23.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 A Django custom authentication backend for [Sentry](https://github.com/getsentry/sentry). This module extends the functionality of [django-auth-ldap](https://github.com/django-auth-ldap/django-auth-ldap) with Sentry specific features.
 
 ## Features
 * Users created by this backend are managed users. Managed fields are not editable through the Sentry account page.
 * Users may be auto-added to an Organization upon creation.
 
 ## Prerequisites
-Plugin 21.9.x support Sentry 21.9.0 or higher. For legacy Sentry support, you can use another project [sentry-ldap-auth](https://github.com/Banno/getsentry-ldap-auth)
+* Sentry < 21.9.0 should work with [sentry-ldap-auth==2.9.0](https://github.com/Banno/getsentry-ldap-auth) (which is another project for legacy support)
+* Sentry >= 21.9.0 and Sentry < 23.6.0 should work with sentry-auth-ldap==21.9.11
+* Sentry >= 23.6.0 should work with sentry-auth-ldap==23.6.0
 
 ## Installation
 To install, simply add `sentry-auth-ldap` to your *requirements.txt* for your Sentry environment (or `pip install sentry-auth-ldap`).
 
 For container environment, because of the minimal base image, it may miss some dependencies.
 
 You can easily enhance the image by `sentry/enhance-image.sh` script (need [getsentry/self-hosted](https://github.com/getsentry/self-hosted) 22.6.0 or higher):
@@ -143,15 +145,15 @@
 AUTH_LDAP_SENTRY_ORGANIZATION_GLOBAL_ACCESS = True
 
 AUTHENTICATION_BACKENDS = AUTHENTICATION_BACKENDS + (
     'sentry_auth_ldap.backend.SentryLdapBackend',
 )
 
 # Optional logging for diagnostics.
-# Make sure LOGGING.disable_existing_loggers is set to False (in sentry/conf/server.py)
+LOGGING['disable_existing_loggers'] = False
 import logging
 logger = logging.getLogger('django_auth_ldap')
 logger.setLevel(logging.DEBUG)
 ```
 
 ### Troubleshooting
```

### Comparing `sentry-auth-ldap-21.9.9/sentry_auth_ldap/backend.py` & `sentry-auth-ldap-23.6.0/sentry_auth_ldap/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,17 +57,14 @@
             defaults = { 'is_verified': True }
         else:
             defaults = None
 
         for mail in mail_attr or [email]:
             UserEmail.objects.update_or_create(defaults = defaults, user=user, email=mail)
 
-        if not built:
-            return (user, built)
-
         # Check to see if we need to add the user to an organization
         organization_slug = getattr(settings, 'AUTH_LDAP_SENTRY_DEFAULT_ORGANIZATION', None)
         # For backward compatibility
         organization_name = getattr(settings, 'AUTH_LDAP_DEFAULT_SENTRY_ORGANIZATION', None)
 
         # Find the default organization
         if organization_slug:
@@ -81,20 +78,22 @@
             return (user, built)
 
         member_role = _get_effective_sentry_role(ldap_user) or getattr(settings, 'AUTH_LDAP_SENTRY_ORGANIZATION_ROLE_TYPE', None)
 
         has_global_access = getattr(settings, 'AUTH_LDAP_SENTRY_ORGANIZATION_GLOBAL_ACCESS', False)
 
         # Add the user to the organization with global access
-        OrganizationMember.objects.create(
+        OrganizationMember.objects.update_or_create(
             organization=organizations[0],
-            user=user,
-            role=member_role,
-            has_global_access=has_global_access,
-            flags=getattr(OrganizationMember.flags, 'sso:linked'),
+            user_id=user.id,
+            defaults={
+                'role': member_role,
+                'has_global_access': has_global_access,
+                'flags': getattr(OrganizationMember.flags, 'sso:linked')
+            }
         )
 
         if not getattr(settings, 'AUTH_LDAP_SENTRY_SUBSCRIBE_BY_DEFAULT', True):
             UserOption.objects.set_value(
                 user=user,
                 project=None,
                 key='subscribe_by_default',
```

### Comparing `sentry-auth-ldap-21.9.9/sentry_auth_ldap.egg-info/PKG-INFO` & `sentry-auth-ldap-23.6.0/sentry_auth_ldap.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-auth-ldap
-Version: 21.9.9
+Version: 23.6.0
 Summary: A Sentry extension to add an LDAP server as an authentication source.
 Home-page: https://github.com/PMExtra/sentry-auth-ldap
 Download-URL: https://github.com/PMExtra/sentry-auth-ldap
 Author: Chad Killingsworth <chad.killingsworth@banno.com>, Barron Hagerman <barron.hagerman@banno.com>, PM Extra <pm@jubeat.net>
 Author-email: pm@jubeat.net
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/PMExtra/sentry-auth-ldap/issues
@@ -28,15 +28,17 @@
 A Django custom authentication backend for [Sentry](https://github.com/getsentry/sentry). This module extends the functionality of [django-auth-ldap](https://github.com/django-auth-ldap/django-auth-ldap) with Sentry specific features.
 
 ## Features
 * Users created by this backend are managed users. Managed fields are not editable through the Sentry account page.
 * Users may be auto-added to an Organization upon creation.
 
 ## Prerequisites
-Plugin 21.9.x support Sentry 21.9.0 or higher. For legacy Sentry support, you can use another project [sentry-ldap-auth](https://github.com/Banno/getsentry-ldap-auth)
+* Sentry < 21.9.0 should work with [sentry-ldap-auth==2.9.0](https://github.com/Banno/getsentry-ldap-auth) (which is another project for legacy support)
+* Sentry >= 21.9.0 and Sentry < 23.6.0 should work with sentry-auth-ldap==21.9.11
+* Sentry >= 23.6.0 should work with sentry-auth-ldap==23.6.0
 
 ## Installation
 To install, simply add `sentry-auth-ldap` to your *requirements.txt* for your Sentry environment (or `pip install sentry-auth-ldap`).
 
 For container environment, because of the minimal base image, it may miss some dependencies.
 
 You can easily enhance the image by `sentry/enhance-image.sh` script (need [getsentry/self-hosted](https://github.com/getsentry/self-hosted) 22.6.0 or higher):
@@ -164,15 +166,15 @@
 AUTH_LDAP_SENTRY_ORGANIZATION_GLOBAL_ACCESS = True
 
 AUTHENTICATION_BACKENDS = AUTHENTICATION_BACKENDS + (
     'sentry_auth_ldap.backend.SentryLdapBackend',
 )
 
 # Optional logging for diagnostics.
-# Make sure LOGGING.disable_existing_loggers is set to False (in sentry/conf/server.py)
+LOGGING['disable_existing_loggers'] = False
 import logging
 logger = logging.getLogger('django_auth_ldap')
 logger.setLevel(logging.DEBUG)
 ```
 
 ### Troubleshooting
```

### Comparing `sentry-auth-ldap-21.9.9/setup.py` & `sentry-auth-ldap-23.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 install_requires = [
     'django-auth-ldap==4.1.0',
-    'sentry>=21.9.0',
+    'sentry>=23.6.0',
 ]
 
 setup(
     name='sentry-auth-ldap',
-    version='21.9.9',
+    version='23.6.0',
     author='Chad Killingsworth <chad.killingsworth@banno.com>, Barron Hagerman <barron.hagerman@banno.com>, PM Extra <pm@jubeat.net>',
     author_email='pm@jubeat.net',
     url='https://github.com/PMExtra/sentry-auth-ldap',
     description='A Sentry extension to add an LDAP server as an authentication source.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(),
```

