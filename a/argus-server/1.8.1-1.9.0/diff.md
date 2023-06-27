# Comparing `tmp/argus-server-1.8.1.tar.gz` & `tmp/argus-server-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argus-server-1.8.1.tar", last modified: Fri Oct 28 11:51:24 2022, max compression
+gzip compressed data, was "argus-server-1.9.0.tar", last modified: Tue Nov  8 11:47:47 2022, max compression
```

## Comparing `argus-server-1.8.1.tar` & `argus-server-1.9.0.tar`

### file list

```diff
@@ -1,251 +1,255 @@
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.521973 argus-server-1.8.1/
--rw-rw-r--   0 hm        (1000) hm        (1000)      292 2022-10-06 09:21:59.000000 argus-server-1.8.1/.git-blame-ignore-revs
--rw-rw-r--   0 hm        (1000) hm        (1000)       34 2022-10-03 07:28:14.000000 argus-server-1.8.1/.gitattributes
--rw-rw-r--   0 hm        (1000) hm        (1000)     4158 2022-10-03 07:28:14.000000 argus-server-1.8.1/.gitignore
--rw-rw-r--   0 hm        (1000) hm        (1000)      530 2022-10-06 09:21:59.000000 argus-server-1.8.1/.pre-commit-config.yaml
--rw-rw-r--   0 hm        (1000) hm        (1000)     4268 2022-10-28 11:46:31.000000 argus-server-1.8.1/CHANGELOG.md
--rw-rw-r--   0 hm        (1000) hm        (1000)      579 2022-10-03 07:28:14.000000 argus-server-1.8.1/CONTRIBUTORS.md
--rw-rw-r--   0 hm        (1000) hm        (1000)      643 2022-10-03 07:28:14.000000 argus-server-1.8.1/Dockerfile
--rw-rw-r--   0 hm        (1000) hm        (1000)    35149 2022-10-03 07:28:14.000000 argus-server-1.8.1/LICENSE
--rw-rw-r--   0 hm        (1000) hm        (1000)       50 2022-10-11 10:29:27.000000 argus-server-1.8.1/MANIFEST.in
--rw-rw-r--   0 hm        (1000) hm        (1000)     3610 2022-10-28 11:43:50.000000 argus-server-1.8.1/NOTES.md
--rw-rw-r--   0 hm        (1000) hm        (1000)     7621 2022-10-28 11:51:24.521973 argus-server-1.8.1/PKG-INFO
--rw-rw-r--   0 hm        (1000) hm        (1000)     6656 2022-10-06 06:11:00.000000 argus-server-1.8.1/README.md
--rw-rw-r--   0 hm        (1000) hm        (1000)      480 2022-10-28 11:43:50.000000 argus-server-1.8.1/UPGRADING.md
--rw-rw-r--   0 hm        (1000) hm        (1000)      739 2022-10-03 07:28:14.000000 argus-server-1.8.1/cmd.sh-template
--rw-rw-r--   0 hm        (1000) hm        (1000)      338 2022-10-03 07:28:14.000000 argus-server-1.8.1/codecov.yml
--rw-rw-r--   0 hm        (1000) hm        (1000)      711 2022-10-03 07:28:14.000000 argus-server-1.8.1/docker-compose.yml
--rwxrwxr-x   0 hm        (1000) hm        (1000)      162 2022-10-28 11:43:50.000000 argus-server-1.8.1/docker-entrypoint.sh
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.505973 argus-server-1.8.1/docs/
--rw-rw-r--   0 hm        (1000) hm        (1000)      580 2022-10-03 07:28:14.000000 argus-server-1.8.1/docs/Makefile
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.505973 argus-server-1.8.1/docs/_exts/
--rw-rw-r--   0 hm        (1000) hm        (1000)      153 2022-10-06 09:21:59.000000 argus-server-1.8.1/docs/_exts/djangodocs.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.505973 argus-server-1.8.1/docs/_static/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/docs/_static/.gitkeep
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.505973 argus-server-1.8.1/docs/_templates/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/docs/_templates/.gitkeep
--rw-rw-r--   0 hm        (1000) hm        (1000)     3462 2022-10-04 11:09:03.000000 argus-server-1.8.1/docs/about-argus.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)    43619 2022-10-28 11:43:50.000000 argus-server-1.8.1/docs/api.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)     1495 2022-10-04 11:09:03.000000 argus-server-1.8.1/docs/authentication.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)     5756 2022-10-06 09:21:59.000000 argus-server-1.8.1/docs/conf.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.505973 argus-server-1.8.1/docs/development/
--rw-rw-r--   0 hm        (1000) hm        (1000)     3767 2022-10-06 06:11:00.000000 argus-server-1.8.1/docs/development/management-commands.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)     2218 2022-10-03 07:28:14.000000 argus-server-1.8.1/docs/development/notes.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)     2076 2022-10-06 09:21:59.000000 argus-server-1.8.1/docs/development/release-checklist.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)      140 2022-10-06 06:11:00.000000 argus-server-1.8.1/docs/development.rst
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.505973 argus-server-1.8.1/docs/img/
--rw-rw-r--   0 hm        (1000) hm        (1000)   287284 2022-10-03 07:28:14.000000 argus-server-1.8.1/docs/img/ER_model.png
--rw-rw-r--   0 hm        (1000) hm        (1000)      671 2022-10-03 07:28:14.000000 argus-server-1.8.1/docs/index.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)     2931 2022-10-03 07:28:14.000000 argus-server-1.8.1/docs/integrating-monitoring-systems.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)      787 2022-10-03 07:28:14.000000 argus-server-1.8.1/docs/make.bat
--rw-rw-r--   0 hm        (1000) hm        (1000)     2333 2022-10-03 07:28:14.000000 argus-server-1.8.1/docs/models.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)      602 2022-10-03 12:34:14.000000 argus-server-1.8.1/docs/notifications.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)     8686 2022-10-06 09:21:59.000000 argus-server-1.8.1/docs/site-specific-settings.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)    13073 2022-10-06 09:21:59.000000 argus-server-1.8.1/docs/writing-glueservices.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)      109 2022-10-03 07:28:14.000000 argus-server-1.8.1/docs/writing-plugins.rst
--rw-rw-r--   0 hm        (1000) hm        (1000)      660 2022-10-03 07:28:14.000000 argus-server-1.8.1/manage.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2435 2022-10-10 12:29:50.000000 argus-server-1.8.1/pyproject.toml
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.505973 argus-server-1.8.1/requirements/
--rw-rw-r--   0 hm        (1000) hm        (1000)      382 2022-10-03 07:28:14.000000 argus-server-1.8.1/requirements/base.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)      120 2022-10-03 07:28:14.000000 argus-server-1.8.1/requirements/dev.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)       19 2022-10-03 07:28:14.000000 argus-server-1.8.1/requirements/django32.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)       46 2022-10-03 07:28:14.000000 argus-server-1.8.1/requirements/forced-upgrade.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)      484 2022-10-03 07:28:14.000000 argus-server-1.8.1/requirements/please-pip-sync.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        9 2022-10-03 07:28:14.000000 argus-server-1.8.1/requirements/test.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)     4152 2022-10-06 09:21:59.000000 argus-server-1.8.1/requirements-django32.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)     4152 2022-10-06 09:21:59.000000 argus-server-1.8.1/requirements.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)       38 2022-10-28 11:51:24.521973 argus-server-1.8.1/setup.cfg
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.501973 argus-server-1.8.1/src/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.505973 argus-server-1.8.1/src/argus/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/__init__.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.505973 argus-server-1.8.1/src/argus/auth/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.509973 argus-server-1.8.1/src/argus/auth/V1/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 12:34:14.000000 argus-server-1.8.1/src/argus/auth/V1/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1410 2022-10-03 12:44:04.000000 argus-server-1.8.1/src/argus/auth/V1/serializers.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      609 2022-10-03 12:43:24.000000 argus-server-1.8.1/src/argus/auth/V1/urls.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     4625 2022-10-03 12:44:04.000000 argus-server-1.8.1/src/argus/auth/V1/views.py
--rw-rw-r--   0 hm        (1000) hm        (1000)       50 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      274 2022-10-04 11:09:03.000000 argus-server-1.8.1/src/argus/auth/admin.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      114 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/apps.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      652 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/authentication.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1088 2022-10-06 09:21:59.000000 argus-server-1.8.1/src/argus/auth/factories.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.509973 argus-server-1.8.1/src/argus/auth/management/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/management/__init__.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.509973 argus-server-1.8.1/src/argus/auth/management/commands/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/management/commands/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      578 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/management/commands/grantsuperuser.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      588 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/management/commands/revokesuperuser.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      545 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/management/commands/setpassword.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.509973 argus-server-1.8.1/src/argus/auth/migrations/
--rw-rw-r--   0 hm        (1000) hm        (1000)     3450 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/migrations/0001_initial.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      418 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/migrations/0002_alter_user_first_name.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      976 2022-10-05 11:48:13.000000 argus-server-1.8.1/src/argus/auth/migrations/0003_delete_phonenumber.py
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/migrations/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      264 2022-10-05 11:48:13.000000 argus-server-1.8.1/src/argus/auth/models.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      711 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/auth/serializers.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      485 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/auth/urls.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      641 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/auth/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2403 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/auth/views.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.509973 argus-server-1.8.1/src/argus/dataporten/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/dataporten/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2824 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/dataporten/social.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      924 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/dataporten/views.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.509973 argus-server-1.8.1/src/argus/dev/
--rw-rw-r--   0 hm        (1000) hm        (1000)       58 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/dev/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      121 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/dev/apps.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.509973 argus-server-1.8.1/src/argus/dev/management/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/dev/management/__init__.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.509973 argus-server-1.8.1/src/argus/dev/management/commands/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/dev/management/commands/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2116 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/dev/management/commands/create_fake_incident.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      768 2022-10-06 09:21:59.000000 argus-server-1.8.1/src/argus/dev/management/commands/create_source.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      286 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/dev/management/commands/gen_secret_key.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2422 2022-10-10 12:29:50.000000 argus-server-1.8.1/src/argus/dev/management/commands/initial_setup.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.509973 argus-server-1.8.1/src/argus/drf/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/drf/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      696 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/drf/permissions.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.513973 argus-server-1.8.1/src/argus/incident/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.513973 argus-server-1.8.1/src/argus/incident/V1/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/V1/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1531 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/V1/serializers.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1705 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/V1/urls.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     5692 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/incident/V1/views.py
--rw-rw-r--   0 hm        (1000) hm        (1000)       58 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    11041 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/admin.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      671 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/incident/apps.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      273 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/constants.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2183 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/incident/factories.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     3074 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/fields.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2233 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/incident/filters.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1629 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/forms.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.513973 argus-server-1.8.1/src/argus/incident/migrations/
--rw-rw-r--   0 hm        (1000) hm        (1000)     8570 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/migrations/0001_initial.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      860 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/migrations/0002_empty_source_incident_id.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      455 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/migrations/0003_incident_level.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      844 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/migrations/0004_add_ChangeEvent_proxy.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1294 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/migrations/0005_alter_event_type.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1123 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/migrations/0006_incident_search_text.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      569 2022-10-03 12:34:14.000000 argus-server-1.8.1/src/argus/incident/migrations/0007_alter_event_type.py
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/migrations/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    17104 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/incident/models.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    12163 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/incident/serializers.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1245 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/incident/signals.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.497973 argus-server-1.8.1/src/argus/incident/templates/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.513973 argus-server-1.8.1/src/argus/incident/templates/incident/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.497973 argus-server-1.8.1/src/argus/incident/templates/incident/admin/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.513973 argus-server-1.8.1/src/argus/incident/templates/incident/admin/widgets/
--rw-rw-r--   0 hm        (1000) hm        (1000)     1076 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/templates/incident/admin/widgets/split_datetime_infinity.html
--rw-rw-r--   0 hm        (1000) hm        (1000)      258 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/templates/incident/incident_change_list.html
--rw-rw-r--   0 hm        (1000) hm        (1000)     1596 2022-10-19 08:36:56.000000 argus-server-1.8.1/src/argus/incident/urls.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      906 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/validators.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    17708 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/incident/views.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1125 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/incident/widgets.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.513973 argus-server-1.8.1/src/argus/notificationprofile/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.517973 argus-server-1.8.1/src/argus/notificationprofile/V1/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/V1/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     5513 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/notificationprofile/V1/serializers.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      459 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/V1/urls.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     3146 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/V1/views.py
--rw-rw-r--   0 hm        (1000) hm        (1000)       80 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     3885 2022-10-06 09:21:59.000000 argus-server-1.8.1/src/argus/notificationprofile/admin.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1652 2022-10-03 12:34:14.000000 argus-server-1.8.1/src/argus/notificationprofile/apps.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      695 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/checks.py
--rw-rw-r--   0 hm        (1000) hm        (1000)       54 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/constants.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2369 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/notificationprofile/factories.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.517973 argus-server-1.8.1/src/argus/notificationprofile/media/
--rw-rw-r--   0 hm        (1000) hm        (1000)     3127 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/notificationprofile/media/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2163 2022-10-10 12:29:50.000000 argus-server-1.8.1/src/argus/notificationprofile/media/base.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     6392 2022-10-10 12:29:50.000000 argus-server-1.8.1/src/argus/notificationprofile/media/email.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     3534 2022-10-28 11:43:53.000000 argus-server-1.8.1/src/argus/notificationprofile/media/sms_as_email.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.517973 argus-server-1.8.1/src/argus/notificationprofile/migrations/
--rw-rw-r--   0 hm        (1000) hm        (1000)     3797 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/0001_initial.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      456 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/0002_filter_filter.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      396 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/0003_alter_filter_filter.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1264 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/0004_copy_notificationprofile_media_to_media_v1.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     6448 2022-10-03 12:34:14.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/0005_destinationconfig_media.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      626 2022-10-04 11:09:03.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/0006_related_name_destinations.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2094 2022-10-05 11:48:13.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/0007_copy_phone_number_from_destinations.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      615 2022-10-05 11:48:13.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/0008_remove_media_phone_number.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      965 2022-10-10 12:29:50.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/0009_notificationprofile_id.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     4220 2022-10-10 12:29:50.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/0010_notificationprofile_id.py
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/migrations/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    11032 2022-10-06 09:21:59.000000 argus-server-1.8.1/src/argus/notificationprofile/models.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1063 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/primitive_serializers.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     6791 2022-10-10 12:29:50.000000 argus-server-1.8.1/src/argus/notificationprofile/serializers.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2361 2022-10-03 12:44:04.000000 argus-server-1.8.1/src/argus/notificationprofile/signals.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.517973 argus-server-1.8.1/src/argus/notificationprofile/templates/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.517973 argus-server-1.8.1/src/argus/notificationprofile/templates/notificationprofile/
--rw-rw-r--   0 hm        (1000) hm        (1000)      815 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/templates/notificationprofile/email.html
--rw-rw-r--   0 hm        (1000) hm        (1000)      157 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/templates/notificationprofile/email.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)       17 2022-10-03 12:34:14.000000 argus-server-1.8.1/src/argus/notificationprofile/templates/schemawrapper.html
--rw-rw-r--   0 hm        (1000) hm        (1000)      541 2022-10-03 12:34:14.000000 argus-server-1.8.1/src/argus/notificationprofile/urls.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1778 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/notificationprofile/validators.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     9614 2022-10-10 12:29:50.000000 argus-server-1.8.1/src/argus/notificationprofile/views.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.517973 argus-server-1.8.1/src/argus/site/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/site/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      780 2022-10-03 12:34:14.000000 argus-server-1.8.1/src/argus/site/api_v1_urls.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      772 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/site/api_v2_urls.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2459 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/site/logging.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.517973 argus-server-1.8.1/src/argus/site/settings/
--rw-rw-r--   0 hm        (1000) hm        (1000)     2332 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/site/settings/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     9251 2022-10-03 08:12:56.000000 argus-server-1.8.1/src/argus/site/settings/base.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1821 2022-10-10 12:29:50.000000 argus-server-1.8.1/src/argus/site/settings/dev.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      193 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/site/settings/dockerdev.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1661 2022-10-03 12:34:14.000000 argus-server-1.8.1/src/argus/site/settings/prod.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2214 2022-10-03 12:34:14.000000 argus-server-1.8.1/src/argus/site/settings/test_CI.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2062 2022-10-06 09:21:59.000000 argus-server-1.8.1/src/argus/site/urls.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     3104 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/site/views.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      392 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/site/wsgi.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.517973 argus-server-1.8.1/src/argus/util/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/util/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2904 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/util/admin_utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2142 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/util/datetime_utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      501 2022-10-06 09:21:59.000000 argus-server-1.8.1/src/argus/util/testing.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      967 2022-10-28 11:43:50.000000 argus-server-1.8.1/src/argus/util/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      176 2022-10-28 11:51:24.000000 argus-server-1.8.1/src/argus/version.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.517973 argus-server-1.8.1/src/argus/ws/
--rw-rw-r--   0 hm        (1000) hm        (1000)       46 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/ws/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      108 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/ws/apps.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      865 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/ws/asgi.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1771 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/ws/consumers.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1052 2022-10-03 07:28:14.000000 argus-server-1.8.1/src/argus/ws/models.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.521973 argus-server-1.8.1/src/argus_server.egg-info/
--rw-rw-r--   0 hm        (1000) hm        (1000)     7621 2022-10-28 11:51:24.000000 argus-server-1.8.1/src/argus_server.egg-info/PKG-INFO
--rw-rw-r--   0 hm        (1000) hm        (1000)     7131 2022-10-28 11:51:24.000000 argus-server-1.8.1/src/argus_server.egg-info/SOURCES.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        1 2022-10-28 11:51:24.000000 argus-server-1.8.1/src/argus_server.egg-info/dependency_links.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        1 2022-10-28 11:51:23.000000 argus-server-1.8.1/src/argus_server.egg-info/not-zip-safe
--rw-rw-r--   0 hm        (1000) hm        (1000)      536 2022-10-28 11:51:24.000000 argus-server-1.8.1/src/argus_server.egg-info/requires.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        6 2022-10-28 11:51:24.000000 argus-server-1.8.1/src/argus_server.egg-info/top_level.txt
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.521973 argus-server-1.8.1/tests/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/__init__.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.521973 argus-server-1.8.1/tests/auth/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/auth/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     7089 2022-10-28 11:43:50.000000 argus-server-1.8.1/tests/auth/test_auth.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.521973 argus-server-1.8.1/tests/incident/
--rw-rw-r--   0 hm        (1000) hm        (1000)      802 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/incident/__init__.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.521973 argus-server-1.8.1/tests/incident/fixtures/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/incident/fixtures/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     9613 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/incident/test_event.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     5768 2022-10-28 11:43:50.000000 argus-server-1.8.1/tests/incident/test_filters.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     6526 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/incident/test_incident_fields.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2561 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/incident/test_queryset.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    11878 2022-10-10 12:26:34.000000 argus-server-1.8.1/tests/incident/test_serializers.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     7316 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/incident/test_source_system.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1233 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/incident/test_source_system_type.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1495 2022-10-28 11:43:50.000000 argus-server-1.8.1/tests/incident/test_tags.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     9493 2022-10-28 11:43:50.000000 argus-server-1.8.1/tests/incident/test_views.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.521973 argus-server-1.8.1/tests/incident/unit/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/incident/unit/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2290 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/incident/unit/test_incident_details_url.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.521973 argus-server-1.8.1/tests/notificationprofile/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-10-28 11:51:24.521973 argus-server-1.8.1/tests/notificationprofile/V1/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/notificationprofile/V1/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     3086 2022-10-28 11:43:50.000000 argus-server-1.8.1/tests/notificationprofile/V1/test_views.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1330 2022-10-04 11:09:03.000000 argus-server-1.8.1/tests/notificationprofile/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2466 2022-10-06 09:21:59.000000 argus-server-1.8.1/tests/notificationprofile/test_github236.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      484 2022-10-03 07:28:14.000000 argus-server-1.8.1/tests/notificationprofile/test_media.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    13500 2022-10-10 12:29:50.000000 argus-server-1.8.1/tests/notificationprofile/test_models.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    15394 2022-10-06 09:21:59.000000 argus-server-1.8.1/tests/notificationprofile/test_serializers.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1874 2022-10-28 11:43:50.000000 argus-server-1.8.1/tests/notificationprofile/test_signals.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    11359 2022-10-28 11:43:50.000000 argus-server-1.8.1/tests/notificationprofile/test_views.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1945 2022-10-10 12:29:50.000000 argus-server-1.8.1/tox.ini
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.972112 argus-server-1.9.0/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      292 2022-10-06 09:21:59.000000 argus-server-1.9.0/.git-blame-ignore-revs
+-rw-rw-r--   0 hm        (1000) hm        (1000)       34 2022-10-03 07:28:14.000000 argus-server-1.9.0/.gitattributes
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4158 2022-10-03 07:28:14.000000 argus-server-1.9.0/.gitignore
+-rw-rw-r--   0 hm        (1000) hm        (1000)      530 2022-10-06 09:21:59.000000 argus-server-1.9.0/.pre-commit-config.yaml
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4914 2022-11-08 10:52:27.000000 argus-server-1.9.0/CHANGELOG.md
+-rw-rw-r--   0 hm        (1000) hm        (1000)      579 2022-10-03 07:28:14.000000 argus-server-1.9.0/CONTRIBUTORS.md
+-rw-rw-r--   0 hm        (1000) hm        (1000)      643 2022-10-03 07:28:14.000000 argus-server-1.9.0/Dockerfile
+-rw-rw-r--   0 hm        (1000) hm        (1000)    35149 2022-10-03 07:28:14.000000 argus-server-1.9.0/LICENSE
+-rw-rw-r--   0 hm        (1000) hm        (1000)       50 2022-10-11 10:29:27.000000 argus-server-1.9.0/MANIFEST.in
+-rw-rw-r--   0 hm        (1000) hm        (1000)      424 2022-11-07 06:54:56.000000 argus-server-1.9.0/Makefile
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3990 2022-11-08 10:48:35.000000 argus-server-1.9.0/NOTES.md
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7621 2022-11-08 11:47:47.972112 argus-server-1.9.0/PKG-INFO
+-rw-rw-r--   0 hm        (1000) hm        (1000)     6656 2022-10-06 06:11:00.000000 argus-server-1.9.0/README.md
+-rw-rw-r--   0 hm        (1000) hm        (1000)      485 2022-11-07 06:56:39.000000 argus-server-1.9.0/UPGRADING.md
+-rw-rw-r--   0 hm        (1000) hm        (1000)      739 2022-10-03 07:28:14.000000 argus-server-1.9.0/cmd.sh-template
+-rw-rw-r--   0 hm        (1000) hm        (1000)      338 2022-10-03 07:28:14.000000 argus-server-1.9.0/codecov.yml
+-rw-rw-r--   0 hm        (1000) hm        (1000)      711 2022-10-03 07:28:14.000000 argus-server-1.9.0/docker-compose.yml
+-rwxrwxr-x   0 hm        (1000) hm        (1000)      190 2022-11-07 06:56:39.000000 argus-server-1.9.0/docker-entrypoint.sh
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.956112 argus-server-1.9.0/docs/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      580 2022-10-03 07:28:14.000000 argus-server-1.9.0/docs/Makefile
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.956112 argus-server-1.9.0/docs/_exts/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      153 2022-10-06 09:21:59.000000 argus-server-1.9.0/docs/_exts/djangodocs.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.956112 argus-server-1.9.0/docs/_static/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/docs/_static/.gitkeep
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.956112 argus-server-1.9.0/docs/_templates/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/docs/_templates/.gitkeep
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3462 2022-10-04 11:09:03.000000 argus-server-1.9.0/docs/about-argus.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)    44267 2022-11-07 06:56:39.000000 argus-server-1.9.0/docs/api.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1495 2022-10-04 11:09:03.000000 argus-server-1.9.0/docs/authentication.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)     5756 2022-10-06 09:21:59.000000 argus-server-1.9.0/docs/conf.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.956112 argus-server-1.9.0/docs/development/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3767 2022-10-06 06:11:00.000000 argus-server-1.9.0/docs/development/management-commands.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2218 2022-10-03 07:28:14.000000 argus-server-1.9.0/docs/development/notes.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2076 2022-10-06 09:21:59.000000 argus-server-1.9.0/docs/development/release-checklist.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)      140 2022-10-06 06:11:00.000000 argus-server-1.9.0/docs/development.rst
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.956112 argus-server-1.9.0/docs/img/
+-rw-rw-r--   0 hm        (1000) hm        (1000)   287284 2022-10-03 07:28:14.000000 argus-server-1.9.0/docs/img/ER_model.png
+-rw-rw-r--   0 hm        (1000) hm        (1000)      671 2022-10-03 07:28:14.000000 argus-server-1.9.0/docs/index.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2931 2022-10-03 07:28:14.000000 argus-server-1.9.0/docs/integrating-monitoring-systems.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)      787 2022-10-03 07:28:14.000000 argus-server-1.9.0/docs/make.bat
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2333 2022-10-03 07:28:14.000000 argus-server-1.9.0/docs/models.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)      602 2022-10-03 12:34:14.000000 argus-server-1.9.0/docs/notifications.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)     8686 2022-10-06 09:21:59.000000 argus-server-1.9.0/docs/site-specific-settings.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)    13073 2022-10-06 09:21:59.000000 argus-server-1.9.0/docs/writing-glueservices.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)      109 2022-10-03 07:28:14.000000 argus-server-1.9.0/docs/writing-plugins.rst
+-rw-rw-r--   0 hm        (1000) hm        (1000)      660 2022-10-03 07:28:14.000000 argus-server-1.9.0/manage.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2435 2022-10-10 12:29:50.000000 argus-server-1.9.0/pyproject.toml
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.956112 argus-server-1.9.0/requirements/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      382 2022-10-03 07:28:14.000000 argus-server-1.9.0/requirements/base.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)      120 2022-10-03 07:28:14.000000 argus-server-1.9.0/requirements/dev.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)       19 2022-10-03 07:28:14.000000 argus-server-1.9.0/requirements/django32.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)       46 2022-10-03 07:28:14.000000 argus-server-1.9.0/requirements/forced-upgrade.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)      484 2022-10-03 07:28:14.000000 argus-server-1.9.0/requirements/please-pip-sync.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        9 2022-10-03 07:28:14.000000 argus-server-1.9.0/requirements/test.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4152 2022-10-06 09:21:59.000000 argus-server-1.9.0/requirements-django32.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4152 2022-10-06 09:21:59.000000 argus-server-1.9.0/requirements.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)       38 2022-11-08 11:47:47.972112 argus-server-1.9.0/setup.cfg
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.948112 argus-server-1.9.0/src/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.956112 argus-server-1.9.0/src/argus/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/__init__.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.956112 argus-server-1.9.0/src/argus/auth/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.956112 argus-server-1.9.0/src/argus/auth/V1/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 12:34:14.000000 argus-server-1.9.0/src/argus/auth/V1/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1410 2022-10-03 12:44:04.000000 argus-server-1.9.0/src/argus/auth/V1/serializers.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      609 2022-10-03 12:43:24.000000 argus-server-1.9.0/src/argus/auth/V1/urls.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4827 2022-11-08 10:48:35.000000 argus-server-1.9.0/src/argus/auth/V1/views.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)       50 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      274 2022-10-04 11:09:03.000000 argus-server-1.9.0/src/argus/auth/admin.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      114 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/apps.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      652 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/authentication.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1088 2022-10-06 09:21:59.000000 argus-server-1.9.0/src/argus/auth/factories.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.960112 argus-server-1.9.0/src/argus/auth/management/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/management/__init__.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.960112 argus-server-1.9.0/src/argus/auth/management/commands/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/management/commands/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      578 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/management/commands/grantsuperuser.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      588 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/management/commands/revokesuperuser.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      545 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/management/commands/setpassword.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.960112 argus-server-1.9.0/src/argus/auth/migrations/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3450 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/migrations/0001_initial.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      418 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/migrations/0002_alter_user_first_name.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      976 2022-10-05 11:48:13.000000 argus-server-1.9.0/src/argus/auth/migrations/0003_delete_phonenumber.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/migrations/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      264 2022-10-05 11:48:13.000000 argus-server-1.9.0/src/argus/auth/models.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      954 2022-11-07 06:56:39.000000 argus-server-1.9.0/src/argus/auth/serializers.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      569 2022-11-07 06:56:39.000000 argus-server-1.9.0/src/argus/auth/urls.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      641 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/auth/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3315 2022-11-07 06:56:39.000000 argus-server-1.9.0/src/argus/auth/views.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.960112 argus-server-1.9.0/src/argus/dataporten/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/dataporten/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2824 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/dataporten/social.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      924 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/dataporten/views.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.960112 argus-server-1.9.0/src/argus/dev/
+-rw-rw-r--   0 hm        (1000) hm        (1000)       58 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/dev/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      121 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/dev/apps.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.960112 argus-server-1.9.0/src/argus/dev/management/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/dev/management/__init__.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.960112 argus-server-1.9.0/src/argus/dev/management/commands/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/dev/management/commands/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2116 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/dev/management/commands/create_fake_incident.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      768 2022-10-06 09:21:59.000000 argus-server-1.9.0/src/argus/dev/management/commands/create_source.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      286 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/dev/management/commands/gen_secret_key.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2422 2022-10-10 12:29:50.000000 argus-server-1.9.0/src/argus/dev/management/commands/initial_setup.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.960112 argus-server-1.9.0/src/argus/drf/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/drf/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      696 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/drf/permissions.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.960112 argus-server-1.9.0/src/argus/incident/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.960112 argus-server-1.9.0/src/argus/incident/V1/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/V1/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1531 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/V1/serializers.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1850 2022-11-08 08:30:29.000000 argus-server-1.9.0/src/argus/incident/V1/urls.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     5902 2022-11-07 06:56:39.000000 argus-server-1.9.0/src/argus/incident/V1/views.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)       58 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    11041 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/admin.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      949 2022-11-07 06:56:39.000000 argus-server-1.9.0/src/argus/incident/apps.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      273 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/constants.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3009 2022-11-08 08:30:29.000000 argus-server-1.9.0/src/argus/incident/factories.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3074 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/fields.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2445 2022-11-07 06:56:39.000000 argus-server-1.9.0/src/argus/incident/filters.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1629 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/forms.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.964112 argus-server-1.9.0/src/argus/incident/migrations/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     8570 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/migrations/0001_initial.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      860 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/migrations/0002_empty_source_incident_id.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      455 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/migrations/0003_incident_level.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      844 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/migrations/0004_add_ChangeEvent_proxy.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1294 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/migrations/0005_alter_event_type.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1123 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/migrations/0006_incident_search_text.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      569 2022-10-03 12:34:14.000000 argus-server-1.9.0/src/argus/incident/migrations/0007_alter_event_type.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/migrations/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    17502 2022-11-08 10:03:50.000000 argus-server-1.9.0/src/argus/incident/models.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    13215 2022-11-08 10:03:50.000000 argus-server-1.9.0/src/argus/incident/serializers.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2443 2022-11-07 06:56:39.000000 argus-server-1.9.0/src/argus/incident/signals.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.948112 argus-server-1.9.0/src/argus/incident/templates/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.964112 argus-server-1.9.0/src/argus/incident/templates/incident/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.948112 argus-server-1.9.0/src/argus/incident/templates/incident/admin/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.964112 argus-server-1.9.0/src/argus/incident/templates/incident/admin/widgets/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1076 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/templates/incident/admin/widgets/split_datetime_infinity.html
+-rw-rw-r--   0 hm        (1000) hm        (1000)      258 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/templates/incident/incident_change_list.html
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1741 2022-11-08 08:30:29.000000 argus-server-1.9.0/src/argus/incident/urls.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      906 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/validators.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    20238 2022-11-08 10:03:50.000000 argus-server-1.9.0/src/argus/incident/views.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1125 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/incident/widgets.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.964112 argus-server-1.9.0/src/argus/notificationprofile/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.964112 argus-server-1.9.0/src/argus/notificationprofile/V1/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/V1/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     5659 2022-11-07 06:56:39.000000 argus-server-1.9.0/src/argus/notificationprofile/V1/serializers.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      459 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/V1/urls.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3146 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/V1/views.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)       80 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3885 2022-10-06 09:21:59.000000 argus-server-1.9.0/src/argus/notificationprofile/admin.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1652 2022-10-03 12:34:14.000000 argus-server-1.9.0/src/argus/notificationprofile/apps.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      695 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/checks.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)       54 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/constants.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2436 2022-11-08 08:30:29.000000 argus-server-1.9.0/src/argus/notificationprofile/factories.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.964112 argus-server-1.9.0/src/argus/notificationprofile/media/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2941 2022-11-07 06:57:57.000000 argus-server-1.9.0/src/argus/notificationprofile/media/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2214 2022-11-08 10:48:35.000000 argus-server-1.9.0/src/argus/notificationprofile/media/base.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     6674 2022-11-08 10:48:35.000000 argus-server-1.9.0/src/argus/notificationprofile/media/email.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3789 2022-11-08 10:48:35.000000 argus-server-1.9.0/src/argus/notificationprofile/media/sms_as_email.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.964112 argus-server-1.9.0/src/argus/notificationprofile/migrations/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3797 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/0001_initial.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      456 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/0002_filter_filter.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      396 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/0003_alter_filter_filter.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1264 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/0004_copy_notificationprofile_media_to_media_v1.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     6448 2022-10-03 12:34:14.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/0005_destinationconfig_media.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      626 2022-10-04 11:09:03.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/0006_related_name_destinations.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2094 2022-10-05 11:48:13.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/0007_copy_phone_number_from_destinations.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      615 2022-10-05 11:48:13.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/0008_remove_media_phone_number.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      965 2022-10-10 12:29:50.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/0009_notificationprofile_id.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4220 2022-10-10 12:29:50.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/0010_notificationprofile_id.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/migrations/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    11032 2022-10-06 09:21:59.000000 argus-server-1.9.0/src/argus/notificationprofile/models.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1063 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/primitive_serializers.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7061 2022-11-08 10:48:35.000000 argus-server-1.9.0/src/argus/notificationprofile/serializers.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2361 2022-10-03 12:44:04.000000 argus-server-1.9.0/src/argus/notificationprofile/signals.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.964112 argus-server-1.9.0/src/argus/notificationprofile/templates/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.964112 argus-server-1.9.0/src/argus/notificationprofile/templates/notificationprofile/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      815 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/templates/notificationprofile/email.html
+-rw-rw-r--   0 hm        (1000) hm        (1000)      157 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/templates/notificationprofile/email.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)       17 2022-10-03 12:34:14.000000 argus-server-1.9.0/src/argus/notificationprofile/templates/schemawrapper.html
+-rw-rw-r--   0 hm        (1000) hm        (1000)      541 2022-10-03 12:34:14.000000 argus-server-1.9.0/src/argus/notificationprofile/urls.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1778 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/notificationprofile/validators.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     9614 2022-10-10 12:29:50.000000 argus-server-1.9.0/src/argus/notificationprofile/views.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.968112 argus-server-1.9.0/src/argus/site/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/site/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      780 2022-10-03 12:34:14.000000 argus-server-1.9.0/src/argus/site/api_v1_urls.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      772 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/site/api_v2_urls.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2459 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/site/logging.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.968112 argus-server-1.9.0/src/argus/site/settings/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2332 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/site/settings/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     9251 2022-10-03 08:12:56.000000 argus-server-1.9.0/src/argus/site/settings/base.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1821 2022-10-10 12:29:50.000000 argus-server-1.9.0/src/argus/site/settings/dev.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      193 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/site/settings/dockerdev.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1661 2022-10-03 12:34:14.000000 argus-server-1.9.0/src/argus/site/settings/prod.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2214 2022-10-03 12:34:14.000000 argus-server-1.9.0/src/argus/site/settings/test_CI.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2062 2022-10-06 09:21:59.000000 argus-server-1.9.0/src/argus/site/urls.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3104 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/site/views.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      392 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/site/wsgi.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.968112 argus-server-1.9.0/src/argus/util/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/util/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2904 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/util/admin_utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2142 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/util/datetime_utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      501 2022-10-06 09:21:59.000000 argus-server-1.9.0/src/argus/util/testing.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1206 2022-11-07 06:57:57.000000 argus-server-1.9.0/src/argus/util/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      176 2022-11-08 11:47:47.000000 argus-server-1.9.0/src/argus/version.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.968112 argus-server-1.9.0/src/argus/ws/
+-rw-rw-r--   0 hm        (1000) hm        (1000)       46 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/ws/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      108 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/ws/apps.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      865 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/ws/asgi.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1771 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/ws/consumers.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1052 2022-10-03 07:28:14.000000 argus-server-1.9.0/src/argus/ws/models.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.968112 argus-server-1.9.0/src/argus_server.egg-info/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7621 2022-11-08 11:47:47.000000 argus-server-1.9.0/src/argus_server.egg-info/PKG-INFO
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7201 2022-11-08 11:47:47.000000 argus-server-1.9.0/src/argus_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        1 2022-11-08 11:47:47.000000 argus-server-1.9.0/src/argus_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        1 2022-11-08 11:47:47.000000 argus-server-1.9.0/src/argus_server.egg-info/not-zip-safe
+-rw-rw-r--   0 hm        (1000) hm        (1000)      536 2022-11-08 11:47:47.000000 argus-server-1.9.0/src/argus_server.egg-info/requires.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        6 2022-11-08 11:47:47.000000 argus-server-1.9.0/src/argus_server.egg-info/top_level.txt
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.968112 argus-server-1.9.0/tests/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/__init__.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.968112 argus-server-1.9.0/tests/auth/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.968112 argus-server-1.9.0/tests/auth/V1/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     6064 2022-11-08 10:48:35.000000 argus-server-1.9.0/tests/auth/V1/test_views.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/auth/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7519 2022-11-07 06:56:39.000000 argus-server-1.9.0/tests/auth/test_auth.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1150 2022-11-07 06:56:39.000000 argus-server-1.9.0/tests/auth/test_views.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.972112 argus-server-1.9.0/tests/incident/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      802 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/incident/__init__.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.972112 argus-server-1.9.0/tests/incident/fixtures/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/incident/fixtures/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4179 2022-11-07 06:56:39.000000 argus-server-1.9.0/tests/incident/test_change_event.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     9613 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/incident/test_event.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7245 2022-11-07 06:56:39.000000 argus-server-1.9.0/tests/incident/test_filters.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     6526 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/incident/test_incident_fields.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2561 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/incident/test_queryset.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    11878 2022-10-10 12:26:34.000000 argus-server-1.9.0/tests/incident/test_serializers.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7316 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/incident/test_source_system.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1233 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/incident/test_source_system_type.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    40547 2022-11-08 10:03:50.000000 argus-server-1.9.0/tests/incident/test_views.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.972112 argus-server-1.9.0/tests/incident/unit/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/incident/unit/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2290 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/incident/unit/test_incident_details_url.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.972112 argus-server-1.9.0/tests/notificationprofile/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2022-11-08 11:47:47.972112 argus-server-1.9.0/tests/notificationprofile/V1/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/notificationprofile/V1/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    12813 2022-11-07 06:59:22.000000 argus-server-1.9.0/tests/notificationprofile/V1/test_views.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1330 2022-10-04 11:09:03.000000 argus-server-1.9.0/tests/notificationprofile/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2466 2022-10-06 09:21:59.000000 argus-server-1.9.0/tests/notificationprofile/test_github236.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      484 2022-10-03 07:28:14.000000 argus-server-1.9.0/tests/notificationprofile/test_media.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    13500 2022-10-10 12:29:50.000000 argus-server-1.9.0/tests/notificationprofile/test_models.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    15394 2022-10-06 09:21:59.000000 argus-server-1.9.0/tests/notificationprofile/test_serializers.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1922 2022-11-07 06:56:39.000000 argus-server-1.9.0/tests/notificationprofile/test_signals.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    14077 2022-11-08 10:48:35.000000 argus-server-1.9.0/tests/notificationprofile/test_views.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1945 2022-10-10 12:29:50.000000 argus-server-1.9.0/tox.ini
```

### Comparing `argus-server-1.8.1/.gitignore` & `argus-server-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/.pre-commit-config.yaml` & `argus-server-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/CHANGELOG.md` & `argus-server-1.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 # Changes
 This file documents all changes to Argus. This file is primarily meant to be
 read by developers.
 
 ## [Unreleased]
 
