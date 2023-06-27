# Comparing `tmp/pretix-payone-1.3.1.tar.gz` & `tmp/pretix-payone-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-payone-1.3.1.tar", last modified: Sun May 28 23:20:01 2023, max compression
+gzip compressed data, was "pretix-payone-1.3.2.tar", last modified: Tue Jun 27 13:01:31 2023, max compression
```

## Comparing `pretix-payone-1.3.1.tar` & `pretix-payone-1.3.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2462 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1390 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.233943 pretix-payone-1.3.1/pretix_payone/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.229943 pretix-payone-1.3.1/pretix_payone/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10537 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10484 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     8146 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1197 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/migrations/0002_auto_20220204_1638.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/models.py
--rw-rw-rw-   0 root         (0) root         (0)    33634 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     2484 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.229943 pretix-payone-1.3.1/pretix_payone/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/pretix_payone/static/pretix_payone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/static/pretix_payone/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     6372 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/static/pretix_payone/cc.js
--rw-rw-rw-   0 root         (0) root         (0)     3517 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/static/pretix_payone/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.229943 pretix-payone-1.3.1/pretix_payone/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/control.html
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/pending.html
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/redirect.html
--rw-rw-rw-   0 root         (0) root         (0)      601 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     8795 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-05-28 23:20:01.000000 pretix-payone-1.3.1/pretix_payone.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-28 23:20:01.000000 pretix-payone-1.3.1/pretix_payone.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:20:01.000000 pretix-payone-1.3.1/pretix_payone.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-28 23:20:01.000000 pretix-payone-1.3.1/pretix_payone.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-28 23:20:01.000000 pretix-payone-1.3.1/pretix_payone.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.123327 pretix-payone-1.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-27 13:01:31.123327 pretix-payone-1.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1390 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.111327 pretix-payone-1.3.2/pretix_payone/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10537 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10484 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     8146 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/migrations/0002_auto_20220204_1638.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    33634 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2484 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.115327 pretix-payone-1.3.2/pretix_payone/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/static/pretix_payone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/static/pretix_payone/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     6372 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/static/pretix_payone/cc.js
+-rw-rw-rw-   0 root         (0) root         (0)     3517 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/static/pretix_payone/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.115327 pretix-payone-1.3.2/pretix_payone/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.123327 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/control.html
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)      601 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     8795 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-27 13:01:31.000000 pretix-payone-1.3.2/pretix_payone.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-06-27 13:01:31.000000 pretix-payone-1.3.2/pretix_payone.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 13:01:31.000000 pretix-payone-1.3.2/pretix_payone.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-27 13:01:31.000000 pretix-payone-1.3.2/pretix_payone.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-27 13:01:31.000000 pretix-payone-1.3.2/pretix_payone.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-27 13:01:31.123327 pretix-payone-1.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.123327 pretix-payone-1.3.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/tests/test_main.py
```

### Comparing `pretix-payone-1.3.1/LICENSE` & `pretix-payone-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/PKG-INFO` & `pretix-payone-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-payone
-Version: 1.3.1
+Version: 1.3.2
 Summary: Allows to process payments through PAYONE (formerly BS Payone)
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: 
         Copyright 2021 pretix team
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `pretix-payone-1.3.1/README.rst` & `pretix-payone-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/apps.py` & `pretix-payone-1.3.2/pretix_payone/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/locale/de/LC_MESSAGES/django.po` & `pretix-payone-1.3.2/pretix_payone/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-payone-1.3.2/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/locale/django.pot` & `pretix-payone-1.3.2/pretix_payone/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/migrations/0001_initial.py` & `pretix-payone-1.3.2/pretix_payone/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/migrations/0002_auto_20220204_1638.py` & `pretix-payone-1.3.2/pretix_payone/migrations/0002_auto_20220204_1638.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/payment.py` & `pretix-payone-1.3.2/pretix_payone/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/signals.py` & `pretix-payone-1.3.2/pretix_payone/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/static/pretix_payone/cc.js` & `pretix-payone-1.3.2/pretix_payone/static/pretix_payone/cc.js`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/static/pretix_payone/logo.svg` & `pretix-payone-1.3.2/pretix_payone/static/pretix_payone/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html` & `pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/control.html` & `pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/control.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/pending.html` & `pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/redirect.html` & `pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/urls.py` & `pretix-payone-1.3.2/pretix_payone/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone/views.py` & `pretix-payone-1.3.2/pretix_payone/views.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pretix_payone.egg-info/PKG-INFO` & `pretix-payone-1.3.2/pretix_payone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-payone
-Version: 1.3.1
+Version: 1.3.2
 Summary: Allows to process payments through PAYONE (formerly BS Payone)
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: 
         Copyright 2021 pretix team
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `pretix-payone-1.3.1/pretix_payone.egg-info/SOURCES.txt` & `pretix-payone-1.3.2/pretix_payone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/pyproject.toml` & `pretix-payone-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.1/setup.cfg` & `pretix-payone-1.3.2/setup.cfg`

 * *Files identical despite different names*

