# Comparing `tmp/django-tables2-2.5.3.tar.gz` & `tmp/django-tables2-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tables2-2.5.3.tar", last modified: Mon Mar  6 06:18:48 2023, max compression
+gzip compressed data, was "django-tables2-2.6.0.tar", last modified: Tue Jun 27 09:41:05 2023, max compression
```

## Comparing `django-tables2-2.5.3.tar` & `django-tables2-2.6.0.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.373144 django-tables2-2.5.3/
--rw-r--r--   0 jieter     (501) staff       (20)    42506 2023-03-06 06:18:14.000000 django-tables2-2.5.3/CHANGELOG.md
--rw-r--r--   0 jieter     (501) staff       (20)     1655 2022-07-28 14:35:10.000000 django-tables2-2.5.3/LICENSE
--rw-r--r--   0 jieter     (501) staff       (20)      327 2022-07-28 14:35:10.000000 django-tables2-2.5.3/MANIFEST.in
--rw-r--r--   0 jieter     (501) staff       (20)     4315 2023-03-06 06:18:48.372965 django-tables2-2.5.3/PKG-INFO
--rw-r--r--   0 jieter     (501) staff       (20)     2533 2022-07-28 14:35:10.000000 django-tables2-2.5.3/README.md
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.354816 django-tables2-2.5.3/django_tables2/
--rw-r--r--   0 jieter     (501) staff       (20)      946 2023-03-06 06:18:14.000000 django-tables2-2.5.3/django_tables2/__init__.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.358279 django-tables2-2.5.3/django_tables2/columns/
--rw-r--r--   0 jieter     (501) staff       (20)      887 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/columns/__init__.py
--rw-r--r--   0 jieter     (501) staff       (20)    32631 2022-12-27 10:35:42.000000 django-tables2-2.5.3/django_tables2/columns/base.py
--rw-r--r--   0 jieter     (501) staff       (20)     2481 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/columns/booleancolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)     3203 2022-12-27 10:35:42.000000 django-tables2-2.5.3/django_tables2/columns/checkboxcolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)      947 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/columns/datecolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)      992 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/columns/datetimecolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)     1092 2022-12-27 10:35:42.000000 django-tables2-2.5.3/django_tables2/columns/emailcolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)     2948 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/columns/filecolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)     2028 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/columns/jsoncolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)     6118 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/columns/linkcolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)     3638 2022-12-27 10:35:42.000000 django-tables2-2.5.3/django_tables2/columns/manytomanycolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)     3061 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/columns/templatecolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)      822 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/columns/timecolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)      926 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/columns/urlcolumn.py
--rw-r--r--   0 jieter     (501) staff       (20)     2459 2023-02-07 07:45:01.000000 django-tables2-2.5.3/django_tables2/config.py
--rw-r--r--   0 jieter     (501) staff       (20)     7492 2022-12-27 10:35:42.000000 django-tables2-2.5.3/django_tables2/data.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.358714 django-tables2-2.5.3/django_tables2/export/
--rw-r--r--   0 jieter     (501) staff       (20)      105 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/export/__init__.py
--rw-r--r--   0 jieter     (501) staff       (20)     3424 2022-12-27 10:35:42.000000 django-tables2-2.5.3/django_tables2/export/export.py
--rw-r--r--   0 jieter     (501) staff       (20)     2420 2022-12-27 10:35:42.000000 django-tables2-2.5.3/django_tables2/export/views.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.350767 django-tables2-2.5.3/django_tables2/locale/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.348585 django-tables2-2.5.3/django_tables2/locale/cs/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.359018 django-tables2-2.5.3/django_tables2/locale/cs/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      533 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      998 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.348699 django-tables2-2.5.3/django_tables2/locale/de/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.359312 django-tables2-2.5.3/django_tables2/locale/de/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      497 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      964 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.348816 django-tables2-2.5.3/django_tables2/locale/el/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.359621 django-tables2-2.5.3/django_tables2/locale/el/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      449 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      848 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.348932 django-tables2-2.5.3/django_tables2/locale/en/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.359911 django-tables2-2.5.3/django_tables2/locale/en/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      434 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      812 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.349044 django-tables2-2.5.3/django_tables2/locale/es/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.360222 django-tables2-2.5.3/django_tables2/locale/es/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      463 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      812 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.349163 django-tables2-2.5.3/django_tables2/locale/fa/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.360536 django-tables2-2.5.3/django_tables2/locale/fa/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      672 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)     1104 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.349279 django-tables2-2.5.3/django_tables2/locale/fr/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.360817 django-tables2-2.5.3/django_tables2/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      493 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      961 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.349389 django-tables2-2.5.3/django_tables2/locale/hu/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.361195 django-tables2-2.5.3/django_tables2/locale/hu/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      496 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      849 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.349504 django-tables2-2.5.3/django_tables2/locale/it/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.361635 django-tables2-2.5.3/django_tables2/locale/it/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      492 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      843 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.349637 django-tables2-2.5.3/django_tables2/locale/lt/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.361960 django-tables2-2.5.3/django_tables2/locale/lt/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      511 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)     1463 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.349768 django-tables2-2.5.3/django_tables2/locale/nb/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.362289 django-tables2-2.5.3/django_tables2/locale/nb/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      446 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      794 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.349880 django-tables2-2.5.3/django_tables2/locale/nl/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.362642 django-tables2-2.5.3/django_tables2/locale/nl/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      505 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      856 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.349995 django-tables2-2.5.3/django_tables2/locale/pl/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.362954 django-tables2-2.5.3/django_tables2/locale/pl/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      594 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)     1064 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.350115 django-tables2-2.5.3/django_tables2/locale/pt_BR/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.363264 django-tables2-2.5.3/django_tables2/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      527 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      952 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.350236 django-tables2-2.5.3/django_tables2/locale/pt_PT/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.363559 django-tables2-2.5.3/django_tables2/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      464 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      828 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.350356 django-tables2-2.5.3/django_tables2/locale/ru/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.363879 django-tables2-2.5.3/django_tables2/locale/ru/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      582 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)     1093 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.350485 django-tables2-2.5.3/django_tables2/locale/sv/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.364483 django-tables2-2.5.3/django_tables2/locale/sv/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      460 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      809 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.350654 django-tables2-2.5.3/django_tables2/locale/uk/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.364832 django-tables2-2.5.3/django_tables2/locale/uk/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      603 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)     1085 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.350818 django-tables2-2.5.3/django_tables2/locale/zh_Hans/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.365186 django-tables2-2.5.3/django_tables2/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 jieter     (501) staff       (20)      421 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 jieter     (501) staff       (20)      914 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 jieter     (501) staff       (20)     4288 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/paginators.py
--rw-r--r--   0 jieter     (501) staff       (20)    11295 2023-02-07 07:49:17.000000 django-tables2-2.5.3/django_tables2/rows.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.350986 django-tables2-2.5.3/django_tables2/static/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.365370 django-tables2-2.5.3/django_tables2/static/django_tables2/
--rw-r--r--   0 jieter     (501) staff       (20)      167 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/bootstrap.css
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.351154 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.351314 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.365548 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/css/
--rw-r--r--   0 jieter     (501) staff       (20)     2774 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/css/screen.css
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.367035 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/img/
--rw-r--r--   0 jieter     (501) staff       (20)      216 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/img/arrow-active-down.png
--rw-r--r--   0 jieter     (501) staff       (20)      202 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/img/arrow-active-up.png
--rw-r--r--   0 jieter     (501) staff       (20)      246 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/img/arrow-inactive-down.png
--rw-r--r--   0 jieter     (501) staff       (20)      210 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/img/arrow-inactive-up.png
--rw-r--r--   0 jieter     (501) staff       (20)      176 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/img/false.gif
--rw-r--r--   0 jieter     (501) staff       (20)      130 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/img/header-bg.png
--rw-r--r--   0 jieter     (501) staff       (20)      509 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/img/missing.png
--rw-r--r--   0 jieter     (501) staff       (20)      273 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/img/pagination-bg.gif
--rw-r--r--   0 jieter     (501) staff       (20)      299 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/img/true.gif
--rw-r--r--   0 jieter     (501) staff       (20)    27221 2023-02-07 07:49:17.000000 django-tables2-2.5.3/django_tables2/tables.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.351492 django-tables2-2.5.3/django_tables2/templates/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.368806 django-tables2-2.5.3/django_tables2/templates/django_tables2/
--rw-r--r--   0 jieter     (501) staff       (20)      379 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/templates/django_tables2/bootstrap-responsive.html
--rw-r--r--   0 jieter     (501) staff       (20)     4479 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/templates/django_tables2/bootstrap.html
--rw-r--r--   0 jieter     (501) staff       (20)      380 2022-12-27 07:03:41.000000 django-tables2-2.5.3/django_tables2/templates/django_tables2/bootstrap4-responsive.html
--rw-r--r--   0 jieter     (501) staff       (20)     4260 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/templates/django_tables2/bootstrap4.html
--rw-r--r--   0 jieter     (501) staff       (20)      314 2023-03-05 14:02:11.000000 django-tables2-2.5.3/django_tables2/templates/django_tables2/bootstrap5-responsive.html
--rw-r--r--   0 jieter     (501) staff       (20)     4272 2022-12-27 07:47:24.000000 django-tables2-2.5.3/django_tables2/templates/django_tables2/bootstrap5.html
--rw-r--r--   0 jieter     (501) staff       (20)     4788 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/templates/django_tables2/semantic.html
--rw-r--r--   0 jieter     (501) staff       (20)     4201 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/templates/django_tables2/table.html
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.369304 django-tables2-2.5.3/django_tables2/templatetags/
--rw-r--r--   0 jieter     (501) staff       (20)        0 2022-07-28 14:35:10.000000 django-tables2-2.5.3/django_tables2/templatetags/__init__.py
--rw-r--r--   0 jieter     (501) staff       (20)     8658 2022-12-27 10:35:42.000000 django-tables2-2.5.3/django_tables2/templatetags/django_tables2.py
--rw-r--r--   0 jieter     (501) staff       (20)    19582 2023-02-07 07:49:17.000000 django-tables2-2.5.3/django_tables2/utils.py
--rw-r--r--   0 jieter     (501) staff       (20)     8490 2023-03-05 14:01:05.000000 django-tables2-2.5.3/django_tables2/views.py
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.355562 django-tables2-2.5.3/django_tables2.egg-info/
--rw-r--r--   0 jieter     (501) staff       (20)     4315 2023-03-06 06:18:48.000000 django-tables2-2.5.3/django_tables2.egg-info/PKG-INFO
--rw-r--r--   0 jieter     (501) staff       (20)     4783 2023-03-06 06:18:48.000000 django-tables2-2.5.3/django_tables2.egg-info/SOURCES.txt
--rw-r--r--   0 jieter     (501) staff       (20)        1 2023-03-06 06:18:48.000000 django-tables2-2.5.3/django_tables2.egg-info/dependency_links.txt
--rw-r--r--   0 jieter     (501) staff       (20)       29 2023-03-06 06:18:48.000000 django-tables2-2.5.3/django_tables2.egg-info/requires.txt
--rw-r--r--   0 jieter     (501) staff       (20)       15 2023-03-06 06:18:48.000000 django-tables2-2.5.3/django_tables2.egg-info/top_level.txt
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.351796 django-tables2-2.5.3/example/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.351731 django-tables2-2.5.3/example/app/
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.369559 django-tables2-2.5.3/example/app/fixtures/
--rw-r--r--   0 jieter     (501) staff       (20)      809 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/app/fixtures/initial_data.json
-drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-03-06 06:18:48.372681 django-tables2-2.5.3/example/templates/
--rw-r--r--   0 jieter     (501) staff       (20)      617 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/base.html
--rw-r--r--   0 jieter     (501) staff       (20)     1137 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/bootstrap4_template.html
--rw-r--r--   0 jieter     (501) staff       (20)     1172 2022-12-27 07:47:24.000000 django-tables2-2.5.3/example/templates/bootstrap5_template.html
--rw-r--r--   0 jieter     (501) staff       (20)     1662 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/bootstrap_template.html
--rw-r--r--   0 jieter     (501) staff       (20)      811 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/checkbox_example.html
--rw-r--r--   0 jieter     (501) staff       (20)      253 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/class_based.html
--rw-r--r--   0 jieter     (501) staff       (20)      211 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/country_detail.html
--rw-r--r--   0 jieter     (501) staff       (20)      189 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/extended_table.html
--rw-r--r--   0 jieter     (501) staff       (20)     2947 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/index.html
--rw-r--r--   0 jieter     (501) staff       (20)      766 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/multiTable.html
--rw-r--r--   0 jieter     (501) staff       (20)     2443 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/multiple.html
--rw-r--r--   0 jieter     (501) staff       (20)      203 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/person_detail.html
--rw-r--r--   0 jieter     (501) staff       (20)      702 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/semantic_template.html
--rw-r--r--   0 jieter     (501) staff       (20)      323 2022-07-28 14:35:10.000000 django-tables2-2.5.3/example/templates/tutorial.html
--rw-r--r--   0 jieter     (501) staff       (20)       31 2022-07-28 14:35:10.000000 django-tables2-2.5.3/pyproject.toml
--rw-r--r--   0 jieter     (501) staff       (20)       38 2023-03-06 06:18:48.373201 django-tables2-2.5.3/setup.cfg
--rwxr-xr-x   0 jieter     (501) staff       (20)     1737 2022-12-27 10:36:51.000000 django-tables2-2.5.3/setup.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.433876 django-tables2-2.6.0/
+-rw-r--r--   0 jieter     (501) staff       (20)    42825 2023-06-27 09:40:40.000000 django-tables2-2.6.0/CHANGELOG.md
+-rw-r--r--   0 jieter     (501) staff       (20)     1655 2022-07-28 14:35:10.000000 django-tables2-2.6.0/LICENSE
+-rw-r--r--   0 jieter     (501) staff       (20)      327 2022-07-28 14:35:10.000000 django-tables2-2.6.0/MANIFEST.in
+-rw-r--r--   0 jieter     (501) staff       (20)     4265 2023-06-27 09:41:05.433701 django-tables2-2.6.0/PKG-INFO
+-rw-r--r--   0 jieter     (501) staff       (20)     2533 2022-07-28 14:35:10.000000 django-tables2-2.6.0/README.md
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.417298 django-tables2-2.6.0/django_tables2/
+-rw-r--r--   0 jieter     (501) staff       (20)      946 2023-06-27 09:40:40.000000 django-tables2-2.6.0/django_tables2/__init__.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.420014 django-tables2-2.6.0/django_tables2/columns/
+-rw-r--r--   0 jieter     (501) staff       (20)      887 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/columns/__init__.py
+-rw-r--r--   0 jieter     (501) staff       (20)    32631 2022-12-27 10:35:42.000000 django-tables2-2.6.0/django_tables2/columns/base.py
+-rw-r--r--   0 jieter     (501) staff       (20)     2481 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/columns/booleancolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)     3203 2022-12-27 10:35:42.000000 django-tables2-2.6.0/django_tables2/columns/checkboxcolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)      947 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/columns/datecolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)      992 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/columns/datetimecolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)     1092 2022-12-27 10:35:42.000000 django-tables2-2.6.0/django_tables2/columns/emailcolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)     2948 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/columns/filecolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)     2028 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/columns/jsoncolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)     6118 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/columns/linkcolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)     3638 2022-12-27 10:35:42.000000 django-tables2-2.6.0/django_tables2/columns/manytomanycolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)     3061 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/columns/templatecolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)      822 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/columns/timecolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)      926 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/columns/urlcolumn.py
+-rw-r--r--   0 jieter     (501) staff       (20)     2459 2023-02-07 07:45:01.000000 django-tables2-2.6.0/django_tables2/config.py
+-rw-r--r--   0 jieter     (501) staff       (20)     7492 2022-12-27 10:35:42.000000 django-tables2-2.6.0/django_tables2/data.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.420715 django-tables2-2.6.0/django_tables2/export/
+-rw-r--r--   0 jieter     (501) staff       (20)      105 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/export/__init__.py
+-rw-r--r--   0 jieter     (501) staff       (20)     3424 2022-12-27 10:35:42.000000 django-tables2-2.6.0/django_tables2/export/export.py
+-rw-r--r--   0 jieter     (501) staff       (20)     2420 2022-12-27 10:35:42.000000 django-tables2-2.6.0/django_tables2/export/views.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.413653 django-tables2-2.6.0/django_tables2/locale/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.411488 django-tables2-2.6.0/django_tables2/locale/cs/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.421258 django-tables2-2.6.0/django_tables2/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      533 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      998 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.411605 django-tables2-2.6.0/django_tables2/locale/de/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.421833 django-tables2-2.6.0/django_tables2/locale/de/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      497 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      964 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.411720 django-tables2-2.6.0/django_tables2/locale/el/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.422141 django-tables2-2.6.0/django_tables2/locale/el/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      449 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      848 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.411831 django-tables2-2.6.0/django_tables2/locale/en/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.422426 django-tables2-2.6.0/django_tables2/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      434 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      812 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.411947 django-tables2-2.6.0/django_tables2/locale/es/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.422721 django-tables2-2.6.0/django_tables2/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      463 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      812 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.412064 django-tables2-2.6.0/django_tables2/locale/fa/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.423129 django-tables2-2.6.0/django_tables2/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      672 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)     1104 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.412177 django-tables2-2.6.0/django_tables2/locale/fr/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.423408 django-tables2-2.6.0/django_tables2/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      493 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      961 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.412287 django-tables2-2.6.0/django_tables2/locale/hu/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.423789 django-tables2-2.6.0/django_tables2/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      496 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      849 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.412407 django-tables2-2.6.0/django_tables2/locale/it/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.424184 django-tables2-2.6.0/django_tables2/locale/it/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      492 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      843 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.412551 django-tables2-2.6.0/django_tables2/locale/lt/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.424462 django-tables2-2.6.0/django_tables2/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      511 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)     1463 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.412668 django-tables2-2.6.0/django_tables2/locale/nb/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.424837 django-tables2-2.6.0/django_tables2/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      446 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      794 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.412783 django-tables2-2.6.0/django_tables2/locale/nl/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.425123 django-tables2-2.6.0/django_tables2/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      505 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      856 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.412901 django-tables2-2.6.0/django_tables2/locale/pl/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.425427 django-tables2-2.6.0/django_tables2/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      594 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)     1064 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.413025 django-tables2-2.6.0/django_tables2/locale/pt_BR/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.425736 django-tables2-2.6.0/django_tables2/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      527 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      952 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.413144 django-tables2-2.6.0/django_tables2/locale/pt_PT/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.426211 django-tables2-2.6.0/django_tables2/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      464 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      828 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.413255 django-tables2-2.6.0/django_tables2/locale/ru/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.426497 django-tables2-2.6.0/django_tables2/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      582 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)     1093 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.413375 django-tables2-2.6.0/django_tables2/locale/sv/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.426766 django-tables2-2.6.0/django_tables2/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      460 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      809 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.413543 django-tables2-2.6.0/django_tables2/locale/uk/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.427044 django-tables2-2.6.0/django_tables2/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      603 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)     1085 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.413717 django-tables2-2.6.0/django_tables2/locale/zh_Hans/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.427401 django-tables2-2.6.0/django_tables2/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 jieter     (501) staff       (20)      421 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 jieter     (501) staff       (20)      914 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 jieter     (501) staff       (20)     4288 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/paginators.py
+-rw-r--r--   0 jieter     (501) staff       (20)    11295 2023-02-07 07:49:17.000000 django-tables2-2.6.0/django_tables2/rows.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.413882 django-tables2-2.6.0/django_tables2/static/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.427538 django-tables2-2.6.0/django_tables2/static/django_tables2/
+-rw-r--r--   0 jieter     (501) staff       (20)      167 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/bootstrap.css
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.414060 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.414234 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.427693 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/css/
+-rw-r--r--   0 jieter     (501) staff       (20)     2774 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/css/screen.css
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.429079 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/img/
+-rw-r--r--   0 jieter     (501) staff       (20)      216 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/img/arrow-active-down.png
+-rw-r--r--   0 jieter     (501) staff       (20)      202 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/img/arrow-active-up.png
+-rw-r--r--   0 jieter     (501) staff       (20)      246 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/img/arrow-inactive-down.png
+-rw-r--r--   0 jieter     (501) staff       (20)      210 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/img/arrow-inactive-up.png
+-rw-r--r--   0 jieter     (501) staff       (20)      176 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/img/false.gif
+-rw-r--r--   0 jieter     (501) staff       (20)      130 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/img/header-bg.png
+-rw-r--r--   0 jieter     (501) staff       (20)      509 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/img/missing.png
+-rw-r--r--   0 jieter     (501) staff       (20)      273 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/img/pagination-bg.gif
+-rw-r--r--   0 jieter     (501) staff       (20)      299 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/img/true.gif
+-rw-r--r--   0 jieter     (501) staff       (20)    27221 2023-02-07 07:49:17.000000 django-tables2-2.6.0/django_tables2/tables.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.414399 django-tables2-2.6.0/django_tables2/templates/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.430582 django-tables2-2.6.0/django_tables2/templates/django_tables2/
+-rw-r--r--   0 jieter     (501) staff       (20)      379 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/templates/django_tables2/bootstrap-responsive.html
+-rw-r--r--   0 jieter     (501) staff       (20)     4479 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/templates/django_tables2/bootstrap.html
+-rw-r--r--   0 jieter     (501) staff       (20)      380 2022-12-27 07:03:41.000000 django-tables2-2.6.0/django_tables2/templates/django_tables2/bootstrap4-responsive.html
+-rw-r--r--   0 jieter     (501) staff       (20)     4260 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/templates/django_tables2/bootstrap4.html
+-rw-r--r--   0 jieter     (501) staff       (20)      314 2023-04-03 08:52:34.000000 django-tables2-2.6.0/django_tables2/templates/django_tables2/bootstrap5-responsive.html
+-rw-r--r--   0 jieter     (501) staff       (20)     4272 2022-12-27 07:47:24.000000 django-tables2-2.6.0/django_tables2/templates/django_tables2/bootstrap5.html
+-rw-r--r--   0 jieter     (501) staff       (20)     4788 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/templates/django_tables2/semantic.html
+-rw-r--r--   0 jieter     (501) staff       (20)     4201 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/templates/django_tables2/table.html
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.430836 django-tables2-2.6.0/django_tables2/templatetags/
+-rw-r--r--   0 jieter     (501) staff       (20)        0 2022-07-28 14:35:10.000000 django-tables2-2.6.0/django_tables2/templatetags/__init__.py
+-rw-r--r--   0 jieter     (501) staff       (20)     8658 2022-12-27 10:35:42.000000 django-tables2-2.6.0/django_tables2/templatetags/django_tables2.py
+-rw-r--r--   0 jieter     (501) staff       (20)    19582 2023-02-07 07:49:17.000000 django-tables2-2.6.0/django_tables2/utils.py
+-rw-r--r--   0 jieter     (501) staff       (20)     8490 2023-03-05 14:01:05.000000 django-tables2-2.6.0/django_tables2/views.py
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.418058 django-tables2-2.6.0/django_tables2.egg-info/
+-rw-r--r--   0 jieter     (501) staff       (20)     4265 2023-06-27 09:41:05.000000 django-tables2-2.6.0/django_tables2.egg-info/PKG-INFO
+-rw-r--r--   0 jieter     (501) staff       (20)     4783 2023-06-27 09:41:05.000000 django-tables2-2.6.0/django_tables2.egg-info/SOURCES.txt
+-rw-r--r--   0 jieter     (501) staff       (20)        1 2023-06-27 09:41:05.000000 django-tables2-2.6.0/django_tables2.egg-info/dependency_links.txt
+-rw-r--r--   0 jieter     (501) staff       (20)       29 2023-06-27 09:41:05.000000 django-tables2-2.6.0/django_tables2.egg-info/requires.txt
+-rw-r--r--   0 jieter     (501) staff       (20)       15 2023-06-27 09:41:05.000000 django-tables2-2.6.0/django_tables2.egg-info/top_level.txt
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.414755 django-tables2-2.6.0/example/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.414666 django-tables2-2.6.0/example/app/
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.430991 django-tables2-2.6.0/example/app/fixtures/
+-rw-r--r--   0 jieter     (501) staff       (20)      809 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/app/fixtures/initial_data.json
+drwxr-xr-x   0 jieter     (501) staff       (20)        0 2023-06-27 09:41:05.433445 django-tables2-2.6.0/example/templates/
+-rw-r--r--   0 jieter     (501) staff       (20)      617 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/base.html
+-rw-r--r--   0 jieter     (501) staff       (20)     1137 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/bootstrap4_template.html
+-rw-r--r--   0 jieter     (501) staff       (20)     1172 2022-12-27 07:47:24.000000 django-tables2-2.6.0/example/templates/bootstrap5_template.html
+-rw-r--r--   0 jieter     (501) staff       (20)     1662 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/bootstrap_template.html
+-rw-r--r--   0 jieter     (501) staff       (20)      811 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/checkbox_example.html
+-rw-r--r--   0 jieter     (501) staff       (20)      253 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/class_based.html
+-rw-r--r--   0 jieter     (501) staff       (20)      211 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/country_detail.html
+-rw-r--r--   0 jieter     (501) staff       (20)      189 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/extended_table.html
+-rw-r--r--   0 jieter     (501) staff       (20)     2947 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/index.html
+-rw-r--r--   0 jieter     (501) staff       (20)      766 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/multiTable.html
+-rw-r--r--   0 jieter     (501) staff       (20)     2443 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/multiple.html
+-rw-r--r--   0 jieter     (501) staff       (20)      203 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/person_detail.html
+-rw-r--r--   0 jieter     (501) staff       (20)      702 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/semantic_template.html
+-rw-r--r--   0 jieter     (501) staff       (20)      323 2022-07-28 14:35:10.000000 django-tables2-2.6.0/example/templates/tutorial.html
+-rw-r--r--   0 jieter     (501) staff       (20)       31 2022-07-28 14:35:10.000000 django-tables2-2.6.0/pyproject.toml
+-rw-r--r--   0 jieter     (501) staff       (20)       38 2023-06-27 09:41:05.433929 django-tables2-2.6.0/setup.cfg
+-rwxr-xr-x   0 jieter     (501) staff       (20)     1708 2023-06-27 09:35:46.000000 django-tables2-2.6.0/setup.py
```

### Comparing `django-tables2-2.5.3/CHANGELOG.md` & `django-tables2-2.6.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Change log
 