+## [1.9.0] - 2022-11-08
+
+### Added
+- Add test for updating phone number in V1
+- Add test for posting tag with invalid key
+- Added an endpoint to acknowledge incidents in bulk
+- Added an endpoint to get a refreshed auth token.
+- Add a filter to find incidents with a duration longer than a given amount of
+ minutes.
+- Added tests for previously untested incident endpoints
+- A Makefile that cleans away generated files
+
+### Fixed
+- Validate that user doesn't have destination with same settings before
+  creating/updating destination
+- Properly catch tag validtion errors
+- The FilterFactory no longer leads to random UniqueViolations on testing
+
 ## [1.8.1] - 2022-10-28
 
 ### Fixed
 - Fix typo that prevented SMS messages from being sent.
 
 ## [1.8.0] - 2022-10-06
```

### Comparing `argus-server-1.8.1/CONTRIBUTORS.md` & `argus-server-1.9.0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/Dockerfile` & `argus-server-1.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/LICENSE` & `argus-server-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/NOTES.md` & `argus-server-1.9.0/NOTES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 # Release Notes
 This file documents changes to Argus that are relevant for the users to know.
 
 ## [Unreleased]
 
+## [1.9.0] - 2022-11-08
+
+### Added
+
+- Added an endpoint to acknowledge incidents in bulk
+- Added an endpoint to get a refreshed auth token.
+- Add a filter to find incidents with a duration longer than a given amount of
+  minutes.
+- Added tests for previously untested incident endpoints
+
+## [1.8.1] - 2022-10-28
+
+### Fixed
+- Fix typo that prevented SMS messages from being sent.
+
 ## [1.8.0] - 2022-10-06
 
 ### Added
 - A notification profile can now have a name.
 - Added endpoint that returns True if another user has a destination with the
   same medium and settings as the destination with the given primary key
