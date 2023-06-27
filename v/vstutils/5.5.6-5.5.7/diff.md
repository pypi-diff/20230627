# Comparing `tmp/vstutils-5.5.6.tar.gz` & `tmp/vstutils-5.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.5.6.tar", last modified: Sat Jun 24 04:51:54 2023, max compression
+gzip compressed data, was "vstutils-5.5.7.tar", last modified: Tue Jun 27 04:49:46 2023, max compression
```

## Comparing `vstutils-5.5.6.tar` & `vstutils-5.5.7.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.271229 vstutils-5.5.6/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.5.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.5.6/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.5.6/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4427 2023-06-24 04:51:54.271229 vstutils-5.5.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2389 2023-06-22 02:12:27.000000 vstutils-5.5.6/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-01 04:31:00.000000 vstutils-5.5.6/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.5.6/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.5.6/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-13 04:11:10.000000 vstutils-5.5.6/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-07 23:11:01.000000 vstutils-5.5.6/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-20 04:07:06.000000 vstutils-5.5.6/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-14 22:04:13.000000 vstutils-5.5.6/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-23 05:26:08.000000 vstutils-5.5.6/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-06-24 04:51:54.275230 vstutils-5.5.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16558 2023-06-21 00:04:50.000000 vstutils-5.5.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.215229 vstutils-5.5.6/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-24 04:44:36.000000 vstutils-5.5.6/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.227229 vstutils-5.5.6/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-14 22:04:13.000000 vstutils-5.5.6/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.5.6/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:54.000000 vstutils-5.5.6/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    29374 2023-06-14 22:04:13.000000 vstutils-5.5.6/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:43.000000 vstutils-5.5.6/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.5.6/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-14 22:04:13.000000 vstutils-5.5.6/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:43.000000 vstutils-5.5.6/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    13792 2023-06-15 03:16:13.000000 vstutils-5.5.6/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:17:53.000000 vstutils-5.5.6/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2990 2023-06-24 04:44:36.000000 vstutils-5.5.6/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.227229 vstutils-5.5.6/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-14 22:04:13.000000 vstutils-5.5.6/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.5.6/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.5.6/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.231229 vstutils-5.5.6/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.5.6/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.5.6/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    28314 2023-06-22 02:12:27.000000 vstutils-5.5.6/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)     9995 2023-06-15 03:16:13.000000 vstutils-5.5.6/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-14 22:04:13.000000 vstutils-5.5.6/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:17:53.000000 vstutils-5.5.6/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5660 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3351 2023-06-24 04:44:36.000000 vstutils-5.5.6/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1872 2023-06-23 05:26:08.000000 vstutils-5.5.6/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:04.000000 vstutils-5.5.6/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.5.6/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.5.6/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.207229 vstutils-5.5.6/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.231229 vstutils-5.5.6/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.231229 vstutils-5.5.6/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.5.6/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.231229 vstutils-5.5.6/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3487 2023-06-23 05:26:08.000000 vstutils-5.5.6/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.5.6/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.5.6/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.231229 vstutils-5.5.6/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.235229 vstutils-5.5.6/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7832 2023-03-16 06:05:23.000000 vstutils-5.5.6/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.5.6/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.5.6/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.5.6/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10689 2023-06-07 00:01:28.000000 vstutils-5.5.6/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.235229 vstutils-5.5.6/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:54.000000 vstutils-5.5.6/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25943 2023-06-14 22:04:13.000000 vstutils-5.5.6/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2023-06-24 04:44:36.000000 vstutils-5.5.6/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:54.000000 vstutils-5.5.6/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.5.6/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:17:53.000000 vstutils-5.5.6/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    55954 2023-06-23 05:26:08.000000 vstutils-5.5.6/vstutils/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:31:00.000000 vstutils-5.5.6/vstutils/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.207229 vstutils-5.5.6/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.247229 vstutils-5.5.6/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126387 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      321 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38355 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    73740 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536116 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    87131 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355745 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)  1026670 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/957.js
--rw-r--r--   0 root         (0) root         (0)     2030 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/957.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    81737 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)   303699 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      748 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3621 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   435118 2023-06-24 04:51:53.000000 vstutils-5.5.6/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.247229 vstutils-5.5.6/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.247229 vstutils-5.5.6/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5182 2023-05-29 08:17:53.000000 vstutils-5.5.6/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.251229 vstutils-5.5.6/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.5.6/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.5.6/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.5.6/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.5.6/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.251229 vstutils-5.5.6/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.5.6/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.5.6/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.251229 vstutils-5.5.6/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.251229 vstutils-5.5.6/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.5.6/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.255229 vstutils-5.5.6/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.259230 vstutils-5.5.6/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.263229 vstutils-5.5.6/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.263229 vstutils-5.5.6/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.263229 vstutils-5.5.6/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.263229 vstutils-5.5.6/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.5.6/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.267229 vstutils-5.5.6/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.5.6/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.267229 vstutils-5.5.6/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.271229 vstutils-5.5.6/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.271229 vstutils-5.5.6/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.271229 vstutils-5.5.6/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.5.6/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.5.6/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    18153 2023-06-14 22:04:13.000000 vstutils-5.5.6/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.271229 vstutils-5.5.6/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.5.6/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.5.6/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.5.6/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.5.6/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    47153 2023-06-14 22:04:13.000000 vstutils-5.5.6/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.5.6/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.5.6/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 04:51:54.219229 vstutils-5.5.6/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4427 2023-06-24 04:51:54.000000 vstutils-5.5.6/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7664 2023-06-24 04:51:54.000000 vstutils-5.5.6/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-24 04:51:54.000000 vstutils-5.5.6/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-24 04:51:54.000000 vstutils-5.5.6/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 04:51:54.000000 vstutils-5.5.6/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1794 2023-06-24 04:51:54.000000 vstutils-5.5.6/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-24 04:51:54.000000 vstutils-5.5.6/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.922981 vstutils-5.5.7/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.5.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.5.7/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.5.7/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-06-27 04:49:46.922981 vstutils-5.5.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2389 2023-06-22 02:12:27.000000 vstutils-5.5.7/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-01 04:31:00.000000 vstutils-5.5.7/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.5.7/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.5.7/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-13 04:11:10.000000 vstutils-5.5.7/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-07 23:11:01.000000 vstutils-5.5.7/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-20 04:07:06.000000 vstutils-5.5.7/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-14 22:04:13.000000 vstutils-5.5.7/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-23 05:26:08.000000 vstutils-5.5.7/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-06-27 04:49:46.922981 vstutils-5.5.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16558 2023-06-21 00:04:50.000000 vstutils-5.5.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.882980 vstutils-5.5.7/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-27 04:42:54.000000 vstutils-5.5.7/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.890980 vstutils-5.5.7/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-14 22:04:13.000000 vstutils-5.5.7/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.5.7/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:54.000000 vstutils-5.5.7/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    29374 2023-06-14 22:04:13.000000 vstutils-5.5.7/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:43.000000 vstutils-5.5.7/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.5.7/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-14 22:04:13.000000 vstutils-5.5.7/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:43.000000 vstutils-5.5.7/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    13792 2023-06-15 03:16:13.000000 vstutils-5.5.7/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:17:53.000000 vstutils-5.5.7/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-27 04:42:54.000000 vstutils-5.5.7/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.890980 vstutils-5.5.7/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-14 22:04:13.000000 vstutils-5.5.7/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.5.7/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.5.7/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.890980 vstutils-5.5.7/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.5.7/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.5.7/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    28314 2023-06-22 02:12:27.000000 vstutils-5.5.7/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     9995 2023-06-15 03:16:13.000000 vstutils-5.5.7/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-14 22:04:13.000000 vstutils-5.5.7/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:17:53.000000 vstutils-5.5.7/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5667 2023-06-27 04:42:54.000000 vstutils-5.5.7/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3351 2023-06-24 04:44:36.000000 vstutils-5.5.7/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1872 2023-06-23 05:26:08.000000 vstutils-5.5.7/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:04.000000 vstutils-5.5.7/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.5.7/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.5.7/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.874980 vstutils-5.5.7/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.894980 vstutils-5.5.7/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.894980 vstutils-5.5.7/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.5.7/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.894980 vstutils-5.5.7/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3487 2023-06-23 05:26:08.000000 vstutils-5.5.7/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.5.7/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.5.7/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.894980 vstutils-5.5.7/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.894980 vstutils-5.5.7/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2023-06-27 04:42:54.000000 vstutils-5.5.7/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.5.7/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.5.7/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.5.7/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10689 2023-06-07 00:01:28.000000 vstutils-5.5.7/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.898980 vstutils-5.5.7/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:54.000000 vstutils-5.5.7/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25943 2023-06-14 22:04:13.000000 vstutils-5.5.7/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2023-06-24 04:44:36.000000 vstutils-5.5.7/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:54.000000 vstutils-5.5.7/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.5.7/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:17:53.000000 vstutils-5.5.7/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    55979 2023-06-27 04:42:54.000000 vstutils-5.5.7/vstutils/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:31:00.000000 vstutils-5.5.7/vstutils/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.874980 vstutils-5.5.7/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.906980 vstutils-5.5.7/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126387 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38355 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    73740 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536116 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    87131 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355745 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)  1026670 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/957.js
+-rw-r--r--   0 root         (0) root         (0)     2030 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/957.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    81737 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)   303699 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      748 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   435118 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.906980 vstutils-5.5.7/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.906980 vstutils-5.5.7/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5182 2023-05-29 08:17:53.000000 vstutils-5.5.7/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.910980 vstutils-5.5.7/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.5.7/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.5.7/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.5.7/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.5.7/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.910980 vstutils-5.5.7/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.5.7/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.5.7/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.910980 vstutils-5.5.7/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.910980 vstutils-5.5.7/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.5.7/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.910980 vstutils-5.5.7/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.914981 vstutils-5.5.7/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.914981 vstutils-5.5.7/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.914981 vstutils-5.5.7/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.918980 vstutils-5.5.7/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.918980 vstutils-5.5.7/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.5.7/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.918980 vstutils-5.5.7/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.5.7/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.918980 vstutils-5.5.7/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.918980 vstutils-5.5.7/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.918980 vstutils-5.5.7/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.918980 vstutils-5.5.7/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.5.7/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.5.7/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18153 2023-06-14 22:04:13.000000 vstutils-5.5.7/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.922981 vstutils-5.5.7/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.5.7/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.5.7/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.5.7/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.5.7/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    47153 2023-06-14 22:04:13.000000 vstutils-5.5.7/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.5.7/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.5.7/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 04:49:46.882980 vstutils-5.5.7/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7664 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-27 04:49:46.000000 vstutils-5.5.7/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.5.6/LICENSE` & `vstutils-5.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/MANIFEST.in` & `vstutils-5.5.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/NOTICE` & `vstutils-5.5.7/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/PKG-INFO` & `vstutils-5.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.5.6
+Version: 5.5.7
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.5.6/README.rst` & `vstutils-5.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/setup.cfg` & `vstutils-5.5.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/setup.py` & `vstutils-5.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/actions.py` & `vstutils-5.5.7/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/admin.py` & `vstutils-5.5.7/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/auth.py` & `vstutils-5.5.7/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/base.py` & `vstutils-5.5.7/vstutils/api/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/decorators.py` & `vstutils-5.5.7/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/decorators.pyi` & `vstutils-5.5.7/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/doc_generator.py` & `vstutils-5.5.7/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/endpoint.py` & `vstutils-5.5.7/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/fields.py` & `vstutils-5.5.7/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/filter_backends.py` & `vstutils-5.5.7/vstutils/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/filters.py` & `vstutils-5.5.7/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/health.py` & `vstutils-5.5.7/vstutils/api/health.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,52 @@
-from typing import Text, Iterable, Callable, Dict, Tuple
+from typing import Dict, Tuple, ClassVar, Callable
+from functools import wraps
 
 from django.db import connections
