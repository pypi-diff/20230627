# Comparing `tmp/huscy.consents-0.8.0a21.tar.gz` & `tmp/huscy.consents-0.8.0a22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.consents-0.8.0a21.tar", last modified: Fri May 26 17:29:45 2023, max compression
+gzip compressed data, was "huscy.consents-0.8.0a22.tar", last modified: Tue Jun 27 15:38:26 2023, max compression
```

## Comparing `huscy.consents-0.8.0a21.tar` & `huscy.consents-0.8.0a22.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.353955 huscy.consents-0.8.0a21/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       59 2022-11-22 11:01:15.000000 huscy.consents-0.8.0a21/MANIFEST.in
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-26 17:29:45.353955 huscy.consents-0.8.0a21/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       17 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a21/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/consents/
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)       82 2023-05-26 11:36:57.000000 huscy.consents-0.8.0a21/huscy/consents/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      597 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a21/huscy/consents/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      319 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a21/huscy/consents/api_urls.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)      186 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a21/huscy/consents/apps.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1557 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a21/huscy/consents/forms.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/consents/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1800 2023-05-26 17:29:44.000000 huscy.consents-0.8.0a21/huscy/consents/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a21/huscy/consents/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1085 2023-05-26 11:36:57.000000 huscy.consents-0.8.0a21/huscy/consents/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      938 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a21/huscy/consents/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     6948 2023-05-26 11:36:57.000000 huscy.consents-0.8.0a21/huscy/consents/services.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/consents/static/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/consents/static/consents/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.341955 huscy.consents-0.8.0a21/huscy/consents/static/consents/css/
--rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/css/fomantic.min.css
--rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/css/fomantic2.9.0.min.css
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.341955 huscy.consents-0.8.0a21/huscy/consents/static/consents/img/
--rw-r--r--   0 jenkins    (111) jenkins    (115)    33728 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/img/logo.svg
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.345955 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/
--rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/fomantic.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/fomantic2.9.0.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/jquery.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/jquery3.6.1.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/popper.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/popper1.16.1.min.js
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/consents/templates/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.349955 huscy.consents-0.8.0a21/huscy/consents/templates/consents/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      599 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/base.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)     6660 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/create_consent.html
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4342 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/sign_consent.html
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     3129 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/signed_consent.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)        8 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/success.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.349955 huscy.consents-0.8.0a21/huscy/consents/templates/consents/text_fragments/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      275 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/text_fragments/checkbox.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)      113 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/text_fragments/heading.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)       72 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/text_fragments/markdown.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)      176 2023-01-10 14:57:17.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/text_fragments/paragraph.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.349955 huscy.consents-0.8.0a21/huscy/consents/templates/consents/widgets/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      165 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/widgets/select_date.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.353955 huscy.consents-0.8.0a21/huscy/consents/templatetags/
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a21/huscy/consents/templatetags/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      155 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a21/huscy/consents/templatetags/dict_extras.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)      436 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a21/huscy/consents/urls.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4544 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a21/huscy/consents/views.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      580 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a21/huscy/consents/viewsets.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy.consents.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-26 17:29:45.000000 huscy.consents-0.8.0a21/huscy.consents.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1685 2023-05-26 17:29:45.000000 huscy.consents-0.8.0a21/huscy.consents.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-05-26 17:29:45.000000 huscy.consents-0.8.0a21/huscy.consents.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      208 2023-05-26 17:29:45.000000 huscy.consents-0.8.0a21/huscy.consents.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-05-26 17:29:45.000000 huscy.consents-0.8.0a21/huscy.consents.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-05-26 17:29:45.353955 huscy.consents-0.8.0a21/setup.cfg
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1766 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a21/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.470975 huscy.consents-0.8.0a22/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       59 2022-11-22 11:01:15.000000 huscy.consents-0.8.0a22/MANIFEST.in
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-06-27 15:38:26.470975 huscy.consents-0.8.0a22/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       17 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a22/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.442975 huscy.consents-0.8.0a22/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.442975 huscy.consents-0.8.0a22/huscy/consents/
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)       82 2023-06-27 09:30:08.000000 huscy.consents-0.8.0a22/huscy/consents/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      597 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a22/huscy/consents/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      319 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a22/huscy/consents/api_urls.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)      186 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a22/huscy/consents/apps.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1557 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a22/huscy/consents/forms.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.442975 huscy.consents-0.8.0a22/huscy/consents/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1800 2023-06-27 15:38:25.000000 huscy.consents-0.8.0a22/huscy/consents/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a22/huscy/consents/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1085 2023-05-26 11:36:57.000000 huscy.consents-0.8.0a22/huscy/consents/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      938 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a22/huscy/consents/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6948 2023-05-26 11:36:57.000000 huscy.consents-0.8.0a22/huscy/consents/services.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.442975 huscy.consents-0.8.0a22/huscy/consents/static/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.442975 huscy.consents-0.8.0a22/huscy/consents/static/consents/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.446975 huscy.consents-0.8.0a22/huscy/consents/static/consents/css/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/static/consents/css/fomantic.min.css
+-rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/static/consents/css/fomantic2.9.0.min.css
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.446975 huscy.consents-0.8.0a22/huscy/consents/static/consents/img/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    33728 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/static/consents/img/logo.svg
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.454975 huscy.consents-0.8.0a22/huscy/consents/static/consents/js/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/static/consents/js/fomantic.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/static/consents/js/fomantic2.9.0.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/static/consents/js/jquery.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/static/consents/js/jquery3.6.1.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/static/consents/js/popper.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/static/consents/js/popper1.16.1.min.js
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.442975 huscy.consents-0.8.0a22/huscy/consents/templates/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.462975 huscy.consents-0.8.0a22/huscy/consents/templates/consents/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      599 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/base.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6660 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/create_consent.html
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4342 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/sign_consent.html
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     3129 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/signed_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        8 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/success.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.466975 huscy.consents-0.8.0a22/huscy/consents/templates/consents/text_fragments/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      275 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/text_fragments/checkbox.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      113 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/text_fragments/heading.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       72 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/text_fragments/markdown.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       61 2023-06-27 09:30:08.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/text_fragments/page-break.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      176 2023-01-10 14:57:17.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/text_fragments/paragraph.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.470975 huscy.consents-0.8.0a22/huscy/consents/templates/consents/widgets/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      165 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a22/huscy/consents/templates/consents/widgets/select_date.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.470975 huscy.consents-0.8.0a22/huscy/consents/templatetags/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a22/huscy/consents/templatetags/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      155 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a22/huscy/consents/templatetags/dict_extras.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)      436 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a22/huscy/consents/urls.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4544 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a22/huscy/consents/views.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      580 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a22/huscy/consents/viewsets.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-06-27 15:38:26.442975 huscy.consents-0.8.0a22/huscy.consents.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-06-27 15:38:26.000000 huscy.consents-0.8.0a22/huscy.consents.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1750 2023-06-27 15:38:26.000000 huscy.consents-0.8.0a22/huscy.consents.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-06-27 15:38:26.000000 huscy.consents-0.8.0a22/huscy.consents.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      208 2023-06-27 15:38:26.000000 huscy.consents-0.8.0a22/huscy.consents.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-06-27 15:38:26.000000 huscy.consents-0.8.0a22/huscy.consents.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-06-27 15:38:26.470975 huscy.consents-0.8.0a22/setup.cfg
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1766 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a22/setup.py
```

### Comparing `huscy.consents-0.8.0a21/PKG-INFO` & `huscy.consents-0.8.0a22/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.consents
-Version: 0.8.0a21
+Version: 0.8.0a22
 Summary: consents
 Home-page: https://bitbucket.org/huscy/consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.consents