```

### Comparing `argus-server-1.8.1/PKG-INFO` & `argus-server-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argus-server
-Version: 1.8.1
+Version: 1.9.0
 Summary: Argus is an alert aggregator for monitoring systems
 Author-email: Uninett Opensource <opensource@uninett.no>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/Uninett/Argus
 Platform: any
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `argus-server-1.8.1/README.md` & `argus-server-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/cmd.sh-template` & `argus-server-1.9.0/cmd.sh-template`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docker-compose.yml` & `argus-server-1.9.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/Makefile` & `argus-server-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/about-argus.rst` & `argus-server-1.9.0/docs/about-argus.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/api.rst` & `argus-server-1.9.0/docs/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,18 @@
       “unacked” in the case of ``acked=``.
 
       **Filtering parameters**:
 
       ``acked=true|false``
         Fetch only acked (``true``) or unacked (``false``) incidents.
 
+      ``duration__gte=number``
+        Fetch only incidents that are or have been open for equal to or
+        more than (``number``) minutes.
+
       ``end_time__gte=end-time``
         Fetch only incidents that ended on or later than (``end-time``).
 
       ``end_time__isnull=true|false``
         Fetch only stateless (``true``) or stateful (``false``) incidents.
 
       ``end_time__lte=end-time``
@@ -738,14 +742,22 @@
     :caption: Example request body
 
       {
         "username": "alice",
         "password": "secret"
       }
 