-from rest_framework import status as st
+from rest_framework import status as st, request as req
 
 from ..utils import BaseVstObject, import_class
 
 
-class BaseBackend(BaseVstObject):
-    __slots__ = ('__health_methods',)
-
-    def __init__(self):
-        self.__health_methods = {}  # typing: Dict
-
-    def __health_method_wrapper(self, method: Callable):
+def health_wrapper(method):
+    @wraps(method)
+    def wrapper(self):
         try:
-            return method() or 'ok', st.HTTP_200_OK
+            return method(self) or 'ok', st.HTTP_200_OK
         except BaseException as exception:
             code = getattr(exception, 'status', st.HTTP_500_INTERNAL_SERVER_ERROR)
             return str(exception), code
 
-    def __health_types_filter(self, attr_name: Text) -> bool:
-        return attr_name.startswith('check_health_')
+    return wrapper
+
 
-    def __get_health_methods_iterator(self) -> Iterable[Tuple[Text, Callable]]:
-        for method_name in filter(self.__health_types_filter, dir(self)):
-            method = getattr(self, method_name)
-            if callable(method):
-                yield method_name.replace('check_health_', '', 1), method
+class HealthBackendMeta(type):
+    def __new__(mcs, name, bases, attrs):
+        backend = super().__new__(mcs, name, bases, attrs)
+        checks = {}
+        for attr_name, attr in attrs.items():
+            if attr_name.startswith('check_health_') and callable(attr):
+                checks[attr_name.replace('check_health_', '', 1)] = health_wrapper(attr)
+        if checks:
+            original_checks = getattr(backend, 'health_checks', {})
+            backend.health_checks = {**original_checks, **checks}
+        return backend
+
+
+class BaseBackend(BaseVstObject, metaclass=HealthBackendMeta):
+    __slots__ = ('request',)
+    health_checks: ClassVar[Dict[str, Callable]]
+
+    def __init__(self, request: req.Request):
+        self.request = request
 
     def get(self) -> Tuple[Dict, int]:
