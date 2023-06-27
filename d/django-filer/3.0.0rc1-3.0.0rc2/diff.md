# Comparing `tmp/django-filer-3.0.0rc1.tar.gz` & `tmp/django-filer-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-filer-3.0.0rc1.tar", last modified: Mon Jun 26 13:23:51 2023, max compression
+gzip compressed data, was "django-filer-3.0.0rc2.tar", last modified: Tue Jun 27 13:56:57 2023, max compression
```

## Comparing `django-filer-3.0.0rc1.tar` & `django-filer-3.0.0rc2.tar`

### file list

```diff
@@ -1,375 +1,375 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.147806 django-filer-3.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-26 13:23:51.147806 django-filer-3.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.099805 django-filer-3.0.0rc1/django_filer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-26 13:23:51.000000 django-filer-3.0.0rc1/django_filer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-26 13:23:51.000000 django-filer-3.0.0rc1/django_filer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:23:51.000000 django-filer-3.0.0rc1/django_filer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:23:50.000000 django-filer-3.0.0rc1/django_filer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 13:23:51.000000 django-filer-3.0.0rc1/django_filer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 13:23:51.000000 django-filer-3.0.0rc1/django_filer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.099805 django-filer-3.0.0rc1/filer/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.099805 django-filer-3.0.0rc1/filer/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/clipboardadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/fileadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    57162 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/folderadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/imageadmin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.099805 django-filer-3.0.0rc1/filer/admin/patched/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/patched/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/patched/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/permissionadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/thumbnailoptionadmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.099805 django-filer-3.0.0rc1/filer/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/contrib/django_cms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/contrib/django_cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/contrib/django_cms/cms_toolbars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/fields/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/fields/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/fields/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/fields/multistorage_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26987 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18714 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33818 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33463 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.103805 django-filer-3.0.0rc1/filer/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30481 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26373 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17098 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32686 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34069 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.087805 django-filer-3.0.0rc1/filer/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27630 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32519 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31855 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33167 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26374 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26388 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/lt_LT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/lt_LT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/lt_LT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.107805 django-filer-3.0.0rc1/filer/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31143 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33623 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nl_NL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12947 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31075 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    33701 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15418 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    32621 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21923 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37699 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26616 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    29066 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/vi_VN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/vi_VN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26393 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/vi_VN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26373 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.091805 django-filer-3.0.0rc1/filer/locale/zh-Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/zh-Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh-Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    31148 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh-Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26387 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26388 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.111805 django-filer-3.0.0rc1/filer/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.115805 django-filer-3.0.0rc1/filer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/management/commands/filer_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/management/commands/generate_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/management/commands/import_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.115805 django-filer-3.0.0rc1/filer/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0002_auto_20150606_2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0003_thumbnailoption.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0004_auto_20160328_1434.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0005_auto_20160623_1425.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0006_auto_20160623_1627.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0007_auto_20161016_1055.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0008_auto_20171117_1313.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0009_auto_20171220_1635.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0010_auto_20180414_2058.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0011_auto_20190418_0137.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0012_file_mime_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0013_image_width_height_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0014_folder_permission_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/0017_image__transparent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.119805 django-filer-3.0.0rc1/filer/models/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/clipboardmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/filemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/foldermodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/imagemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/thumbnailoptionmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/models/virtualitems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.119805 django-filer-3.0.0rc1/filer/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.119805 django-filer-3.0.0rc1/filer/server/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/backends/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/backends/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/backends/xsendfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/main_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/thumbnails_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/server/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/static/filer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.119805 django-filer-3.0.0rc1/filer/static/filer/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/css/admin_filer.cms.icons.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    92632 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/css/admin_filer.css
--rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/css/admin_filer.fa.icons.css
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/css/admin_folderpermissions.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.119805 django-filer-3.0.0rc1/filer/static/filer/css/maps/
--rw-r--r--   0 runner    (1001) docker     (123)    88599 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/css/maps/admin_filer.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.123805 django-filer-3.0.0rc1/filer/static/filer/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   106260 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    68875 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   355981 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   138204 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    81284 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    64464 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.123805 django-filer-3.0.0rc1/filer/static/filer/fonts/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/expand.svg
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/move-to-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/remove-selection.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/select.svg
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/th-large.svg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/th-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/fonts/src/upload.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.127805 django-filer-3.0.0rc1/filer/static/filer/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/cloud-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/file-zip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/folder-dropdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/folder-root.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/folder-unfiled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/icons/folder.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.127805 django-filer-3.0.0rc1/filer/static/filer/img/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/button-bg.gif
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/close.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/icon_changelink.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/icon_deletelink.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/loading_animation.gif
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/nav-bg.gif
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/select_item-hover.gif
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/select_item.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/img/upload_button.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.127805 django-filer-3.0.0rc1/filer/static/filer/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.131805 django-filer-3.0.0rc1/filer/static/filer/js/addons/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/copy-move-files.js
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/dropdown-menu.js
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/dropzone.init.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/filer_popup_response.js
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/focal-point.js
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/popup_handling.js
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/table-dropzone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/toggler.js
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/tooltip.js
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/upload-button.js
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/addons/widget.js
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.135805 django-filer-3.0.0rc1/filer/static/filer/js/libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/class.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/dropzone.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/fileuploader.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery.cookie.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/static/filer/js/libs/mediator.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.095805 django-filer-3.0.0rc1/filer/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.135805 django-filer-3.0.0rc1/filer/templates/admin/filer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/base_site.html
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/delete_selected_files_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/dismiss_popup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.135805 django-filer-3.0.0rc1/filer/templates/admin/filer/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/file/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/file/popup_response.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.139805 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_copy_destination.html
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_images_resize_options.html
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_move_destination.html
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_rename_format.html
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_listing.html
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_table_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_thumbnail_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/list_type_switcher.html
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/folder/new_folder_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templates/admin/filer/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/image/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templates/admin/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/templatetags/file_icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/clipboard/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/clipboard/clipboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/detail_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/tools/search_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templates/admin/filer/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/widgets/admin_file.html
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templates/admin/filer/widgets/admin_folder.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.143806 django-filer-3.0.0rc1/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templatetags/filer_admin_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templatetags/filer_image_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/templatetags/filer_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/thumbnail_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:51.147806 django-filer-3.0.0rc1/filer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/filer_easy_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/generate_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/model_label.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/pil_exif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/recursive_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/utils/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/filer/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-26 13:23:51.147806 django-filer-3.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-26 13:23:37.000000 django-filer-3.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.461977 django-filer-3.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-27 13:56:57.461977 django-filer-3.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.429977 django-filer-3.0.0rc2/django_filer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-27 13:56:57.000000 django-filer-3.0.0rc2/django_filer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-27 13:56:57.000000 django-filer-3.0.0rc2/django_filer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:56:57.000000 django-filer-3.0.0rc2/django_filer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:56:57.000000 django-filer-3.0.0rc2/django_filer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 13:56:57.000000 django-filer-3.0.0rc2/django_filer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 13:56:57.000000 django-filer-3.0.0rc2/django_filer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.433977 django-filer-3.0.0rc2/filer/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.433977 django-filer-3.0.0rc2/filer/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/clipboardadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/fileadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57162 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/folderadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/imageadmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.433977 django-filer-3.0.0rc2/filer/admin/patched/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/patched/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/patched/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/permissionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/thumbnailoptionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.433977 django-filer-3.0.0rc2/filer/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.433977 django-filer-3.0.0rc2/filer/contrib/django_cms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/contrib/django_cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/contrib/django_cms/cms_toolbars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.433977 django-filer-3.0.0rc2/filer/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/fields/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/fields/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/fields/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/fields/multistorage_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.433977 django-filer-3.0.0rc2/filer/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.421977 django-filer-3.0.0rc2/filer/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.433977 django-filer-3.0.0rc2/filer/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26987 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.421977 django-filer-3.0.0rc2/filer/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.433977 django-filer-3.0.0rc2/filer/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.421977 django-filer-3.0.0rc2/filer/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.433977 django-filer-3.0.0rc2/filer/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.421977 django-filer-3.0.0rc2/filer/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.421977 django-filer-3.0.0rc2/filer/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18714 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33818 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.421977 django-filer-3.0.0rc2/filer/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.421977 django-filer-3.0.0rc2/filer/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33463 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27500 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30481 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26373 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17098 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32686 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34069 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27630 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32519 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31855 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33167 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.437977 django-filer-3.0.0rc2/filer/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26374 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26388 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/lt_LT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/lt_LT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26674 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/lt_LT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31143 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33623 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/nl_NL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12947 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/nn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31075 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    33701 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15418 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    32621 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21923 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37699 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26616 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    29066 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/vi_VN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/vi_VN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26393 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/vi_VN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26373 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/zh-Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.441977 django-filer-3.0.0rc2/filer/locale/zh-Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/zh-Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    31148 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/zh-Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.445977 django-filer-3.0.0rc2/filer/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26387 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.425977 django-filer-3.0.0rc2/filer/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.445977 django-filer-3.0.0rc2/filer/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26388 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.445977 django-filer-3.0.0rc2/filer/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.445977 django-filer-3.0.0rc2/filer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/management/commands/filer_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/management/commands/generate_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/management/commands/import_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.445977 django-filer-3.0.0rc2/filer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0002_auto_20150606_2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0003_thumbnailoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0004_auto_20160328_1434.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0005_auto_20160623_1425.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0006_auto_20160623_1627.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0007_auto_20161016_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0008_auto_20171117_1313.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0009_auto_20171220_1635.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0010_auto_20180414_2058.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0011_auto_20190418_0137.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0012_file_mime_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0013_image_width_height_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0014_folder_permission_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/0017_image__transparent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.449977 django-filer-3.0.0rc2/filer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/models/clipboardmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/models/filemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/models/foldermodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/models/imagemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/models/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/models/thumbnailoptionmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/models/virtualitems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.449977 django-filer-3.0.0rc2/filer/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.449977 django-filer-3.0.0rc2/filer/server/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/server/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/server/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/server/backends/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/server/backends/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/server/backends/xsendfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/server/main_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/server/thumbnails_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.429977 django-filer-3.0.0rc2/filer/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.429977 django-filer-3.0.0rc2/filer/static/filer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.449977 django-filer-3.0.0rc2/filer/static/filer/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/css/admin_filer.cms.icons.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    92632 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/css/admin_filer.css
+-rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/css/admin_filer.fa.icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/css/admin_folderpermissions.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.449977 django-filer-3.0.0rc2/filer/static/filer/css/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)    88599 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/css/maps/admin_filer.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.453977 django-filer-3.0.0rc2/filer/static/filer/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   106260 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/django-filer-iconfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/django-filer-iconfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/django-filer-iconfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/django-filer-iconfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/django-filer-iconfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    68875 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   355981 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   138204 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    81284 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    64464 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.453977 django-filer-3.0.0rc2/filer/static/filer/fonts/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/expand.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/move-to-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/remove-selection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/select.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/th-large.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/th-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/fonts/src/upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.453977 django-filer-3.0.0rc2/filer/static/filer/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/cloud-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/file-zip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/folder-dropdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/folder-root.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/folder-unfiled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/icons/folder.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.457977 django-filer-3.0.0rc2/filer/static/filer/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/img/button-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/img/close.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/img/icon_changelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/img/icon_deletelink.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/img/loading_animation.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/img/nav-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/img/select_item-hover.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/img/select_item.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/img/upload_button.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.457977 django-filer-3.0.0rc2/filer/static/filer/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.457977 django-filer-3.0.0rc2/filer/static/filer/js/addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/copy-move-files.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/dropdown-menu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/dropzone.init.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/filer_popup_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/focal-point.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/popup_handling.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/table-dropzone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/toggler.js
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/tooltip.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/upload-button.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/addons/widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.457977 django-filer-3.0.0rc2/filer/static/filer/js/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/libs/class.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34316 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/libs/dropzone.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/libs/fileuploader.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/libs/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/libs/jquery.cookie.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95957 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/libs/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/static/filer/js/libs/mediator.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.429977 django-filer-3.0.0rc2/filer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.429977 django-filer-3.0.0rc2/filer/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.457977 django-filer-3.0.0rc2/filer/templates/admin/filer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/delete_selected_files_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/dismiss_popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.457977 django-filer-3.0.0rc2/filer/templates/admin/filer/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/file/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/file/popup_response.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.461977 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/choose_copy_destination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/choose_images_resize_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/choose_move_destination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/choose_rename_format.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/directory_listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/directory_table_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/directory_thumbnail_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/list_type_switcher.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/folder/new_folder_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.461977 django-filer-3.0.0rc2/filer/templates/admin/filer/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/image/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.461977 django-filer-3.0.0rc2/filer/templates/admin/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/templatetags/file_icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.461977 django-filer-3.0.0rc2/filer/templates/admin/filer/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.461977 django-filer-3.0.0rc2/filer/templates/admin/filer/tools/clipboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/tools/clipboard/clipboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/tools/detail_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/tools/search_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.461977 django-filer-3.0.0rc2/filer/templates/admin/filer/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/widgets/admin_file.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templates/admin/filer/widgets/admin_folder.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.461977 django-filer-3.0.0rc2/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templatetags/filer_admin_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templatetags/filer_image_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/templatetags/filer_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/thumbnail_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:57.461977 django-filer-3.0.0rc2/filer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/utils/filer_easy_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/utils/generate_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/utils/model_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/utils/pil_exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/utils/recursive_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/utils/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/filer/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-27 13:56:57.465977 django-filer-3.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-27 13:56:48.000000 django-filer-3.0.0rc2/setup.py
```

### Comparing `django-filer-3.0.0rc1/LICENSE` & `django-filer-3.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/PKG-INFO` & `django-filer-3.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -24,27 +24,25 @@
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django CMS
-Classifier: Framework :: Django CMS :: 3.6
-Classifier: Framework :: Django CMS :: 3.7
 Classifier: Framework :: Django CMS :: 3.8
 Classifier: Framework :: Django CMS :: 3.9
 Classifier: Framework :: Django CMS :: 3.10
 Classifier: Framework :: Django CMS :: 3.11
 Classifier: Framework :: Django CMS :: 4.0
 Classifier: Framework :: Django CMS :: 4.1
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 ============
 Django Filer
 ============
 
 |pypi| |python| |django| |coverage|