+-  ``POST`` to ``/api/v2/refresh-token/``: returns an auth token for the
+   currently logged in user
+
+   -  Note that this token will expire after a certain amout of days that is
+      set in the variable ``AUTH_TOKEN_EXPIRES_AFTER_DAYS`` in
+      :ref:`site-specific-settings` (by default 14 days), and can be replaced
+      by posting to the same endpoint.
+
 -  ``/oidc/login/dataporten_feide/``: redirects to Feide login
 
 
 .. _api-incident-endpoints-v2:
 
 Incident endpoints
 ==============================
@@ -762,14 +774,18 @@
       “unacked” in the case of ``acked=``.
 
       **Filtering parameters**:
 
       ``acked=true|false``
         Fetch only acked (``true``) or unacked (``false``) incidents.
 
+      ``duration__gte=number``
+        Fetch only incidents that are or have been open for equal to or
+        more than (``number``) minutes.
+
       ``end_time__gte=end-time``
         Fetch only incidents that ended on or later than (``end-time``).
 
       ``end_time__isnull=true|false``
         Fetch only stateless (``true``) or stateful (``false``) incidents.
 
       ``end_time__lte=end-time``
```

### Comparing `argus-server-1.8.1/docs/authentication.rst` & `argus-server-1.9.0/docs/authentication.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/conf.py` & `argus-server-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/development/management-commands.rst` & `argus-server-1.9.0/docs/development/management-commands.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/development/notes.rst` & `argus-server-1.9.0/docs/development/notes.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/development/release-checklist.rst` & `argus-server-1.9.0/docs/development/release-checklist.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/img/ER_model.png` & `argus-server-1.9.0/docs/img/ER_model.png`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/index.rst` & `argus-server-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/integrating-monitoring-systems.rst` & `argus-server-1.9.0/docs/integrating-monitoring-systems.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/make.bat` & `argus-server-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/models.rst` & `argus-server-1.9.0/docs/models.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/notifications.rst` & `argus-server-1.9.0/docs/notifications.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/site-specific-settings.rst` & `argus-server-1.9.0/docs/site-specific-settings.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/docs/writing-glueservices.rst` & `argus-server-1.9.0/docs/writing-glueservices.rst`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/manage.py` & `argus-server-1.9.0/manage.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/pyproject.toml` & `argus-server-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/requirements-django32.txt` & `argus-server-1.9.0/requirements-django32.txt`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/requirements.txt` & `argus-server-1.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/V1/serializers.py` & `argus-server-1.9.0/src/argus/auth/V1/serializers.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/V1/urls.py` & `argus-server-1.9.0/src/argus/auth/V1/urls.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/V1/views.py` & `argus-server-1.9.0/src/argus/auth/V1/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,21 @@
     def list(self, request):
         serializer = self.serializer_class(self.queryset.filter(user=request.user), many=True)
         return Response(serializer.data, status=status.HTTP_200_OK)
 
     def create(self, request, pk=None):
         if pk:
             destination = get_object_or_404(self.queryset.filter(user=request.user), pk=pk)
-            serializer = self.write_serializer_class(destination, data={"media": "sms", "settings": request.data})
+            serializer = self.write_serializer_class(
+                destination, data={"media": "sms", "settings": request.data}, context={"request": request}
+            )
         else:
-            serializer = self.write_serializer_class(data={"media": "sms", "settings": request.data})
+            serializer = self.write_serializer_class(
+                data={"media": "sms", "settings": request.data}, context={"request": request}
+            )
         if serializer.is_valid():
             serializer.save(user=request.user)
             response_serializer = self.serializer_class(serializer.instance)
             return Response(response_serializer.data, status=status.HTTP_201_CREATED)
         response_serializer = self.serializer_class(
             data={"user": request.user.pk, "phone_number": serializer.data["settings"]["phone_number"]}
         )
@@ -62,28 +66,30 @@
         return Response(serializer.data, status=status.HTTP_200_OK)
 
     def update(self, request, pk=None):
         if request.stream.method == "PUT":
             destination = self.queryset.filter(user=request.user).filter(pk=pk).first()
         elif request.stream.method == "PATCH":
             destination = get_object_or_404(self.queryset.filter(user=request.user), pk=pk)
-        serializer = self.write_serializer_class(destination, data={"media": "sms", "settings": request.data})
+        serializer = self.write_serializer_class(
+            destination, data={"media": "sms", "settings": request.data}, context={"request": request}
+        )
         if serializer.is_valid():
             serializer.save(user=request.user)
             response_serializer = self.serializer_class(serializer.instance)
             return Response(response_serializer.data, status=status.HTTP_201_CREATED)
         response_serializer = self.serializer_class(
             data={"user": request.user.pk, "phone_number": serializer.data["settings"]["phone_number"]}
         )
         return Response(serializer.errors, status=status.HTTP_400_BAD_REQUEST)
 
     def partial_update(self, request, pk=None):
         destination = get_object_or_404(self.queryset.filter(user=request.user), pk=pk)
         serializer = self.write_serializer_class(
-            destination, data={"media": "sms", "settings": request.data}, partial=True
+            destination, data={"media": "sms", "settings": request.data}, partial=True, context={"request": request}
         )
         if serializer.is_valid():
             serializer.save()
             response_serializer = self.serializer_class(serializer.instance)
             return Response(response_serializer.data, status=status.HTTP_201_CREATED)
         response_serializer = self.serializer_class(
             data={"user": request.user.pk, "phone_number": serializer.data["settings"]["phone_number"]}
```

### Comparing `argus-server-1.8.1/src/argus/auth/authentication.py` & `argus-server-1.9.0/src/argus/auth/authentication.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/factories.py` & `argus-server-1.9.0/src/argus/auth/factories.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/management/commands/grantsuperuser.py` & `argus-server-1.9.0/src/argus/auth/management/commands/grantsuperuser.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/management/commands/revokesuperuser.py` & `argus-server-1.9.0/src/argus/auth/management/commands/revokesuperuser.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/management/commands/setpassword.py` & `argus-server-1.9.0/src/argus/auth/management/commands/setpassword.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/migrations/0001_initial.py` & `argus-server-1.9.0/src/argus/auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/migrations/0003_delete_phonenumber.py` & `argus-server-1.9.0/src/argus/auth/migrations/0003_delete_phonenumber.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/utils.py` & `argus-server-1.9.0/src/argus/auth/utils.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/auth/views.py` & `argus-server-1.9.0/src/argus/auth/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from django.contrib.auth import logout
 from django.conf import settings
+from django.db import transaction
 
-from drf_spectacular.utils import extend_schema
+from drf_spectacular.utils import extend_schema, extend_schema_view
 from rest_framework import generics
 from rest_framework.authtoken.models import Token
 from rest_framework.authtoken.views import ObtainAuthToken
+from rest_framework.exceptions import ValidationError
 from rest_framework.permissions import IsAuthenticated, AllowAny
 from rest_framework.response import Response
 from rest_framework.reverse import reverse
 from rest_framework.views import APIView
 
 from .models import User
-from .serializers import BasicUserSerializer, UserSerializer
+from .serializers import BasicUserSerializer, EmptySerializer, RefreshTokenSerializer, UserSerializer
 from .utils import get_psa_authentication_names
 
 
 class ObtainNewAuthToken(ObtainAuthToken):
     def post(self, request, *args, **kwargs):
         serializer = self.serializer_class(data=request.data, context={"request": request})
         serializer.is_valid(raise_exception=True)