-        if not self.__health_methods:
-            self.__health_methods = dict(self.__get_health_methods_iterator())
         result, status = {}, st.HTTP_200_OK
-        for key, method in self.__health_methods.items():
-            method_result, method_status = self.__health_method_wrapper(method)
-            result[key] = method_result
+        for key, method in self.health_checks.items():
+            result[key], method_status = method(self)
             if method_status > status:
                 status = method_status
         return result, status
 
 
 class DefaultBackend(BaseBackend):
     db_check_sql = 'SELECT 1;'
@@ -76,7 +84,12 @@
             celery_app = import_class(
                 self.get_django_settings('WORKER_OPTIONS')['app'].replace(':', '.')
             )
         except ImportError:  # nocv
             return "disabled"
         else:
             return self.celery_check(celery_app)
+
+    def check_health_session_engine(self):
+        # pylint: disable=pointless-statement
+        tuple(self.request.session.values())
+        self.request.user.is_active
```

### Comparing `vstutils-5.5.6/vstutils/api/meta.py` & `vstutils-5.5.7/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/metrics.py` & `vstutils-5.5.7/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/migrations/0001_initial.py` & `vstutils-5.5.7/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.5.7/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.5.7/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.5.7/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.5.7/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.5.7/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/models.py` & `vstutils-5.5.7/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/pagination.py` & `vstutils-5.5.7/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/parsers.py` & `vstutils-5.5.7/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/permissions.py` & `vstutils-5.5.7/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/renderers.py` & `vstutils-5.5.7/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/responses.py` & `vstutils-5.5.7/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/responses.pyi` & `vstutils-5.5.7/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/routers.py` & `vstutils-5.5.7/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/routers.pyi` & `vstutils-5.5.7/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/schema/generators.py` & `vstutils-5.5.7/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/schema/info.py` & `vstutils-5.5.7/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/schema/inspectors.py` & `vstutils-5.5.7/vstutils/api/schema/inspectors.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/schema/schema.py` & `vstutils-5.5.7/vstutils/api/schema/schema.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/serializers.py` & `vstutils-5.5.7/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/throttling.py` & `vstutils-5.5.7/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/validators.py` & `vstutils-5.5.7/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/api/views.py` & `vstutils-5.5.7/vstutils/api/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,18 +107,18 @@
     }
 
 
 class HealthView(base.ListNonModelViewSet):
     permission_classes = (rest_permissions.AllowAny,)
     authentication_classes = ()
     throttle_classes = (HealthThrottle,)