```

### Comparing `huscy.consents-0.8.0a21/huscy/consents/admin.py` & `huscy.consents-0.8.0a22/huscy/consents/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/forms.py` & `huscy.consents-0.8.0a22/huscy/consents/forms.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/migrations/0001_initial.py` & `huscy.consents-0.8.0a22/huscy/consents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/models.py` & `huscy.consents-0.8.0a22/huscy/consents/models.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/serializer.py` & `huscy.consents-0.8.0a22/huscy/consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/services.py` & `huscy.consents-0.8.0a22/huscy/consents/services.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/static/consents/css/fomantic.min.css` & `huscy.consents-0.8.0a22/huscy/consents/static/consents/css/fomantic.min.css`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/static/consents/css/fomantic2.9.0.min.css` & `huscy.consents-0.8.0a22/huscy/consents/static/consents/css/fomantic2.9.0.min.css`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/static/consents/img/logo.svg` & `huscy.consents-0.8.0a22/huscy/consents/static/consents/img/logo.svg`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/fomantic.min.js` & `huscy.consents-0.8.0a22/huscy/consents/static/consents/js/fomantic.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/fomantic2.9.0.min.js` & `huscy.consents-0.8.0a22/huscy/consents/static/consents/js/fomantic2.9.0.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/jquery.min.js` & `huscy.consents-0.8.0a22/huscy/consents/static/consents/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/jquery3.6.1.min.js` & `huscy.consents-0.8.0a22/huscy/consents/static/consents/js/jquery3.6.1.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/popper.min.js` & `huscy.consents-0.8.0a22/huscy/consents/static/consents/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/popper1.16.1.min.js` & `huscy.consents-0.8.0a22/huscy/consents/static/consents/js/popper1.16.1.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/templates/consents/base.html` & `huscy.consents-0.8.0a22/huscy/consents/templates/consents/base.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/templates/consents/create_consent.html` & `huscy.consents-0.8.0a22/huscy/consents/templates/consents/create_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/templates/consents/sign_consent.html` & `huscy.consents-0.8.0a22/huscy/consents/templates/consents/sign_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/templates/consents/signed_consent.html` & `huscy.consents-0.8.0a22/huscy/consents/templates/consents/signed_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/views.py` & `huscy.consents-0.8.0a22/huscy/consents/views.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy/consents/viewsets.py` & `huscy.consents-0.8.0a22/huscy/consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a21/huscy.consents.egg-info/PKG-INFO` & `huscy.consents-0.8.0a22/huscy.consents.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.consents
-Version: 0.8.0a21
+Version: 0.8.0a22
 Summary: consents
 Home-page: https://bitbucket.org/huscy/consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.consents
```

### Comparing `huscy.consents-0.8.0a21/huscy.consents.egg-info/SOURCES.txt` & `huscy.consents-0.8.0a22/huscy.consents.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,11 +32,12 @@
 huscy/consents/templates/consents/create_consent.html
 huscy/consents/templates/consents/sign_consent.html
 huscy/consents/templates/consents/signed_consent.html
 huscy/consents/templates/consents/success.html
 huscy/consents/templates/consents/text_fragments/checkbox.html
 huscy/consents/templates/consents/text_fragments/heading.html
 huscy/consents/templates/consents/text_fragments/markdown.html
+huscy/consents/templates/consents/text_fragments/page-break.html
 huscy/consents/templates/consents/text_fragments/paragraph.html
 huscy/consents/templates/consents/widgets/select_date.html
 huscy/consents/templatetags/__init__.py
 huscy/consents/templatetags/dict_extras.py
```

### Comparing `huscy.consents-0.8.0a21/setup.py` & `huscy.consents-0.8.0a22/setup.py`

 * *Files identical despite different names*