@@ -65,7 +67,31 @@
     http_method_names = ["get", "head", "options", "trace"]
     permission_classes = [AllowAny]
 
     def get(self, request, *args, **kwargs):
         names = get_psa_authentication_names()
         data = {name: reverse("social:begin", kwargs={"backend": name}, request=request) for name in names}
         return Response(data)
+
+
+@extend_schema_view(
+    post=extend_schema(
+        request=EmptySerializer,
+    ),
+)
+class RefreshTokenView(APIView):
+    http_method_names = ["post", "head", "options", "trace"]
+    permission_classes = [IsAuthenticated]
+    serializer_class = RefreshTokenSerializer
+    write_serializer_class = EmptySerializer
+
+    @transaction.atomic
+    def post(self, request, *args, **kwargs):
+        user = request.user
+        try:
+            Token.objects.get(user=user).delete()
+        except Token.DoesNotExist:
+            raise ValidationError(
+                f"No token for the user '{user}' exists, one needs to be created in the admin interface."
+            )
+        token = Token.objects.create(user=user)
+        return Response({"token": token.key})
```

### Comparing `argus-server-1.8.1/src/argus/dataporten/social.py` & `argus-server-1.9.0/src/argus/dataporten/social.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/dataporten/views.py` & `argus-server-1.9.0/src/argus/dataporten/views.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/dev/management/commands/create_fake_incident.py` & `argus-server-1.9.0/src/argus/dev/management/commands/create_fake_incident.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/dev/management/commands/create_source.py` & `argus-server-1.9.0/src/argus/dev/management/commands/create_source.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/dev/management/commands/initial_setup.py` & `argus-server-1.9.0/src/argus/dev/management/commands/initial_setup.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/drf/permissions.py` & `argus-server-1.9.0/src/argus/drf/permissions.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/V1/serializers.py` & `argus-server-1.9.0/src/argus/incident/V1/serializers.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/V1/urls.py` & `argus-server-1.9.0/src/argus/incident/V1/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 sourced_incident_list = views_V1.SourceLockedIncidentViewSetV1.as_view({"get": "list", "post": "create"})
 
 event_list = views.EventViewSet.as_view({"get": "list", "post": "create"})
 event_detail = views.EventViewSet.as_view({"get": "retrieve"})
 
 ack_list = views.AcknowledgementViewSet.as_view({"get": "list", "post": "create"})
 ack_detail = views.AcknowledgementViewSet.as_view({"get": "retrieve", "put": "update", "patch": "partial_update"})