-    health_backend = import_class(settings.HEALTH_BACKEND_CLASS)()
+    health_backend = import_class(settings.HEALTH_BACKEND_CLASS)
 
     def list(self, request, *args, **kwargs):
-        return responses.HTTP_200_OK(*self.health_backend.get())
+        return responses.HTTP_200_OK(*self.health_backend(request).get())
 
 
 class MetricsView(base.ListNonModelViewSet):
     permission_classes = (rest_permissions.AllowAny,)
     authentication_classes = ()
     throttle_classes = (MetricsThrottle,)
     metrics_backend = import_class(settings.METRICS_BACKEND_CLASS)()
```

### Comparing `vstutils-5.5.6/vstutils/asgi.py` & `vstutils-5.5.7/vstutils/asgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/asgi_worker.py` & `vstutils-5.5.7/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/auth.py` & `vstutils-5.5.7/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/auth.pyi` & `vstutils-5.5.7/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/celery_beat_scheduler.py` & `vstutils-5.5.7/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.5.7/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/environment.py` & `vstutils-5.5.7/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/exceptions.py` & `vstutils-5.5.7/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/gui/context.py` & `vstutils-5.5.7/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/gui/forms.py` & `vstutils-5.5.7/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/gui/pwa_manifest.py` & `vstutils-5.5.7/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/gui/views.py` & `vstutils-5.5.7/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/ldap_utils.py` & `vstutils-5.5.7/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/management/commands/_base.py` & `vstutils-5.5.7/vstutils/management/commands/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from collections import OrderedDict
 
 from django.conf import settings
 from django.core.management.base import (
     BaseCommand as _BaseCommand,
     CommandError as CmdError,
 )