+## 2.6.0 (2023-06-27)
+- Fix bootstrap5-responsive template to extend bootstrap5 ([#909](https://github.com/jieter/django-tables2/pull/909)) by [@mschoettle](https://github.com/mschoettle)
+- Add support for django 4.2
+- Drop python 3.7 and django 4.0 support ([#920](https://github.com/jieter/django-tables2/pull/920))
+
 ## 2.5.3 (2023-03-05)
  - Assign request to table before anything else in `RequestConfig.configure()` ([#888](https://github.com/jieter/django-tables2/pull/888)) fixes: [#865](https://github.com/jieter/django-tables2/issues/865)
  - Add type hints to get_context_data ([#895](https://github.com/jieter/django-tables2/pull/895)) by [@mschoettle](https://github.com/mschoettle)
  - Document hidden table attributes setting ([#897](https://github.com/jieter/django-tables2/pull/897)) by [@mschoettle](https://github.com/mschoettle)
  - Fix building of the docs ([#900](https://github.com/jieter/django-tables2/pull/900)) by [@danielroseman](https://github.com/danielroseman)
  - Add template bootstrap5-responsive.html ([#896](https://github.com/jieter/django-tables2/pull/896)) by [@mschoettle](https://github.com/mschoettle)
```

### Comparing `django-tables2-2.5.3/LICENSE` & `django-tables2-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/PKG-INFO` & `django-tables2-2.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tables2
-Version: 2.5.3
+Version: 2.6.0
 Summary: Table/data-grid framework for Django
 Home-page: https://github.com/jieter/django-tables2/
 Author: Bradley Ayers
 Author-email: bradley.ayers@gmail.com
 License: Simplified BSD
 Description: # django-tables2 - An app for creating HTML tables
         
@@ -78,23 +78,22 @@
         Check out the [documentation](https://django-tables2.readthedocs.io/en/latest/) for more details.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
```

### Comparing `django-tables2-2.5.3/README.md` & `django-tables2-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/__init__.py` & `django-tables2-2.6.0/django_tables2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 from .config import RequestConfig
 from .paginators import LazyPaginator
 from .tables import Table, table_factory
 from .utils import A
 from .views import MultiTableMixin, SingleTableMixin, SingleTableView
 
-__version__ = "2.5.3"
+__version__ = "2.6.0"
 
 __all__ = (
     "Table",
     "table_factory",
     "BooleanColumn",
     "Column",
     "CheckBoxColumn",
```

### Comparing `django-tables2-2.5.3/django_tables2/columns/__init__.py` & `django-tables2-2.6.0/django_tables2/columns/__init__.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/base.py` & `django-tables2-2.6.0/django_tables2/columns/base.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/booleancolumn.py` & `django-tables2-2.6.0/django_tables2/columns/booleancolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/checkboxcolumn.py` & `django-tables2-2.6.0/django_tables2/columns/checkboxcolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/datecolumn.py` & `django-tables2-2.6.0/django_tables2/columns/datecolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/datetimecolumn.py` & `django-tables2-2.6.0/django_tables2/columns/datetimecolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/emailcolumn.py` & `django-tables2-2.6.0/django_tables2/columns/emailcolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/filecolumn.py` & `django-tables2-2.6.0/django_tables2/columns/filecolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/jsoncolumn.py` & `django-tables2-2.6.0/django_tables2/columns/jsoncolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/linkcolumn.py` & `django-tables2-2.6.0/django_tables2/columns/linkcolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/manytomanycolumn.py` & `django-tables2-2.6.0/django_tables2/columns/manytomanycolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/templatecolumn.py` & `django-tables2-2.6.0/django_tables2/columns/templatecolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/timecolumn.py` & `django-tables2-2.6.0/django_tables2/columns/timecolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/columns/urlcolumn.py` & `django-tables2-2.6.0/django_tables2/columns/urlcolumn.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/config.py` & `django-tables2-2.6.0/django_tables2/config.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/data.py` & `django-tables2-2.6.0/django_tables2/data.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/export/export.py` & `django-tables2-2.6.0/django_tables2/export/export.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/export/views.py` & `django-tables2-2.6.0/django_tables2/export/views.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/cs/LC_MESSAGES/django.mo` & `django-tables2-2.6.0/django_tables2/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/cs/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/de/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/el/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/en/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/es/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/fa/LC_MESSAGES/django.mo` & `django-tables2-2.6.0/django_tables2/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/fa/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/fr/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/hu/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/it/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/lt/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/nb/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/nl/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/pl/LC_MESSAGES/django.mo` & `django-tables2-2.6.0/django_tables2/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/pl/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/pt_BR/LC_MESSAGES/django.mo` & `django-tables2-2.6.0/django_tables2/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/pt_BR/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/pt_PT/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/ru/LC_MESSAGES/django.mo` & `django-tables2-2.6.0/django_tables2/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/ru/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/sv/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/uk/LC_MESSAGES/django.mo` & `django-tables2-2.6.0/django_tables2/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/uk/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/locale/zh_Hans/LC_MESSAGES/django.po` & `django-tables2-2.6.0/django_tables2/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/paginators.py` & `django-tables2-2.6.0/django_tables2/paginators.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/rows.py` & `django-tables2-2.6.0/django_tables2/rows.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/static/django_tables2/themes/paleblue/css/screen.css` & `django-tables2-2.6.0/django_tables2/static/django_tables2/themes/paleblue/css/screen.css`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/tables.py` & `django-tables2-2.6.0/django_tables2/tables.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/templates/django_tables2/bootstrap.html` & `django-tables2-2.6.0/django_tables2/templates/django_tables2/bootstrap.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/templates/django_tables2/bootstrap4.html` & `django-tables2-2.6.0/django_tables2/templates/django_tables2/bootstrap4.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/templates/django_tables2/bootstrap5.html` & `django-tables2-2.6.0/django_tables2/templates/django_tables2/bootstrap5.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/templates/django_tables2/semantic.html` & `django-tables2-2.6.0/django_tables2/templates/django_tables2/semantic.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/templates/django_tables2/table.html` & `django-tables2-2.6.0/django_tables2/templates/django_tables2/table.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/templatetags/django_tables2.py` & `django-tables2-2.6.0/django_tables2/templatetags/django_tables2.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/utils.py` & `django-tables2-2.6.0/django_tables2/utils.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2/views.py` & `django-tables2-2.6.0/django_tables2/views.py`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/django_tables2.egg-info/PKG-INFO` & `django-tables2-2.6.0/django_tables2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tables2
-Version: 2.5.3
+Version: 2.6.0
 Summary: Table/data-grid framework for Django
 Home-page: https://github.com/jieter/django-tables2/
 Author: Bradley Ayers
 Author-email: bradley.ayers@gmail.com
 License: Simplified BSD
 Description: # django-tables2 - An app for creating HTML tables
         
@@ -78,23 +78,22 @@
         Check out the [documentation](https://django-tables2.readthedocs.io/en/latest/) for more details.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
```

### Comparing `django-tables2-2.5.3/django_tables2.egg-info/SOURCES.txt` & `django-tables2-2.6.0/django_tables2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/example/app/fixtures/initial_data.json` & `django-tables2-2.6.0/example/app/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/example/templates/base.html` & `django-tables2-2.6.0/example/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/example/templates/bootstrap4_template.html` & `django-tables2-2.6.0/example/templates/bootstrap4_template.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/example/templates/bootstrap5_template.html` & `django-tables2-2.6.0/example/templates/bootstrap5_template.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/example/templates/bootstrap_template.html` & `django-tables2-2.6.0/example/templates/bootstrap_template.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/example/templates/checkbox_example.html` & `django-tables2-2.6.0/example/templates/checkbox_example.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/example/templates/index.html` & `django-tables2-2.6.0/example/templates/index.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/example/templates/multiTable.html` & `django-tables2-2.6.0/example/templates/multiTable.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/example/templates/multiple.html` & `django-tables2-2.6.0/example/templates/multiple.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/example/templates/semantic_template.html` & `django-tables2-2.6.0/example/templates/semantic_template.html`

 * *Files identical despite different names*

### Comparing `django-tables2-2.5.3/setup.py` & `django-tables2-2.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,24 +21,23 @@
     include_package_data=True,  # declarations in MANIFEST.in
     install_requires=["Django>=3.2"],
     extras_require={"tablib": ["tablib"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
-        "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 3.2",  # Until April 2024
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development :: Libraries",
     ],
```