+acks_bulk_list = views.BulkAcknowledgementViewSet.as_view({"post": "create"})
 
 tag_list = views.IncidentTagViewSet.as_view({"get": "list", "post": "create"})
 tag_detail = views.IncidentTagViewSet.as_view({"get": "retrieve", "delete": "destroy"})
 
 app_name = "incident"
 urlpatterns = [
+    path("acks/bulk/", acks_bulk_list, name="incident-acks-bulk"),
     path("mine/", sourced_incident_list, name="source_locked_incidents"),
     path("<int:incident_pk>/events/", event_list, name="incident-events"),
     path("<int:incident_pk>/events/<int:pk>/", event_detail, name="incident-event"),
     path("<int:incident_pk>/acks/", ack_list, name="incident-acks"),
     path("<int:incident_pk>/acks/<int:pk>/", ack_detail, name="incident-ack"),
     path("<int:incident_pk>/tags/", tag_list, name="incident-tags"),
     path("<int:incident_pk>/tags/<str:tag>/", tag_detail, name="incident-tag"),
```

### Comparing `argus-server-1.8.1/src/argus/incident/V1/views.py` & `argus-server-1.9.0/src/argus/incident/V1/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     list=extend_schema(
         parameters=[
             OpenApiParameter(
                 name="acked",
                 description="Fetch acked (`true`) or unacked (`false`) incidents.",
                 enum=BooleanStringOAEnum,
             ),
+            OpenApiParameter(
+                name="duration__gte",
+                description="Fetch incidents with a duration longer of equal to `DURATION` minutes",
+                type=int,
+            ),
             OpenApiParameter(name="cursor", description="The pagination cursor value.", type=str),
             OpenApiParameter(
                 name="end_time__gte",
                 description="Fetch incidents that ended on or after `END_TIME`",
                 type=OpenApiTypes.DATETIME,
             ),
             OpenApiParameter(
```

### Comparing `argus-server-1.8.1/src/argus/incident/admin.py` & `argus-server-1.9.0/src/argus/incident/admin.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/apps.py` & `argus-server-1.9.0/src/argus/incident/apps.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from django.apps import AppConfig
-from django.db.models.signals import post_delete, post_save
+from django.db.models.signals import post_delete, post_save, pre_save
 
 
 class IncidentConfig(AppConfig):
     name = "argus.incident"
     label = "argus_incident"
 
     def ready(self):
-        from .signals import delete_associated_user, delete_associated_event, create_first_event, send_notification
+        from .signals import (
+            create_change_events,
+            create_first_event,
+            delete_associated_user,
+            delete_associated_event,
+            detect_changes,
+            send_notification,
+        )
 
         post_delete.connect(delete_associated_user, "argus_incident.SourceSystem")
         post_delete.connect(delete_associated_event, "argus_incident.Acknowledgement")
         post_save.connect(create_first_event, "argus_incident.Incident")
         post_save.connect(send_notification, "argus_incident.Event", dispatch_uid="send_notification")
+        pre_save.connect(detect_changes, "argus_incident.Incident"),
+        post_save.connect(create_change_events, "argus_incident.Incident"),
```

### Comparing `argus-server-1.8.1/src/argus/incident/factories.py` & `argus-server-1.9.0/src/argus/incident/factories.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,45 +18,45 @@
 
 
 class SourceSystemTypeFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = models.SourceSystemType
         django_get_or_create = ("name",)
 
-    name = factory.Faker("word")
+    name = factory.Sequence(lambda s: "SourceSystemType %s" % s)
 
 
 class SourceSystemFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = models.SourceSystem
         django_get_or_create = ("name", "user")
 
-    name = factory.Faker("word")
+    name = factory.Sequence(lambda s: "SourceSystem %s" % s)
     type = factory.SubFactory(SourceSystemTypeFactory)
     user = factory.SubFactory(SourceUserFactory)
     base_url = factory.Faker("url")
 
 
 class TagFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = models.Tag
         django_get_or_create = ("key", "value")
 
-    key = factory.Faker("word")
-    value = factory.Faker("word")
+    key = factory.Sequence(lambda s: "key_%s" % s)
+    value = factory.Sequence(lambda s: "value_%s" % s)
 
 
 class IncidentFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = models.Incident
 
     start_time = factory.Faker("date_time_between", start_date="-1d", end_date="+1d", tzinfo=pytz.UTC)
     end_time = INFINITY_REPR
     source = factory.SubFactory(SourceSystemFactory)
-    source_incident_id = factory.Faker("md5")
+    source_incident_id = factory.Sequence(lambda s: s)
     details_url = factory.Faker("uri")
     description = factory.Faker("sentence")
     level = factory.fuzzy.FuzzyChoice(models.Incident.LEVELS)  # Random valid level
     ticket_url = factory.Faker("uri")
 
 
 class StatefulIncidentFactory(IncidentFactory):
@@ -71,7 +71,27 @@
     class Meta:
         model = models.IncidentTagRelation
 
     tag = factory.SubFactory(TagFactory)
     incident = factory.SubFactory(IncidentFactory)
     added_by = factory.SubFactory(SourceUserFactory)
     added_time = factory.Faker("date_time_between", start_date="-1d", end_date="+1d", tzinfo=pytz.UTC)
+
+
+class EventFactory(factory.django.DjangoModelFactory):
+    class Meta:
+        model = models.Event
+
+    incident = factory.SubFactory(IncidentFactory)
+    actor = factory.SubFactory(SourceUserFactory)
+    timestamp = factory.Faker("date_time_between", start_date="-1d", end_date="+1d", tzinfo=pytz.UTC)
+    received = timestamp
+    type = models.Event.Type.OTHER
+    description = factory.Faker("sentence")
+
+
+class AcknowledgementFactory(factory.django.DjangoModelFactory):
+    class Meta:
+        model = models.Acknowledgement
+
+    event = factory.SubFactory(EventFactory, type=models.Event.Type.ACKNOWLEDGE)
+    expiration = factory.Faker("date_time_between", start_date="+1d", end_date="+2d", tzinfo=pytz.UTC)
```

### Comparing `argus-server-1.8.1/src/argus/incident/fields.py` & `argus-server-1.9.0/src/argus/incident/fields.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/filters.py` & `argus-server-1.9.0/src/argus/incident/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 class IncidentFilter(filters.FilterSet):
     open = filters.BooleanFilter(label="Open", method="incident_filter")
     acked = filters.BooleanFilter(label="Acked", method="incident_filter")
     stateful = filters.BooleanFilter(label="Stateful", method="incident_filter")
     ticket = filters.BooleanFilter(label="Ticket", method="incident_filter")
     tags = TagInFilter(label="Tags", method="incident_filter")
+    duration__gte = filters.NumberFilter(label="Duration", method="incident_filter")
 
     @classmethod
     def incident_filter(cls, queryset, name, value):
         if name == "open":
             if value:
                 return queryset.open()
             else:
@@ -48,14 +49,17 @@
                     value = [value]
                 return queryset.from_tags(*value)
         elif name == "ticket":
             if value:
                 return queryset.has_ticket()
             else:
                 return queryset.lacks_ticket()
+        elif name == "duration__gte":
+            if value:
+                return queryset.is_longer_than_minutes(int(value))
         return queryset
 
     class Meta:
         model = Incident
         fields = {
             "source__id": ["in"],
             "source__name": ["in"],
```

### Comparing `argus-server-1.8.1/src/argus/incident/forms.py` & `argus-server-1.9.0/src/argus/incident/forms.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/migrations/0001_initial.py` & `argus-server-1.9.0/src/argus/incident/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/migrations/0002_empty_source_incident_id.py` & `argus-server-1.9.0/src/argus/incident/migrations/0002_empty_source_incident_id.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/migrations/0004_add_ChangeEvent_proxy.py` & `argus-server-1.9.0/src/argus/incident/migrations/0004_add_ChangeEvent_proxy.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/migrations/0005_alter_event_type.py` & `argus-server-1.9.0/src/argus/incident/migrations/0005_alter_event_type.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/migrations/0006_incident_search_text.py` & `argus-server-1.9.0/src/argus/incident/migrations/0006_incident_search_text.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/migrations/0007_alter_event_type.py` & `argus-server-1.9.0/src/argus/incident/migrations/0007_alter_event_type.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/models.py` & `argus-server-1.9.0/src/argus/incident/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from collections import defaultdict
+from datetime import timedelta
 from functools import reduce
 import logging
 from operator import and_
 from random import randint
 from urllib.parse import urljoin
 
 from django.core.exceptions import ValidationError
 from django.core.validators import URLValidator
-from django.db import models, transaction
-from django.db.models import Q
+from django.db import models
+from django.db.models import F, Q
 from django.utils import timezone
 
 from argus.auth.models import User
 from argus.util.datetime_utils import INFINITY_REPR, get_infinity_repr
 from .constants import INCIDENT_LEVELS, INCIDENT_LEVEL_CHOICES, MIN_INCIDENT_LEVEL, MAX_INCIDENT_LEVEL
 from .fields import DateTimeInfinityField
 from .validators import validate_lowercase, validate_key
@@ -50,15 +51,15 @@
         level=level or randint(MIN_INCIDENT_LEVEL, MAX_INCIDENT_LEVEL),
     )
 
     taglist = [("location", "argus"), ("object", f"{incident.id}"), ("problem_type", "test")]
     if tags:
         try:
             tags = [Tag.split(tag) for tag in tags]
-        except ValueError as e:
+        except (ValueError, ValidationError) as e:
             raise ValidationError(str(e))
         taglist.extend(tags)
     for k, v in taglist:
         tag, _ = Tag.objects.get_or_create(key=k, value=v)
         IncidentTagRelation.objects.create(tag=tag, incident=incident, added_by=argus_user)
     return incident
 
@@ -202,14 +203,20 @@
         tag_qss = Tag.objects.parse(*tags)
         qs = []
         for tag_qs in tag_qss:
             qs.append(self.filter(incident_tag_relations__tag__in=tag_qs))
         qs = reduce(and_, qs)
         return qs.distinct()
 
+    def is_longer_than_minutes(self, minutes):
+        min_duration = timedelta(minutes=minutes)
+        open = self.open().annotate(duration=timezone.now() - F("start_time"))
+        closed = self.closed().annotate(duration=F("end_time") - F("start_time"))
+        return open.filter(duration__gte=min_duration) | closed.filter(duration__gte=min_duration)
+
     # Cannot be a constant, because `timezone.now()` would have been evaluated at compile time
     @staticmethod
     def _get_acked_incident_ids():
         current_acks = Acknowledgement.objects.active().prefetch_related("event__incident")
         return current_acks.values_list("event__incident", flat=True).distinct()
```

### Comparing `argus-server-1.8.1/src/argus/incident/serializers.py` & `argus-server-1.9.0/src/argus/incident/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from collections import OrderedDict
 from typing import List
 
+from django.core.exceptions import ValidationError
 from django.core.validators import URLValidator
 from django.utils import timezone
 
 from rest_framework import serializers
 
 from argus.auth.models import User
 from argus.auth.serializers import UsernameSerializer
 from argus.util.datetime_utils import INFINITY_REPR
 from . import fields
 from .models import (
     Acknowledgement,
+    ChangeEvent,
     Event,
     Incident,
     IncidentTagRelation,
     SourceSystem,
     SourceSystemType,
     Tag,
 )
@@ -38,26 +40,26 @@
 
 class TagSerializer(serializers.Serializer):
     tag = serializers.CharField()
 
     def validate_tag(self, value: str):
         try:
             [key, value] = Tag.split(value)
-        except ValueError as e:
+        except (ValueError, ValidationError) as e:
             raise serializers.ValidationError(str(e))
 
         return Tag.join(key, value)
 
     def to_internal_value(self, data: dict):
         if not "tag" in data:
             return data
 
         try:
             [key, value] = Tag.split(data.pop("tag"))
-        except ValueError as e:
+        except (ValueError, ValidationError) as e:
             raise serializers.ValidationError({"tag": str(e)})
 
         return {"key": key, "value": value}
 
     def to_representation(self, instance):
         if isinstance(instance, Tag):
             tagstr = instance.representation
@@ -74,35 +76,35 @@
         model = IncidentTagRelation
         fields = ["tag", "added_by", "added_time"]
         read_only_fields = ["added_by", "added_time"]
 
     def validate_tag(self, value: str):
         try:
             [key, value] = Tag.split(value)
-        except ValueError as e:
+        except (ValueError, ValidationError) as e:
             raise serializers.ValidationError(str(e))
 
         return Tag.join(key, value)
 
     def create(self, validated_data: dict):
         tag = validated_data.pop("tag")
         try:
             [key, value] = Tag.split(tag)
-        except ValueError as e:
+        except (ValueError, ValidationError) as e:
             raise serializers.ValidationError(str(e))
 
         return Tag.objects.create(key=key, value=value, **validated_data)
 
     def to_internal_value(self, data: dict):
         if not "tag" in data:
             return data
 
         try:
             [key, value] = Tag.split(data.pop("tag"))
-        except ValueError as e:
+        except (ValueError, ValidationError) as e:
             raise serializers.ValidationError({"tag": str(e)})
 
         return {"key": key, "value": value}
 
     def to_representation(self, instance: IncidentTagRelation):
         tag_repr = super().to_representation(instance)
         tag_repr["tag"] = instance.tag.representation
@@ -221,14 +223,19 @@
             errors = {}
             for tag_relation in remove_tag_relations:
                 if tag_relation.added_by != user:
                     errors[str(tag_relation.tag)] = "Cannot remove this tag when you're not the one who added it."
             if errors:
                 raise serializers.ValidationError(errors)
 
+        # Post change events
+        if remove_tag_relations or add_tags:
+            description = f"Change: tags {[str(tag) for tag in existing_tags]} → {[str(tag) for tag in posted_tags]}"
+            ChangeEvent.objects.create(incident=instance, actor=user, timestamp=timezone.now(), description=description)
+
         for tag_relation in remove_tag_relations:
             tag_relation.delete()
             # XXX: remove tag object as well if no incident is connected to it?
 
         for tag in add_tags:
             IncidentTagRelation.objects.create(tag=tag, incident=instance, added_by=user)
 
@@ -283,19 +290,28 @@
         if user.is_end_user and "timestamp" not in data:
             data["timestamp"] = timezone.now()
         return super().to_internal_value(data)
 
     def to_representation(self, instance: Event):
         event_repr = super().to_representation(instance)
 
-        type_tuples = [
-            ("value", instance.type),
-            ("display", instance.get_type_display()),
-        ]
+        if isinstance(instance, Event):
+            type_tuples = [
+                ("value", instance.type),
+                ("display", instance.get_type_display()),
+            ]
+        else:
+            # Specific case for bulk operations
+            type_tuples = [
+                ("value", instance["type"]),
+                ("display", dict(Event.type.field.choices)[instance["type"]]),
+            ]
+
         event_repr["type"] = OrderedDict(type_tuples)
+
         return event_repr
 
 
 class UpdateAcknowledgementSerializer(serializers.ModelSerializer):
     _later_than_func = timezone.now
 
     class Meta:
@@ -363,7 +379,16 @@
         return value
 
     def validate(self, attrs: dict):
         expiration = attrs.get("expiration")
         if expiration and expiration <= attrs["event"]["timestamp"]:
             raise serializers.ValidationError("'expiration' is earlier than creation timestamp.")
         return attrs
+
+
+class RequestBulkAcknowledgementSerializer(serializers.Serializer):
+    ids = serializers.ListField(child=serializers.IntegerField(), allow_empty=False)
+    ack = AcknowledgementSerializer()
+
+
+class ResponseBulkSerializer(serializers.Serializer):
+    changes = serializers.JSONField()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `argus-server-1.8.1/src/argus/incident/templates/incident/admin/widgets/split_datetime_infinity.html` & `argus-server-1.9.0/src/argus/incident/templates/incident/admin/widgets/split_datetime_infinity.html`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/urls.py` & `argus-server-1.9.0/src/argus/incident/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 
 all_events_list = views.AllEventsViewSet.as_view({"get": "list"})
 event_list = views.EventViewSet.as_view({"get": "list", "post": "create"})
 event_detail = views.EventViewSet.as_view({"get": "retrieve"})
 
 ack_list = views.AcknowledgementViewSet.as_view({"get": "list", "post": "create"})
 ack_detail = views.AcknowledgementViewSet.as_view({"get": "retrieve", "put": "update", "patch": "partial_update"})
+acks_bulk_list = views.BulkAcknowledgementViewSet.as_view({"post": "create"})
 
 tag_list = views.IncidentTagViewSet.as_view({"get": "list", "post": "create"})
 tag_detail = views.IncidentTagViewSet.as_view({"get": "retrieve", "delete": "destroy"})
 
 app_name = "incident"
 urlpatterns = [
+    path("acks/bulk/", acks_bulk_list, name="incident-acks-bulk"),
     path("events/", all_events_list, name="events"),
     path("mine/", sourced_incident_list, name="source_locked_incidents"),
     path("<int:incident_pk>/events/", event_list, name="incident-events"),
     path("<int:incident_pk>/events/<int:pk>/", event_detail, name="incident-event"),
     path("<int:incident_pk>/acks/", ack_list, name="incident-acks"),
     path("<int:incident_pk>/acks/<int:pk>/", ack_detail, name="incident-ack"),
     path("<int:incident_pk>/tags/", tag_list, name="incident-tags"),
```

### Comparing `argus-server-1.8.1/src/argus/incident/validators.py` & `argus-server-1.9.0/src/argus/incident/validators.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/incident/views.py` & `argus-server-1.9.0/src/argus/incident/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,41 +4,44 @@
 
 from django_filters import rest_framework as filters
 from rest_framework.filters import SearchFilter
 from drf_spectacular.types import OpenApiTypes
 from drf_spectacular.utils import extend_schema, extend_schema_view, OpenApiParameter
 from rest_framework import generics, mixins, serializers, status, viewsets
 from rest_framework.decorators import action
-from rest_framework.exceptions import NotFound
+from rest_framework.exceptions import NotFound, ValidationError
 from rest_framework.generics import get_object_or_404
 from rest_framework.pagination import CursorPagination
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.reverse import reverse
 
 from argus.auth.models import User
 from argus.drf.permissions import IsSuperuserOrReadOnly
 from argus.util.datetime_utils import INFINITY_REPR
 
 from .forms import AddSourceSystemForm
 from .filters import IncidentFilter, SourceLockedIncidentFilter
 from .models import (
+    Acknowledgement,
     Event,
     Incident,
     SourceSystem,
     SourceSystemType,
     Tag,
 )
 from .serializers import (
     UpdateAcknowledgementSerializer,
     AcknowledgementSerializer,
     EventSerializer,
     IncidentPureDeserializer,
     IncidentSerializer,
     IncidentTicketUrlSerializer,
+    RequestBulkAcknowledgementSerializer,
+    ResponseBulkSerializer,
     SourceSystemSerializer,
     SourceSystemTypeSerializer,
     TagSerializer,
     IncidentTagRelation,
 )
 
 
@@ -104,14 +107,19 @@
     list=extend_schema(
         parameters=[
             OpenApiParameter(
                 name="acked",
                 description="Fetch acked (`true`) or unacked (`false`) incidents.",
                 enum=BooleanStringOAEnum,
             ),
+            OpenApiParameter(
+                name="duration__gte",
+                description="Fetch incidents with a duration longer of equal to `DURATION` minutes",
+                type=int,
+            ),
             OpenApiParameter(name="cursor", description="The pagination cursor value.", type=str),
             OpenApiParameter(
                 name="end_time__gte",
                 description="Fetch incidents that ended on or after `END_TIME`",
                 type=OpenApiTypes.DATETIME,
             ),
             OpenApiParameter(
@@ -231,15 +239,14 @@
     @action(detail=True, methods=["put"])
     def ticket_url(self, request, pk=None):
         incident = self.get_object()
         serializer = IncidentTicketUrlSerializer(data=request.data)
         if serializer.is_valid():
             incident.ticket_url = serializer.data["ticket_url"]
             incident.save()
-            # TODO: make argus stateless incident about the url being saved? event?
             return Response(serializer.data)
         else:
             return Response(serializer.errors, status=status.HTTP_400_BAD_REQUEST)
 
 
 class IncidentTagViewSet(
     mixins.ListModelMixin,
@@ -267,15 +274,15 @@
         assert lookup_url_kwarg in self.kwargs, (
             "Expected view %s to be called with a URL keyword argument "
             'named "%s". Fix your URL conf, or set the `.lookup_field` '
             "attribute on the view correctly." % (self.__class__.__name__, lookup_url_kwarg)
         )
         try:
             key, value = Tag.split(self.kwargs[lookup_url_kwarg])
-        except ValueError as e:
+        except (ValueError, ValidationError) as e:
             # Not a valid tag. Misses the delimiter, or multiple delimiters
             raise NotFound(str(e))
         filter_kwargs = {"key": key, "value": value}
         obj = get_object_or_404(queryset, **filter_kwargs)
 
         self.check_object_permissions(self.request, obj)
         return obj
@@ -442,7 +449,67 @@
     def get_queryset(self):
         return self.get_incident().acks
 
     def perform_create(self, serializer: AcknowledgementSerializer):
         user = self.request.user
         incident = self.get_incident()
         serializer.save(incident=incident, actor=user)
+
+
+@extend_schema_view(
+    create=extend_schema(
+        request=RequestBulkAcknowledgementSerializer,
+        responses=ResponseBulkSerializer,
+    )
+)
+class BulkAcknowledgementViewSet(viewsets.ViewSet):
+    permission_classes = [IsAuthenticated]
+    serializer_class = ResponseBulkSerializer
+    write_serializer_class = RequestBulkAcknowledgementSerializer
+    queryset = Incident.objects.all()
+
+    def create(self, request):
+        serializer = self.write_serializer_class(data=request.data, context={"request": request})
+
+        if not serializer.is_valid():
+            return Response(data=serializer.errors, status=status.HTTP_400_BAD_REQUEST)
+
+        incident_ids = serializer.data["ids"]
+        ack_data = serializer.data["ack"]
+        actor = request.user
+
+        incidents = {i.id: i for i in self.queryset.filter(pk__in=incident_ids)}
+        changes = {}
+        status_codes_seen = set()
+
+        for incident_id in incident_ids:
+            incident = incidents.get(incident_id)
+
+            if not incident:
+                changes[str(incident_id)] = {
+                    "ack": None,
+                    "status": status.HTTP_400_BAD_REQUEST,
+                    "errors": {"ids": f"Incident with id {incident_id} could not be found."},
+                }
+                status_codes_seen.add(status.HTTP_400_BAD_REQUEST)
+                continue
+
+            event = Event.objects.create(
+                incident=incident,
+                actor=actor,
+                timestamp=ack_data["event"]["timestamp"],
+                type=Event.Type.ACKNOWLEDGE,
+                description=ack_data["event"]["description"],
+            )
+            ack = Acknowledgement.objects.create(event=event, expiration=ack_data["expiration"])
+            changes[str(incident_id)] = {
+                "ack": AcknowledgementSerializer(instance=ack).to_representation(instance=ack),
+                "status": status.HTTP_201_CREATED,
+                "errors": None,
+            }
+            status_codes_seen.add(status.HTTP_201_CREATED)
+
+        all_bad = status_codes_seen == set((status.HTTP_400_BAD_REQUEST,))
+
+        return Response(
+            data={"changes": changes}, status=status.HTTP_400_BAD_REQUEST if all_bad else status.HTTP_201_CREATED
+        )
```

### Comparing `argus-server-1.8.1/src/argus/incident/widgets.py` & `argus-server-1.9.0/src/argus/incident/widgets.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/V1/serializers.py` & `argus-server-1.9.0/src/argus/notificationprofile/V1/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,20 @@
         profile.destinations.set(destinations)
         return profile
 
     def update(self, instance: NotificationProfile, validated_data: dict):
         phone_number = validated_data.pop("phone_number", None)
         media = validated_data.pop("media", None)
 
-        # Update media
-        if media:
+        # Update media to be empty
+        if media == set():
+            instance.destinations.set([])
+
+        # Update media to not be empty
+        if "SM" in media or "EM" in media:
             if "SM" in media and "EM" not in media:
                 email_destinations = instance.destinations.filter(media_id="email")
                 instance.destinations.remove(*email_destinations)
 
             if "EM" in media:
                 if not instance.user.email and not instance.destinations.filter(media_id="email").exists():
                     raise serializers.ValidationError(
```

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/V1/views.py` & `argus-server-1.9.0/src/argus/notificationprofile/V1/views.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/admin.py` & `argus-server-1.9.0/src/argus/notificationprofile/admin.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/apps.py` & `argus-server-1.9.0/src/argus/notificationprofile/apps.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/checks.py` & `argus-server-1.9.0/src/argus/notificationprofile/checks.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/factories.py` & `argus-server-1.9.0/src/argus/notificationprofile/factories.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 class TimeslotFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = models.Timeslot
 
     user = factory.SubFactory(PersonUserFactory)
-    name = factory.Faker("word")
+    name = factory.Sequence(lambda s: "Timeslot %s" % s)
 
 
 class TimeRecurrenceFactory(factory.django.DjangoModelFactory):
     "A random TimeRecurrence"
 
     class Meta:
         model = models.TimeRecurrence
@@ -56,15 +56,15 @@
     days = list(range(1, 7 + 1))
 
 
 class MediaFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = models.Media
 
-    slug = factory.Faker("word")
+    slug = factory.Sequence(lambda s: "Media %s" % s)
     name = factory.LazyAttribute(lambda obj: obj.slug.capitalize())
 
 
 class DestinationConfigFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = models.DestinationConfig
 
@@ -82,9 +82,9 @@
 
 
 class FilterFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = models.Filter
 
     user = factory.SubFactory(PersonUserFactory)
-    name = factory.Faker("word")
+    name = factory.Sequence(lambda s: "Filter %s" % s)
     filter_string = '{"sourceSystemIds": [], "tags": []}'
```

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/media/__init__.py` & `argus-server-1.9.0/src/argus/notificationprofile/media/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from multiprocessing import Process
 from typing import TYPE_CHECKING
 
 from django.conf import settings
 from django.db import connections
 
 from ..models import NotificationProfile
+from argus.util.utils import import_class_from_dotted_path
 
 if TYPE_CHECKING:
     from typing import List
 
     from argus.incident.models import Event  # noqa: Break circular import
 
     from ..models import DestinationConfig
@@ -23,25 +24,18 @@
 __all__ = [
     "send_notifications_to_users",
     "background_send_notifications_to_users",
     "send_notification",
     "get_notification_media",
 ]
 
-# Import media classes
-def _import_class_from_dotted_path(dotted_path: str):
-    module_name, class_name = dotted_path.rsplit(".", 1)
-    module = importlib.import_module(module_name)
-    class_ = getattr(module, class_name)
-    return class_
-
 
 # TODO: Raise Incident if media_class not importable?
 MEDIA_PLUGINS = getattr(settings, "MEDIA_PLUGINS")
-MEDIA_CLASSES = [_import_class_from_dotted_path(media_plugin) for media_plugin in MEDIA_PLUGINS]
+MEDIA_CLASSES = [import_class_from_dotted_path(media_plugin) for media_plugin in MEDIA_PLUGINS]
 MEDIA_CLASSES_DICT = {media_class.MEDIA_SLUG: media_class for media_class in MEDIA_CLASSES}
 
 
 def send_notifications_to_users(event: Event):
     if not getattr(settings, "SEND_NOTIFICATIONS", False):
         LOG.info('Notification: turned off sitewide, not sending for "%s"', event)
         return
```

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/media/base.py` & `argus-server-1.9.0/src/argus/notificationprofile/media/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from django.db.models.query import QuerySet
 
 if TYPE_CHECKING:
     from types import NoneType
     from typing import Union
     from django.db.models.query import QuerySet
+    from argus.auth.models import User
     from argus.incident.models import Event
     from ..models import DestinationConfig
     from ..serializers import RequestDestinationConfigSerializer
 
 
 __all__ = ["NotificationMedium"]
 
@@ -22,15 +23,15 @@
         """
         Custom exception class that is raised when a destination cannot be
         deleted
         """
 
     @classmethod
     @abstractmethod
-    def validate(cls, instance: RequestDestinationConfigSerializer, dict: dict) -> dict:
+    def validate(cls, instance: RequestDestinationConfigSerializer, dict: dict, user: User) -> dict:
         """
         Validates the settings of destination and returns a dict with
         validated and cleaned data
         """
         pass
 
     @classmethod
```

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/media/email.py` & `argus-server-1.9.0/src/argus/notificationprofile/media/email.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .base import NotificationMedium
 from ..models import DestinationConfig
 
 if TYPE_CHECKING:
     from types import NoneType
     from typing import Union
     from django.db.models.query import QuerySet
+    from argus.auth.models import User
     from ..serializers import RequestDestinationConfigSerializer
 
 LOG = logging.getLogger(__name__)
 
 __all__ = [
     "send_email_safely",
     "EmailNotification",
@@ -63,24 +64,28 @@
     }
 
     class Form(forms.Form):
         synced = forms.BooleanField(disabled=True, required=False, initial=False)
         email_address = forms.EmailField()
 
     @classmethod
-    def validate(cls, instance: RequestDestinationConfigSerializer, email_dict: dict) -> dict:
+    def validate(cls, instance: RequestDestinationConfigSerializer, email_dict: dict, user: User) -> dict:
         """
         Validates the settings of an email destination and returns a dict
         with validated and cleaned data
         """
         form = cls.Form(email_dict["settings"])
         if not form.is_valid():
             raise ValidationError(form.errors)
         if form.cleaned_data["email_address"] == instance.context["request"].user.email:
             raise ValidationError("This email address is already registered in another destination.")
+        if user.destinations.filter(
+            media_id="email", settings__email_address=form.cleaned_data["email_address"]
+        ).exists():
+            raise ValidationError({"email_address": "Email address already exists"})
 
         return form.cleaned_data
 
     @classmethod
     def raise_if_not_deletable(cls, destination: DestinationConfig) -> Union[str, NoneType]:
         """
         Raises a NotDeletableError if the given email destination is not able
```

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/media/sms_as_email.py` & `argus-server-1.9.0/src/argus/notificationprofile/media/sms_as_email.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from ...incident.models import Event
 from .base import NotificationMedium
 from .email import send_email_safely
 
 if TYPE_CHECKING:
     from django.db.models.query import QuerySet
+    from argus.auth.models import User
     from ..models import DestinationConfig
     from ..serializers import RequestDestinationConfigSerializer
 
 LOG = logging.getLogger(__name__)
 
 
 class SMSNotification(NotificationMedium):
@@ -43,25 +44,28 @@
         },
     }
 
     class PhoneNumberForm(forms.Form):
         phone_number = PhoneNumberField()
 
     @classmethod
-    def validate(cls, instance: RequestDestinationConfigSerializer, sms_dict: dict) -> dict:
+    def validate(cls, instance: RequestDestinationConfigSerializer, sms_dict: dict, user: User) -> dict:
         """
         Validates the settings of an SMS destination and returns a dict
         with validated and cleaned data
         """
         form = cls.PhoneNumberForm(sms_dict["settings"])
         if not form.is_valid():
             raise ValidationError(form.errors)
 
         form.cleaned_data["phone_number"] = form.cleaned_data["phone_number"].as_e164
 
+        if user.destinations.filter(media_id="sms", settings__phone_number=form.cleaned_data["phone_number"]).exists():
+            raise ValidationError({"phone_number": "Phone number already exists"})
+
         return form.cleaned_data
 
     @staticmethod
     def get_label(destination: DestinationConfig) -> str:
         """
         Returns the phone number represented by this SMS destination
         """
```

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/migrations/0001_initial.py` & `argus-server-1.9.0/src/argus/notificationprofile/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/migrations/0004_copy_notificationprofile_media_to_media_v1.py` & `argus-server-1.9.0/src/argus/notificationprofile/migrations/0004_copy_notificationprofile_media_to_media_v1.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/migrations/0005_destinationconfig_media.py` & `argus-server-1.9.0/src/argus/notificationprofile/migrations/0005_destinationconfig_media.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/migrations/0006_related_name_destinations.py` & `argus-server-1.9.0/src/argus/notificationprofile/migrations/0006_related_name_destinations.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/migrations/0007_copy_phone_number_from_destinations.py` & `argus-server-1.9.0/src/argus/notificationprofile/migrations/0007_copy_phone_number_from_destinations.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/migrations/0008_remove_media_phone_number.py` & `argus-server-1.9.0/src/argus/notificationprofile/migrations/0008_remove_media_phone_number.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/migrations/0009_notificationprofile_id.py` & `argus-server-1.9.0/src/argus/notificationprofile/migrations/0009_notificationprofile_id.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/migrations/0010_notificationprofile_id.py` & `argus-server-1.9.0/src/argus/notificationprofile/migrations/0010_notificationprofile_id.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/models.py` & `argus-server-1.9.0/src/argus/notificationprofile/models.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/primitive_serializers.py` & `argus-server-1.9.0/src/argus/notificationprofile/primitive_serializers.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/serializers.py` & `argus-server-1.9.0/src/argus/notificationprofile/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,18 +151,24 @@
             "settings",
         ]
 
     def validate(self, attrs: dict):
         if self.instance and "media" in attrs.keys() and not attrs["media"].slug == self.instance.media.slug:
             raise serializers.ValidationError("Media cannot be updated, only settings.")
         if "settings" in attrs.keys():
+            if type(attrs["settings"]) != dict:
+                raise serializers.ValidationError("Settings has to be a dictionary.")
             if self.instance:
-                attrs["settings"] = MEDIA_CLASSES_DICT[self.instance.media.slug].validate(self, attrs)
+                attrs["settings"] = MEDIA_CLASSES_DICT[self.instance.media.slug].validate(
+                    self, attrs, self.context["request"].user
+                )
             else:
-                attrs["settings"] = MEDIA_CLASSES_DICT[attrs["media"].slug].validate(self, attrs)
+                attrs["settings"] = MEDIA_CLASSES_DICT[attrs["media"].slug].validate(
+                    self, attrs, self.context["request"].user
+                )
 
         return attrs
 
     def update(self, destination: DestinationConfig, validated_data: dict):
         updated_destination = MEDIA_CLASSES_DICT[destination.media.slug].update(destination, validated_data)
 
         if updated_destination:
```

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/signals.py` & `argus-server-1.9.0/src/argus/notificationprofile/signals.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/templates/notificationprofile/email.html` & `argus-server-1.9.0/src/argus/notificationprofile/templates/notificationprofile/email.html`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/urls.py` & `argus-server-1.9.0/src/argus/notificationprofile/urls.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/validators.py` & `argus-server-1.9.0/src/argus/notificationprofile/validators.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/notificationprofile/views.py` & `argus-server-1.9.0/src/argus/notificationprofile/views.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/site/api_v1_urls.py` & `argus-server-1.9.0/src/argus/site/api_v1_urls.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/site/api_v2_urls.py` & `argus-server-1.9.0/src/argus/site/api_v2_urls.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/site/logging.py` & `argus-server-1.9.0/src/argus/site/logging.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/site/settings/__init__.py` & `argus-server-1.9.0/src/argus/site/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/site/settings/base.py` & `argus-server-1.9.0/src/argus/site/settings/base.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/site/settings/dev.py` & `argus-server-1.9.0/src/argus/site/settings/dev.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/site/settings/prod.py` & `argus-server-1.9.0/src/argus/site/settings/prod.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/site/settings/test_CI.py` & `argus-server-1.9.0/src/argus/site/settings/test_CI.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/site/urls.py` & `argus-server-1.9.0/src/argus/site/urls.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/site/views.py` & `argus-server-1.9.0/src/argus/site/views.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/util/admin_utils.py` & `argus-server-1.9.0/src/argus/util/admin_utils.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/util/datetime_utils.py` & `argus-server-1.9.0/src/argus/util/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/util/utils.py` & `argus-server-1.9.0/src/argus/util/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import importlib
+
 from django.db.models import Model
 
 
 def duplicate(obj: Model, **set_attrs):
     obj_copy = obj._meta.model.objects.get(pk=obj.pk)
     obj_copy.pk = None
     for attr, value in set_attrs.items():
@@ -33,7 +35,14 @@
         for attr_name in self._attr_names:
             obj_attr = getattr(obj_attr, attr_name)
         return obj_attr
 
     @property
     def query(self):
         return self._attr_query
+
+
+def import_class_from_dotted_path(dotted_path: str):
+    module_name, class_name = dotted_path.rsplit(".", 1)
+    module = importlib.import_module(module_name)
+    class_ = getattr(module, class_name)
+    return class_
```

### Comparing `argus-server-1.8.1/src/argus/ws/asgi.py` & `argus-server-1.9.0/src/argus/ws/asgi.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/ws/consumers.py` & `argus-server-1.9.0/src/argus/ws/consumers.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus/ws/models.py` & `argus-server-1.9.0/src/argus/ws/models.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/src/argus_server.egg-info/PKG-INFO` & `argus-server-1.9.0/src/argus_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argus-server
-Version: 1.8.1
+Version: 1.9.0
 Summary: Argus is an alert aggregator for monitoring systems
 Author-email: Uninett Opensource <opensource@uninett.no>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/Uninett/Argus
 Platform: any
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `argus-server-1.8.1/src/argus_server.egg-info/SOURCES.txt` & `argus-server-1.9.0/src/argus_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
 CONTRIBUTORS.md
 Dockerfile
 LICENSE
 MANIFEST.in
+Makefile
 NOTES.md
 README.md
 UPGRADING.md
 cmd.sh-template
 codecov.yml
 docker-compose.yml
 docker-entrypoint.sh
@@ -176,23 +177,25 @@
 src/argus_server.egg-info/dependency_links.txt
 src/argus_server.egg-info/not-zip-safe
 src/argus_server.egg-info/requires.txt
 src/argus_server.egg-info/top_level.txt
 tests/__init__.py
 tests/auth/__init__.py
 tests/auth/test_auth.py
+tests/auth/test_views.py
+tests/auth/V1/test_views.py
 tests/incident/__init__.py
+tests/incident/test_change_event.py
 tests/incident/test_event.py
 tests/incident/test_filters.py
 tests/incident/test_incident_fields.py
 tests/incident/test_queryset.py
 tests/incident/test_serializers.py
 tests/incident/test_source_system.py
 tests/incident/test_source_system_type.py
-tests/incident/test_tags.py
 tests/incident/test_views.py
 tests/incident/fixtures/__init__.py
 tests/incident/unit/__init__.py
 tests/incident/unit/test_incident_details_url.py
 tests/notificationprofile/__init__.py
 tests/notificationprofile/test_github236.py
 tests/notificationprofile/test_media.py
```

### Comparing `argus-server-1.8.1/src/argus_server.egg-info/requires.txt` & `argus-server-1.9.0/src/argus_server.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/auth/test_auth.py` & `argus-server-1.9.0/tests/auth/test_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,7 +143,14 @@
             self.assertEqual(response_data["username"], user.username)
             self.assertIn("first_name", response_data)
             self.assertIn("last_name", response_data)
             self.assertIn("email", response_data)
 
         assert_correct_fields_for_user(self.normal_user1)
         assert_correct_fields_for_user(self.superuser1)
+
+    def test_refresh_token_returns_correct_new_token(self):
+        auth_token_path = reverse("v2:auth:refresh-token")
+        response = self.normal_user1_client.post(auth_token_path)
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+        self.assertNotEqual(response.data["token"], self.normal_user1_token.key)
+        self.assertEqual(response.data["token"], Token.objects.get(user=self.normal_user1).key)
```

### Comparing `argus-server-1.8.1/tests/incident/__init__.py` & `argus-server-1.9.0/tests/incident/__init__.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/incident/test_event.py` & `argus-server-1.9.0/tests/incident/test_event.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/incident/test_incident_fields.py` & `argus-server-1.9.0/tests/incident/test_incident_fields.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/incident/test_queryset.py` & `argus-server-1.9.0/tests/incident/test_queryset.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/incident/test_serializers.py` & `argus-server-1.9.0/tests/incident/test_serializers.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/incident/test_source_system.py` & `argus-server-1.9.0/tests/incident/test_source_system.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/incident/test_source_system_type.py` & `argus-server-1.9.0/tests/incident/test_source_system_type.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/incident/unit/test_incident_details_url.py` & `argus-server-1.9.0/tests/incident/unit/test_incident_details_url.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/notificationprofile/__init__.py` & `argus-server-1.9.0/tests/notificationprofile/__init__.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/notificationprofile/test_github236.py` & `argus-server-1.9.0/tests/notificationprofile/test_github236.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/notificationprofile/test_models.py` & `argus-server-1.9.0/tests/notificationprofile/test_models.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/notificationprofile/test_serializers.py` & `argus-server-1.9.0/tests/notificationprofile/test_serializers.py`

 * *Files identical despite different names*

### Comparing `argus-server-1.8.1/tests/notificationprofile/test_signals.py` & `argus-server-1.9.0/tests/notificationprofile/test_signals.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def test_default_email_destination_should_be_created_if_user_has_email(self):
         # PersonUserFactory creates user with email address
         default_destination = self.user1.destinations.first()
         self.assertTrue(default_destination)
         self.assertTrue(default_destination.settings["synced"])
 
     def test_default_email_destination_should_not_be_created_if_user_has_no_email(self):
-        self.assertFalse(self.user2.destinations.exists())
+        self.assertFalse(self.user2.destinations.filter(media_id="email", settings__synced=True).exists())
 
     def test_default_email_destination_should_be_added_if_email_is_added_to_user(self):
         self.user2.email = self.user2.username
         self.user2.save(update_fields=["email"])
         default_destination = self.user2.destinations.first()
         self.assertTrue(default_destination)
         self.assertTrue(default_destination.settings["synced"])
```

### Comparing `argus-server-1.8.1/tests/notificationprofile/test_views.py` & `argus-server-1.9.0/tests/notificationprofile/test_views.py`

 * *Files 12% similar despite different names*

```diff
@@ -110,14 +110,36 @@
                 settings={
                     "email_address": "test2@example.com",
                     "synced": False,
                 },
             ).exists()
         )
 
+    def test_cannot_create_email_destination_with_duplicate_email_address(self):
+        settings = {"email_address": "test2@example.com"}
+        DestinationConfigFactory(
+            user=self.user1,
+            media=Media.objects.get(slug="email"),
+            settings=settings,
+        )
+        response = self.user1_rest_client.post(
+            path="/api/v2/notificationprofiles/destinations/",
+            data={
+                "media": "email",
+                "settings": settings,
+            },
+        )
+        self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
+        self.assertEqual(
+            DestinationConfig.objects.filter(
+                media_id="email", settings__email_address=settings["email_address"]
+            ).count(),
+            1,
+        )
+
     def test_can_create_sms_destination_with_valid_values(self):
         response = self.user1_rest_client.post(
             path="/api/v2/notificationprofiles/destinations/",
             data={
                 "media": "sms",
                 "settings": {
                     "phone_number": "+4747474740",
@@ -129,14 +151,31 @@
             DestinationConfig.objects.filter(
                 settings={
                     "phone_number": "+4747474740",
                 },
             ).exists()
         )
 
+    def test_cannot_create_sms_destination_with_duplicate_phone_number(self):
+        settings = {"phone_number": "+4747474701"}
+        DestinationConfigFactory(
+            user=self.user1,
+            media=Media.objects.get(slug="sms"),
+            settings=settings,
+        )
+        response = self.user1_rest_client.post(
+            path="/api/v2/notificationprofiles/destinations/",
+            data={
+                "media": "sms",
+                "settings": settings,
+            },
+        )
+        self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
+        self.assertEqual(DestinationConfig.objects.filter(media_id="sms", settings=settings).count(), 1)
+
     def test_can_update_email_destination_with_same_medium(self):
         email_destination = self.non_synced_email_destination
         new_settings = {
             "email_address": "test2@example.com",
         }
         response = self.user1_rest_client.patch(
             path=f"/api/v2/notificationprofiles/destinations/{email_destination.pk}/",
@@ -148,14 +187,30 @@
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         email_destination.refresh_from_db()
         self.assertEqual(
             email_destination.settings["email_address"],
             new_settings["email_address"],
         )
 
+    def test_cannot_update_email_destination_with_duplicate_email_address(self):
+        settings = {"email_address": "test2@example.com"}
+        email_destination_pk = DestinationConfigFactory(
+            user=self.user1,
+            media=Media.objects.get(slug="email"),
+            settings=settings,
+        ).pk
+        response = self.user1_rest_client.patch(
+            path=f"/api/v2/notificationprofiles/destinations/{email_destination_pk}/",
+            data={"settings": {"email_address": self.non_synced_email_destination.settings["email_address"]}},
+        )
+        self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
+        self.assertEqual(
+            DestinationConfig.objects.get(pk=email_destination_pk).settings["email_address"], settings["email_address"]
+        )
+
     def test_can_update_sms_destination_with_same_medium(self):
         sms_destination = self.sms_destination
         new_settings = {
             "phone_number": "+4747474746",
         }
         response = self.user1_rest_client.patch(
             path=f"/api/v2/notificationprofiles/destinations/{sms_destination.pk}/",
@@ -167,47 +222,61 @@
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         sms_destination.refresh_from_db()
         self.assertEqual(
             sms_destination.settings,
             new_settings,
         )
 
+    def test_cannot_update_sms_destination_with_duplicate_phone_number(self):
+        settings1 = {"phone_number": "+4747474701"}
+        settings2 = {"phone_number": "+4747474702"}
+        DestinationConfigFactory(
+            user=self.user1,
+            media=Media.objects.get(slug="sms"),
+            settings=settings1,
+        )
+        sms_destination_pk = DestinationConfigFactory(
+            user=self.user1,
+            media=Media.objects.get(slug="sms"),
+            settings=settings2,
+        ).pk
+        response = self.user1_rest_client.patch(
+            path=f"/api/v2/notificationprofiles/destinations/{sms_destination_pk}/", data={"settings": settings1}
+        )
+        self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
+        self.assertEqual(DestinationConfig.objects.get(pk=sms_destination_pk).settings, settings2)
+
     def test_can_delete_sms_destination(self):
-        self.assertTrue(DestinationConfig.objects.filter(media_id="sms").exists())
         response = self.user1_rest_client.delete(
             path=f"/api/v2/notificationprofiles/destinations/{self.sms_destination.pk}/"
         )
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
-        self.assertFalse(DestinationConfig.objects.filter(media_id="sms").exists())
+        self.assertFalse(DestinationConfig.objects.filter(id=self.sms_destination.pk).exists())
 
     def test_can_delete_unsynced_unconnected_email_destination(self):
-        self.assertTrue(DestinationConfig.objects.filter(media_id="email").filter(settings__synced=False).exists())
         response = self.user1_rest_client.delete(
             path=f"/api/v2/notificationprofiles/destinations/{self.non_synced_email_destination.pk}/"
         )
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
-        self.assertFalse(DestinationConfig.objects.filter(media_id="email").filter(settings__synced=False).exists())
+        self.assertFalse(DestinationConfig.objects.filter(id=self.non_synced_email_destination.pk).exists())
 
     def test_cannot_delete_synced_email_destination(self):
-        self.assertTrue(DestinationConfig.objects.filter(media_id="email").filter(settings__synced=True).exists())
         response = self.user1_rest_client.delete(
             path=f"/api/v2/notificationprofiles/destinations/{self.synced_email_destination.pk}/"
         )
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
-        self.assertTrue(DestinationConfig.objects.filter(media_id="email").filter(settings__synced=True).exists())
+        self.assertTrue(DestinationConfig.objects.filter(id=self.synced_email_destination.pk).exists())
 
     def test_cannot_delete_connected_email_destination(self):
         self.notification_profile1.destinations.add(self.non_synced_email_destination)
-
-        self.assertTrue(DestinationConfig.objects.filter(media_id="email").filter(settings__synced=False).exists())
         response = self.user1_rest_client.delete(
             path=f"/api/v2/notificationprofiles/destinations/{self.non_synced_email_destination.pk}/"
         )
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
-        self.assertTrue(DestinationConfig.objects.filter(media_id="email").filter(settings__synced=False).exists())
+        self.assertTrue(DestinationConfig.objects.filter(id=self.non_synced_email_destination.pk).exists())
 
     def test_can_get_all_media(self):
         response = self.user1_rest_client.get(path=f"/api/v2/notificationprofiles/media/")
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         self.assertEqual(len(response.data), 2)
         self.assertEqual(set([medium["slug"] for medium in response.data]), set(["sms", "email"]))
```

### Comparing `argus-server-1.8.1/tox.ini` & `argus-server-1.9.0/tox.ini`

 * *Files identical despite different names*