-from configparserc.config import ConfigParserC
 from vstutils.utils import Lock
 
 logger = logging.getLogger(settings.VST_PROJECT)
 logger_lib = logging.getLogger(settings.VST_PROJECT_LIB)
 
 
 class BaseCommand(_BaseCommand):
@@ -117,29 +116,28 @@
         super().handle(*args, **options)
         self.prefix = self._settings('VST_PROJECT_LIB', 'vstutils').upper()
         self.project_name = self._settings('VST_PROJECT', 'vstutils')
 
         logger.debug(f'Prefix={self.prefix} | Project={self.project_name}')
 
         self.env = os.environ.copy()
-        config = self.prepare_config()
-        self.env[self._settings('CONFIG_ENV_DATA_NAME')] = config.generate_config_string()
+        self.config = self.prepare_config()
         self.env[f'{settings.ENV_NAME}_DAEMON'] = 'false'
         default_envs = {
             'UWSGI_PROCESSES': 'UWSGI_WORKERS',
             'UWSGI_THREADS': 'UWSGI_THREADS'
         }
         for key in default_envs:  # pylint: disable=consider-using-dict-items
             value = os.environ.get(f"{self.prefix}_{key}", '')
             if value:
                 self.env[default_envs[key]] = value  # nocv
 
-        if config['main']['debug'] or self._settings('TESTS_RUN', False):
+        if self.config['main']['debug'] or self._settings('TESTS_RUN', False):
             logger.debug(f'Env:\n{json.dumps(self.env, indent=4)}')
-            logger.debug(f'Config:\n{self.env[self._settings("CONFIG_ENV_DATA_NAME")]}')
+            logger.debug(f'Config:\n{self.config.generate_config_string()}')
 
     @property
     def databases_to_migrate(self):
         allowed_databases = ('default',) + tuple(set(getattr(settings, 'DOCKER_DATABASES_TO_MIGRATE', ())))
         for db in settings.DATABASES.keys():
             if db in allowed_databases:
                 yield db
@@ -181,28 +179,17 @@
                 time.sleep(options.get('attempts_timeout', 1))
             else:
                 success = True
                 break
         return success, error
 
     def prepare_config(self):
-        # pylint: disable=too-many-locals,too-many-branches,too-many-statements
-        prefix = self.prefix
-
         # Start configuring config file
-        self.config = ConfigParserC(
-            format_kwargs=self._settings('KWARGS', {}),
-            format_exclude_sections=('uwsgi',)
-        )
-        config = self.config
-        config.parse_text(settings.CONFIG.generate_config_string())
-
-        # Set log level
-        self.log_level = os.getenv(f'{prefix}_LOG_LEVEL', 'WARNING')
+        config = settings.CONFIG
 
         # Set secret key
         os.environ.setdefault('SECRET_KEY', 'DISABLE')
         if os.environ['SECRET_KEY'] != 'DISABLE':  # nocv
-            with open(f'/etc/{prefix.lower()}/secret', 'w', encoding='utf-8') as secretfile:
+            with open(f'/etc/{self.prefix.lower()}/secret', 'w', encoding='utf-8') as secretfile:
                 secretfile.write(os.environ['SECRET_KEY'])
 
         return config
