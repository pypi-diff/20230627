# Comparing `tmp/pretix-mollie-1.5.3.tar.gz` & `tmp/pretix-mollie-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-mollie-1.5.3.tar", last modified: Sun May 28 23:08:30 2023, max compression
+gzip compressed data, was "pretix-mollie-1.6.0.tar", last modified: Tue Jun 27 12:58:20 2023, max compression
```

## Comparing `pretix-mollie-1.5.3.tar` & `pretix-mollie-1.6.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.480964 pretix-mollie-1.5.3/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1955 2023-05-28 23:08:30.480964 pretix-mollie-1.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.456963 pretix-mollie-1.5.3/pretix_mollie/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    12020 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.456963 pretix-mollie-1.5.3/pretix_mollie/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15938 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:08:00.000000 pretix-mollie-1.5.3/pretix_mollie/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15783 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    10733 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10708 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11506 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11735 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15802 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10711 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15845 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10969 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10717 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10708 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10708 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10879 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11446 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    26131 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     3365 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/static/pretix_mollie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:08:00.000000 pretix-mollie-1.5.3/pretix_mollie/static/pretix_mollie/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/static/pretix_mollie/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.480964 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:08:00.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/checkout_payment_form_banktransfer.html
--rw-rw-rw-   0 root         (0) root         (0)     2220 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/control.html
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/order_pending.txt
--rw-rw-rw-   0 root         (0) root         (0)     4832 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/pending.html
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/redirect.html
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2002 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14737 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1955 2023-05-28 23:08:30.000000 pretix-mollie-1.5.3/pretix_mollie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1934 2023-05-28 23:08:30.000000 pretix-mollie-1.5.3/pretix_mollie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:08:30.000000 pretix-mollie-1.5.3/pretix_mollie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-28 23:08:30.000000 pretix-mollie-1.5.3/pretix_mollie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-28 23:08:30.000000 pretix-mollie-1.5.3/pretix_mollie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-28 23:08:30.480964 pretix-mollie-1.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.494539 pretix-mollie-1.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-06-27 12:58:20.494539 pretix-mollie-1.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    12020 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15938 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15783 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    10733 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10708 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11506 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11735 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15802 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10711 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.478538 pretix-mollie-1.6.0/pretix_mollie/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15845 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.478538 pretix-mollie-1.6.0/pretix_mollie/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10969 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.478538 pretix-mollie-1.6.0/pretix_mollie/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10717 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.478538 pretix-mollie-1.6.0/pretix_mollie/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10708 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10708 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10879 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11446 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    27447 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/static/pretix_mollie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/static/pretix_mollie/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/static/pretix_mollie/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.494539 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/checkout_payment_form_banktransfer.html
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/control.html
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/order_pending.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4832 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14737 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-06-27 12:58:20.000000 pretix-mollie-1.6.0/pretix_mollie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-06-27 12:58:20.000000 pretix-mollie-1.6.0/pretix_mollie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 12:58:20.000000 pretix-mollie-1.6.0/pretix_mollie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-27 12:58:20.000000 pretix-mollie-1.6.0/pretix_mollie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-27 12:58:20.000000 pretix-mollie-1.6.0/pretix_mollie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-27 12:58:20.494539 pretix-mollie-1.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/setup.py
```

### Comparing `pretix-mollie-1.5.3/LICENSE` & `pretix-mollie-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/PKG-INFO` & `pretix-mollie-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mollie
-Version: 1.5.3
+Version: 1.6.0
 Summary: Integration for the Mollie payment provider.
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2018 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-mollie-1.5.3/README.rst` & `pretix-mollie-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/apps.py` & `pretix-mollie-1.6.0/pretix_mollie/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/forms.py` & `pretix-mollie-1.6.0/pretix_mollie/forms.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/ca/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/de/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/django.pot` & `pretix-mollie-1.6.0/pretix_mollie/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/el/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/fi/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/ja/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/lv/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/nl/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/pl/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/pt/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/ru/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/si/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/sl/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/sv/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-mollie-1.6.0/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/payment.py` & `pretix-mollie-1.6.0/pretix_mollie/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from django.urls import reverse
 from django.utils.crypto import get_random_string
 from urllib.parse import quote
 from django.utils.timezone import now
 from django.utils.translation import pgettext, gettext_lazy as _
 from i18nfield.strings import LazyI18nString
 