```

### Comparing `django-filer-3.0.0rc1/README.rst` & `django-filer-3.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/django_filer.egg-info/PKG-INFO` & `django-filer-3.0.0rc2/django_filer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -24,27 +24,25 @@
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django CMS
-Classifier: Framework :: Django CMS :: 3.6
-Classifier: Framework :: Django CMS :: 3.7
 Classifier: Framework :: Django CMS :: 3.8
 Classifier: Framework :: Django CMS :: 3.9
 Classifier: Framework :: Django CMS :: 3.10
 Classifier: Framework :: Django CMS :: 3.11
 Classifier: Framework :: Django CMS :: 4.0
 Classifier: Framework :: Django CMS :: 4.1
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 ============
 Django Filer
 ============
 
 |pypi| |python| |django| |coverage|
```

### Comparing `django-filer-3.0.0rc1/django_filer.egg-info/SOURCES.txt` & `django-filer-3.0.0rc2/django_filer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/__init__.py` & `django-filer-3.0.0rc2/filer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,10 +9,10 @@
  5. git push
  6. Assure that all tests pass on https://github.com/django-cms/django-filer/actions
  7. Create a new release on github. Create the new tag against the latest master commit and auto generate
     the release notes https://github.com/django-cms/django-filer/releases/new
  8. Publish the release and it will automatically release to pypi
 """
 
-__version__ = '3.0.0rc1'
+__version__ = '3.0.0rc2'
 
 default_app_config = 'filer.apps.FilerConfig'
```

### Comparing `django-filer-3.0.0rc1/filer/admin/__init__.py` & `django-filer-3.0.0rc2/filer/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/admin/clipboardadmin.py` & `django-filer-3.0.0rc2/filer/admin/clipboardadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/admin/fileadmin.py` & `django-filer-3.0.0rc2/filer/admin/fileadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/admin/folderadmin.py` & `django-filer-3.0.0rc2/filer/admin/folderadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/admin/forms.py` & `django-filer-3.0.0rc2/filer/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/admin/imageadmin.py` & `django-filer-3.0.0rc2/filer/admin/imageadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/admin/patched/admin_utils.py` & `django-filer-3.0.0rc2/filer/admin/patched/admin_utils.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/admin/permissionadmin.py` & `django-filer-3.0.0rc2/filer/admin/permissionadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/admin/permissions.py` & `django-filer-3.0.0rc2/filer/admin/permissions.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/admin/tools.py` & `django-filer-3.0.0rc2/filer/admin/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/admin/views.py` & `django-filer-3.0.0rc2/filer/admin/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/apps.py` & `django-filer-3.0.0rc2/filer/apps.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/contrib/django_cms/cms_toolbars.py` & `django-filer-3.0.0rc2/filer/contrib/django_cms/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/fields/file.py` & `django-filer-3.0.0rc2/filer/fields/file.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/fields/folder.py` & `django-filer-3.0.0rc2/filer/fields/folder.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/fields/multistorage_file.py` & `django-filer-3.0.0rc2/filer/fields/multistorage_file.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/ar/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/ar/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/bg/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/ca/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/ca/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/cs/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/cs/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/de/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/de/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/en/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/en/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/es/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/es/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/et/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/et/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/eu/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/eu/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/fa/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/fi/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/fi/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/fr/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/fr/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/gl/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/gl/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/he/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/he/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/hr/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/hr/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/hu/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/hu/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/it/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/it/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/ja/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/ja_JP/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/lt/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/lt/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/lt_LT/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/lt_LT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/lt_LT/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/lt_LT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/nb/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/nb/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/nl_NL/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/nl_NL/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/nn/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/nn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/nn/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/nn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/pl/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/pl/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/pt/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/pt_BR/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/pt_BR/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/ru/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/ru/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/sk/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/tr/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/tr/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/vi_VN/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/vi_VN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/zh/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/zh-Hans/LC_MESSAGES/django.mo` & `django-filer-3.0.0rc2/filer/locale/zh-Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/zh-Hans/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/zh-Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/zh_CN/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/locale/zh_TW/LC_MESSAGES/django.po` & `django-filer-3.0.0rc2/filer/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/management/commands/filer_check.py` & `django-filer-3.0.0rc2/filer/management/commands/filer_check.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/management/commands/generate_thumbnails.py` & `django-filer-3.0.0rc2/filer/management/commands/generate_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/management/commands/import_files.py` & `django-filer-3.0.0rc2/filer/management/commands/import_files.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0001_initial.py` & `django-filer-3.0.0rc2/filer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0002_auto_20150606_2003.py` & `django-filer-3.0.0rc2/filer/migrations/0002_auto_20150606_2003.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0003_thumbnailoption.py` & `django-filer-3.0.0rc2/filer/migrations/0003_thumbnailoption.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0005_auto_20160623_1425.py` & `django-filer-3.0.0rc2/filer/migrations/0005_auto_20160623_1425.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0006_auto_20160623_1627.py` & `django-filer-3.0.0rc2/filer/migrations/0006_auto_20160623_1627.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0008_auto_20171117_1313.py` & `django-filer-3.0.0rc2/filer/migrations/0008_auto_20171117_1313.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0010_auto_20180414_2058.py` & `django-filer-3.0.0rc2/filer/migrations/0010_auto_20180414_2058.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0011_auto_20190418_0137.py` & `django-filer-3.0.0rc2/filer/migrations/0011_auto_20190418_0137.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0012_file_mime_type.py` & `django-filer-3.0.0rc2/filer/migrations/0012_file_mime_type.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0013_image_width_height_to_float.py` & `django-filer-3.0.0rc2/filer/migrations/0013_image_width_height_to_float.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0014_folder_permission_choices.py` & `django-filer-3.0.0rc2/filer/migrations/0014_folder_permission_choices.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py` & `django-filer-3.0.0rc2/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py` & `django-filer-3.0.0rc2/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/models/abstract.py` & `django-filer-3.0.0rc2/filer/models/abstract.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/models/clipboardmodels.py` & `django-filer-3.0.0rc2/filer/models/clipboardmodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/models/filemodels.py` & `django-filer-3.0.0rc2/filer/models/filemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/models/foldermodels.py` & `django-filer-3.0.0rc2/filer/models/foldermodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/models/imagemodels.py` & `django-filer-3.0.0rc2/filer/models/imagemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/models/mixins.py` & `django-filer-3.0.0rc2/filer/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/models/thumbnailoptionmodels.py` & `django-filer-3.0.0rc2/filer/models/thumbnailoptionmodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/models/tools.py` & `django-filer-3.0.0rc2/filer/models/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/models/virtualitems.py` & `django-filer-3.0.0rc2/filer/models/virtualitems.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/server/backends/base.py` & `django-filer-3.0.0rc2/filer/server/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/server/backends/default.py` & `django-filer-3.0.0rc2/filer/server/backends/default.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/server/backends/nginx.py` & `django-filer-3.0.0rc2/filer/server/backends/nginx.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/server/backends/xsendfile.py` & `django-filer-3.0.0rc2/filer/server/backends/xsendfile.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/server/views.py` & `django-filer-3.0.0rc2/filer/server/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/settings.py` & `django-filer-3.0.0rc2/filer/settings.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/css/admin_filer.cms.icons.css` & `django-filer-3.0.0rc2/filer/static/filer/css/admin_filer.cms.icons.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/css/admin_filer.css` & `django-filer-3.0.0rc2/filer/static/filer/css/admin_filer.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/css/admin_filer.fa.icons.css` & `django-filer-3.0.0rc2/filer/static/filer/css/admin_filer.fa.icons.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/css/maps/admin_filer.css.map` & `django-filer-3.0.0rc2/filer/static/filer/css/maps/admin_filer.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/FontAwesome.otf` & `django-filer-3.0.0rc2/filer/static/filer/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.eot` & `django-filer-3.0.0rc2/filer/static/filer/fonts/django-filer-iconfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.svg` & `django-filer-3.0.0rc2/filer/static/filer/fonts/django-filer-iconfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.ttf` & `django-filer-3.0.0rc2/filer/static/filer/fonts/django-filer-iconfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.woff` & `django-filer-3.0.0rc2/filer/static/filer/fonts/django-filer-iconfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/django-filer-iconfont.woff2` & `django-filer-3.0.0rc2/filer/static/filer/fonts/django-filer-iconfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.eot` & `django-filer-3.0.0rc2/filer/static/filer/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.svg` & `django-filer-3.0.0rc2/filer/static/filer/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.ttf` & `django-filer-3.0.0rc2/filer/static/filer/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.woff` & `django-filer-3.0.0rc2/filer/static/filer/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/fontawesome-webfont.woff2` & `django-filer-3.0.0rc2/filer/static/filer/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/src/arrow-down.svg` & `django-filer-3.0.0rc2/filer/static/filer/fonts/src/arrow-down.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/src/link.svg` & `django-filer-3.0.0rc2/filer/static/filer/fonts/src/link.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/src/move-to-folder.svg` & `django-filer-3.0.0rc2/filer/static/filer/fonts/src/move-to-folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/src/th-list.svg` & `django-filer-3.0.0rc2/filer/static/filer/fonts/src/th-list.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/fonts/src/upload.svg` & `django-filer-3.0.0rc2/filer/static/filer/fonts/src/upload.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/cloud-up.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/cloud-up.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/file-audio.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/file-empty.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/file-font.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/file-missing.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/file-pdf.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/file-picture.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/file-unknown.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/file-video.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/file-zip.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/folder-dropdown.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/folder-dropdown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/folder-root.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/folder-root.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/folder-unfiled.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/folder-unfiled.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/icons/folder.svg` & `django-filer-3.0.0rc2/filer/static/filer/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/img/icon_changelink.gif` & `django-filer-3.0.0rc2/filer/static/filer/img/icon_changelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/img/icon_deletelink.gif` & `django-filer-3.0.0rc2/filer/static/filer/img/icon_deletelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/img/loading_animation.gif` & `django-filer-3.0.0rc2/filer/static/filer/img/loading_animation.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/img/upload_button.png` & `django-filer-3.0.0rc2/filer/static/filer/img/upload_button.png`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/copy-move-files.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/copy-move-files.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/dropdown-menu.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/dropdown-menu.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/dropzone.init.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/dropzone.init.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/filer_popup_response.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/filer_popup_response.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/focal-point.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/focal-point.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/popup_handling.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/popup_handling.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/table-dropzone.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/table-dropzone.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/toggler.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/toggler.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/tooltip.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/tooltip.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/upload-button.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/upload-button.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/addons/widget.js` & `django-filer-3.0.0rc2/filer/static/filer/js/addons/widget.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/base.js` & `django-filer-3.0.0rc2/filer/static/filer/js/base.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/libs/class.min.js` & `django-filer-3.0.0rc2/filer/static/filer/js/libs/class.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/libs/dropzone.min.js` & `django-filer-3.0.0rc2/filer/static/filer/js/libs/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/libs/fileuploader.min.js` & `django-filer-3.0.0rc2/filer/static/filer/js/libs/fileuploader.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery-ui.min.js` & `django-filer-3.0.0rc2/filer/static/filer/js/libs/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery.cookie.min.js` & `django-filer-3.0.0rc2/filer/static/filer/js/libs/jquery.cookie.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/libs/jquery.min.js` & `django-filer-3.0.0rc2/filer/static/filer/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/static/filer/js/libs/mediator.min.js` & `django-filer-3.0.0rc2/filer/static/filer/js/libs/mediator.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/storage.py` & `django-filer-3.0.0rc2/filer/storage.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/actions.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/actions.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/base_site.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/base_site.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/breadcrumbs.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/change_form.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/delete_selected_files_confirmation.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/delete_selected_files_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/file/change_form.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/file/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/change_form.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/folder/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_copy_destination.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/folder/choose_copy_destination.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_images_resize_options.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/folder/choose_images_resize_options.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_move_destination.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/folder/choose_move_destination.html`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 {% block breadcrumbs %}
     {% include "admin/filer/breadcrumbs.html" %}
 {% endblock %}
 
 {% block extrastyle %}
     {{ block.super }}
     <link rel="stylesheet" type="text/css" href="{% static 'admin/css/forms.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% static 'filer/css/admin_filer.icons.css' %}">
     <link rel="stylesheet" type="text/css" href="{% static 'filer/css/admin_filer.css' %}">
 {% endblock %}
 
 {% block extrahead %}
     {{ block.super }}
     <script src="{% static 'admin/js/jquery.init.js' %}"></script>
     <script type="text/javascript">
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 {% extends "admin/base_site.html" %} {% load i18n static %} {% block
 breadcrumbs %} {% include "admin/filer/breadcrumbs.html" %} {% endblock %} {%
 block extrastyle %} {{ block.super }}
 
-
  {% endblock %} {% block extrahead %} {{ block.super }}
  {% endblock %} {% block content %} {% if perms_lacking %}
 {% blocktrans %}Your account doesn't have permissions to move all of the
 selected files and/or folders.{% endblocktrans %}
 {%_translate_"Take_me_back"_%}
 {% else %} {% if not destination_folders %}
 {% blocktrans %}There are no destination folders available.{% endblocktrans %}
```

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/choose_rename_format.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/folder/choose_rename_format.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_listing.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/folder/directory_listing.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_table_list.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/folder/directory_table_list.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/directory_thumbnail_list.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/folder/directory_thumbnail_list.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/folder/new_folder_form.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/folder/new_folder_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/image/change_form.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/image/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/templatetags/file_icon.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/templatetags/file_icon.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/tools/clipboard/clipboard.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/tools/clipboard/clipboard.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/tools/detail_info.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/tools/detail_info.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/tools/search_form.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/tools/search_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/widgets/admin_file.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/widgets/admin_file.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templates/admin/filer/widgets/admin_folder.html` & `django-filer-3.0.0rc2/filer/templates/admin/filer/widgets/admin_folder.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templatetags/filer_admin_tags.py` & `django-filer-3.0.0rc2/filer/templatetags/filer_admin_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templatetags/filer_image_tags.py` & `django-filer-3.0.0rc2/filer/templatetags/filer_image_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/templatetags/filer_tags.py` & `django-filer-3.0.0rc2/filer/templatetags/filer_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/thumbnail_processors.py` & `django-filer-3.0.0rc2/filer/thumbnail_processors.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/utils/compatibility.py` & `django-filer-3.0.0rc2/filer/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/utils/filer_easy_thumbnails.py` & `django-filer-3.0.0rc2/filer/utils/filer_easy_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/utils/files.py` & `django-filer-3.0.0rc2/filer/utils/files.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/utils/generate_filename.py` & `django-filer-3.0.0rc2/filer/utils/generate_filename.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/utils/loader.py` & `django-filer-3.0.0rc2/filer/utils/loader.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/utils/pil_exif.py` & `django-filer-3.0.0rc2/filer/utils/pil_exif.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/utils/recursive_dictionary.py` & `django-filer-3.0.0rc2/filer/utils/recursive_dictionary.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/utils/zip.py` & `django-filer-3.0.0rc2/filer/utils/zip.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/filer/validation.py` & `django-filer-3.0.0rc2/filer/validation.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/setup.cfg` & `django-filer-3.0.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-filer-3.0.0rc1/setup.py` & `django-filer-3.0.0rc2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,16 +28,14 @@
     'Framework :: Django :: 3.0',
     'Framework :: Django :: 3.1',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
     'Framework :: Django :: 4.2',
     'Framework :: Django CMS',
-    'Framework :: Django CMS :: 3.6',
-    'Framework :: Django CMS :: 3.7',
     'Framework :: Django CMS :: 3.8',
     'Framework :: Django CMS :: 3.9',
     'Framework :: Django CMS :: 3.10',
     'Framework :: Django CMS :: 3.11',
     'Framework :: Django CMS :: 4.0',
     'Framework :: Django CMS :: 4.1',
     'Topic :: Internet :: WWW/HTTP',
@@ -59,11 +57,11 @@
     description='A file management application for django that makes handling '
                 'of files and images a breeze.',
     long_description=open('README.rst').read(),
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=REQUIREMENTS,
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     classifiers=CLASSIFIERS,
     test_suite='tests.settings.run',
 )
```