```

### Comparing `vstutils-5.5.6/vstutils/management/commands/celery_inspect.py` & `vstutils-5.5.7/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/management/commands/dockerrun.py` & `vstutils-5.5.7/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/management/commands/newproject.py` & `vstutils-5.5.7/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/management/commands/run_task.py` & `vstutils-5.5.7/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/management/commands/runrpc.py` & `vstutils-5.5.7/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/management/commands/runserver.py` & `vstutils-5.5.7/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/management/commands/web.py` & `vstutils-5.5.7/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/middleware.py` & `vstutils-5.5.7/vstutils/middleware.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/models/__init__.py` & `vstutils-5.5.7/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/models/base.py` & `vstutils-5.5.7/vstutils/models/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/models/cent_notify.py` & `vstutils-5.5.7/vstutils/models/cent_notify.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/models/custom_model.py` & `vstutils-5.5.7/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/models/custom_model.pyi` & `vstutils-5.5.7/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/models/decorators.py` & `vstutils-5.5.7/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/models/fields.py` & `vstutils-5.5.7/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/models/queryset.py` & `vstutils-5.5.7/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/settings.ini` & `vstutils-5.5.7/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/settings.py` & `vstutils-5.5.7/vstutils/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,18 +114,23 @@
     def convert(self, value: _t.Any) -> _t.SupportsFloat:
         return float(value)
 
 
 class LocationsType(cconfig.ListType):
     def convert(self, value: _t.Any) -> _t.Union[_t.Iterable, _t.Text]:  # type: ignore
         result: _t.Iterable[_t.Text] = super().convert(value)
-        if any(filter(lambda x: x.startswith('redis'), result)):  # type: ignore
+        if len(result) > 1:  # type: ignore
             return result
         return value
 
+    def str_convert(self, value):
+        if isinstance(value, str):
+            return value
+        return super().str_convert(value)
+
 
 ConfigBoolType = cconfig.BoolType()
 ConfigIntType = cconfig.IntType()
 ConfigFloatType = FloatType()
 ConfigIntSecondsType = cconfig.IntSecondsType()
 ConfigListType = cconfig.ListType()
 ConfigStringType = cconfig.StrType()
@@ -261,27 +266,31 @@
 class CacheOptionsSection(BackendSection):
     parent: BaseAppendSection
     types_map = {
         'binary': ConfigBoolType,
         'no_delay': ConfigBoolType,
         'ignore_exc': ConfigBoolType,
         'ignore_exceptions': ConfigBoolType,
+        'socket_keepalive': ConfigBoolType,
+        'retry_on_timeout': ConfigBoolType,
         'use_pooling': ConfigBoolType,
         'close_connection': ConfigBoolType,
+        'single_connection_client': ConfigBoolType,
         'max_entries': ConfigIntType,
         'cull_frequency': ConfigIntType,
         'max_pool_size': ConfigIntType,
         'pickle_version': ConfigIntType,
         'socket_connect_timeout': ConfigIntSecondsType,
         'socket_timeout': ConfigIntSecondsType,
+        'health_check_interval': ConfigIntSecondsType,
     }
 
     def key_handler_to_all(self, key):
         backend = self.parent['backend']
-        if backend.split('.')[-1] in ('PyLibMCCache', 'PyMemcacheCache'):
+        if key not in {'max_entries', 'cull_frequency', }:
             return key
         return super(CacheOptionsSection, self).key_handler_to_all(key)
 
 
 class SentinelsSection(cconfig.Section):
     def all(self) -> _t.List[_t.Tuple[_t.Text, _t.SupportsInt]]:  # type: ignore
         return list((k, int(v)) for k, v in super().all().items())
@@ -397,15 +406,14 @@
 
     def key_handler_to_all(self, key):
         key_uppercase = super().key_handler_to_all(key).upper()
         if key_uppercase != 'GZIP_CONTENT_TYPES':
             return f'AWS_{key_uppercase}'
         return key_uppercase
 