-from pretix.base.reldate import RelativeDateField, RelativeDateWrapper
+from pretix.base.reldate import RelativeDateField, RelativeDateWrapper, RelativeDateWidget, BASE_CHOICES
 from pretix.helpers import OF_SELF
 from pretix_mollie.utils import refresh_mollie_token
 from requests import HTTPError
 
 from pretix.base.models import Event, OrderPayment, OrderRefund, Order, CartPosition
 from pretix.base.payment import BasePaymentProvider, PaymentException
 from pretix.base.settings import SettingsSandbox
@@ -230,14 +230,36 @@
                      required=False,
                  )),
                 ('method_banktransfer_availability_date',
                  RelativeDateField(
                      label=_('Bank transfer available until'),
                      help_text=_('Users will not be able to choose this payment provider after the given date.'),
                      required=False,
+                     widget=RelativeDateWidget(
+                         status_choices=[
+                             ('unset', _('Not set')),
+                             ('absolute', _('Fixed date:')),
+                             ('relative', _('Relative date:')),
+                         ],
+                         base_choices=BASE_CHOICES,
+                         attrs={
+                             "data-display-dependency": "#id_payment_mollie_method_banktransfer",
+                         }
+                     )
+                 )),
+                ('method_banktransfer_invoice_immediately',
+                 forms.BooleanField(
+                     label=_('Create an invoice for orders using bank transfer immediately if the event is otherwise '
+                             'configured to create invoices after payment is completed.'),
+                     required=False,
+                     widget=forms.CheckboxInput(
+                         attrs={
+                             "data-display-dependency": "#id_payment_mollie_method_banktransfer",
+                         }
+                     ),
                  )),
             ] + list(super().settings_form_fields.items())
         )
         d['_availability_date'].label = _('All payment methods available until')
         d.move_to_end('_enabled', last=False)
         return d
 
@@ -559,14 +581,18 @@
 
 
 class MollieBanktransfer(MollieMethod):
     method = 'banktransfer'
     verbose_name = _('Bank transfer via Mollie')
     public_name = _('Bank transfer')
 
+    @property
+    def requires_invoice_immediately(self):
+        return self.settings.get('method_banktransfer_invoice_immediately', False, as_type=bool)
+
     @transaction.atomic()
     def execute_payment(self, request: HttpRequest, payment: OrderPayment, retry=True):
         p_orig = payment
         if retry:
             payment = OrderPayment.objects.select_for_update(of=OF_SELF).get(pk=payment.pk)
         super().execute_payment(request, payment, retry)
         p_orig.refresh_from_db()
```

### Comparing `pretix-mollie-1.5.3/pretix_mollie/signals.py` & `pretix-mollie-1.6.0/pretix_mollie/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/static/pretix_mollie/logo.svg` & `pretix-mollie-1.6.0/pretix_mollie/static/pretix_mollie/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/control.html` & `pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/control.html`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/pending.html` & `pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/redirect.html` & `pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/urls.py` & `pretix-mollie-1.6.0/pretix_mollie/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/utils.py` & `pretix-mollie-1.6.0/pretix_mollie/utils.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie/views.py` & `pretix-mollie-1.6.0/pretix_mollie/views.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pretix_mollie.egg-info/PKG-INFO` & `pretix-mollie-1.6.0/pretix_mollie.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mollie
-Version: 1.5.3
+Version: 1.6.0
 Summary: Integration for the Mollie payment provider.
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2018 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-mollie-1.5.3/pretix_mollie.egg-info/SOURCES.txt` & `pretix-mollie-1.6.0/pretix_mollie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.3/pyproject.toml` & `pretix-mollie-1.6.0/pyproject.toml`

 * *Files identical despite different names*

