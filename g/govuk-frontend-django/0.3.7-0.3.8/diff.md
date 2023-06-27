# Comparing `tmp/govuk_frontend_django-0.3.7.tar.gz` & `tmp/govuk_frontend_django-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk_frontend_django-0.3.7.tar", max compression
+gzip compressed data, was "govuk_frontend_django-0.3.8.tar", max compression
```

## Comparing `govuk_frontend_django-0.3.7.tar` & `govuk_frontend_django-0.3.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1091 2023-04-18 16:00:56.529873 govuk_frontend_django-0.3.7/LICENSE
--rw-r--r--   0        0        0     1863 2023-06-15 15:40:06.070689 govuk_frontend_django-0.3.7/README.md
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.556313 govuk_frontend_django-0.3.7/govuk_frontend_django/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.561863 govuk_frontend_django-0.3.7/govuk_frontend_django/components/__init__.py
--rw-r--r--   0        0        0     1296 2023-05-30 14:32:14.384262 govuk_frontend_django-0.3.7/govuk_frontend_django/components/accordion.py
--rw-r--r--   0        0        0      939 2023-05-05 10:03:14.953137 govuk_frontend_django-0.3.7/govuk_frontend_django/components/back_link.py
--rw-r--r--   0        0        0     4249 2023-05-15 10:53:55.388602 govuk_frontend_django-0.3.7/govuk_frontend_django/components/base.py
--rw-r--r--   0        0        0     1170 2023-05-05 10:03:14.959254 govuk_frontend_django-0.3.7/govuk_frontend_django/components/breadcrumbs.py
--rw-r--r--   0        0        0     1221 2023-05-30 14:32:14.385042 govuk_frontend_django-0.3.7/govuk_frontend_django/components/button.py
--rw-r--r--   0        0        0     1838 2023-05-30 14:32:14.384394 govuk_frontend_django-0.3.7/govuk_frontend_django/components/character_count.py
--rw-r--r--   0        0        0     1892 2023-05-15 10:53:55.389249 govuk_frontend_django-0.3.7/govuk_frontend_django/components/checkboxes.py
--rw-r--r--   0        0        0     1723 2023-05-05 10:03:14.969605 govuk_frontend_django-0.3.7/govuk_frontend_django/components/cookie_banner.py
--rw-r--r--   0        0        0     1598 2023-05-05 10:03:14.973469 govuk_frontend_django-0.3.7/govuk_frontend_django/components/date_input.py
--rw-r--r--   0        0        0     1053 2023-05-05 10:03:14.970069 govuk_frontend_django-0.3.7/govuk_frontend_django/components/details.py
--rw-r--r--   0        0        0     1023 2023-05-05 10:03:14.970097 govuk_frontend_django-0.3.7/govuk_frontend_django/components/error_message.py
--rw-r--r--   0        0        0     1349 2023-05-05 10:03:14.980970 govuk_frontend_django-0.3.7/govuk_frontend_django/components/error_summary.py
--rw-r--r--   0        0        0     1024 2023-05-05 10:03:14.972317 govuk_frontend_django-0.3.7/govuk_frontend_django/components/fieldset.py
--rw-r--r--   0        0        0     1251 2023-05-30 14:32:14.384930 govuk_frontend_django-0.3.7/govuk_frontend_django/components/file_upload.py
--rw-r--r--   0        0        0     2007 2023-05-05 10:03:14.983853 govuk_frontend_django-0.3.7/govuk_frontend_django/components/footer.py
--rw-r--r--   0        0        0     1552 2023-05-05 10:03:14.980377 govuk_frontend_django-0.3.7/govuk_frontend_django/components/header.py
--rw-r--r--   0        0        0      927 2023-05-05 10:03:14.977728 govuk_frontend_django-0.3.7/govuk_frontend_django/components/hint.py
--rw-r--r--   0        0        0     1890 2023-05-30 14:32:14.384989 govuk_frontend_django-0.3.7/govuk_frontend_django/components/input.py
--rw-r--r--   0        0        0      960 2023-05-05 10:03:14.978389 govuk_frontend_django-0.3.7/govuk_frontend_django/components/inset_text.py
--rw-r--r--   0        0        0     1024 2023-05-05 10:03:14.977072 govuk_frontend_django-0.3.7/govuk_frontend_django/components/label.py
--rw-r--r--   0        0        0     1241 2023-05-05 10:03:14.983591 govuk_frontend_django-0.3.7/govuk_frontend_django/components/notification_banner.py
--rw-r--r--   0        0        0     1729 2023-05-05 10:03:14.985577 govuk_frontend_django-0.3.7/govuk_frontend_django/components/pagination.py
--rw-r--r--   0        0        0     1015 2023-05-05 10:03:14.982457 govuk_frontend_django-0.3.7/govuk_frontend_django/components/panel.py
--rw-r--r--   0        0        0      980 2023-05-05 10:03:14.984779 govuk_frontend_django-0.3.7/govuk_frontend_django/components/phase_banner.py
--rw-r--r--   0        0        0     1753 2023-05-05 10:03:14.988699 govuk_frontend_django-0.3.7/govuk_frontend_django/components/radios.py
--rw-r--r--   0        0        0     1504 2023-05-30 14:32:14.385089 govuk_frontend_django-0.3.7/govuk_frontend_django/components/select.py
--rw-r--r--   0        0        0      956 2023-05-05 10:03:14.987832 govuk_frontend_django-0.3.7/govuk_frontend_django/components/skip_link.py
--rw-r--r--   0        0        0     1850 2023-05-05 10:03:14.992204 govuk_frontend_django-0.3.7/govuk_frontend_django/components/summary_list.py
--rw-r--r--   0        0        0     1653 2023-05-05 10:03:14.996881 govuk_frontend_django-0.3.7/govuk_frontend_django/components/table.py
--rw-r--r--   0        0        0     1171 2023-05-05 10:03:14.991905 govuk_frontend_django-0.3.7/govuk_frontend_django/components/tabs.py
--rw-r--r--   0        0        0      892 2023-05-05 10:03:14.989454 govuk_frontend_django-0.3.7/govuk_frontend_django/components/tag.py
--rw-r--r--   0        0        0     1344 2023-05-30 14:32:14.385191 govuk_frontend_django-0.3.7/govuk_frontend_django/components/textarea.py
--rw-r--r--   0        0        0      986 2023-05-30 14:32:14.385251 govuk_frontend_django-0.3.7/govuk_frontend_django/components/warning_text.py
--rw-r--r--   0        0        0        0 2023-05-03 19:40:36.710697 govuk_frontend_django-0.3.7/govuk_frontend_django/py.typed
--rw-r--r--   0        0        0     2744 2023-05-30 14:32:14.385323 govuk_frontend_django-0.3.7/govuk_frontend_django/templates/govuk_frontend_django/base.html
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.543579 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/__init__.py
--rw-r--r--   0        0        0    13302 2023-06-12 10:50:46.623563 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py
--rw-r--r--   0        0        0     1518 2023-06-09 13:56:40.062345 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py
--rw-r--r--   0        0        0     1207 2023-06-09 13:56:40.061827 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py
--rw-r--r--   0        0        0     3291 2023-06-09 13:56:40.062135 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py
--rw-r--r--   0        0        0     2198 2023-06-09 13:56:40.062484 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py
--rw-r--r--   0        0        0     1532 2023-06-09 13:56:40.062567 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py
--rw-r--r--   0        0        0     5243 2023-06-09 13:56:40.062739 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py
--rw-r--r--   0        0        0     1600 2023-06-09 13:56:40.062823 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/header.py
--rw-r--r--   0        0        0     2322 2023-06-15 15:38:00.058150 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py
--rw-r--r--   0        0        0     1388 2023-06-09 13:56:40.063524 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py
--rw-r--r--   0        0        0     7121 2023-06-09 16:42:09.396299 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py
--rw-r--r--   0        0        0     1439 2023-04-26 11:55:41.163769 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/table.py
--rw-r--r--   0        0        0     1286 2023-06-09 13:56:40.063840 govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py
--rw-r--r--   0        0        0     2100 2023-06-15 15:39:57.435624 govuk_frontend_django-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     2797 1970-01-01 00:00:00.000000 govuk_frontend_django-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-18 16:00:56.529873 govuk_frontend_django-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1863 2023-06-27 10:58:09.656213 govuk_frontend_django-0.3.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.556313 govuk_frontend_django-0.3.8/govuk_frontend_django/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.561863 govuk_frontend_django-0.3.8/govuk_frontend_django/components/__init__.py
+-rw-r--r--   0        0        0     1296 2023-05-30 14:32:14.384262 govuk_frontend_django-0.3.8/govuk_frontend_django/components/accordion.py
+-rw-r--r--   0        0        0      939 2023-05-05 10:03:14.953137 govuk_frontend_django-0.3.8/govuk_frontend_django/components/back_link.py
+-rw-r--r--   0        0        0     4249 2023-05-15 10:53:55.388602 govuk_frontend_django-0.3.8/govuk_frontend_django/components/base.py
+-rw-r--r--   0        0        0     1170 2023-05-05 10:03:14.959254 govuk_frontend_django-0.3.8/govuk_frontend_django/components/breadcrumbs.py
+-rw-r--r--   0        0        0     1221 2023-05-30 14:32:14.385042 govuk_frontend_django-0.3.8/govuk_frontend_django/components/button.py
+-rw-r--r--   0        0        0     1838 2023-05-30 14:32:14.384394 govuk_frontend_django-0.3.8/govuk_frontend_django/components/character_count.py
+-rw-r--r--   0        0        0     1892 2023-05-15 10:53:55.389249 govuk_frontend_django-0.3.8/govuk_frontend_django/components/checkboxes.py
+-rw-r--r--   0        0        0     1723 2023-05-05 10:03:14.969605 govuk_frontend_django-0.3.8/govuk_frontend_django/components/cookie_banner.py
+-rw-r--r--   0        0        0     1598 2023-05-05 10:03:14.973469 govuk_frontend_django-0.3.8/govuk_frontend_django/components/date_input.py
+-rw-r--r--   0        0        0     1053 2023-05-05 10:03:14.970069 govuk_frontend_django-0.3.8/govuk_frontend_django/components/details.py
+-rw-r--r--   0        0        0     1023 2023-05-05 10:03:14.970097 govuk_frontend_django-0.3.8/govuk_frontend_django/components/error_message.py
+-rw-r--r--   0        0        0     1349 2023-05-05 10:03:14.980970 govuk_frontend_django-0.3.8/govuk_frontend_django/components/error_summary.py
+-rw-r--r--   0        0        0     1024 2023-05-05 10:03:14.972317 govuk_frontend_django-0.3.8/govuk_frontend_django/components/fieldset.py
+-rw-r--r--   0        0        0     1251 2023-05-30 14:32:14.384930 govuk_frontend_django-0.3.8/govuk_frontend_django/components/file_upload.py
+-rw-r--r--   0        0        0     2007 2023-05-05 10:03:14.983853 govuk_frontend_django-0.3.8/govuk_frontend_django/components/footer.py
+-rw-r--r--   0        0        0     1552 2023-05-05 10:03:14.980377 govuk_frontend_django-0.3.8/govuk_frontend_django/components/header.py
+-rw-r--r--   0        0        0      927 2023-05-05 10:03:14.977728 govuk_frontend_django-0.3.8/govuk_frontend_django/components/hint.py
+-rw-r--r--   0        0        0     1890 2023-05-30 14:32:14.384989 govuk_frontend_django-0.3.8/govuk_frontend_django/components/input.py
+-rw-r--r--   0        0        0      960 2023-05-05 10:03:14.978389 govuk_frontend_django-0.3.8/govuk_frontend_django/components/inset_text.py
+-rw-r--r--   0        0        0     1024 2023-05-05 10:03:14.977072 govuk_frontend_django-0.3.8/govuk_frontend_django/components/label.py
+-rw-r--r--   0        0        0     1241 2023-05-05 10:03:14.983591 govuk_frontend_django-0.3.8/govuk_frontend_django/components/notification_banner.py
+-rw-r--r--   0        0        0     1729 2023-05-05 10:03:14.985577 govuk_frontend_django-0.3.8/govuk_frontend_django/components/pagination.py
+-rw-r--r--   0        0        0     1015 2023-05-05 10:03:14.982457 govuk_frontend_django-0.3.8/govuk_frontend_django/components/panel.py
+-rw-r--r--   0        0        0      980 2023-05-05 10:03:14.984779 govuk_frontend_django-0.3.8/govuk_frontend_django/components/phase_banner.py
+-rw-r--r--   0        0        0     1753 2023-05-05 10:03:14.988699 govuk_frontend_django-0.3.8/govuk_frontend_django/components/radios.py
+-rw-r--r--   0        0        0     1504 2023-05-30 14:32:14.385089 govuk_frontend_django-0.3.8/govuk_frontend_django/components/select.py
+-rw-r--r--   0        0        0      956 2023-05-05 10:03:14.987832 govuk_frontend_django-0.3.8/govuk_frontend_django/components/skip_link.py
+-rw-r--r--   0        0        0     1850 2023-05-05 10:03:14.992204 govuk_frontend_django-0.3.8/govuk_frontend_django/components/summary_list.py
+-rw-r--r--   0        0        0     1653 2023-05-05 10:03:14.996881 govuk_frontend_django-0.3.8/govuk_frontend_django/components/table.py
+-rw-r--r--   0        0        0     1171 2023-05-05 10:03:14.991905 govuk_frontend_django-0.3.8/govuk_frontend_django/components/tabs.py
+-rw-r--r--   0        0        0      892 2023-05-05 10:03:14.989454 govuk_frontend_django-0.3.8/govuk_frontend_django/components/tag.py
+-rw-r--r--   0        0        0     1344 2023-05-30 14:32:14.385191 govuk_frontend_django-0.3.8/govuk_frontend_django/components/textarea.py
+-rw-r--r--   0        0        0      986 2023-05-30 14:32:14.385251 govuk_frontend_django-0.3.8/govuk_frontend_django/components/warning_text.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:40:36.710697 govuk_frontend_django-0.3.8/govuk_frontend_django/py.typed
+-rw-r--r--   0        0        0     2744 2023-06-27 10:54:47.729871 govuk_frontend_django-0.3.8/govuk_frontend_django/templates/govuk_frontend_django/base.html
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.543579 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/__init__.py
+-rw-r--r--   0        0        0    13302 2023-06-12 10:50:46.623563 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py
+-rw-r--r--   0        0        0     1518 2023-06-09 13:56:40.062345 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py
+-rw-r--r--   0        0        0     1207 2023-06-09 13:56:40.061827 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py
+-rw-r--r--   0        0        0     3291 2023-06-09 13:56:40.062135 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py
+-rw-r--r--   0        0        0     2198 2023-06-09 13:56:40.062484 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py
+-rw-r--r--   0        0        0     1532 2023-06-09 13:56:40.062567 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py
+-rw-r--r--   0        0        0     5243 2023-06-09 13:56:40.062739 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py
+-rw-r--r--   0        0        0     1600 2023-06-09 13:56:40.062823 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/header.py
+-rw-r--r--   0        0        0     2322 2023-06-15 15:38:00.058150 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py
+-rw-r--r--   0        0        0     1388 2023-06-09 13:56:40.063524 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py
+-rw-r--r--   0        0        0     7121 2023-06-09 16:42:09.396299 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py
+-rw-r--r--   0        0        0     1439 2023-04-26 11:55:41.163769 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/table.py
+-rw-r--r--   0        0        0     1286 2023-06-09 13:56:40.063840 govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py
+-rw-r--r--   0        0        0     2100 2023-06-27 10:58:03.027656 govuk_frontend_django-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     2797 1970-01-01 00:00:00.000000 govuk_frontend_django-0.3.8/PKG-INFO
```

### Comparing `govuk_frontend_django-0.3.7/LICENSE` & `govuk_frontend_django-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/README.md` & `govuk_frontend_django-0.3.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 ## Compatibility table
 
 Below is a list of the versions of this package and the versions of the GOV.UK Frontend that they are compatible with.
 
 | Package Version | GOV.UK Frontend Version |
 | --------------- | ----------------------- |
 | [0.2.0](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.2.0) - [0.2.3](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.2.3) | [v4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
-| [0.3.0](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.3.0) - [0.3.7](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.3.7) | [v4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
+| [0.3.0](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.3.0) - [0.3.8](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.3.8) | [v4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
```

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/accordion.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/accordion.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/back_link.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/back_link.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/base.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/base.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/breadcrumbs.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/button.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/button.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/character_count.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/character_count.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/checkboxes.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/checkboxes.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/cookie_banner.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/date_input.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/date_input.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/details.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/details.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/error_message.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/error_message.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/error_summary.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/error_summary.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/fieldset.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/fieldset.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/file_upload.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/file_upload.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/footer.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/footer.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/header.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/header.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/hint.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/hint.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/input.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/input.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/inset_text.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/inset_text.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/label.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/label.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/notification_banner.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/notification_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/pagination.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/pagination.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/panel.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/panel.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/phase_banner.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/phase_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/radios.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/radios.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/select.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/select.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/skip_link.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/skip_link.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/summary_list.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/summary_list.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/table.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/table.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/tabs.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/tabs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/tag.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/tag.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/textarea.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/textarea.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/components/warning_text.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/components/warning_text.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templates/govuk_frontend_django/base.html` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templates/govuk_frontend_django/base.html`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/header.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/header.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/table.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/table.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py` & `govuk_frontend_django-0.3.8/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.3.7/pyproject.toml` & `govuk_frontend_django-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "govuk-frontend-django"
-version = "0.3.7"
+version = "0.3.8"
 description = "Django functionality to help when building a GOV.UK website."
 authors = [
     "DBT Live Service Team <live.services@digital.trade.gov.uk>",
     "Cam Lamb <cameron.lamb@digital.trade.gov.uk>",
     "Sam Dudley <samuel.dudley@digital.trade.gov.uk>",
 ]
 license = "MIT"
```

### Comparing `govuk_frontend_django-0.3.7/PKG-INFO` & `govuk_frontend_django-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-django
-Version: 0.3.7
+Version: 0.3.8
 Summary: Django functionality to help when building a GOV.UK website.
 Home-page: https://uktrade.github.io/govuk-frontend-django/
 License: MIT
 Author: DBT Live Service Team
 Author-email: live.services@digital.trade.gov.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -58,9 +58,9 @@
 ## Compatibility table
 
 Below is a list of the versions of this package and the versions of the GOV.UK Frontend that they are compatible with.
 
 | Package Version | GOV.UK Frontend Version |
 | --------------- | ----------------------- |
 | [0.2.0](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.2.0) - [0.2.3](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.2.3) | [v4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
-| [0.3.0](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.3.0) - [0.3.7](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.3.7) | [v4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
+| [0.3.0](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.3.0) - [0.3.8](https://github.com/uktrade/govuk-frontend-django/releases/tag/0.3.8) | [v4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
```