-environ.environ.REDIS_DRIVER = 'django.core.cache.backends.redis.RedisCache'
 
 class DjangoEnv(environ.Env):
     BOOLEAN_TRUE_STRINGS = environ.Env.BOOLEAN_TRUE_STRINGS + ('enable', 'ENABLE')
 
 
 env = DjangoEnv(
     # set casting, default value
@@ -962,17 +970,14 @@
 CACHES: SIMPLE_OBJECT_SETTINGS_TYPE = {
     'default': default_cache,
     "locks": config['locks'].all() or default_cache,
     "session": session_cache,
     "etag": etag_cache,
 }
 
-if any([True for c in CACHES.values() if 'OPTIONS' in c and c['OPTIONS'].get('SENTINELS')]):
-    DJANGO_REDIS_CONNECTION_FACTORY = 'django_redis.pool.SentinelConnectionFactory'
-
 
 # E-Mail settings
 # https://docs.djangoproject.com/en/3.2/ref/settings/#email-host
 ##############################################################
 mail = config['mail']
 EMAIL_HOST_USER = mail["user"]
```

### Comparing `vstutils-5.5.6/vstutils/static/bundle/281.chunk.js` & `vstutils-5.5.7/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/296.chunk.js` & `vstutils-5.5.7/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/345.chunk.js` & `vstutils-5.5.7/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/368.chunk.js` & `vstutils-5.5.7/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/421.js` & `vstutils-5.5.7/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.5.7/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/618.js` & `vstutils-5.5.7/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/683.chunk.js` & `vstutils-5.5.7/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/686.js` & `vstutils-5.5.7/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/742.chunk.js` & `vstutils-5.5.7/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.5.7/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/755.js` & `vstutils-5.5.7/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/826.chunk.js` & `vstutils-5.5.7/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.5.7/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/844.js` & `vstutils-5.5.7/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/957.js` & `vstutils-5.5.7/vstutils/static/bundle/957.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/957.js.LICENSE.txt` & `vstutils-5.5.7/vstutils/static/bundle/957.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/app_loader.js` & `vstutils-5.5.7/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/base.js` & `vstutils-5.5.7/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.5.7/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.5.7/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/output.json` & `vstutils-5.5.7/vstutils/static/bundle/output.json`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/spa.js` & `vstutils-5.5.7/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/bundle/vstutils.js` & `vstutils-5.5.7/vstutils/static/bundle/vstutils.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static/img/anonymous.png` & `vstutils-5.5.7/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/static_files.py` & `vstutils-5.5.7/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/tasks.py` & `vstutils-5.5.7/vstutils/tasks.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/auth/base.html` & `vstutils-5.5.7/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/auth/language_selector.html` & `vstutils-5.5.7/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/auth/tfa.html` & `vstutils-5.5.7/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/base.html` & `vstutils-5.5.7/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/gui/base.html` & `vstutils-5.5.7/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/gui/offline.html` & `vstutils-5.5.7/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/gui/service-worker.js` & `vstutils-5.5.7/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.5.7/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.5.7/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/newproject/package.json.template` & `vstutils-5.5.7/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.5.7/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.5.7/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/newproject/setup.py.template` & `vstutils-5.5.7/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/newproject/test.py.template` & `vstutils-5.5.7/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.5.7/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.5.7/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.5.7/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/registration/confirm_email.html` & `vstutils-5.5.7/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.5.7/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.5.7/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/registration/user_registration.html` & `vstutils-5.5.7/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/rest_framework/admin.html` & `vstutils-5.5.7/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.5.7/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.5.7/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templatetags/request_static.py` & `vstutils-5.5.7/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templatetags/translation.py` & `vstutils-5.5.7/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.5.7/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.5.7/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/templatetags/vstconfigs.py` & `vstutils-5.5.7/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/tests.py` & `vstutils-5.5.7/vstutils/tests.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/tools.py` & `vstutils-5.5.7/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/translations/cn.py` & `vstutils-5.5.7/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/translations/ru.py` & `vstutils-5.5.7/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/translations/vi.py` & `vstutils-5.5.7/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/urls.py` & `vstutils-5.5.7/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/utils.py` & `vstutils-5.5.7/vstutils/utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/web.ini` & `vstutils-5.5.7/vstutils/web.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils/wsgi.py` & `vstutils-5.5.7/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils.egg-info/PKG-INFO` & `vstutils-5.5.7/vstutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.5.6
+Version: 5.5.7
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.5.6/vstutils.egg-info/SOURCES.txt` & `vstutils-5.5.7/vstutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.6/vstutils.egg-info/requires.txt` & `vstutils-5.5.7/vstutils.egg-info/requires.txt`

 * *Files identical despite different names*

