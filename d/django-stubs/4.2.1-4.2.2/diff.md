# Comparing `tmp/django-stubs-4.2.1.tar.gz` & `tmp/django-stubs-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stubs-4.2.1.tar", last modified: Fri Jun  2 14:11:31 2023, max compression
+gzip compressed data, was "django-stubs-4.2.2.tar", last modified: Tue Jun 27 17:51:06 2023, max compression
```

## Comparing `django-stubs-4.2.1.tar` & `django-stubs-4.2.2.tar`

### file list

```diff
@@ -1,833 +1,837 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.264431 django-stubs-4.2.1/
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-06-02 14:08:54.000000 django-stubs-4.2.1/LICENSE.md
--rw-r--r--   0 marti     (1000) marti      (121)    13907 2023-06-02 14:11:31.264431 django-stubs-4.2.1/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)    12832 2023-06-02 14:08:54.000000 django-stubs-4.2.1/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.141099 django-stubs-4.2.1/django-stubs/
--rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.141099 django-stubs-4.2.1/django-stubs/apps/
--rw-r--r--   0 marti     (1000) marti      (121)       78 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/apps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      855 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/apps/config.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1963 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/apps/registry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.141099 django-stubs-4.2.1/django-stubs/conf/
--rw-r--r--   0 marti     (1000) marti      (121)     1453 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/conf/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    16655 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/conf/global_settings.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.141099 django-stubs-4.2.1/django-stubs/conf/locale/
--rw-r--r--   0 marti     (1000) marti      (121)       50 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/conf/locale/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.144432 django-stubs-4.2.1/django-stubs/conf/urls/
--rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/conf/urls/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      231 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/conf/urls/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/conf/urls/static.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.144432 django-stubs-4.2.1/django-stubs/contrib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.147765 django-stubs-4.2.1/django-stubs/contrib/admin/
--rw-r--r--   0 marti     (1000) marti      (121)     1157 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      313 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/actions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2208 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3887 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/filters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      237 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5562 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/helpers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.147765 django-stubs-4.2.1/django-stubs/contrib/admin/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1032 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    16126 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4087 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/admin/sites.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.147765 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1981 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/admin_list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      690 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/admin_modify.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      503 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/admin_urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      605 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/log.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1629 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/tests.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3665 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/admin/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.147765 django-stubs-4.2.1/django-stubs/contrib/admin/views/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/views/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      374 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/views/autocomplete.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      383 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/views/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3104 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/views/main.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5670 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/admin/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.147765 django-stubs-4.2.1/django-stubs/contrib/admindocs/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      478 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/middleware.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1018 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/auth/
--rw-r--r--   0 marti     (1000) marti      (121)     1272 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1891 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/backends.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1532 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/base_user.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      662 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      934 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3944 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/auth/forms.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/auth/handlers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/handlers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/handlers/modwsgi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1962 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/hashers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/auth/management/
--rw-r--r--   0 marti     (1000) marti      (121)      405 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/auth/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      125 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/management/commands/changepassword.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/auth/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1228 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4613 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/contrib/auth/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2081 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/password_validation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      735 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/auth/tokens.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      153 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2387 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/contenttypes/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      655 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       76 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      414 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3850 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1420 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/forms.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/
--rw-r--r--   0 marti     (1000) marti      (121)     1297 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/contenttypes/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1020 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.161098 django-stubs-4.2.1/django-stubs/contrib/flatpages/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.161098 django-stubs-4.2.1/django-stubs/contrib/flatpages/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      402 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       81 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/sitemaps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.161098 django-stubs-4.2.1/django-stubs/contrib/flatpages/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      484 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.161098 django-stubs-4.2.1/django-stubs/contrib/gis/
--rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.164432 django-stubs-4.2.1/django-stubs/contrib/gis/admin/
--rw-r--r--   0 marti     (1000) marti      (121)      872 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/admin/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1174 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/admin/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      272 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/admin/widgets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       67 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.164432 django-stubs-4.2.1/django-stubs/contrib/gis/db/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.164432 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.164432 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1443 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      836 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1348 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/operations.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.164432 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      251 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      781 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      333 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1134 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      699 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.167765 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      226 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      254 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      444 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      287 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      729 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1440 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.167765 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      399 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      351 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      189 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/const.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      407 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      360 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      798 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2218 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      340 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.167765 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      477 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      127 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      358 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      451 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      808 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1286 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1103 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      656 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.171098 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/
--rw-r--r--   0 marti     (1000) marti      (121)      847 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      800 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/aggregates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6077 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6016 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2955 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/proxy.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.171098 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/sql/
--rw-r--r--   0 marti     (1000) marti      (121)      166 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/sql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/sql/conversion.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      866 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/feeds.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.171098 django-stubs-4.2.1/django-stubs/contrib/gis/forms/
--rw-r--r--   0 marti     (1000) marti      (121)      642 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/forms/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      951 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/forms/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.171098 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/
--rw-r--r--   0 marti     (1000) marti      (121)     1070 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      137 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      574 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/datasource.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      324 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/driver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      688 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/envelope.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/error.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      947 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/feature.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1460 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/field.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4844 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/geometries.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      304 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/geomtype.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1721 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/layer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      510 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/libgdal.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.174432 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1036 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      961 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1077 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      970 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1053 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      614 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.174432 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1594 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/band.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/const.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2180 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/source.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2191 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/srs.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.174432 django-stubs-4.2.1/django-stubs/contrib/gis/geoip2/
--rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geoip2/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1202 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geoip2/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       99 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geoip2/resources.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       97 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geometry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.177765 django-stubs-4.2.1/django-stubs/contrib/gis/geos/
--rw-r--r--   0 marti     (1000) marti      (121)      883 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      604 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/collections.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1250 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/coordseq.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       36 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/error.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      276 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/factory.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5258 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/geometry.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      491 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/io.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      896 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/libgeos.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      766 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/linestring.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/mutable_list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      816 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/point.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      713 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/polygon.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      737 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prepared.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.177765 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/
--rw-r--r--   0 marti     (1000) marti      (121)     4249 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      795 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      474 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      792 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/geom.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/io.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/misc.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      553 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      434 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      609 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/topology.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1418 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/measure.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/ptr.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.177765 django-stubs-4.2.1/django-stubs/contrib/gis/serializers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/serializers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      493 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/serializers/geojson.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      244 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.181098 django-stubs-4.2.1/django-stubs/contrib/gis/sitemaps/
--rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/sitemaps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      328 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/sitemaps/kml.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      352 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/sitemaps/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.181098 django-stubs-4.2.1/django-stubs/contrib/gis/utils/
--rw-r--r--   0 marti     (1000) marti      (121)      436 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2526 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/utils/layermapping.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      153 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/utils/ogrinfo.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      320 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/utils/ogrinspect.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      199 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/utils/srs.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      202 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.181098 django-stubs-4.2.1/django-stubs/contrib/humanize/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/humanize/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/humanize/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.181098 django-stubs-4.2.1/django-stubs/contrib/humanize/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/humanize/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      859 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/humanize/templatetags/humanize.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.181098 django-stubs-4.2.1/django-stubs/contrib/messages/
--rw-r--r--   0 marti     (1000) marti      (121)      715 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1294 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/api.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      349 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.184431 django-stubs-4.2.1/django-stubs/contrib/messages/storage/
--rw-r--r--   0 marti     (1000) marti      (121)      192 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/storage/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      906 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/storage/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      463 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/storage/cookie.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      228 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/storage/fallback.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      468 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/storage/session.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       44 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      347 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.184431 django-stubs-4.2.1/django-stubs/contrib/postgres/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.184431 django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/
--rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      357 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/general.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       29 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      470 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/statistics.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      270 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      846 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/constraints.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.187765 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/
--rw-r--r--   0 marti     (1000) marti      (121)      759 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1897 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/array.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/citext.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      573 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/hstore.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      376 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/jsonb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3038 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/ranges.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.187765 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/
--rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2340 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/array.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      462 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/hstore.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      207 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/jsonb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1486 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/ranges.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3972 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/indexes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      532 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2055 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3627 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/search.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/serializers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      230 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      635 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/validators.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.187765 django-stubs-4.2.1/django-stubs/contrib/redirects/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.187765 django-stubs-4.2.1/django-stubs/contrib/redirects/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      150 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/models.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sessions/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1869 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/cached_db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      508 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      239 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/file.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/signed_cookies.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      676 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/base_session.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/exceptions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sessions/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sessions/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      447 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sessions/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      243 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      337 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/serializers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sitemaps/
--rw-r--r--   0 marti     (1000) marti      (121)     1697 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sitemaps/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sitemaps/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      710 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.194431 django-stubs-4.2.1/django-stubs/contrib/sites/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       69 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      288 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/management.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/managers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      209 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.194431 django-stubs-4.2.1/django-stubs/contrib/sites/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      585 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      292 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/requests.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      221 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.194431 django-stubs-4.2.1/django-stubs/contrib/staticfiles/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      263 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2742 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/finders.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1674 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/handlers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.194431 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.194431 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1055 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       87 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2152 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/storage.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/testing.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.197765 django-stubs-4.2.1/django-stubs/contrib/syndication/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/syndication/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      131 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/syndication/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1924 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/contrib/syndication/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.197765 django-stubs-4.2.1/django-stubs/core/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/asgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.197765 django-stubs-4.2.1/django-stubs/core/cache/
--rw-r--r--   0 marti     (1000) marti      (121)      624 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.197765 django-stubs-4.2.1/django-stubs/core/cache/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4052 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      593 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      204 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/filebased.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      180 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/memcached.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.201098 django-stubs-4.2.1/django-stubs/core/checks/
--rw-r--r--   0 marti     (1000) marti      (121)      652 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/async_checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      529 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/caches.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.201098 django-stubs-4.2.1/django-stubs/core/checks/compatibility/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/compatibility/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      229 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/database.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1084 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/messages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/model_checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1799 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/registry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.201098 django-stubs-4.2.1/django-stubs/core/checks/security/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/security/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1847 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/security/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      399 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/security/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/security/sessions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      407 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/templates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      625 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/translation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      706 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1912 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/exceptions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.204431 django-stubs-4.2.1/django-stubs/core/files/
--rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1606 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      359 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/images.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/locks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      130 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/move.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.204431 django-stubs-4.2.1/django-stubs/core/files/storage/
--rw-r--r--   0 marti     (1000) marti      (121)      634 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      751 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/filesystem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      450 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/handler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      725 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/memory.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      337 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/temp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1459 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/uploadedfile.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3017 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/uploadhandler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      736 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.204431 django-stubs-4.2.1/django-stubs/core/handlers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/handlers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2043 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/handlers/asgi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1220 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/handlers/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      770 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/handlers/exception.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1405 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/handlers/wsgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.204431 django-stubs-4.2.1/django-stubs/core/mail/
--rw-r--r--   0 marti     (1000) marti      (121)     1714 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/mail/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.207765 django-stubs-4.2.1/django-stubs/core/mail/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      668 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      189 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/console.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/filebased.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      395 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/smtp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4639 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/mail/message.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.207765 django-stubs-4.2.1/django-stubs/core/management/
--rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3646 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1099 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/color.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.211098 django-stubs-4.2.1/django-stubs/core/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      179 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/check.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      430 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/compilemessages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/createcachetable.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/dbshell.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      519 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/diffsettings.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      123 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/dumpdata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/flush.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      789 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/inspectdb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1140 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/loaddata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1227 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/makemessages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/makemigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      643 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/migrate.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/runserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      111 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/sendtestemail.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      268 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/shell.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      371 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/showmigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      110 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/sqlflush.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      203 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/sqlmigrate.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       83 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/sqlsequencereset.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      330 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/squashmigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/startapp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/startproject.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/test.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/testserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/sql.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      964 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/templates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      850 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2313 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/paginator.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.211098 django-stubs-4.2.1/django-stubs/core/serializers/
--rw-r--r--   0 marti     (1000) marti      (121)     1437 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3192 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/jsonl.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      490 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/python.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      831 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/pyyaml.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2320 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/xml_serializer.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.211098 django-stubs-4.2.1/django-stubs/core/servers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/servers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1165 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/servers/basehttp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      139 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1846 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/signing.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4397 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/wsgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.214431 django-stubs-4.2.1/django-stubs/db/
--rw-r--r--   0 marti     (1000) marti      (121)     1047 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.214431 django-stubs-4.2.1/django-stubs/db/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.214431 django-stubs-4.2.1/django-stubs/db/backends/base/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5296 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/backends/base/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      555 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1132 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5147 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1826 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6660 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3557 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/validation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3134 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/ddl_references.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.214431 django-stubs-4.2.1/django-stubs/db/backends/dummy/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/dummy/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      949 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/dummy/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      176 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/dummy/features.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.217764 django-stubs-4.2.1/django-stubs/db/backends/mysql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2522 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      483 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      734 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/compiler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      255 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3434 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1159 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2760 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      902 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      354 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/validation.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.217764 django-stubs-4.2.1/django-stubs/db/backends/oracle/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2711 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      546 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      373 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1923 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1004 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3888 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      924 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      308 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/validation.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.221098 django-stubs-4.2.1/django-stubs/db/backends/postgresql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1382 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      524 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2197 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      820 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      809 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       63 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/signals.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.221098 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1052 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      322 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      205 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      125 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2876 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.224431 django-stubs-4.2.1/django-stubs/db/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2830 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/autodetector.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      664 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1739 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/executor.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2420 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/graph.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1960 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/loader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1111 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/migration.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.224431 django-stubs-4.2.1/django-stubs/db/migrations/operations/
--rw-r--r--   0 marti     (1000) marti      (121)     1090 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1426 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1171 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4451 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1977 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/special.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      985 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      290 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/optimizer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/questioner.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      755 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/recorder.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1835 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/serializer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2939 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/state.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      195 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1235 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/writer.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.227764 django-stubs-4.2.1/django-stubs/db/models/
--rw-r--r--   0 marti     (1000) marti      (121)     5016 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/aggregates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3728 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       16 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2255 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/constraints.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3487 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/deletion.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1008 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/enums.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     9496 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/expressions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.231098 django-stubs-4.2.1/django-stubs/db/models/fields/
--rw-r--r--   0 marti     (1000) marti      (121)    21253 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/models/fields/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4001 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/models/fields/files.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3142 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/fields/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/fields/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      161 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/fields/proxy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10684 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/models/fields/related.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3554 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/models/fields/related_descriptors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1393 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/fields/related_lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4605 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/fields/reverse_related.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.231098 django-stubs-4.2.1/django-stubs/db/models/functions/
--rw-r--r--   0 marti     (1000) marti      (121)     3378 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      547 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/functions/comparison.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1343 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/datetime.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1222 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/math.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4623 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/text.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/window.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2228 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/indexes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5904 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     8468 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/manager.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5334 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10808 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/query.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3306 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/models/query_utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      911 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/signals.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.234431 django-stubs-4.2.1/django-stubs/db/models/sql/
--rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6464 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/compiler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      344 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1791 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/datastructures.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     9565 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/sql/query.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1663 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/subqueries.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2075 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/where.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      473 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2178 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/transaction.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2061 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.234431 django-stubs-4.2.1/django-stubs/dispatch/
--rw-r--r--   0 marti     (1000) marti      (121)      116 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/dispatch/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      930 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/dispatch/dispatcher.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.234431 django-stubs-4.2.1/django-stubs/forms/
--rw-r--r--   0 marti     (1000) marti      (121)     4083 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2874 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/boundfield.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    20436 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3196 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3777 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/formsets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    12234 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/forms/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1125 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/renderers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2337 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10456 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/forms/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.237764 django-stubs-4.2.1/django-stubs/http/
--rw-r--r--   0 marti     (1000) marti      (121)     1332 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/http/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       96 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/http/cookie.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2076 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/http/multipartparser.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     8346 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/http/request.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5847 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/http/response.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.237764 django-stubs-4.2.1/django-stubs/middleware/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1062 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      387 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/clickjacking.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      968 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/common.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1098 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      339 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/gzip.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      369 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/locale.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      645 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/security.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1543 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.241098 django-stubs-4.2.1/django-stubs/template/
--rw-r--r--   0 marti     (1000) marti      (121)      756 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.241098 django-stubs-4.2.1/django-stubs/template/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      925 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1062 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/django.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      575 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/jinja2.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5673 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3410 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/context.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      631 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3483 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/defaultfilters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6912 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/defaulttags.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2158 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/engine.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3244 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/library.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2266 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loader_tags.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.244431 django-stubs-4.2.1/django-stubs/template/loaders/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       88 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/app_directories.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      554 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/cached.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      518 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/filesystem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      323 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/response.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1246 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/smartif.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      589 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.244431 django-stubs-4.2.1/django-stubs/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      629 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3492 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      410 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/l10n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1123 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/static.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1076 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/tz.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.244431 django-stubs-4.2.1/django-stubs/test/
--rw-r--r--   0 marti     (1000) marti      (121)      848 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     7476 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6619 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/runner.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      539 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/selenium.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      905 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10511 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/testcases.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6313 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.247764 django-stubs-4.2.1/django-stubs/urls/
--rw-r--r--   0 marti     (1000) marti      (121)     1576 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      886 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1349 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/conf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      778 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/converters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      102 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4497 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/resolvers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.254431 django-stubs-4.2.1/django-stubs/utils/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/_os.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1485 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/archive.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      235 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/asyncio.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2830 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/autoreload.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      591 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/baseconv.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1287 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1173 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/connection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      557 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/crypto.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4498 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/datastructures.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2062 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/dateformat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      525 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/dateparse.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/dates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      386 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/datetime_safe.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      325 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/deconstruct.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1185 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/utils/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1361 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/utils/deprecation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/duration.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3255 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/encoding.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2622 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/feedgenerator.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1804 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/formats.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4146 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/functional.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       66 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/hashable.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1399 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1766 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/utils/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      483 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/inspect.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/ipv6.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       61 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/itercompat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      714 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/jslex.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1691 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/utils/log.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      242 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/lorem_ipsum.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/module_loading.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      319 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/numberformat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      917 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/regex_helper.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      616 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/safestring.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      557 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/termcolors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1969 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/text.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      387 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/timesince.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2011 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/timezone.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/topological_sort.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.254431 django-stubs-4.2.1/django-stubs/utils/translation/
--rw-r--r--   0 marti     (1000) marti      (121)     2914 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/translation/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/translation/reloader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      298 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/translation/template.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      825 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/translation/trans_null.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2929 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/translation/trans_real.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      800 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/tree.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      499 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/version.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/xmlutils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.257764 django-stubs-4.2.1/django-stubs/views/
--rw-r--r--   0 marti     (1000) marti      (121)       39 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2691 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/debug.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.257764 django-stubs-4.2.1/django-stubs/views/decorators/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      347 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/views/decorators/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/clickjacking.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      162 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/common.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      427 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      259 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/views/decorators/debug.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      146 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/gzip.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      718 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/views/decorators/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/vary.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/defaults.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.257764 django-stubs-4.2.1/django-stubs/views/generic/
--rw-r--r--   0 marti     (1000) marti      (121)      797 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2272 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4525 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/dates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/detail.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3422 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/edit.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1818 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1035 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      482 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/static.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.261098 django-stubs-4.2.1/django_stubs.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)    13907 2023-06-02 14:11:31.000000 django-stubs-4.2.1/django_stubs.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)    30271 2023-06-02 14:11:31.000000 django-stubs-4.2.1/django_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-02 14:11:31.000000 django-stubs-4.2.1/django_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)      155 2023-06-02 14:11:31.000000 django-stubs-4.2.1/django_stubs.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       32 2023-06-02 14:11:31.000000 django-stubs-4.2.1/django_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.261098 django-stubs-4.2.1/mypy_django_plugin/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     3484 2023-06-02 14:08:54.000000 django-stubs-4.2.1/mypy_django_plugin/config.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.261098 django-stubs-4.2.1/mypy_django_plugin/django/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/django/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)    20567 2023-06-02 14:08:54.000000 django-stubs-4.2.1/mypy_django_plugin/django/context.py
--rw-r--r--   0 marti     (1000) marti      (121)      227 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/errorcodes.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.261098 django-stubs-4.2.1/mypy_django_plugin/lib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/lib/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     2289 2023-04-27 12:45:58.000000 django-stubs-4.2.1/mypy_django_plugin/lib/fullnames.py
--rw-r--r--   0 marti     (1000) marti      (121)    13031 2023-04-27 12:45:58.000000 django-stubs-4.2.1/mypy_django_plugin/lib/helpers.py
--rw-r--r--   0 marti     (1000) marti      (121)    15645 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/main.py
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/py.typed
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.264431 django-stubs-4.2.1/mypy_django_plugin/transformers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     9647 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/fields.py
--rw-r--r--   0 marti     (1000) marti      (121)     1809 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/forms.py
--rw-r--r--   0 marti     (1000) marti      (121)     1335 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/functional.py
--rw-r--r--   0 marti     (1000) marti      (121)     3104 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/init_create.py
--rw-r--r--   0 marti     (1000) marti      (121)    20879 2023-06-02 14:08:54.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/managers.py
--rw-r--r--   0 marti     (1000) marti      (121)     1960 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/meta.py
--rw-r--r--   0 marti     (1000) marti      (121)    32471 2023-04-27 12:45:58.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/models.py
--rw-r--r--   0 marti     (1000) marti      (121)     2659 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/orm_lookups.py
--rw-r--r--   0 marti     (1000) marti      (121)    13195 2023-04-27 12:45:58.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/querysets.py
--rw-r--r--   0 marti     (1000) marti      (121)     2070 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/request.py
--rw-r--r--   0 marti     (1000) marti      (121)     2003 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/settings.py
--rw-r--r--   0 marti     (1000) marti      (121)      227 2023-03-15 16:53:32.000000 django-stubs-4.2.1/pyproject.toml
--rw-r--r--   0 marti     (1000) marti      (121)      308 2023-06-02 14:11:31.264431 django-stubs-4.2.1/setup.cfg
--rw-r--r--   0 marti     (1000) marti      (121)     2262 2023-06-02 14:08:54.000000 django-stubs-4.2.1/setup.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.264431 django-stubs-4.2.1/tests/
--rw-r--r--   0 marti     (1000) marti      (121)     4735 2023-06-02 14:08:54.000000 django-stubs-4.2.1/tests/test_error_handling.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.593821 django-stubs-4.2.2/
+-rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-06-02 14:08:54.000000 django-stubs-4.2.2/LICENSE.md
+-rw-r--r--   0 marti     (1000) marti      (121)    15867 2023-06-27 17:51:06.593821 django-stubs-4.2.2/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)    14909 2023-06-27 17:49:10.000000 django-stubs-4.2.2/README.md
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.480488 django-stubs-4.2.2/django-stubs/
+-rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.480488 django-stubs-4.2.2/django-stubs/apps/
+-rw-r--r--   0 marti     (1000) marti      (121)       78 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/apps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      960 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/apps/config.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1963 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/apps/registry.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.483821 django-stubs-4.2.2/django-stubs/conf/
+-rw-r--r--   0 marti     (1000) marti      (121)     1438 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/conf/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    17261 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/conf/global_settings.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.483821 django-stubs-4.2.2/django-stubs/conf/locale/
+-rw-r--r--   0 marti     (1000) marti      (121)       50 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/conf/locale/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.483821 django-stubs-4.2.2/django-stubs/conf/urls/
+-rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/conf/urls/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      231 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/conf/urls/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/conf/urls/static.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.483821 django-stubs-4.2.2/django-stubs/contrib/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.487155 django-stubs-4.2.2/django-stubs/contrib/admin/
+-rw-r--r--   0 marti     (1000) marti      (121)     1157 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      313 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/actions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1068 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2208 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3887 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/filters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      237 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/forms.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5562 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/helpers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.487155 django-stubs-4.2.2/django-stubs/contrib/admin/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1032 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    16372 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/options.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4088 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/sites.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.487155 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1981 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/admin_list.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      690 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/admin_modify.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      503 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/admin_urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      605 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/log.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1629 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/tests.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3665 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.490488 django-stubs-4.2.2/django-stubs/contrib/admin/views/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/views/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      374 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/views/autocomplete.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      383 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admin/views/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3055 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/views/main.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5652 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/admin/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.490488 django-stubs-4.2.2/django-stubs/contrib/admindocs/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      478 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/middleware.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1018 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/admindocs/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.493821 django-stubs-4.2.2/django-stubs/contrib/auth/
+-rw-r--r--   0 marti     (1000) marti      (121)     1272 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1891 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/backends.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1503 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/auth/base_user.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      662 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      934 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3944 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/contrib/auth/forms.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.493821 django-stubs-4.2.2/django-stubs/contrib/auth/handlers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/handlers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/handlers/modwsgi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1962 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/hashers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.493821 django-stubs-4.2.2/django-stubs/contrib/auth/management/
+-rw-r--r--   0 marti     (1000) marti      (121)      406 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/auth/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.493821 django-stubs-4.2.2/django-stubs/contrib/auth/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      125 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/management/commands/changepassword.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.493821 django-stubs-4.2.2/django-stubs/contrib/auth/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1228 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4613 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/auth/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2081 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/password_validation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      735 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/contrib/auth/tokens.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      153 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/validators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2387 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/auth/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/contenttypes/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      655 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       76 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      414 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3851 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1421 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/forms.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/
+-rw-r--r--   0 marti     (1000) marti      (121)     1305 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/contenttypes/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1020 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/contenttypes/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/flatpages/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/forms.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/flatpages/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      402 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       81 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/sitemaps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.497155 django-stubs-4.2.2/django-stubs/contrib/flatpages/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      484 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/flatpages/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.500488 django-stubs-4.2.2/django-stubs/contrib/gis/
+-rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.500488 django-stubs-4.2.2/django-stubs/contrib/gis/admin/
+-rw-r--r--   0 marti     (1000) marti      (121)      872 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/admin/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1174 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/admin/options.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      272 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/admin/widgets.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       67 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.500488 django-stubs-4.2.2/django-stubs/contrib/gis/db/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.500488 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.500488 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1443 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      836 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1348 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/operations.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.503821 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      251 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      781 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      333 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1134 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      699 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.503821 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      226 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      254 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      444 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      287 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      729 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1440 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.503821 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      399 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      351 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      189 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/const.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      407 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      360 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      798 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2189 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      340 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.507155 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      835 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      127 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      358 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      451 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      808 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1286 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1103 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      656 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.507155 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/
+-rw-r--r--   0 marti     (1000) marti      (121)      847 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      800 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/aggregates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6077 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6232 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/functions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2955 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/proxy.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.507155 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/sql/
+-rw-r--r--   0 marti     (1000) marti      (121)      166 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/sql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/db/models/sql/conversion.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      866 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/feeds.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.507155 django-stubs-4.2.2/django-stubs/contrib/gis/forms/
+-rw-r--r--   0 marti     (1000) marti      (121)      642 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/forms/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      951 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/forms/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.510488 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/
+-rw-r--r--   0 marti     (1000) marti      (121)     1070 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      137 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      574 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/datasource.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      324 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/driver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      688 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/envelope.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/error.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      947 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/feature.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1460 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/field.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4844 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/geometries.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      304 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/geomtype.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1692 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/layer.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      510 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/libgdal.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.510488 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1036 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      961 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1077 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      970 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1053 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      614 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.510488 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1565 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/band.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/const.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2329 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/source.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2191 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/gdal/srs.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.510488 django-stubs-4.2.2/django-stubs/contrib/gis/geoip2/
+-rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geoip2/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1202 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geoip2/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       99 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geoip2/resources.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       97 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geometry.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.513821 django-stubs-4.2.2/django-stubs/contrib/gis/geos/
+-rw-r--r--   0 marti     (1000) marti      (121)      883 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      604 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/collections.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1250 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/coordseq.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       36 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/error.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      276 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/factory.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5258 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/geometry.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      467 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/io.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      896 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/libgeos.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      766 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/linestring.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/mutable_list.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      816 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/point.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      713 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/polygon.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      737 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prepared.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.513821 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/
+-rw-r--r--   0 marti     (1000) marti      (121)     4249 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      795 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      474 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      792 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/geom.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/io.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/misc.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      553 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      434 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      609 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/topology.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1418 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/measure.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/ptr.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/gis/serializers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/serializers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      493 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/serializers/geojson.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      244 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/gis/sitemaps/
+-rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/sitemaps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      328 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/sitemaps/kml.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      352 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/sitemaps/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/gis/utils/
+-rw-r--r--   0 marti     (1000) marti      (121)      436 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2526 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/utils/layermapping.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/gis/utils/ogrinfo.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      320 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/utils/ogrinspect.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      199 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/utils/srs.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      202 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/gis/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/humanize/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/humanize/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/humanize/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/humanize/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/humanize/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      859 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/humanize/templatetags/humanize.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.517155 django-stubs-4.2.2/django-stubs/contrib/messages/
+-rw-r--r--   0 marti     (1000) marti      (121)      715 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1294 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/api.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/constants.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      349 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.520488 django-stubs-4.2.2/django-stubs/contrib/messages/storage/
+-rw-r--r--   0 marti     (1000) marti      (121)      168 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/messages/storage/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      906 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/storage/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      463 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/storage/cookie.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      228 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/storage/fallback.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      468 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/storage/session.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       44 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      347 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/messages/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.520488 django-stubs-4.2.2/django-stubs/contrib/postgres/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.520488 django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/
+-rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      357 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/general.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       29 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      470 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/statistics.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      270 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      847 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/constraints.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.523821 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/
+-rw-r--r--   0 marti     (1000) marti      (121)      759 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1897 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/array.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/citext.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      573 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/hstore.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      376 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/jsonb.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3009 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/ranges.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/fields/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.523821 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/
+-rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2341 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/array.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      462 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/hstore.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      207 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/jsonb.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1486 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/forms/ranges.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/functions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3972 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/indexes.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      631 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2045 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3653 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/search.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      230 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      635 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/postgres/validators.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.523821 django-stubs-4.2.2/django-stubs/contrib/redirects/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.523821 django-stubs-4.2.2/django-stubs/contrib/redirects/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      150 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/redirects/models.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sessions/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1869 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/cached_db.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      490 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/db.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      239 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/file.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/backends/signed_cookies.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      676 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/base_session.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/exceptions.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sessions/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sessions/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      447 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sessions/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      243 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      337 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sessions/serializers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sitemaps/
+-rw-r--r--   0 marti     (1000) marti      (121)     1909 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sitemaps/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.527155 django-stubs-4.2.2/django-stubs/contrib/sitemaps/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      694 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sitemaps/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.530488 django-stubs-4.2.2/django-stubs/contrib/sites/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       69 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      247 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sites/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      289 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sites/management.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/managers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      209 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.530488 django-stubs-4.2.2/django-stubs/contrib/sites/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      585 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      307 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/sites/requests.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      221 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/sites/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.530488 django-stubs-4.2.2/django-stubs/contrib/staticfiles/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      263 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2489 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/finders.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1674 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/handlers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.530488 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.533821 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1055 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       87 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2292 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/storage.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/testing.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/staticfiles/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.533821 django-stubs-4.2.2/django-stubs/contrib/syndication/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/syndication/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      131 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/contrib/syndication/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1889 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/contrib/syndication/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.533821 django-stubs-4.2.2/django-stubs/core/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/asgi.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.533821 django-stubs-4.2.2/django-stubs/core/cache/
+-rw-r--r--   0 marti     (1000) marti      (121)      624 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.537155 django-stubs-4.2.2/django-stubs/core/cache/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4121 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      593 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/db.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      204 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/filebased.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      180 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/backends/memcached.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/cache/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.537155 django-stubs-4.2.2/django-stubs/core/checks/
+-rw-r--r--   0 marti     (1000) marti      (121)      652 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/async_checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      529 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/caches.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.537155 django-stubs-4.2.2/django-stubs/core/checks/compatibility/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/compatibility/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      256 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/compatibility/django_4_0.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      229 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/database.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      268 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/files.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1084 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/messages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/model_checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1837 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/registry.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.537155 django-stubs-4.2.2/django-stubs/core/checks/security/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/security/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2087 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/security/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      514 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/security/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/security/sessions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      565 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/checks/templates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      625 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/translation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      706 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/checks/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1883 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/exceptions.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.540488 django-stubs-4.2.2/django-stubs/core/files/
+-rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1606 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      359 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/images.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/locks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      130 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/move.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.540488 django-stubs-4.2.2/django-stubs/core/files/storage/
+-rw-r--r--   0 marti     (1000) marti      (121)      634 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/files/storage/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/files/storage/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      751 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/files/storage/filesystem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      450 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/files/storage/handler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      725 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/files/storage/memory.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      338 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/files/storage/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/temp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1450 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/files/uploadedfile.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3017 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/uploadhandler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      736 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/files/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.540488 django-stubs-4.2.2/django-stubs/core/handlers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/handlers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2043 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/handlers/asgi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1220 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/handlers/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      770 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/handlers/exception.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1405 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/handlers/wsgi.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.540488 django-stubs-4.2.2/django-stubs/core/mail/
+-rw-r--r--   0 marti     (1000) marti      (121)     1714 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/core/mail/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.543821 django-stubs-4.2.2/django-stubs/core/mail/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      668 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      303 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/console.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/filebased.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      395 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/backends/smtp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4640 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/mail/message.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/mail/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.543821 django-stubs-4.2.2/django-stubs/core/management/
+-rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3617 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/management/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1099 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/color.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.547154 django-stubs-4.2.2/django-stubs/core/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      179 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/check.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      430 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/compilemessages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/createcachetable.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/dbshell.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      519 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/diffsettings.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      123 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/dumpdata.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/flush.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      789 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/inspectdb.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1140 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/loaddata.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1227 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/makemessages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/makemigrations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      643 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/migrate.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/runserver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      111 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/sendtestemail.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      268 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/shell.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      371 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/showmigrations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      110 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/sqlflush.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      203 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/sqlmigrate.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       83 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/sqlsequencereset.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      330 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/squashmigrations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/startapp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/startproject.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/test.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/commands/testserver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/sql.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      964 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/templates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      850 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/management/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2229 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/paginator.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.550488 django-stubs-4.2.2/django-stubs/core/serializers/
+-rw-r--r--   0 marti     (1000) marti      (121)     1437 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/serializers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3193 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/serializers/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/serializers/json.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/serializers/jsonl.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      490 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/serializers/python.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      831 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/serializers/pyyaml.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2321 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/serializers/xml_serializer.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.550488 django-stubs-4.2.2/django-stubs/core/servers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/servers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1165 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/servers/basehttp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      139 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1846 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/signing.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4218 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/core/validators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/core/wsgi.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.550488 django-stubs-4.2.2/django-stubs/db/
+-rw-r--r--   0 marti     (1000) marti      (121)     1047 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.550488 django-stubs-4.2.2/django-stubs/db/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.550488 django-stubs-4.2.2/django-stubs/db/backends/base/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/base/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5296 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/db/backends/base/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      555 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/base/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1132 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/base/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5118 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/base/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1870 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/base/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     7157 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/base/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3557 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/base/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/base/validation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3134 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/ddl_references.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.553821 django-stubs-4.2.2/django-stubs/db/backends/dummy/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/dummy/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      924 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/dummy/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      176 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/dummy/features.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.553821 django-stubs-4.2.2/django-stubs/db/backends/mysql/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2493 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      473 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      734 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/compiler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      255 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3434 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      568 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2872 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      902 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      354 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/mysql/validation.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.553821 django-stubs-4.2.2/django-stubs/db/backends/oracle/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2711 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      546 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      373 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1923 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/functions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      351 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3990 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      924 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      308 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/oracle/validation.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.557154 django-stubs-4.2.2/django-stubs/db/backends/postgresql/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1382 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      524 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2197 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      304 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      529 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      809 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/postgresql/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       63 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/signals.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.557154 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1052 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      322 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      205 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1014 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/backends/sqlite3/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2876 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/backends/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.560488 django-stubs-4.2.2/django-stubs/db/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2830 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/autodetector.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      664 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1739 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/executor.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2404 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/graph.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1960 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/loader.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1111 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/migration.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.560488 django-stubs-4.2.2/django-stubs/db/migrations/operations/
+-rw-r--r--   0 marti     (1000) marti      (121)     1159 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1522 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1251 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5342 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2043 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/special.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      974 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/operations/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      290 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/optimizer.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/questioner.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      755 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/recorder.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1835 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/serializer.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4952 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/migrations/state.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      195 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1235 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/migrations/writer.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.563821 django-stubs-4.2.2/django-stubs/db/models/
+-rw-r--r--   0 marti     (1000) marti      (121)     5016 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/aggregates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3699 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       96 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/constants.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2248 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/constraints.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3475 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/deletion.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1074 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/enums.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10062 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/expressions.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.563821 django-stubs-4.2.2/django-stubs/db/models/fields/
+-rw-r--r--   0 marti     (1000) marti      (121)    21191 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/fields/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4001 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/db/models/fields/files.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3504 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/fields/json.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/fields/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      161 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/fields/proxy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10684 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/fields/related.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3463 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/fields/related_descriptors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1393 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/fields/related_lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4576 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/fields/reverse_related.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.567154 django-stubs-4.2.2/django-stubs/db/models/functions/
+-rw-r--r--   0 marti     (1000) marti      (121)     3378 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      547 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/db/models/functions/comparison.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1343 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/datetime.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1222 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/math.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4623 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/text.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/functions/window.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2228 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/indexes.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5850 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     8468 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/db/models/manager.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5363 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/options.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10883 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/query.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3277 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/query_utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      888 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/signals.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.567154 django-stubs-4.2.2/django-stubs/db/models/sql/
+-rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/sql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6507 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/sql/compiler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/sql/constants.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1791 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/sql/datastructures.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     9499 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/sql/query.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1619 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/db/models/sql/subqueries.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2075 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/sql/where.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      473 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/models/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2178 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/db/transaction.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2061 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/db/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.567154 django-stubs-4.2.2/django-stubs/dispatch/
+-rw-r--r--   0 marti     (1000) marti      (121)      116 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/dispatch/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1251 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/dispatch/dispatcher.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.570488 django-stubs-4.2.2/django-stubs/forms/
+-rw-r--r--   0 marti     (1000) marti      (121)     4083 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2874 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/forms/boundfield.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    20422 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/forms/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3196 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/forms/forms.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3777 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/forms/formsets.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    12444 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/forms/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1125 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/forms/renderers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2337 2023-04-27 12:45:58.000000 django-stubs-4.2.2/django-stubs/forms/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10456 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/forms/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.570488 django-stubs-4.2.2/django-stubs/http/
+-rw-r--r--   0 marti     (1000) marti      (121)     1332 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/http/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       96 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/http/cookie.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1979 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/http/multipartparser.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     8346 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/http/request.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5819 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/http/response.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.570488 django-stubs-4.2.2/django-stubs/middleware/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1063 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/middleware/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      387 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/clickjacking.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      968 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/common.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1098 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      339 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/gzip.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      369 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/http.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/locale.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      645 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/middleware/security.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1514 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.573821 django-stubs-4.2.2/django-stubs/template/
+-rw-r--r--   0 marti     (1000) marti      (121)      756 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.573821 django-stubs-4.2.2/django-stubs/template/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      876 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/template/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1062 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/backends/django.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      575 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/backends/jinja2.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/backends/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5644 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/template/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3401 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/template/context.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      631 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3483 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/defaultfilters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6912 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/defaulttags.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2158 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/engine.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3244 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/library.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loader.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2267 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/template/loader_tags.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.577154 django-stubs-4.2.2/django-stubs/template/loaders/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       88 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/app_directories.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      554 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/cached.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      518 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/filesystem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      323 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/loaders/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/response.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1246 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/smartif.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      589 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/template/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.577154 django-stubs-4.2.2/django-stubs/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      629 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3492 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      410 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/l10n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1123 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/static.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1076 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/templatetags/tz.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.577154 django-stubs-4.2.2/django-stubs/test/
+-rw-r--r--   0 marti     (1000) marti      (121)      848 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/test/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     9121 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/test/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/test/html.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6591 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/test/runner.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      539 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/test/selenium.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      905 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/test/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10511 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/test/testcases.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6314 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/test/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.580487 django-stubs-4.2.2/django-stubs/urls/
+-rw-r--r--   0 marti     (1000) marti      (121)     1576 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/urls/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      857 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/urls/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1349 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/urls/conf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      778 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/urls/converters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      102 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/urls/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4722 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/urls/resolvers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/urls/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.583821 django-stubs-4.2.2/django-stubs/utils/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/_os.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1485 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/archive.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      230 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/asyncio.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2872 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/autoreload.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      591 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/baseconv.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1287 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1300 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/connection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      570 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/crypto.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4679 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/datastructures.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2033 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/dateformat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      505 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/dateparse.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/dates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      547 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/datetime_safe.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      325 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/deconstruct.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      876 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1746 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/deprecation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/duration.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3177 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/encoding.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2676 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/feedgenerator.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1814 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/formats.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4544 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/functional.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       66 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/hashable.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2481 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/html.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1283 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/http.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      483 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/inspect.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/ipv6.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       61 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/itercompat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      714 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/jslex.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1692 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/log.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      242 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/lorem_ipsum.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      312 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/module_loading.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      319 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/numberformat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      917 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/regex_helper.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      616 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/safestring.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      557 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/termcolors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1933 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/text.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      423 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/timesince.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2011 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/timezone.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/topological_sort.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.587154 django-stubs-4.2.2/django-stubs/utils/translation/
+-rw-r--r--   0 marti     (1000) marti      (121)     2033 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/translation/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/translation/reloader.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      335 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/translation/template.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      801 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/translation/trans_null.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2986 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/translation/trans_real.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      986 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/tree.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      518 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/utils/version.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/utils/xmlutils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.587154 django-stubs-4.2.2/django-stubs/views/
+-rw-r--r--   0 marti     (1000) marti      (121)       39 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2741 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/views/debug.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.590487 django-stubs-4.2.2/django-stubs/views/decorators/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      347 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/views/decorators/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/clickjacking.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      162 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/common.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      427 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      259 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/views/decorators/debug.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      146 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/gzip.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      718 2023-06-02 14:08:54.000000 django-stubs-4.2.2/django-stubs/views/decorators/http.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/decorators/vary.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/defaults.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.590487 django-stubs-4.2.2/django-stubs/views/generic/
+-rw-r--r--   0 marti     (1000) marti      (121)      797 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/generic/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2272 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/generic/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4525 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/generic/dates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/generic/detail.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3393 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/views/generic/edit.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1819 2023-06-27 17:49:10.000000 django-stubs-4.2.2/django-stubs/views/generic/list.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1035 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      482 2023-03-15 16:53:32.000000 django-stubs-4.2.2/django-stubs/views/static.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.590487 django-stubs-4.2.2/django_stubs.egg-info/
+-rw-r--r--   0 marti     (1000) marti      (121)    15867 2023-06-27 17:51:06.000000 django-stubs-4.2.2/django_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)    30431 2023-06-27 17:51:06.000000 django-stubs-4.2.2/django_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-27 17:51:06.000000 django-stubs-4.2.2/django_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti      (121)      150 2023-06-27 17:51:06.000000 django-stubs-4.2.2/django_stubs.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       32 2023-06-27 17:51:06.000000 django-stubs-4.2.2/django_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.590487 django-stubs-4.2.2/mypy_django_plugin/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     4295 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/config.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.590487 django-stubs-4.2.2/mypy_django_plugin/django/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/django/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)    21306 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/django/context.py
+-rw-r--r--   0 marti     (1000) marti      (121)      227 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/errorcodes.py
+-rw-r--r--   0 marti     (1000) marti      (121)       89 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/exceptions.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.593821 django-stubs-4.2.2/mypy_django_plugin/lib/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/lib/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2289 2023-04-27 12:45:58.000000 django-stubs-4.2.2/mypy_django_plugin/lib/fullnames.py
+-rw-r--r--   0 marti     (1000) marti      (121)    13634 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/lib/helpers.py
+-rw-r--r--   0 marti     (1000) marti      (121)    15544 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/main.py
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/py.typed
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.593821 django-stubs-4.2.2/mypy_django_plugin/transformers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     9704 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/fields.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1787 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/forms.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1313 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/functional.py
+-rw-r--r--   0 marti     (1000) marti      (121)     3104 2023-03-15 16:53:32.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/init_create.py
+-rw-r--r--   0 marti     (1000) marti      (121)    20857 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/managers.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1938 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/meta.py
+-rw-r--r--   0 marti     (1000) marti      (121)    32277 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/models.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2826 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/orm_lookups.py
+-rw-r--r--   0 marti     (1000) marti      (121)    13086 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/querysets.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2048 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/request.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2495 2023-06-27 17:49:10.000000 django-stubs-4.2.2/mypy_django_plugin/transformers/settings.py
+-rw-r--r--   0 marti     (1000) marti      (121)      458 2023-06-27 17:49:10.000000 django-stubs-4.2.2/pyproject.toml
+-rw-r--r--   0 marti     (1000) marti      (121)      308 2023-06-27 17:51:06.593821 django-stubs-4.2.2/setup.cfg
+-rw-r--r--   0 marti     (1000) marti      (121)     2233 2023-06-27 17:49:10.000000 django-stubs-4.2.2/setup.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:51:06.593821 django-stubs-4.2.2/tests/
+-rw-r--r--   0 marti     (1000) marti      (121)     5766 2023-06-27 17:49:10.000000 django-stubs-4.2.2/tests/test_error_handling.py
```

### Comparing `django-stubs-4.2.1/LICENSE.md` & `django-stubs-4.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/PKG-INFO` & `django-stubs-4.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs
-Version: 4.2.1
+Version: 4.2.2
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -13,17 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: compatible-mypy
 License-File: LICENSE.md
@@ -75,14 +72,15 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
 | 1.16.0         | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.15.0         | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.14.0         | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 
 ## Features
@@ -102,14 +100,34 @@
     class Meta(TypedModelMeta):
         ordering = ["example"]
         constraints = [
             models.UniqueConstraint(fields=["example"], name="unique_example"),
         ]
 ```
 
+### Other typed base classes
+
+* `django_stubs_ext.db.router.TypedDatabaseRouter` can be used as base when implementing custom database routers.
+
+## Settings
+
+django-stubs has a few settings, which you can list in:
+
+* `pyproject.toml`, under the table `[tool.django-stubs]`
+* `mypy.ini` under the table `[mypy.plugins.django-stubs]`
+
+The supported settings are:
+
+- `django_settings_module`, a string.
+
+  Specify the import path of your settings module, the same as Django’s [`DJANGO_SETTINGS_MODULE` environment variable](https://docs.djangoproject.com/en/stable/topics/settings/#designating-the-settings).
+
+- `strict_settings`, a boolean, default `true`.
+
+  Set to `false` if using dynamic settings, as [described below](https://github.com/typeddjango/django-stubs#how-to-use-a-custom-library-to-handle-django-settings).
 
 ## FAQ
 
 ### Is this an official Django project?
 
 No, it is not. We are independent from Django at the moment.
 There's a [proposal](https://github.com/django/deps/pull/65) to merge our project into the Django itself.
@@ -334,14 +352,61 @@
 
 The lazy translation functions of Django (such as `gettext_lazy`) return a `Promise` instead of `str`. These two types [cannot be used interchangeably](https://github.com/typeddjango/django-stubs/pull/1139#issuecomment-1232167698). The return type of these functions was therefore [changed](https://github.com/typeddjango/django-stubs/pull/689) to reflect that.
 
 If you encounter this error in your own code, you can either cast the `Promise` to `str` (causing the translation to be evaluated), or use the `StrPromise` or `StrOrPromise` types from `django-stubs-ext` in type hints. Which solution to choose depends depends on the particular case. See [working with lazy translation objects](https://docs.djangoproject.com/en/4.1/topics/i18n/translation/#working-with-lazy-translation-objects) in the Django documentation for more information.
 
 If this is reported on Django code, please report an issue or open a pull request to fix the type hints.
 
+### How to use a custom library to handle Django settings?
+
+Using something like [`django-split-settings`](https://github.com/wemake-services/django-split-settings) or [`django-configurations`](https://github.com/jazzband/django-configurations) will make it hard for mypy to infer your settings.
+
+This might also be the case when using something like:
+
+```python
+try:
+    from .local_settings import *
+except Exception:
+    pass
+```
+
+So, mypy would not like this code:
+
+```python
+from django.conf import settings
+
+settings.CUSTOM_VALUE  # E: 'Settings' object has no attribute 'CUSTOM_SETTING'
+```
+
+To handle this corner case we have a special setting `strict_settings` (`True` by default),
+you can switch it to `False` to always return `Any` and not raise any errors if runtime settings module has the given value,
+for example `pyproject.toml`:
+
+```toml
+[tool.django-stubs]
+strict_settings = false
+```
+
+or `mypy.ini`:
+
+```ini
+[mypy.plugins.django-stubs]
+strict_settings = false
+```
+
+And then:
+
+```python
+# Works:
+reveal_type(settings.EXISTS_IN_RUNTIME)  # N: Any
+
+# Errors:
+reveal_type(settings.MISSING)  # E: 'Settings' object has no attribute 'MISSING'
+```
+
 ## Related projects
 
 - [`awesome-python-typing`](https://github.com/typeddjango/awesome-python-typing) - Awesome list of all typing-related things in Python.
 - [`djangorestframework-stubs`](https://github.com/typeddjango/djangorestframework-stubs) - Stubs for Django REST Framework.
 - [`pytest-mypy-plugins`](https://github.com/typeddjango/pytest-mypy-plugins) - `pytest` plugin that we use for testing `mypy` stubs and plugins.
 - [`wemake-django-template`](https://github.com/wemake-services/wemake-django-template) - Create new typed Django projects in seconds.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-stubs-4.2.1/README.md` & `django-stubs-4.2.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
 | 1.16.0         | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.15.0         | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.14.0         | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 
 ## Features
@@ -72,14 +73,34 @@
     class Meta(TypedModelMeta):
         ordering = ["example"]
         constraints = [
             models.UniqueConstraint(fields=["example"], name="unique_example"),
         ]
 ```
 
+### Other typed base classes
+
+* `django_stubs_ext.db.router.TypedDatabaseRouter` can be used as base when implementing custom database routers.
+
+## Settings
+
+django-stubs has a few settings, which you can list in:
+
+* `pyproject.toml`, under the table `[tool.django-stubs]`
+* `mypy.ini` under the table `[mypy.plugins.django-stubs]`
+
+The supported settings are:
+
+- `django_settings_module`, a string.
+
+  Specify the import path of your settings module, the same as Django’s [`DJANGO_SETTINGS_MODULE` environment variable](https://docs.djangoproject.com/en/stable/topics/settings/#designating-the-settings).
+
+- `strict_settings`, a boolean, default `true`.
+
+  Set to `false` if using dynamic settings, as [described below](https://github.com/typeddjango/django-stubs#how-to-use-a-custom-library-to-handle-django-settings).
 
 ## FAQ
 
 ### Is this an official Django project?
 
 No, it is not. We are independent from Django at the moment.
 There's a [proposal](https://github.com/django/deps/pull/65) to merge our project into the Django itself.
@@ -304,14 +325,61 @@
 
 The lazy translation functions of Django (such as `gettext_lazy`) return a `Promise` instead of `str`. These two types [cannot be used interchangeably](https://github.com/typeddjango/django-stubs/pull/1139#issuecomment-1232167698). The return type of these functions was therefore [changed](https://github.com/typeddjango/django-stubs/pull/689) to reflect that.
 
 If you encounter this error in your own code, you can either cast the `Promise` to `str` (causing the translation to be evaluated), or use the `StrPromise` or `StrOrPromise` types from `django-stubs-ext` in type hints. Which solution to choose depends depends on the particular case. See [working with lazy translation objects](https://docs.djangoproject.com/en/4.1/topics/i18n/translation/#working-with-lazy-translation-objects) in the Django documentation for more information.
 
 If this is reported on Django code, please report an issue or open a pull request to fix the type hints.
 
+### How to use a custom library to handle Django settings?
+
+Using something like [`django-split-settings`](https://github.com/wemake-services/django-split-settings) or [`django-configurations`](https://github.com/jazzband/django-configurations) will make it hard for mypy to infer your settings.
+
+This might also be the case when using something like:
+
+```python
+try:
+    from .local_settings import *
+except Exception:
+    pass
+```
+
+So, mypy would not like this code:
+
+```python
+from django.conf import settings
+
+settings.CUSTOM_VALUE  # E: 'Settings' object has no attribute 'CUSTOM_SETTING'
+```
+
+To handle this corner case we have a special setting `strict_settings` (`True` by default),
+you can switch it to `False` to always return `Any` and not raise any errors if runtime settings module has the given value,
+for example `pyproject.toml`:
+
+```toml
+[tool.django-stubs]
+strict_settings = false
+```
+
+or `mypy.ini`:
+
+```ini
+[mypy.plugins.django-stubs]
+strict_settings = false
+```
+
+And then:
+
+```python
+# Works:
+reveal_type(settings.EXISTS_IN_RUNTIME)  # N: Any
+
+# Errors:
+reveal_type(settings.MISSING)  # E: 'Settings' object has no attribute 'MISSING'
+```
+
 ## Related projects
 
 - [`awesome-python-typing`](https://github.com/typeddjango/awesome-python-typing) - Awesome list of all typing-related things in Python.
 - [`djangorestframework-stubs`](https://github.com/typeddjango/djangorestframework-stubs) - Stubs for Django REST Framework.
 - [`pytest-mypy-plugins`](https://github.com/typeddjango/pytest-mypy-plugins) - `pytest` plugin that we use for testing `mypy` stubs and plugins.
 - [`wemake-django-template`](https://github.com/wemake-services/wemake-django-template) - Create new typed Django projects in seconds.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-stubs-4.2.1/django-stubs/apps/config.pyi` & `django-stubs-4.2.2/django-stubs/apps/config.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import types
 from collections.abc import Iterator
 
 from django.apps.registry import Apps
 from django.db.models.base import Model
-from django.utils.functional import _StrOrPromise
+from django.utils.functional import _StrOrPromise, cached_property
 
+APPS_MODULE_NAME: str
 MODELS_MODULE_NAME: str
 
 class AppConfig:
     name: str
     module: types.ModuleType | None
     apps: Apps | None
     label: str
     verbose_name: _StrOrPromise
     path: str
     models_module: str | None
     models: dict[str, type[Model]]
     def __init__(self, app_name: str, app_module: types.ModuleType | None) -> None: ...
+    @cached_property
+    def default_auto_field(self) -> str: ...
     @classmethod
     def create(cls, entry: str) -> AppConfig: ...
     def get_model(self, model_name: str, require_ready: bool = ...) -> type[Model]: ...
     def get_models(self, include_auto_created: bool = ..., include_swapped: bool = ...) -> Iterator[type[Model]]: ...
     def import_models(self) -> None: ...
     def ready(self) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/apps/registry.pyi` & `django-stubs-4.2.2/django-stubs/apps/registry.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/conf/__init__.pyi` & `django-stubs-4.2.2/django-stubs/conf/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Any
+from typing import Any, Literal
 
 from _typeshed import Self
 from django.utils.functional import LazyObject
-from typing_extensions import Literal
 
 # explicit dependency on standard settings to make it loaded
-from . import global_settings
+from . import global_settings  # noqa: F401
 
 ENVIRONMENT_VARIABLE: Literal["DJANGO_SETTINGS_MODULE"]
 DEFAULT_STORAGE_ALIAS: Literal["default"]
 STATICFILES_STORAGE_ALIAS: Literal["staticfiles"]
 
 # required for plugin to be able to distinguish this specific instance of LazySettings from others
 class _DjangoConfLazyObject(LazyObject):
```

### Comparing `django-stubs-4.2.1/django-stubs/conf/global_settings.pyi` & `django-stubs-4.2.2/django-stubs/conf/global_settings.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Sequence
 from re import Pattern
 
 # This is defined here as a do-nothing function because we can't import
 # django.utils.translation -- that module depends on the settings.
-from typing import Any, Protocol
+from typing import Any, Literal, Protocol
 
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import TypeAlias
 
 _Admins: TypeAlias = list[tuple[str, str]]
 
 ####################
 # CORE             #
 ####################
 DEBUG: bool
@@ -36,14 +36,15 @@
 # https://en.wikipedia.org/wiki/List_of_tz_zones_by_name (although not all
 # systems may support all possibilities). When USE_TZ is True, this is
 # interpreted as the default user time zone.
 TIME_ZONE: str
 
 # If you set this to True, Django will use timezone-aware datetimes.
 USE_TZ: bool
+USE_DEPRECATED_PYTZ: bool
 
 # Language code for this installation. All choices can be found here:
 # http://www.i18nguy.com/unicode/language-identifiers.html
 LANGUAGE_CODE: str
 
 # Languages we provide translations for, out of the box.
 LANGUAGES: list[tuple[str, str]]
@@ -206,14 +207,18 @@
 # read before a SuspiciousOperation (RequestDataTooBig) is raised.
 DATA_UPLOAD_MAX_MEMORY_SIZE: int  # i.e. 2.5 MB
 
 # Maximum number of GET/POST parameters that will be read before a
 # SuspiciousOperation (TooManyFieldsSent) is raised.
 DATA_UPLOAD_MAX_NUMBER_FIELDS: int
 
+# Maximum number of files encoded in a multipart upload that will be read
+# before a SuspiciousOperation (TooManyFilesSent) is raised.
+DATA_UPLOAD_MAX_NUMBER_FILES: int
+
 # Directory in which upload streamed files will be temporarily saved. A value of
 # `None` will make Django use the operating system's default temporary directory
 # (i.e. "/tmp" on *nix systems).
 FILE_UPLOAD_TEMP_DIR: str | None
 
 # The numeric mode to set newly-uploaded files to. The value should be a mode
 # you'd pass directly to os.chmod; see https://docs.python.org/library/os.html#files-and-directories.
@@ -297,14 +302,17 @@
 # Thousand separator symbol
 THOUSAND_SEPARATOR: str
 
 # The tablespaces to use for each model when not specified otherwise.
 DEFAULT_TABLESPACE: str
 DEFAULT_INDEX_TABLESPACE: str
 
+# Default primary key field type.
+DEFAULT_AUTO_FIELD: str
+
 # Default X-Frame-Options header value
 X_FRAME_OPTIONS: str
 
 USE_X_FORWARDED_HOST: bool
 USE_X_FORWARDED_PORT: bool
 
 # The Python dotted path to the WSGI application that Django's internal server
@@ -421,14 +429,18 @@
 CSRF_COOKIE_SECURE: bool
 CSRF_COOKIE_HTTPONLY: bool
 CSRF_COOKIE_SAMESITE: Literal["Lax", "Strict", "None", False]
 CSRF_HEADER_NAME: str
 CSRF_TRUSTED_ORIGINS: list[str]
 CSRF_USE_SESSIONS: bool
 
+# Whether to mask CSRF cookie value. It's a transitional setting helpful in
+# migrating multiple instance of the same project to Django 4.1+.
+CSRF_COOKIE_MASKED: bool
+
 ############
 # MESSAGES #
 ############
 
 # Class to use as messages backend
 MESSAGE_STORAGE: str
 
@@ -441,14 +453,18 @@
 
 # The callable to use to configure logging
 LOGGING_CONFIG: str
 
 # Custom logging configuration.
 LOGGING: dict[str, Any]
 
+# Default exception reporter class used in case none has been
+# specifically assigned to the HttpRequest instance.
+DEFAULT_EXCEPTION_REPORTER: str
+
 # Default exception reporter filter class used in case none has been
 # specifically assigned to the HttpRequest instance.
 DEFAULT_EXCEPTION_REPORTER_FILTER: str
 
 ###########
 # TESTING #
 ###########
@@ -497,15 +513,16 @@
 # serious issues like errors and criticals does not result in hiding the
 # message, but Django will not stop you from e.g. running server.
 SILENCED_SYSTEM_CHECKS: list[str]
 
 #######################
 # SECURITY MIDDLEWARE #
 #######################
-SECURE_BROWSER_XSS_FILTER: bool
 SECURE_CONTENT_TYPE_NOSNIFF: bool
+SECURE_CROSS_ORIGIN_OPENER_POLICY: str
 SECURE_HSTS_INCLUDE_SUBDOMAINS: bool
 SECURE_HSTS_PRELOAD: bool
 SECURE_HSTS_SECONDS: int
 SECURE_REDIRECT_EXEMPT: list[str]
+SECURE_REFERRER_POLICY: str
 SECURE_SSL_HOST: str | None
 SECURE_SSL_REDIRECT: bool
```

### Comparing `django-stubs-4.2.1/django-stubs/conf/urls/__init__.pyi` & `django-stubs-4.2.2/django-stubs/conf/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/checks.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/checks.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Sequence
 from typing import Any
 
 from django.apps.config import AppConfig
 from django.contrib.admin.options import BaseModelAdmin
-from django.core.checks.messages import CheckMessage, Error
+from django.core.checks.messages import CheckMessage
 
 def check_admin_app(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> list[CheckMessage]: ...
 def check_dependencies(**kwargs: Any) -> list[CheckMessage]: ...
 
 class BaseModelAdminChecks:
     def check(self, admin_obj: BaseModelAdmin, **kwargs: Any) -> list[CheckMessage]: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/decorators.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/filters.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/filters.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/helpers.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/helpers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/models.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/options.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/options.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
-from typing import Any, Generic, Optional, TypeVar, Union  # noqa: Y037  # https://github.com/python/mypy/issues/12211
+from typing import (  # noqa: Y037  # https://github.com/python/mypy/issues/12211
+    Any,
+    Generic,
+    Literal,
+    Optional,
+    TypeVar,
+    Union,
+)
 
 from django import forms
 from django.contrib.admin.filters import FieldListFilter, ListFilter
 from django.contrib.admin.models import LogEntry
 from django.contrib.admin.sites import AdminSite
 from django.contrib.admin.views.main import ChangeList
 from django.contrib.auth.forms import AdminPasswordChangeForm
@@ -29,15 +36,15 @@
 from django.http.request import HttpRequest
 from django.http.response import HttpResponse, HttpResponseBase, HttpResponseRedirect
 from django.template.response import _TemplateForResponseT
 from django.urls.resolvers import URLPattern
 from django.utils.datastructures import _ListOrTuple
 from django.utils.functional import _StrOrPromise
 from django.utils.safestring import SafeString
-from typing_extensions import Literal, TypeAlias, TypedDict
+from typing_extensions import TypeAlias, TypedDict
 
 IS_POPUP_VAR: str
 TO_FIELD_VAR: str
 HORIZONTAL: Literal[1]
 VERTICAL: Literal[2]
 
 _Direction: TypeAlias = Literal[1, 2]
@@ -77,15 +84,15 @@
 _ModelT = TypeVar("_ModelT", bound=Model)
 
 class BaseModelAdmin(Generic[_ModelT]):
     autocomplete_fields: Sequence[str]
     raw_id_fields: Sequence[str]
     fields: _FieldGroups | None
     exclude: Sequence[str] | None
-    fieldsets: Optional[_FieldsetSpec]
+    fieldsets: Optional[_FieldsetSpec]  # noqa: UP007
     form: type[forms.ModelForm[_ModelT]]
     filter_vertical: Sequence[str]
     filter_horizontal: Sequence[str]
     radio_fields: Mapping[str, _Direction]
     prepopulated_fields: dict[str, Sequence[str]]
     formfield_overrides: Mapping[type[Field], Mapping[str, Any]]
     readonly_fields: Sequence[str]
@@ -138,14 +145,15 @@
     list_display_links: _DisplayT | None
     list_filter: _ListOrTuple[_ListFilterT]
     list_select_related: bool | Sequence[str]
     list_per_page: int
     list_max_show_all: int
     list_editable: Sequence[str]
     search_fields: Sequence[str]
+    search_help_text: _StrOrPromise | None
     date_hierarchy: str | None
     save_as: bool
     save_as_continue: bool
     save_on_top: bool
     paginator: type
     preserve_filters: bool
     inlines: Sequence[type[InlineModelAdmin]]
@@ -268,14 +276,17 @@
     ) -> tuple[list[Model], dict[str, int], set[str], list[str]]: ...
     def delete_view(
         self, request: HttpRequest, object_id: str, extra_context: dict[str, Any] | None = ...
     ) -> HttpResponse: ...
     def history_view(
         self, request: HttpRequest, object_id: str, extra_context: dict[str, Any] | None = ...
     ) -> HttpResponse: ...
+    def get_formset_kwargs(
+        self, request: HttpRequest, obj: _ModelT, inline: InlineModelAdmin[Any, _ModelT], prefix: str
+    ) -> dict[str, Any]: ...
 
 _ChildModelT = TypeVar("_ChildModelT", bound=Model)
 _ParentModelT = TypeVar("_ParentModelT", bound=Model)
 
 class InlineModelAdmin(Generic[_ChildModelT, _ParentModelT], BaseModelAdmin[_ChildModelT]):
     model: type[_ChildModelT]
     fk_name: str | None
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/sites.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/sites.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     _actions: dict[str, _ActionCallback]
     def __init__(self, name: str = ...) -> None: ...
     def check(self, app_configs: Iterable[AppConfig] | None) -> list[CheckMessage]: ...
     def register(
         self,
         model_or_iterable: type[Model] | Iterable[type[Model]],
         admin_class: type[ModelAdmin] | None = ...,
-        **options: Any
+        **options: Any,
     ) -> None: ...
     def unregister(self, model_or_iterable: type[Model] | Iterable[type[Model]]) -> None: ...
     def is_registered(self, model: type[Model]) -> bool: ...
     def add_action(self, action: _ActionCallback, name: str | None = ...) -> None: ...
     def disable_action(self, name: str) -> None: ...
     def get_action(self, name: str) -> Callable: ...
     @property
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/admin_list.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/admin_list.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/admin_modify.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/admin_modify.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/base.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/templatetags/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/tests.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/tests.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/utils.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import datetime
 from collections.abc import Callable, Iterable, Sequence
-from typing import Any, overload
+from typing import Any, Literal, overload
 from uuid import UUID
 
 from django.contrib.admin.options import BaseModelAdmin
 from django.contrib.admin.sites import AdminSite
 from django.contrib.auth.forms import AdminPasswordChangeForm
 from django.db.models.base import Model
 from django.db.models.deletion import Collector
 from django.db.models.fields import Field, reverse_related
 from django.db.models.options import Options
 from django.db.models.query import QuerySet
 from django.forms.forms import BaseForm
 from django.forms.formsets import BaseFormSet
 from django.http.request import HttpRequest
 from django.utils.datastructures import _IndexableCollection
-from typing_extensions import Literal, TypedDict
+from typing_extensions import TypedDict
 
 class FieldIsAForeignKeyColumnName(Exception): ...
 
 def lookup_spawns_duplicates(opts: Options, lookup_path: str) -> bool: ...
 def prepare_lookup_value(key: str, value: datetime.datetime | str) -> bool | datetime.datetime | str: ...
 def quote(s: int | str | UUID) -> str: ...
 def unquote(s: str) -> str: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/views/main.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/views/main.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from collections.abc import Callable, Iterable, Sequence
-from typing import Any
+from typing import Any, Literal
 
 from django.contrib.admin.filters import ListFilter
 from django.contrib.admin.options import ModelAdmin, _DisplayT, _ListFilterT
 from django.db.models.base import Model
 from django.db.models.expressions import Expression
 from django.db.models.options import Options
 from django.db.models.query import QuerySet
 from django.forms.formsets import BaseFormSet
 from django.http.request import HttpRequest
-from typing_extensions import Literal
 
 ALL_VAR: str
 ORDER_VAR: str
-ORDER_TYPE_VAR: str
 PAGE_VAR: str
 SEARCH_VAR: str
 ERROR_FLAG: str
 IGNORED_PARAMS: tuple[str, ...]
 
 class ChangeList:
     model: type[Model]
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admin/widgets.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admin/widgets.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Iterable, Mapping, Sequence
 from typing import Any
 
 from django import forms
 from django.contrib.admin.sites import AdminSite
 from django.core.files.base import File
 from django.db.models.fields import _FieldChoices
-from django.db.models.fields.reverse_related import ForeignObjectRel, ManyToManyRel, ManyToOneRel
+from django.db.models.fields.reverse_related import ManyToManyRel, ManyToOneRel
 from django.forms.models import ModelChoiceIterator
 from django.forms.widgets import _OptAttrs
 from django.utils.functional import _StrOrPromise
 
 class FilteredSelectMultiple(forms.SelectMultiple):
     verbose_name: _StrOrPromise
     is_stacked: bool
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admindocs/utils.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admindocs/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/admindocs/views.pyi` & `django-stubs-4.2.2/django-stubs/contrib/admindocs/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/backends.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/backends.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/base_user.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/base_user.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Any, TypeVar, overload
+from typing import Any, Literal, TypeVar, overload
 
 from django.db import models
 from django.db.models.base import Model
 from django.db.models.expressions import Combinable
 from django.db.models.fields import BooleanField
-from typing_extensions import Literal
 
 _T = TypeVar("_T", bound=Model)
 
 class BaseUserManager(models.Manager[_T]):
     @classmethod
     def normalize_email(cls, email: str | None) -> str: ...
     def make_random_password(self, length: int = ..., allowed_chars: str = ...) -> str: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/context_processors.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/decorators.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/forms.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/forms.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/hashers.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/hashers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/middleware.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/middleware.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/mixins.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/models.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/models.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections.abc import Iterable
-from typing import Any, TypeVar
+from typing import Any, Literal, TypeVar
 
 from django.contrib.auth.base_user import AbstractBaseUser as AbstractBaseUser
 from django.contrib.auth.base_user import BaseUserManager as BaseUserManager
 from django.contrib.auth.validators import UnicodeUsernameValidator
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.db.models import QuerySet
 from django.db.models.base import Model
 from django.db.models.manager import EmptyManager
 from django.utils.functional import _StrOrPromise
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import TypeAlias
 
 _AnyUser: TypeAlias = Model | AnonymousUser
 
 def update_last_login(sender: type[AbstractBaseUser], user: AbstractBaseUser, **kwargs: Any) -> None: ...
 
 class PermissionManager(models.Manager[Permission]):
     def get_by_natural_key(self, codename: str, app_label: str, model: str) -> Permission: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/password_validation.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/password_validation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/tokens.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/tokens.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/auth/views.pyi` & `django-stubs-4.2.2/django-stubs/contrib/auth/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/contenttypes/admin.pyi` & `django-stubs-4.2.2/django-stubs/contrib/contenttypes/admin.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/contenttypes/fields.pyi` & `django-stubs-4.2.2/django-stubs/contrib/contenttypes/fields.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self,
         to: type[Model] | str,
         object_id_field: str = ...,
         content_type_field: str = ...,
         for_concrete_model: bool = ...,
         related_query_name: str | None = ...,
         limit_choices_to: dict[str, Any] | Callable[[], Any] | None = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None: ...
     def resolve_related_fields(self) -> list[tuple[Field, Field]]: ...
     def get_path_info(self, filtered_relation: FilteredRelation | None = ...) -> list[PathInfo]: ...
     def get_reverse_path_info(self, filtered_relation: FilteredRelation | None = ...) -> list[PathInfo]: ...
     def get_content_type(self) -> ContentType: ...
     def get_extra_restriction(
         self, where_class: type[WhereNode], alias: str | None, remote_alias: str
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/contenttypes/forms.pyi` & `django-stubs-4.2.2/django-stubs/contrib/contenttypes/forms.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self,
         data: Any | None = ...,
         files: Any | None = ...,
         instance: Any | None = ...,
         save_as_new: bool = ...,
         prefix: Any | None = ...,
         queryset: Any | None = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None: ...
     def initial_form_count(self) -> int: ...
     @classmethod
     def get_default_prefix(cls) -> str: ...
     def save_new(self, form: Any, commit: bool = ...) -> _M: ...
 
 def generic_inlineformset_factory(
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/contenttypes/management/__init__.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 from django.db import migrations
 from django.db.backends.sqlite3.schema import DatabaseSchemaEditor
 from django.db.migrations.migration import Migration
 from django.db.migrations.state import StateApps
 from django.db.models.base import Model
 
 class RenameContentType(migrations.RunPython):
-    app_label: Any
-    old_model: Any
-    new_model: Any
+    app_label: str
+    old_model: str
+    new_model: str
     def __init__(self, app_label: str, old_model: str, new_model: str) -> None: ...
     def rename_forward(self, apps: StateApps, schema_editor: DatabaseSchemaEditor) -> None: ...
     def rename_backward(self, apps: StateApps, schema_editor: DatabaseSchemaEditor) -> None: ...
 
 def inject_rename_contenttypes_operations(
-    plan: list[tuple[Migration, bool]] = ..., apps: StateApps = ..., using: str = ..., **kwargs: Any
+    plan: list[tuple[Migration, bool]] | None = ..., apps: StateApps = ..., using: str = ..., **kwargs: Any
 ) -> None: ...
 def get_contenttypes_and_models(
     app_config: AppConfig, using: str, ContentType: type[ContentType]
 ) -> tuple[dict[str, ContentType], dict[str, type[Model]]]: ...
 def create_contenttypes(
     app_config: AppConfig,
     verbosity: int = ...,
     interactive: bool = ...,
     using: str = ...,
     apps: Apps = ...,
-    **kwargs: Any
+    **kwargs: Any,
 ) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/contenttypes/models.pyi` & `django-stubs-4.2.2/django-stubs/contrib/contenttypes/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/admin/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/admin/options.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/admin/options.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/features.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/models.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/operations.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/features.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/operations.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/schema.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/models.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/operations.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/schema.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/models.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/operations.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/postgis/operations.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Any
+from typing import Any, Literal
 
 from django.contrib.gis.db.backends.base.operations import BaseSpatialOperations
 from django.contrib.gis.db.backends.utils import SpatialOperator
 from django.db.backends.postgresql.operations import DatabaseOperations
 from django.db.models import Func
-from typing_extensions import Literal
 
 BILATERAL: Literal["bilateral"]
 
 class PostGISOperator(SpatialOperator):
     geography: Any
     raster: bool | Literal["bilateral"]
     def __init__(self, geography: bool = ..., raster: bool | Literal["bilateral"] = ..., **kwargs: Any) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/models.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/utils.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/backends/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/aggregates.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/fields.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/fields.pyi`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 _ST = TypeVar("_ST")
 # __get__ return type
 _GT = TypeVar("_GT")
 
 class SRIDCacheEntry(NamedTuple):
     units: Any
     units_name: str
-    geodetic: bool
     spheroid: str
+    geodetic: bool
 
 def get_srid_info(srid: int, connection: Any) -> SRIDCacheEntry: ...
 
 class BaseSpatialField(Field[_ST, _GT]):
     form_class: type[forms.GeometryField]
     geom_type: str
     geom_class: type[GEOSGeometry] | None
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/functions.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/functions.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,22 @@
 
 class Envelope(GeomOutputGeoFunc):
     arity: int
 
 class ForcePolygonCW(GeomOutputGeoFunc):
     arity: int
 
+class FromWKB(GeoFunc):
+    output_field: Any
+    arity: int
+
+class FromWKT(GeoFunc):
+    output_field: Any
+    arity: int
+
 class GeoHash(GeoFunc):
     output_field: Any
     def __init__(self, expression: Any, precision: Any | None = ..., **extra: Any) -> None: ...
     def as_mysql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class GeometryDistance(GeoFunc):
     output_field: Any
@@ -108,14 +116,18 @@
     arg_joiner: str
     geom_param_pos: Any
 
 class Intersection(OracleToleranceMixin, GeomOutputGeoFunc):
     arity: int
     geom_param_pos: Any
 
+class IsEmpty(GeoFuncMixin, StandardTransform):
+    lookup_name: str
+    output_field: Any
+
 class IsValid(OracleToleranceMixin, GeoFuncMixin, StandardTransform):
     lookup_name: str
     output_field: Any
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Length(DistanceResultMixin, OracleToleranceMixin, GeoFunc):
     spheroid: Any
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/lookups.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/sql/conversion.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/db/models/sql/conversion.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/feeds.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/feeds.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/forms/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/forms/fields.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/forms/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/forms/widgets.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/forms/widgets.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/datasource.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/datasource.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/envelope.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/envelope.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/feature.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/feature.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/field.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/field.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/geometries.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/geometries.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/layer.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/layer.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from collections.abc import Iterator
-from typing import Any, AnyStr, overload
+from typing import Any, AnyStr, Literal, overload
 
 from django.contrib.gis.gdal.base import GDALBase
 from django.contrib.gis.gdal.envelope import Envelope
 from django.contrib.gis.gdal.feature import Feature
 from django.contrib.gis.gdal.field import Field
 from django.contrib.gis.gdal.geometries import OGRGeometry
 from django.contrib.gis.gdal.geomtype import OGRGeomType
 from django.contrib.gis.gdal.srs import SpatialReference
 from django.contrib.gis.geos.geometry import GEOSGeometry
-from typing_extensions import Literal
 
 class Layer(GDALBase):
     ptr: Any
     def __init__(self, layer_ptr: Any, ds: Any) -> None: ...
     @overload
     def __getitem__(self, index: int) -> Feature: ...
     @overload
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/ds.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/ds.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/generation.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/generation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/geom.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/raster.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/raster.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/srs.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/prototypes/srs.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/band.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/band.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Any, overload
+from typing import Any, Literal, overload
 
 from django.contrib.gis.gdal.raster.base import GDALRasterBase
-from typing_extensions import Literal
 
 class GDALBand(GDALRasterBase):
     source: Any
     def __init__(self, source: Any, index: Any) -> None: ...
     @property
     def description(self) -> str: ...
     @property
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/source.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/raster/source.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from collections.abc import Sequence
+from ctypes import c_void_p
+from pathlib import Path
 from typing import Any
 
 from django.contrib.gis.gdal.driver import Driver
 from django.contrib.gis.gdal.raster.band import BandList
 from django.contrib.gis.gdal.raster.base import GDALRasterBase
 from django.contrib.gis.gdal.srs import SpatialReference
 
@@ -16,15 +18,15 @@
     @property
     def y(self) -> float: ...
     @y.setter
     def y(self, value: float) -> None: ...
 
 class GDALRaster(GDALRasterBase):
     destructor: Any
-    def __init__(self, ds_input: Any, write: bool = ...) -> None: ...
+    def __init__(self, ds_input: str | Path | bytes | dict | c_void_p, write: bool = ...) -> None: ...
     def __del__(self) -> None: ...
     @property
     def vsi_buffer(self) -> bytes | None: ...
     @property
     def is_vsi_based(self) -> bool: ...
     @property
     def name(self) -> str: ...
@@ -53,14 +55,15 @@
     @property
     def skew(self) -> TransformPoint: ...
     @property
     def extent(self) -> tuple[float, float, float, float]: ...
     @property
     def bands(self) -> BandList: ...
     def warp(self, ds_input: Any, resampling: str = ..., max_error: float = ...) -> GDALRaster: ...
+    def clone(self, name: str | None = ...) -> GDALRaster: ...
     def transform(
         self,
         srs: SpatialReference | int | str,
         driver: Any | None = ...,
         name: str | None = ...,
         resampling: str = ...,
         max_error: float = ...,
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/srs.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/gdal/srs.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geoip2/base.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geoip2/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/collections.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/collections.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/coordseq.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/geometry.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/geometry.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/libgeos.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/libgeos.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/linestring.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/linestring.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/mutable_list.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/mutable_list.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/point.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/point.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/polygon.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/polygon.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prepared.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prepared.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/geom.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/io.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/io.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/predicates.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/predicates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/topology.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/geos/prototypes/topology.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/measure.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/measure.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/gis/utils/layermapping.pyi` & `django-stubs-4.2.2/django-stubs/contrib/gis/utils/layermapping.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/humanize/templatetags/humanize.pyi` & `django-stubs-4.2.2/django-stubs/contrib/humanize/templatetags/humanize.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/messages/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/messages/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/messages/api.pyi` & `django-stubs-4.2.2/django-stubs/contrib/messages/api.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/messages/storage/base.pyi` & `django-stubs-4.2.2/django-stubs/contrib/messages/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/aggregates/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/constraints.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/constraints.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -16,9 +16,9 @@
         name: str,
         expressions: Sequence[tuple[str | Combinable, str]],
         index_type: str | None = ...,
         condition: Q | None = ...,
         deferrable: Deferrable | None = ...,
         include: list[str] | tuple[str] | None = ...,
         opclasses: list[str] | tuple[str] = ...,
-        violation_error_message: _StrOrPromise | None = ...
+        violation_error_message: _StrOrPromise | None = ...,
     ) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/fields/__init__.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/fields/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/fields/array.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/fields/array.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/fields/hstore.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/fields/hstore.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/fields/ranges.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/fields/ranges.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Any
+from typing import Any, Literal
 
 from django.db import models
 from django.db.models.lookups import PostgresOperatorLookup
 from psycopg2.extras import DateRange, DateTimeTZRange, NumericRange, Range
-from typing_extensions import Literal
 
 class RangeBoundary(models.Expression):
     lower: str
     upper: str
     def __init__(self, inclusive_lower: bool = ..., inclusive_upper: bool = ...) -> None: ...
 
 class RangeOperators:
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/forms/array.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/forms/array.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(
         self,
         base_field: forms.Field,
         *,
         delimiter: str = ...,
         max_length: int | None = ...,
         min_length: int | None = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None: ...
     def clean(self, value: Any) -> Sequence[Any]: ...
     def prepare_value(self, value: Any) -> Any: ...
     def to_python(self, value: Any) -> Sequence[Any]: ...  # type: ignore
     def validate(self, value: Sequence[Any]) -> None: ...
     def run_validators(self, value: Sequence[Any]) -> None: ...
     def has_changed(self, initial: Any, data: Any) -> bool: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/forms/ranges.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/forms/ranges.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/indexes.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/indexes.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/lookups.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/lookups.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from django.db.models import Lookup, Transform
-from django.db.models.lookups import Exact, PostgresOperatorLookup
+from django.db.models import Transform
+from django.db.models.lookups import PostgresOperatorLookup
 
 from .search import SearchVectorExact
 
 class DataContains(PostgresOperatorLookup): ...
 class ContainedBy(PostgresOperatorLookup): ...
 class Overlap(PostgresOperatorLookup): ...
 class HasKey(PostgresOperatorLookup): ...
 class HasKeys(PostgresOperatorLookup): ...
 class HasAnyKeys(HasKeys): ...
 class Unaccent(Transform): ...
 class SearchLookup(SearchVectorExact): ...
 class TrigramSimilar(PostgresOperatorLookup): ...
+class TrigramWordSimilar(PostgresOperatorLookup): ...
+class TrigramStrictWordSimilar(PostgresOperatorLookup): ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/operations.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/operations.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Literal
+
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.migrations import AddConstraint, AddIndex, RemoveIndex
 from django.db.migrations.operations.base import Operation
-from typing_extensions import Literal
 
 class CreateExtension(Operation):
     reversible: bool
     name: str
     def __init__(self, name: str) -> None: ...
     def extension_exists(self, schema_editor: BaseDatabaseSchemaEditor, extension: str) -> bool: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/search.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/search.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         value: _Expression,
         output_field: Field | None = ...,
         *,
         config: _Expression | None = ...,
         invert: bool = ...,
         search_type: str = ...,
     ) -> None: ...
-    def __invert__(self: Self) -> Self: ...
+    def __invert__(self: Self) -> Self: ...  # type: ignore[override]
 
 class CombinedSearchQuery(SearchQueryCombinable, CombinedExpression):  # type: ignore
     def __init__(
         self,
         lhs: Combinable,
         connector: str,
         rhs: Combinable,
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/postgres/validators.pyi` & `django-stubs-4.2.2/django-stubs/contrib/postgres/validators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/sessions/backends/base.pyi` & `django-stubs-4.2.2/django-stubs/contrib/sessions/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/sessions/base_session.pyi` & `django-stubs-4.2.2/django-stubs/contrib/sessions/base_session.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/sitemaps/__init__.pyi` & `django-stubs-4.2.2/django-stubs/db/models/sql/where.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-from collections.abc import Iterable, Mapping, Sequence
-from datetime import datetime
-from typing import Any, Generic, TypeVar
-
-from django.contrib.sites.models import Site
-from django.contrib.sites.requests import RequestSite
-from django.core.paginator import Paginator
-from django.db.models.base import Model
-from django.db.models.query import QuerySet
-
-PING_URL: str
-
-class SitemapNotFound(Exception): ...
-
-def ping_google(sitemap_url: str | None = ..., ping_url: str = ..., sitemap_uses_https: bool = ...) -> None: ...
-
-_ItemT = TypeVar("_ItemT")
-
-class Sitemap(Generic[_ItemT]):
-    limit: int
-    protocol: str | None
-    i18n: bool
-    languages: Sequence[str] | None
-    alternates: bool
-    x_default: bool
-    def items(self) -> Iterable[_ItemT]: ...
-    def location(self, item: _ItemT) -> str: ...
+from collections.abc import Sequence
+from typing import Any
+
+from django.db.backends.base.base import BaseDatabaseWrapper
+from django.db.models.expressions import Expression
+from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
+from django.db.models.sql.query import Query
+from django.utils import tree
+
+AND: str
+OR: str
+
+class WhereNode(tree.Node):
+    connector: str
+    negated: bool
+    default: str
+    resolved: bool
+    conditional: bool
+    def split_having(self, negated: bool = ...) -> tuple[WhereNode | None, WhereNode | None]: ...
+    def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
+    def get_group_by_cols(self, alias: str | None = ...) -> list[Expression]: ...
+    def relabel_aliases(self, change_map: dict[str | None, str]) -> None: ...
+    def clone(self) -> WhereNode: ...
+    def relabeled_clone(self, change_map: dict[str | None, str]) -> WhereNode: ...
+    def resolve_expression(self, *args: Any, **kwargs: Any) -> WhereNode: ...
+    @property
+    def contains_aggregate(self) -> bool: ...
     @property
-    def paginator(self) -> Paginator: ...
-    def get_urls(
-        self, page: int | str = ..., site: Site | RequestSite | None = ..., protocol: str | None = ...
-    ) -> list[dict[str, Any]]: ...
-    def get_latest_lastmod(self) -> datetime | None: ...
-
-_ModelT = TypeVar("_ModelT", bound=Model)
-
-class GenericSitemap(Sitemap[_ModelT]):
-    priority: float | None
-    changefreq: str | None
-    queryset: QuerySet[_ModelT]
-    date_field: str | None
-    protocol: str | None
-    def __init__(
-        self,
-        info_dict: Mapping[str, datetime | QuerySet[_ModelT] | str],
-        priority: float | None = ...,
-        changefreq: str | None = ...,
-        protocol: str | None = ...,
-    ) -> None: ...
-    def items(self) -> QuerySet[_ModelT]: ...
-    def lastmod(self, item: _ModelT) -> datetime | None: ...
-    def get_latest_lastmod(self) -> datetime | None: ...
+    def contains_over_clause(self) -> bool: ...
+    @property
+    def is_summary(self) -> bool: ...
+
+class NothingNode:
+    contains_aggregate: bool
+    def as_sql(
+        self, compiler: SQLCompiler | None = ..., connection: BaseDatabaseWrapper | None = ...
+    ) -> _AsSqlType: ...
+
+class ExtraWhere:
+    contains_aggregate: bool
+    sqls: Sequence[str]
+    params: Sequence[int] | Sequence[str] | None
+    def __init__(self, sqls: Sequence[str], params: Sequence[int] | Sequence[str] | None) -> None: ...
+    def as_sql(
+        self, compiler: SQLCompiler | None = ..., connection: BaseDatabaseWrapper | None = ...
+    ) -> _AsSqlType: ...
+
+class SubqueryConstraint:
+    contains_aggregate: bool
+    alias: str
+    columns: list[str]
+    targets: list[str]
+    query_object: Query
+    def __init__(self, alias: str, columns: list[str], targets: list[str], query_object: Query) -> None: ...
+    def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/sitemaps/views.pyi` & `django-stubs-4.2.2/django-stubs/contrib/sitemaps/views.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Callable
 from typing import TypeVar
 
-from django.contrib.sitemaps import GenericSitemap, Sitemap
+from django.contrib.sitemaps import Sitemap
 from django.http.request import HttpRequest
 from django.template.response import TemplateResponse
 
 _C = TypeVar("_C", bound=Callable)
 
 def x_robots_tag(func: _C) -> _C: ...
 def index(
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/sites/models.pyi` & `django-stubs-4.2.2/django-stubs/contrib/sites/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/staticfiles/finders.pyi` & `django-stubs-4.2.2/django-stubs/contrib/staticfiles/finders.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from collections.abc import Iterable, Iterator, Sequence
-from typing import Any, overload
+from typing import Any, Literal, overload
 
 from django.core.checks.messages import CheckMessage
 from django.core.files.storage import FileSystemStorage, Storage
-from typing_extensions import Literal
 
 searched_locations: Any
 
 class BaseFinder:
     def check(self, **kwargs: Any) -> list[CheckMessage]: ...
     @overload
     def find(self, path: str, all: Literal[False] = ...) -> str | None: ...
@@ -53,15 +52,8 @@
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
 
 @overload
 def find(path: str, all: Literal[False] = ...) -> str | None: ...
 @overload
 def find(path: str, all: Literal[True]) -> list[str]: ...
 def get_finders() -> Iterator[BaseFinder]: ...
-@overload
-def get_finder(
-    import_path: Literal["django.contrib.staticfiles.finders.FileSystemFinder"],
-) -> FileSystemFinder: ...
-@overload
-def get_finder(
-    import_path: Literal["django.contrib.staticfiles.finders.AppDirectoriesFinder"],
-) -> AppDirectoriesFinder: ...
+def get_finder(import_path: str) -> BaseFinder: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/staticfiles/handlers.pyi` & `django-stubs-4.2.2/django-stubs/contrib/staticfiles/handlers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi` & `django-stubs-4.2.2/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/contrib/staticfiles/storage.pyi` & `django-stubs-4.2.2/django-stubs/contrib/staticfiles/storage.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         self, location: _PathCompatible | None = ..., base_url: str | None = ..., *args: Any, **kwargs: Any
     ) -> None: ...
     def path(self, name: _PathCompatible) -> str: ...
 
 class HashedFilesMixin:
     default_template: str
     max_post_process_passes: int
+    support_js_module_import_aggregation: bool
     patterns: Any
     hashed_files: Any
     keep_intermediate_files: bool
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def file_hash(self, name: str, content: File = ...) -> str: ...
     def hashed_name(self, name: str, content: File | None = ..., filename: str | None = ...) -> str: ...
     def url(self, name: str, force: bool = ...) -> str: ...
@@ -34,14 +35,17 @@
     def stored_name(self, name: str) -> str: ...
 
 class ManifestFilesMixin(HashedFilesMixin):
     manifest_version: str
     manifest_name: str
     manifest_strict: bool
     keep_intermediate_files: bool
+    manifest_storage: Storage | None
+    hashed_files: dict[str, str]
+    manifest_hash: str
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def read_manifest(self) -> str: ...
     def load_manifest(self) -> dict[str, Any]: ...
     def save_manifest(self) -> None: ...
     def post_process(self, *args: Any, **kwargs: Any) -> _PostProcessT: ...
     def stored_name(self, name: str) -> str: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/contrib/syndication/views.pyi` & `django-stubs-4.2.2/django-stubs/contrib/syndication/views.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any, Generic, TypeVar
 
 from django.core.exceptions import ObjectDoesNotExist
-from django.db.models import Model
 from django.http.request import HttpRequest
 from django.http.response import HttpResponse
 from django.utils.feedgenerator import Enclosure, SyndicationFeed
 
 def add_domain(domain: str, url: str, secure: bool = ...) -> str: ...
 
 class FeedDoesNotExist(ObjectDoesNotExist): ...
```

### Comparing `django-stubs-4.2.1/django-stubs/core/cache/__init__.pyi` & `django-stubs-4.2.2/django-stubs/core/cache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/cache/backends/base.pyi` & `django-stubs-4.2.2/django-stubs/core/cache/backends/base.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections.abc import Callable, Iterable
+from collections.abc import Callable, Iterable, Iterator
 from typing import Any
 
 from django.core.exceptions import ImproperlyConfigured
 
 class InvalidCacheBackendError(ImproperlyConfigured): ...
 class CacheKeyWarning(RuntimeWarning): ...
 class InvalidCacheKey(ValueError): ...
@@ -61,7 +61,9 @@
     async def aclear(self) -> None: ...
     def incr_version(self, key: Any, delta: int = ..., version: int | None = ...) -> int: ...
     async def aincr_version(self, key: Any, delta: int = ..., version: int | None = ...) -> int: ...
     def decr_version(self, key: Any, delta: int = ..., version: int | None = ...) -> int: ...
     async def adecr_version(self, key: Any, delta: int = ..., version: int | None = ...) -> int: ...
     def close(self, **kwargs: Any) -> None: ...
     async def aclose(self, **kwargs: Any) -> None: ...
+
+def memcache_key_warnings(key: str) -> Iterator[str]: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/core/cache/backends/db.pyi` & `django-stubs-4.2.2/django-stubs/core/cache/backends/db.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/cache/backends/memcached.pyi` & `django-stubs-4.2.2/django-stubs/core/cache/backends/memcached.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/checks/__init__.pyi` & `django-stubs-4.2.2/django-stubs/core/checks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/checks/caches.pyi` & `django-stubs-4.2.2/django-stubs/core/checks/caches.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/checks/messages.pyi` & `django-stubs-4.2.2/django-stubs/core/checks/messages.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/checks/registry.pyi` & `django-stubs-4.2.2/django-stubs/core/checks/registry.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 from typing import Any, Protocol, TypeVar, overload
 
 from django.apps.config import AppConfig
 from django.core.checks.messages import CheckMessage
 
 class Tags:
     admin: str
+    async_support: str
     caches: str
     compatibility: str
     database: str
+    files: str
     models: str
     security: str
     signals: str
     sites: str
     staticfiles: str
     templates: str
     translation: str
```

### Comparing `django-stubs-4.2.1/django-stubs/core/checks/security/base.pyi` & `django-stubs-4.2.2/django-stubs/core/checks/security/base.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from collections.abc import Sequence
 from typing import Any
 
 from django.apps.config import AppConfig
-from django.core.checks.messages import CheckMessage, Error, Warning
+from django.core.checks.messages import Error, Warning
 
+CROSS_ORIGIN_OPENER_POLICY_VALUES: set[str]
+REFERRER_POLICY_VALUES: set[str]
+SECRET_KEY_INSECURE_PREFIX: str
 SECRET_KEY_MIN_LENGTH: int
 SECRET_KEY_MIN_UNIQUE_CHARACTERS: int
+SECRET_KEY_WARNING_MSG: str
 W001: Warning
 W002: Warning
 W004: Warning
 W005: Warning
 W006: Warning
-W007: Warning
 W008: Warning
 W009: Warning
 W018: Warning
 W019: Warning
 W020: Warning
 W021: Warning
 W022: Warning
 E023: Error
-E100: Error
+E024: Error
+W025: Warning
 
 def check_security_middleware(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
 def check_xframe_options_middleware(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
 def check_sts(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
 def check_sts_include_subdomains(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
 def check_sts_preload(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
 def check_content_type_nosniff(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
 def check_ssl_redirect(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
 def check_secret_key(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
+def check_secret_key_fallbacks(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
 def check_debug(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
 def check_xframe_deny(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
 def check_allowed_hosts(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning]: ...
-def check_referrer_policy(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[CheckMessage]: ...
-def check_default_hashing_algorithm(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Error]: ...
+def check_referrer_policy(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Warning | Error]: ...
+def check_cross_origin_opener_policy(app_configs: Sequence[AppConfig] | None, **kwargs: Any) -> Sequence[Error]: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/core/checks/security/sessions.pyi` & `django-stubs-4.2.2/django-stubs/core/checks/security/sessions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/checks/translation.pyi` & `django-stubs-4.2.2/django-stubs/core/checks/translation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/checks/urls.pyi` & `django-stubs-4.2.2/django-stubs/core/checks/urls.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/exceptions.pyi` & `django-stubs-4.2.2/django-stubs/core/exceptions.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from collections.abc import Iterator
-from typing import Any
+from typing import Any, Literal
 
 from django.utils.functional import _StrOrPromise
-from typing_extensions import Literal
 
 class FieldDoesNotExist(Exception): ...
 class AppRegistryNotReady(Exception): ...
 
 class ObjectDoesNotExist(Exception):
     silent_variable_failure: bool
```

### Comparing `django-stubs-4.2.1/django-stubs/core/files/base.pyi` & `django-stubs-4.2.2/django-stubs/core/files/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/files/storage/__init__.pyi` & `django-stubs-4.2.2/django-stubs/core/files/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/files/storage/base.pyi` & `django-stubs-4.2.2/django-stubs/core/files/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/files/storage/filesystem.pyi` & `django-stubs-4.2.2/django-stubs/core/files/storage/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/files/storage/memory.pyi` & `django-stubs-4.2.2/django-stubs/core/files/storage/memory.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/files/uploadedfile.pyi` & `django-stubs-4.2.2/django-stubs/core/files/uploadedfile.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import IO, TypeVar
+from typing import IO
 
 from _typeshed import Self
 from django.core.files.base import File
 
 class UploadedFile(File):
     content_type: str | None
     charset: str | None
```

### Comparing `django-stubs-4.2.1/django-stubs/core/files/uploadhandler.pyi` & `django-stubs-4.2.2/django-stubs/core/files/uploadhandler.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/files/utils.pyi` & `django-stubs-4.2.2/django-stubs/core/files/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/handlers/asgi.pyi` & `django-stubs-4.2.2/django-stubs/core/handlers/asgi.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/handlers/base.pyi` & `django-stubs-4.2.2/django-stubs/core/handlers/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/handlers/exception.pyi` & `django-stubs-4.2.2/django-stubs/core/handlers/exception.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/handlers/wsgi.pyi` & `django-stubs-4.2.2/django-stubs/core/handlers/wsgi.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/mail/__init__.pyi` & `django-stubs-4.2.2/django-stubs/core/mail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/mail/backends/base.pyi` & `django-stubs-4.2.2/django-stubs/core/mail/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/mail/message.pyi` & `django-stubs-4.2.2/django-stubs/core/mail/message.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     encoding: str
     def __init__(
         self,
         _subtype: str = ...,
         boundary: Any | None = ...,
         _subparts: Any | None = ...,
         encoding: str = ...,
-        **_params: Any
+        **_params: Any,
     ) -> None: ...
     def __setitem__(self, name: str, val: str) -> None: ...
 
 _AttachmentContent: TypeAlias = bytes | EmailMessage | Message | SafeMIMEText | str
 _AttachmentTuple: TypeAlias = (
     tuple[str, _AttachmentContent] | tuple[str | None, _AttachmentContent, str] | tuple[str, _AttachmentContent, None]
 )
```

### Comparing `django-stubs-4.2.1/django-stubs/core/management/__init__.pyi` & `django-stubs-4.2.2/django-stubs/core/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/management/base.pyi` & `django-stubs-4.2.2/django-stubs/core/management/base.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from argparse import ArgumentParser, HelpFormatter, Namespace
 from collections.abc import Callable, Iterable, Sequence
 from io import TextIOBase
-from typing import Any, TextIO
+from typing import Any, Literal, TextIO
 
 from django.apps.config import AppConfig
 from django.core.management.color import Style
 from django.utils.datastructures import _ListOrTuple
-from typing_extensions import Literal
 
 class CommandError(Exception):
     def __init__(self, *args: Any, returncode: int = ..., **kwargs: Any) -> None: ...
 
 class SystemCheckError(CommandError): ...
 
 class CommandParser(ArgumentParser):
```

### Comparing `django-stubs-4.2.1/django-stubs/core/management/color.pyi` & `django-stubs-4.2.2/django-stubs/core/management/color.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/management/commands/diffsettings.pyi` & `django-stubs-4.2.2/django-stubs/core/management/commands/diffsettings.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/management/commands/inspectdb.pyi` & `django-stubs-4.2.2/django-stubs/core/management/commands/inspectdb.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/management/commands/loaddata.pyi` & `django-stubs-4.2.2/django-stubs/core/management/commands/loaddata.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/management/commands/makemessages.pyi` & `django-stubs-4.2.2/django-stubs/core/management/commands/makemessages.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/management/commands/migrate.pyi` & `django-stubs-4.2.2/django-stubs/core/management/commands/migrate.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/management/commands/runserver.pyi` & `django-stubs-4.2.2/django-stubs/core/management/commands/runserver.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/management/templates.pyi` & `django-stubs-4.2.2/django-stubs/core/management/templates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/management/utils.pyi` & `django-stubs-4.2.2/django-stubs/core/management/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/paginator.pyi` & `django-stubs-4.2.2/django-stubs/core/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from collections.abc import Iterable, Iterator, Sequence, Sized
 from typing import Generic, Protocol, TypeVar, overload
 
-from django.db.models.base import Model
-from django.db.models.query import QuerySet
 from typing_extensions import TypeAlias
 
 class UnorderedObjectListWarning(RuntimeWarning): ...
 class InvalidPage(Exception): ...
 class PageNotAnInteger(InvalidPage): ...
 class EmptyPage(InvalidPage): ...
```

### Comparing `django-stubs-4.2.1/django-stubs/core/serializers/__init__.pyi` & `django-stubs-4.2.2/django-stubs/core/serializers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/serializers/base.pyi` & `django-stubs-4.2.2/django-stubs/core/serializers/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         *,
         stream: IO[str] | None = ...,
         fields: Collection[str] | None = ...,
         use_natural_foreign_keys: bool = ...,
         use_natural_primary_keys: bool = ...,
         progress_output: IO[str] | None = ...,
         object_count: int = ...,
-        **options: Any
+        **options: Any,
     ) -> Any: ...
     def start_serialization(self) -> None: ...
     def end_serialization(self) -> None: ...
     def start_object(self, obj: Any) -> None: ...
     def end_object(self, obj: Any) -> None: ...
     def handle_field(self, obj: Any, field: Any) -> None: ...
     def handle_fk_field(self, obj: Any, field: Any) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/core/serializers/json.pyi` & `django-stubs-4.2.2/django-stubs/core/serializers/json.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/serializers/pyyaml.pyi` & `django-stubs-4.2.2/django-stubs/core/serializers/pyyaml.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/serializers/xml_serializer.pyi` & `django-stubs-4.2.2/django-stubs/core/serializers/xml_serializer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     ignore: bool
     def __init__(
         self,
         stream_or_string: bytes | str | IO[bytes] | IO[str],
         *,
         using: str = ...,
         ignorenonexistent: bool = ...,
-        **options: Any
+        **options: Any,
     ) -> None: ...
     def __next__(self) -> base.DeserializedObject: ...
 
 def getInnerText(node: Any) -> str: ...
 
 class DefusedExpatParser(_ExpatParser):
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/core/servers/basehttp.pyi` & `django-stubs-4.2.2/django-stubs/core/servers/basehttp.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/signing.pyi` & `django-stubs-4.2.2/django-stubs/core/signing.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/core/validators.pyi` & `django-stubs-4.2.2/django-stubs/core/validators.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -53,21 +53,15 @@
     literal_regex: Pattern[str]
     domain_allowlist: Sequence[str]
     def __init__(
         self,
         message: _StrOrPromise | None = ...,
         code: str | None = ...,
         allowlist: Sequence[str] | None = ...,
-        *,
-        whitelist: Sequence[str] | None = ...,
     ) -> None: ...
-    @property
-    def domain_whitelist(self) -> Sequence[str]: ...
-    @domain_whitelist.setter
-    def domain_whitelist(self, allowlist: Sequence[str]) -> None: ...
     def __call__(self, value: str | None) -> None: ...
     def validate_domain_part(self, domain_part: str) -> bool: ...
     def __eq__(self, other: object) -> bool: ...
 
 validate_email: EmailValidator
 slug_re: Pattern[str]
 validate_slug: RegexValidator
@@ -96,14 +90,15 @@
     def __call__(self, value: Any) -> None: ...
     def compare(self, a: Any, b: Any) -> bool: ...
     def clean(self, x: Any) -> Any: ...
     def __eq__(self, other: object) -> bool: ...
 
 class MaxValueValidator(BaseValidator): ...
 class MinValueValidator(BaseValidator): ...
+class StepValueValidator(BaseValidator): ...
 
 class MinLengthValidator(BaseValidator):
     def clean(self, x: Sized) -> int: ...
 
 class MaxLengthValidator(BaseValidator):
     def clean(self, x: Sized) -> int: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/__init__.pyi` & `django-stubs-4.2.2/django-stubs/db/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/base/base.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/base/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/base/client.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/base/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/base/creation.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/base/creation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/base/features.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/base/features.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from django.db.models.base import Model
 from django.db.utils import DatabaseError
 
 class BaseDatabaseFeatures:
     minimum_database_version: tuple[int, ...] | None
     gis_enabled: bool
     allows_group_by_lob: bool
-    allows_group_by_pk: bool
     allows_group_by_selected_pks: bool
     empty_fetchmany_value: Sequence[Any]
     update_can_self_select: bool
     interprets_empty_strings_as_nulls: bool
     supports_nullable_unique_constraints: bool
     supports_partially_nullable_unique_constraints: bool
     supports_deferrable_unique_constraints: bool
```

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/base/introspection.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/base/introspection.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -23,11 +23,11 @@
     def get_table_list(self, cursor: CursorWrapper | None) -> Any: ...
     def get_table_description(self, cursor: CursorWrapper | None, table_name: str) -> Any: ...
     def get_migratable_models(self) -> Iterable[type[Model]]: ...
     def django_table_names(self, only_existing: bool = ..., include_views: bool = ...) -> list[str]: ...
     def installed_models(self, tables: list[str]) -> set[type[Model]]: ...
     def sequence_list(self) -> list[dict[str, str]]: ...
     def get_sequences(self, cursor: CursorWrapper | None, table_name: str, table_fields: Any = ...) -> Any: ...
-    def get_relations(self, cursor: CursorWrapper | None, table_name: str) -> Any: ...
-    def get_key_columns(self, cursor: CursorWrapper | None, table_name: str) -> Any: ...
+    def get_relations(self, cursor: CursorWrapper | None, table_name: str) -> dict[str, tuple[str, str]]: ...
     def get_primary_key_column(self, cursor: CursorWrapper | None, table_name: str) -> str | None: ...
+    def get_primary_key_columns(self, cursor: CursorWrapper | None, table_name: str) -> list[str] | None: ...
     def get_constraints(self, cursor: CursorWrapper | None, table_name: str) -> Any: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/base/operations.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/base/operations.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import json
 from collections.abc import Iterable, Sequence
-from datetime import date
+from datetime import date, time, timedelta
 from datetime import datetime as real_datetime
-from datetime import time, timedelta
 from decimal import Decimal
 from typing import Any
 
 from django.core.management.color import Style
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.utils import CursorWrapper
 from django.db.models.base import Model
+from django.db.models.constants import OnConflict
 from django.db.models.expressions import Case, Expression
 from django.db.models.fields import Field
 from django.db.models.sql.compiler import SQLCompiler
 
 class BaseDatabaseOperations:
     compiler_module: str
     integer_field_ranges: dict[str, tuple[int, int]]
@@ -27,23 +28,23 @@
     explain_prefix: str | None
     connection: BaseDatabaseWrapper
     def __init__(self, connection: BaseDatabaseWrapper) -> None: ...
     def autoinc_sql(self, table: str, column: str) -> str | None: ...
     def bulk_batch_size(self, fields: Any, objs: Any) -> int: ...
     def cache_key_culling_sql(self) -> str: ...
     def unification_cast_sql(self, output_field: Field) -> str: ...
-    def date_extract_sql(self, lookup_type: str, field_name: str) -> Any: ...
+    def date_extract_sql(self, lookup_type: str, sql: Any, params: Any) -> tuple[str, Any]: ...
     # def date_interval_sql(self, timedelta: None) -> Any: ...
-    def date_trunc_sql(self, lookup_type: str, field_name: str, tzname: str | None = ...) -> str: ...
-    def datetime_cast_date_sql(self, field_name: str, tzname: str | None) -> str: ...
-    def datetime_cast_time_sql(self, field_name: str, tzname: str | None) -> str: ...
-    def datetime_extract_sql(self, lookup_type: str, field_name: str, tzname: str | None) -> str: ...
-    def datetime_trunc_sql(self, lookup_type: str, field_name: str, tzname: str | None) -> str: ...
-    def time_trunc_sql(self, lookup_type: str, field_name: str, tzname: str | None = ...) -> str: ...
-    def time_extract_sql(self, lookup_type: str, field_name: str) -> str: ...
+    def date_trunc_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None = ...) -> tuple[str, Any]: ...
+    def datetime_cast_date_sql(self, sql: str, params: Any, tzname: str | None) -> tuple[str, Any]: ...
+    def datetime_cast_time_sql(self, sql: str, params: Any, tzname: str | None) -> tuple[str, Any]: ...
+    def datetime_extract_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None) -> tuple[str, Any]: ...
+    def datetime_trunc_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None) -> str: ...
+    def time_trunc_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None = ...) -> str: ...
+    def time_extract_sql(self, lookup_type: str, sql: str, params: Any) -> str: ...
     def deferrable_sql(self) -> str: ...
     def distinct_sql(self, fields: list[str], params: list[Any] | None) -> tuple[list[str], list[str]]: ...
     def fetch_returned_insert_columns(self, cursor: Any, returning_params: Any) -> Any: ...
     def field_cast_sql(self, db_type: str | None, internal_type: str) -> str: ...
     def force_no_ordering(self) -> list[Any]: ...
     def for_update_sql(self, nowait: bool = ..., skip_locked: bool = ..., of: Any = ..., no_key: bool = ...) -> str: ...
     def limit_offset_sql(self, low_mark: int, high_mark: int | None) -> str: ...
@@ -80,16 +81,18 @@
     def adapt_datefield_value(self, value: date | None) -> str | None: ...
     def adapt_datetimefield_value(self, value: real_datetime | None) -> str | None: ...
     def adapt_timefield_value(self, value: real_datetime | time | None) -> str | None: ...
     def adapt_decimalfield_value(
         self, value: Decimal | None, max_digits: int | None = ..., decimal_places: int | None = ...
     ) -> str | None: ...
     def adapt_ipaddressfield_value(self, value: str | None) -> str | None: ...
-    def year_lookup_bounds_for_date_field(self, value: int) -> list[str]: ...
-    def year_lookup_bounds_for_datetime_field(self, value: int) -> list[str]: ...
+    def adapt_json_value(self, value: Any, encoder: type[json.JSONEncoder] | None) -> str: ...
+    def adapt_integerfield_value(self, value: Any, internal_type: Any) -> Any: ...
+    def year_lookup_bounds_for_date_field(self, value: int, iso_year: bool = ...) -> list[str]: ...
+    def year_lookup_bounds_for_datetime_field(self, value: int, iso_year: bool = ...) -> list[str]: ...
     def get_db_converters(self, expression: Expression) -> list[Any]: ...
     def convert_durationfield_value(
         self, value: float | None, expression: Expression, connection: BaseDatabaseWrapper
     ) -> timedelta | None: ...
     def check_expression_support(self, expression: Any) -> None: ...
     def conditional_expression_supported_in_where_clause(self, expression: Any) -> bool: ...
     def combine_expression(self, connector: str, sub_expressions: list[str]) -> str: ...
@@ -99,9 +102,12 @@
     def integer_field_range(self, internal_type: Any) -> tuple[int, int]: ...
     def subtract_temporals(self, internal_type: Any, lhs: Any, rhs: Any) -> tuple[str, tuple[Any, ...]]: ...
     def window_frame_start(self, start: Any) -> str: ...
     def window_frame_end(self, end: Any) -> str: ...
     def window_frame_rows_start_end(self, start: int | None = ..., end: int | None = ...) -> tuple[str, str]: ...
     def window_frame_range_start_end(self, start: int | None = ..., end: int | None = ...) -> tuple[str, str]: ...
     def explain_query_prefix(self, format: str | None = ..., **options: Any) -> str: ...
-    def insert_statement(self, ignore_conflicts: bool = ...) -> str: ...
-    def ignore_conflicts_suffix_sql(self, ignore_conflicts: Any | None = ...) -> str: ...
+    def insert_statement(self, on_conflict: OnConflict | None = ...) -> str: ...
+    def on_conflict_suffix_sql(
+        self, fields: Any, on_conflict: Any, update_fields: Any, unique_fields: Any
+    ) -> str | Any: ...
+    def format_for_duration_arithmetic(self, sql: str) -> str: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/base/schema.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/base/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/ddl_references.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/ddl_references.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/dummy/base.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/dummy/base.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -19,12 +19,11 @@
     destroy_test_db: Any
 
 class DatabaseIntrospection(BaseDatabaseIntrospection):
     get_table_list: Any
     get_table_description: Any
     get_relations: Any
     get_indexes: Any
-    get_key_columns: Any
 
 class DatabaseWrapper(BaseDatabaseWrapper):
     operators: Any
     ensure_connection: Any
```

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/mysql/base.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/mysql/base.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from collections.abc import Container, Iterator
-from typing import Any
+from typing import Any, Literal
 
 from django.db.backends.base.base import BaseDatabaseWrapper
-from typing_extensions import Literal
 
 from .client import DatabaseClient
 from .creation import DatabaseCreation
 from .features import DatabaseFeatures
 from .introspection import DatabaseIntrospection
 from .operations import DatabaseOperations
 from .validation import DatabaseValidation
```

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/mysql/compiler.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/mysql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/mysql/features.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/mysql/operations.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/mysql/operations.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Any
 
 from django.db.backends.base.operations import BaseDatabaseOperations
 from django.db.backends.mysql.base import DatabaseWrapper
+from django.db.models.constants import OnConflict
 
 class DatabaseOperations(BaseDatabaseOperations):
     connection: DatabaseWrapper
     compiler_module: str
     integer_field_ranges: dict[str, tuple[int, int]]
     cast_data_types: dict[str, str]
     cast_char_field_without_max_length: str
     explain_prefix: str
-    def date_extract_sql(self, lookup_type: str, field_name: str) -> Any: ...
-    def date_trunc_sql(self, lookup_type: str, field_name: str, tzname: str | None = ...) -> Any: ...
-    def datetime_cast_date_sql(self, field_name: str, tzname: str | None) -> Any: ...
-    def datetime_cast_time_sql(self, field_name: str, tzname: str | None) -> Any: ...
-    def datetime_extract_sql(self, lookup_type: str, field_name: str, tzname: str | None) -> Any: ...
-    def datetime_trunc_sql(self, lookup_type: str, field_name: str, tzname: str | None) -> Any: ...
-    def time_trunc_sql(self, lookup_type: str, field_name: str, tzname: str | None = ...) -> Any: ...
+    def date_extract_sql(self, lookup_type: str, sql: str, params: Any) -> tuple[str, Any]: ...
+    def date_trunc_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None = ...) -> Any: ...
+    def datetime_cast_date_sql(self, sql: str, params: Any, tzname: str | None) -> Any: ...
+    def datetime_cast_time_sql(self, sql: str, params: Any, tzname: str | None) -> Any: ...
+    def datetime_extract_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None) -> Any: ...
+    def datetime_trunc_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None) -> Any: ...
+    def time_trunc_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None = ...) -> Any: ...
     def fetch_returned_insert_rows(self, cursor: Any) -> Any: ...
     def format_for_duration_arithmetic(self, sql: Any) -> Any: ...
     def force_no_ordering(self) -> Any: ...
     def last_executed_query(self, cursor: Any, sql: Any, params: Any) -> Any: ...
     def no_limit_value(self) -> Any: ...
     def quote_name(self, name: str) -> Any: ...
     def return_insert_columns(self, fields: Any) -> Any: ...
@@ -35,9 +36,9 @@
     def convert_booleanfield_value(self, value: Any, expression: Any, connection: Any) -> Any: ...
     def convert_datetimefield_value(self, value: Any, expression: Any, connection: Any) -> Any: ...
     def convert_uuidfield_value(self, value: Any, expression: Any, connection: Any) -> Any: ...
     def binary_placeholder_sql(self, value: Any) -> Any: ...
     def subtract_temporals(self, internal_type: Any, lhs: Any, rhs: Any) -> Any: ...
     def explain_query_prefix(self, format: Any | None = ..., **options: Any) -> Any: ...
     def regex_lookup(self, lookup_type: str) -> Any: ...
-    def insert_statement(self, ignore_conflicts: bool = ...) -> Any: ...
+    def insert_statement(self, on_conflict: OnConflict | None = ...) -> str: ...
     def lookup_cast(self, lookup_type: str, internal_type: Any | None = ...) -> Any: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/mysql/schema.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/oracle/base.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/oracle/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/oracle/client.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/oracle/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/oracle/features.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/oracle/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/oracle/operations.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/oracle/operations.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 class DatabaseOperations(BaseDatabaseOperations):
     connection: DatabaseWrapper
     integer_field_ranges: Any
     set_operators: Any
     cast_char_field_without_max_length: str
     cast_data_types: Any
     def cache_key_culling_sql(self) -> str: ...
-    def date_extract_sql(self, lookup_type: str, field_name: str) -> str: ...
-    def date_trunc_sql(self, lookup_type: str, field_name: str, tzname: str | None = ...) -> str: ...
-    def datetime_cast_date_sql(self, field_name: str, tzname: str | None) -> str: ...
-    def datetime_cast_time_sql(self, field_name: str, tzname: str | None) -> str: ...
-    def datetime_extract_sql(self, lookup_type: str, field_name: str, tzname: str | None) -> str: ...
-    def datetime_trunc_sql(self, lookup_type: str, field_name: str, tzname: str | None) -> str: ...
-    def time_trunc_sql(self, lookup_type: str, field_name: str, tzname: str | None = ...) -> str: ...
+    def date_extract_sql(self, lookup_type: str, sql: str, params: Any) -> tuple[str, Any]: ...
+    def date_trunc_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None = ...) -> tuple[str, Any]: ...
+    def datetime_cast_date_sql(self, sql: str, params: Any, tzname: str | None) -> tuple[str, Any]: ...
+    def datetime_cast_time_sql(self, sql: str, params: Any, tzname: str | None) -> tuple[str, Any]: ...
+    def datetime_extract_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None) -> tuple[str, Any]: ...
+    def datetime_trunc_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None) -> str: ...
+    def time_trunc_sql(self, lookup_type: str, sql: str, params: Any, tzname: str | None = ...) -> str: ...
     def get_db_converters(self, expression: Any) -> list[Any]: ...
     def convert_textfield_value(self, value: Any, expression: Any, connection: Any) -> Any: ...
     def convert_binaryfield_value(self, value: Any, expression: Any, connection: Any) -> Any: ...
     def convert_booleanfield_value(self, value: Any, expression: Any, connection: Any) -> Any: ...
     def convert_datetimefield_value(self, value: Any, expression: Any, connection: Any) -> Any: ...
     def convert_datefield_value(self, value: Any, expression: Any, connection: Any) -> Any: ...
     def convert_timefield_value(self, value: Any, expression: Any, connection: Any) -> Any: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/oracle/schema.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/postgresql/base.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/postgresql/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/postgresql/client.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/postgresql/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/postgresql/features.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/postgresql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/postgresql/schema.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/postgresql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/sqlite3/base.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/sqlite3/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/backends/utils.pyi` & `django-stubs-4.2.2/django-stubs/db/backends/utils.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import datetime
 from collections.abc import Generator, Iterator, Mapping, Sequence
 from contextlib import contextmanager
 from decimal import Decimal
 from logging import Logger
 from types import TracebackType
-from typing import Any, Protocol, overload
+from typing import Any, Literal, Protocol, overload
 from uuid import UUID
 
 from _typeshed import Self
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import TypeAlias
 
 logger: Logger
 
 # Protocol matching psycopg2.sql.Composable, to avoid depending psycopg2
 class _Composable(Protocol):
     def as_string(self, context: Any) -> str: ...
     def __add__(self, other: _Composable) -> _Composable: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/autodetector.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/autodetector.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/exceptions.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/executor.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/executor.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/graph.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/graph.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Sequence
 from typing import Any
 
-from django.db.migrations.migration import Migration, SwappableTuple
+from django.db.migrations.migration import Migration
 from django.db.migrations.state import ProjectState
 
 RECURSION_DEPTH_WARNING: str
 
 class Node:
     key: tuple[str, str]
     children: set[Any]
```

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/loader.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/loader.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/migration.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/migration.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/operations/__init__.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/operations/__init__.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .fields import RenameField as RenameField
 from .models import AddConstraint as AddConstraint
 from .models import AddIndex as AddIndex
 from .models import AlterIndexTogether as AlterIndexTogether
 from .models import AlterModelManagers as AlterModelManagers
 from .models import AlterModelOptions as AlterModelOptions
 from .models import AlterModelTable as AlterModelTable
+from .models import AlterModelTableComment as AlterModelTableComment
 from .models import AlterOrderWithRespectTo as AlterOrderWithRespectTo
 from .models import AlterUniqueTogether as AlterUniqueTogether
 from .models import CreateModel as CreateModel
 from .models import DeleteModel as DeleteModel
 from .models import RemoveConstraint as RemoveConstraint
 from .models import RemoveIndex as RemoveIndex
 from .models import RenameIndex as RenameIndex
```

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/operations/base.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/operations/base.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from collections.abc import Sequence
 from typing import Any
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.migrations.state import ProjectState
 from django.db.models import Model
+from typing_extensions import Self
 
 class Operation:
     reversible: bool
     reduces_to_sql: bool
     atomic: bool
     elidable: bool
     serialization_expand_args: list[str]
     _constructor_args: tuple[Sequence[Any], dict[str, Any]]
+    def __new__(cls, *args: Any, **kwargs: Any) -> Self: ...
     def deconstruct(self) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
     def state_forwards(self, app_label: str, state: ProjectState) -> None: ...
     def database_forwards(
         self, app_label: str, schema_editor: BaseDatabaseSchemaEditor, from_state: ProjectState, to_state: ProjectState
     ) -> None: ...
     def database_backwards(
         self, app_label: str, schema_editor: BaseDatabaseSchemaEditor, from_state: ProjectState, to_state: ProjectState
```

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/operations/fields.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/operations/fields.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from django.db.models.fields import Field
+from django.utils.functional import cached_property
 
 from .base import Operation
 
 class FieldOperation(Operation):
     model_name: str
     name: str
     def __init__(self, model_name: str, name: str, field: Field | None = ...) -> None: ...
-    @property
+    @cached_property
     def name_lower(self) -> str: ...
-    @property
+    @cached_property
     def model_name_lower(self) -> str: ...
     def is_same_model_operation(self, operation: FieldOperation) -> bool: ...
     def is_same_field_operation(self, operation: FieldOperation) -> bool: ...
 
 class AddField(FieldOperation):
     field: Field
     preserve_default: bool
@@ -25,11 +26,11 @@
     preserve_default: bool
     def __init__(self, model_name: str, name: str, field: Field, preserve_default: bool = ...) -> None: ...
 
 class RenameField(FieldOperation):
     old_name: str
     new_name: str
     def __init__(self, model_name: str, old_name: str, new_name: str) -> None: ...
-    @property
+    @cached_property
     def old_name_lower(self) -> str: ...
-    @property
+    @cached_property
     def new_name_lower(self) -> str: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/operations/models.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/operations/models.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from django.db.migrations.operations.base import Operation
 from django.db.models.base import Model
 from django.db.models.constraints import BaseConstraint
 from django.db.models.fields import Field
 from django.db.models.indexes import Index
 from django.db.models.manager import Manager
 from django.db.models.options import _OptionTogetherT
+from django.utils.functional import cached_property
 
 class ModelOperation(Operation):
     name: str
     def __init__(self, name: str) -> None: ...
-    @property
+    @cached_property
     def name_lower(self) -> str: ...
+    def can_reduce_through(self, operation: Operation, app_label: str) -> bool: ...
 
 class CreateModel(ModelOperation):
     fields: list[tuple[str, Field]]
     options: dict[str, Any]
     bases: Sequence[type[Model] | str] | None
     managers: Sequence[tuple[str, Manager]] | None
     def __init__(
@@ -32,33 +34,48 @@
 
 class DeleteModel(ModelOperation): ...
 
 class RenameModel(ModelOperation):
     old_name: str
     new_name: str
     def __init__(self, old_name: str, new_name: str) -> None: ...
-    @property
+    @cached_property
     def old_name_lower(self) -> str: ...
-    @property
+    @cached_property
     def new_name_lower(self) -> str: ...
 
 class ModelOptionOperation(ModelOperation): ...
 
 class AlterModelTable(ModelOptionOperation):
     table: str | None
     def __init__(self, name: str, table: str | None) -> None: ...
 
+class AlterModelTableComment(ModelOptionOperation):
+    table_comment: str
+    def __init__(self, name: str, table_comment: str) -> None: ...
+    def deconstruct(self) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
+    def state_forwards(self, app_label: str, state: Any) -> None: ...
+    def database_forwards(
+        self, app_label: str, schema_editor: BaseDatabaseSchemaEditor, from_state: Any, to_state: Any
+    ) -> None: ...
+    def database_backwards(
+        self, app_label: str, schema_editor: BaseDatabaseSchemaEditor, from_state: Any, to_state: Any
+    ) -> None: ...
+    def describe(self) -> str: ...
+    @property
+    def migration_name_fragment(self) -> str: ...
+
 class AlterTogetherOptionOperation(ModelOptionOperation):
     option_name: str
     def __init__(
         self,
         name: str,
         option_value: _OptionTogetherT | None,
     ) -> None: ...
-    @property
+    @cached_property
     def option_value(self) -> set[tuple[str, ...]] | None: ...
     def deconstruct(self) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
     def state_forwards(self, app_label: str, state: Any) -> None: ...
     def database_forwards(
         self, app_label: str, schema_editor: BaseDatabaseSchemaEditor, from_state: Any, to_state: Any
     ) -> None: ...
     def database_backwards(
@@ -76,29 +93,30 @@
 
 class AlterIndexTogether(AlterTogetherOptionOperation):
     option_name: str
     index_together: set[tuple[str, ...]] | None
     def __init__(self, name: str, index_together: _OptionTogetherT | None) -> None: ...
 
 class AlterOrderWithRespectTo(ModelOptionOperation):
+    option_name: str
     order_with_respect_to: str
     def __init__(self, name: str, order_with_respect_to: str) -> None: ...
 
 class AlterModelOptions(ModelOptionOperation):
     ALTER_OPTION_KEYS: list[str]
     options: dict[str, Any]
     def __init__(self, name: str, options: dict[str, Any]) -> None: ...
 
 class AlterModelManagers(ModelOptionOperation):
     managers: Sequence[tuple[str, Manager]]
     def __init__(self, name: str, managers: Sequence[tuple[str, Manager]]) -> None: ...
 
 class IndexOperation(Operation):
     option_name: str
-    @property
+    @cached_property
     def model_name_lower(self) -> str: ...
 
 class AddIndex(IndexOperation):
     model_name: str
     index: Index
     def __init__(self, model_name: str, index: Index) -> None: ...
 
@@ -115,17 +133,17 @@
     def __init__(
         self,
         model_name: str,
         new_name: str,
         old_name: str | None = ...,
         old_fields: Sequence[str] | None = ...,
     ) -> None: ...
-    @property
+    @cached_property
     def old_name_lower(self) -> str: ...
-    @property
+    @cached_property
     def new_name_lower(self) -> str: ...
 
 class AddConstraint(IndexOperation):
     def __init__(self, model_name: str, constraint: BaseConstraint) -> None: ...
 
 class RemoveConstraint(IndexOperation):
     def __init__(self, model_name: str, name: str) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/operations/special.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/operations/special.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from collections.abc import Mapping, Sequence
-from typing import Any, Optional, Protocol  # noqa: Y037  # https://github.com/python/mypy/issues/12211
+from typing import Any, Literal, Protocol
 
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.migrations.state import StateApps
 from django.utils.datastructures import _ListOrTuple
-from typing_extensions import Literal
 
 from .base import Operation
 
 class SeparateDatabaseAndState(Operation):
     database_operations: Sequence[Operation]
     state_operations: Sequence[Operation]
+
     def __init__(
-        self, database_operations: Sequence[Operation] = ..., state_operations: Sequence[Operation] = ...
+        self, database_operations: Sequence[Operation] | None = ..., state_operations: Sequence[Operation] | None = ...
     ) -> None: ...
 
 class RunSQL(Operation):
     noop: Literal[""]
-    sql: str | _ListOrTuple[str | tuple[str, dict[str, Any] | Optional[_ListOrTuple[str]]]]
-    reverse_sql: str | None | _ListOrTuple[str | tuple[str, dict[str, Any] | Optional[_ListOrTuple[str]]]]
+    sql: str | _ListOrTuple[str | tuple[str, dict[str, Any] | _ListOrTuple[str] | None]]
+    reverse_sql: str | None | _ListOrTuple[str | tuple[str, dict[str, Any] | _ListOrTuple[str] | None]]
     state_operations: Sequence[Operation]
     hints: Mapping[str, Any]
     def __init__(
         self,
-        sql: str | _ListOrTuple[str | tuple[str, dict[str, Any] | Optional[_ListOrTuple[str]]]],
-        reverse_sql: str | None | _ListOrTuple[str | tuple[str, dict[str, Any] | Optional[_ListOrTuple[str]]]] = ...,
-        state_operations: Sequence[Operation] = ...,
+        sql: str | _ListOrTuple[str | tuple[str, dict[str, Any] | _ListOrTuple[str] | None]],
+        reverse_sql: str | None | _ListOrTuple[str | tuple[str, dict[str, Any] | _ListOrTuple[str] | None]] = ...,
+        state_operations: Sequence[Operation] | None = ...,
         hints: Mapping[str, Any] | None = ...,
         elidable: bool = ...,
     ) -> None: ...
+    @property
+    def reversible(self) -> bool: ...  # type: ignore[override]
 
 class _CodeCallable(Protocol):
     def __call__(self, __state_apps: StateApps, __schema_editor: BaseDatabaseSchemaEditor) -> None: ...
 
 class RunPython(Operation):
     code: _CodeCallable
     reverse_code: _CodeCallable | None
@@ -43,7 +45,9 @@
         reverse_code: _CodeCallable | None = ...,
         atomic: bool | None = ...,
         hints: Mapping[str, Any] | None = ...,
         elidable: bool = ...,
     ) -> None: ...
     @staticmethod
     def noop(apps: StateApps, schema_editor: BaseDatabaseSchemaEditor) -> None: ...
+    @property
+    def reversible(self) -> bool: ...  # type: ignore[override]
```

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/operations/utils.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/operations/utils.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import namedtuple
 from collections.abc import Iterator
+from typing import Literal
 
 from django.db.migrations.state import ModelState, ProjectState
 from django.db.models import Field, Model
-from typing_extensions import Literal
 
 def resolve_relation(
     model: str | type[Model], app_label: str | None = ..., model_name: str | None = ...
 ) -> tuple[str, str]: ...
 
 FieldReference = namedtuple("FieldReference", ["to", "through"])
```

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/questioner.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/questioner.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/recorder.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/recorder.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/serializer.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/serializer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/state.pyi` & `django-stubs-4.2.2/django-stubs/db/models/indexes.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,58 @@
-from collections.abc import Iterator, Sequence
-from contextlib import contextmanager
+from collections.abc import Sequence
 from typing import Any
 
-from django.apps import AppConfig
-from django.apps.registry import Apps
+from django.db.backends.base.base import BaseDatabaseWrapper
+from django.db.backends.base.schema import BaseDatabaseSchemaEditor
+from django.db.backends.ddl_references import Statement
 from django.db.models.base import Model
-from django.db.models.fields import Field
-from django.db.models.manager import Manager
-
-class AppConfigStub(AppConfig): ...
-
-class ModelState:
+from django.db.models.expressions import BaseExpression, Combinable, Expression, Func
+from django.db.models.query_utils import Q
+from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
+
+class Index:
+    model: type[Model]
+    suffix: str
+    max_name_length: int
+    fields: Sequence[str]
+    fields_orders: Sequence[tuple[str, str]]
     name: str
-    app_label: str
-    fields: dict[str, Field]
-    options: dict[str, Any]
-    bases: Sequence[type[Model] | str]
-    managers: list[tuple[str, Manager]]
+    db_tablespace: str | None
+    opclasses: Sequence[str]
+    condition: Q | None
+    expressions: Sequence[BaseExpression | Combinable]
+    include: Sequence[str]
     def __init__(
         self,
-        app_label: str,
-        name: str,
-        fields: list[tuple[str, Field]] | dict[str, Field],
-        options: dict[str, Any] | None = ...,
-        bases: Sequence[type[Model] | str] | None = ...,
-        managers: list[tuple[str, Manager]] | None = ...,
+        *expressions: BaseExpression | Combinable | str,
+        fields: Sequence[str] = ...,
+        name: str | None = ...,
+        db_tablespace: str | None = ...,
+        opclasses: Sequence[str] = ...,
+        condition: Q | None = ...,
+        include: Sequence[str] | None = ...,
     ) -> None: ...
-    def clone(self) -> ModelState: ...
-    def construct_managers(self) -> Iterator[tuple[str, Manager]]: ...
-    @classmethod
-    def from_model(cls, model: type[Model], exclude_rels: bool = ...) -> ModelState: ...
-    # Removed in 3.2, but back in 4.0
-    # def get_field(self, field_name: str) -> Field: ...
     @property
-    def name_lower(self) -> str: ...
-    def render(self, apps: Apps) -> Any: ...
-    def get_index_by_name(self, name: str) -> Any: ...
-    def get_constraint_by_name(self, name: str) -> Any: ...
-    def __eq__(self, other: object) -> bool: ...
-
-def get_related_models_tuples(model: type[Model]) -> set[tuple[str, str]]: ...
-def get_related_models_recursive(model: type[Model]) -> set[tuple[str, str]]: ...
-
-class ProjectState:
-    is_delayed: bool
-    models: dict[Any, Any]
-    real_apps: list[str]
-    def __init__(
-        self, models: dict[tuple[str, str], ModelState] | None = ..., real_apps: list[str] | None = ...
-    ) -> None: ...
-    def add_model(self, model_state: ModelState) -> None: ...
-    @property
-    def apps(self) -> StateApps: ...
-    def clear_delayed_apps_cache(self) -> None: ...
-    def clone(self) -> ProjectState: ...
-    @property
-    def concrete_apps(self) -> StateApps: ...
+    def contains_expressions(self) -> bool: ...
+    def create_sql(
+        self, model: type[Model], schema_editor: BaseDatabaseSchemaEditor, using: str = ..., **kwargs: Any
+    ) -> Statement: ...
+    def remove_sql(self, model: type[Model], schema_editor: BaseDatabaseSchemaEditor, **kwargs: Any) -> str: ...
+    def deconstruct(self) -> Any: ...
+    def clone(self) -> Index: ...
+    def set_name_with_model(self, model: type[Model]) -> None: ...
+
+class IndexExpression(Func):
+    template: str
+    wrapper_classes: Sequence[Expression]
+    def set_wrapper_classes(self, connection: Any | None = ...) -> None: ...
     @classmethod
-    def from_apps(cls, apps: Apps) -> ProjectState: ...
-    def reload_model(self, app_label: str, model_name: str, delay: bool = ...) -> None: ...
-    def reload_models(self, models: list[Any], delay: bool = ...) -> None: ...
-    def remove_model(self, app_label: str, model_name: str) -> None: ...
-
-class StateApps(Apps):
-    real_models: list[ModelState]
-    def __init__(
-        self, real_apps: list[str], models: dict[tuple[str, str], ModelState], ignore_swappable: bool = ...
-    ) -> None: ...
-    @contextmanager
-    def bulk_update(self) -> Iterator[None]: ...
-    def clone(self) -> StateApps: ...
-    def render_multiple(self, model_states: list[ModelState]) -> None: ...
-    def register_model(self, app_label: str, model: type[Model]) -> None: ...
-    def unregister_model(self, app_label: str, model_name: str) -> None: ...
+    def register_wrappers(cls, *wrapper_classes: Expression) -> None: ...
+    def resolve_expression(
+        self,
+        query: Any | None = ...,
+        allow_joins: bool = ...,
+        reuse: set[str] | None = ...,
+        summarize: bool = ...,
+        for_save: bool = ...,
+    ) -> IndexExpression: ...
+    def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/migrations/writer.pyi` & `django-stubs-4.2.2/django-stubs/db/migrations/writer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/__init__.pyi` & `django-stubs-4.2.2/django-stubs/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/aggregates.pyi` & `django-stubs-4.2.2/django-stubs/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/base.pyi` & `django-stubs-4.2.2/django-stubs/db/models/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from collections.abc import Collection, Iterable, Sequence
-from typing import Any, TypeVar
+from typing import Any, Final, TypeVar
 
 from _typeshed import Self
 from django.core.checks.messages import CheckMessage
 from django.core.exceptions import MultipleObjectsReturned as BaseMultipleObjectsReturned
 from django.core.exceptions import ObjectDoesNotExist, ValidationError
 from django.db.models import BaseConstraint, Field
 from django.db.models.manager import BaseManager
 from django.db.models.options import Options
-from typing_extensions import Final
 
 _Self = TypeVar("_Self", bound=Model)
 
 class ModelStateFieldsCacheDescriptor: ...
 
 class ModelState:
     db: str | None
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/constraints.pyi` & `django-stubs-4.2.2/django-stubs/db/models/constraints.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Sequence
 from enum import Enum
-from typing import Any, TypeVar, overload
+from typing import Any, overload
 
 from _typeshed import Self
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.models.base import Model
 from django.db.models.expressions import BaseExpression, Combinable
 from django.db.models.query_utils import Q
 from django.utils.functional import _StrOrPromise
@@ -42,21 +42,21 @@
         *expressions: str | BaseExpression | Combinable,
         fields: None = ...,
         name: str,
         condition: Q | None = ...,
         deferrable: Deferrable | None = ...,
         include: Sequence[str] | None = ...,
         opclasses: Sequence[Any] = ...,
-        violation_error_message: _StrOrPromise | None = ...
+        violation_error_message: _StrOrPromise | None = ...,
     ) -> None: ...
     @overload
     def __init__(
         self,
         *,
         fields: Sequence[str],
         name: str,
         condition: Q | None = ...,
         deferrable: Deferrable | None = ...,
         include: Sequence[str] | None = ...,
         opclasses: Sequence[Any] = ...,
-        violation_error_message: _StrOrPromise | None = ...
+        violation_error_message: _StrOrPromise | None = ...,
     ) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/deletion.pyi` & `django-stubs-4.2.2/django-stubs/db/models/deletion.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections.abc import Callable, Collection, Iterable, Iterator, Sequence
+from collections.abc import Callable, Iterable, Iterator, Sequence
 from typing import Any
 
 from django.db import IntegrityError
 from django.db.models.base import Model
 from django.db.models.fields import Field
 from django.db.models.options import Options
 from django.db.models.query import QuerySet
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/enums.pyi` & `django-stubs-4.2.2/django-stubs/db/models/enums.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     def __contains__(self, member: Any) -> bool: ...
 
 class Choices(enum.Enum, metaclass=ChoicesMeta):
     @property
     def label(self) -> str: ...
     @enum_property
     def value(self) -> Any: ...
+    @property
+    def do_not_call_in_templates(self) -> bool: ...
 
 # fake
 class _IntegerChoicesMeta(ChoicesMeta):
     names: list[str]
     choices: list[tuple[int, str]]
     labels: list[str]
     values: list[int]
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/expressions.pyi` & `django-stubs-4.2.2/django-stubs/db/models/expressions.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import datetime
-from collections.abc import Callable, Iterable, Iterator, Sequence
+from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 from decimal import Decimal
-from typing import Any, TypeVar
+from typing import Any, Generic, Literal, TypeVar
 
 from _typeshed import Self
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Q
 from django.db.models.fields import Field
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.query import QuerySet
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
 from django.db.models.sql.query import Query
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import TypeAlias
 
 class SQLiteNumericMixin:
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 _Numeric: TypeAlias = float | Decimal
 
 class Combinable:
@@ -37,25 +37,28 @@
     def __truediv__(self, other: Combinable | _Numeric) -> CombinedExpression: ...
     def __mod__(self, other: int | Combinable) -> CombinedExpression: ...
     def __pow__(self, other: _Numeric | Combinable) -> CombinedExpression: ...
     def __and__(self, other: Combinable | Q) -> Q: ...
     def bitand(self, other: int) -> CombinedExpression: ...
     def bitleftshift(self, other: int) -> CombinedExpression: ...
     def bitrightshift(self, other: int) -> CombinedExpression: ...
+    def __xor__(self, other: Combinable | Q) -> Q: ...
     def bitxor(self, other: int) -> CombinedExpression: ...
     def __or__(self, other: Combinable | Q) -> Q: ...
     def bitor(self, other: int) -> CombinedExpression: ...
     def __radd__(self, other: datetime.datetime | _Numeric | Combinable | None) -> CombinedExpression: ...
     def __rsub__(self, other: _Numeric | Combinable) -> CombinedExpression: ...
     def __rmul__(self, other: _Numeric | Combinable) -> CombinedExpression: ...
     def __rtruediv__(self, other: _Numeric | Combinable) -> CombinedExpression: ...
     def __rmod__(self, other: int | Combinable) -> CombinedExpression: ...
     def __rpow__(self, other: _Numeric | Combinable) -> CombinedExpression: ...
     def __rand__(self, other: Any) -> Combinable: ...
     def __ror__(self, other: Any) -> Combinable: ...
+    def __rxor__(self, other: Any) -> Combinable: ...
+    def __invert__(self) -> NegatedExpression[Combinable]: ...
 
 class BaseExpression:
     is_summary: bool
     filterable: bool
     window_compatible: bool
     def __init__(self, output_field: Field | None = ...) -> None: ...
     def get_db_converters(self, connection: BaseDatabaseWrapper) -> list[Callable]: ...
@@ -83,28 +86,28 @@
     def output_field(self) -> Field: ...
     @property
     def convert_value(self) -> Callable: ...
     def get_lookup(self, lookup: str) -> type[Lookup] | None: ...
     def get_transform(self, name: str) -> type[Transform] | None: ...
     def relabeled_clone(self: Self, change_map: dict[str | None, str]) -> Self: ...
     def copy(self: Self) -> Self: ...
-    def get_group_by_cols(self: Self, alias: str | None = ...) -> list[Self]: ...
+    def get_group_by_cols(self: Self) -> list[Self]: ...
     def get_source_fields(self) -> list[Field | None]: ...
     def asc(
         self,
         *,
         descending: bool = ...,
-        nulls_first: bool = ...,
-        nulls_last: bool = ...,
+        nulls_first: bool | None = ...,
+        nulls_last: bool | None = ...,
     ) -> OrderBy: ...
     def desc(
         self,
         *,
-        nulls_first: bool = ...,
-        nulls_last: bool = ...,
+        nulls_first: bool | None = ...,
+        nulls_last: bool | None = ...,
     ) -> OrderBy: ...
     def reverse_ordering(self) -> BaseExpression: ...
     def flatten(self) -> Iterator[BaseExpression]: ...
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def deconstruct(self) -> Any: ...  # fake
 
 class Expression(BaseExpression, Combinable): ...
@@ -128,28 +131,29 @@
         self,
         query: Any = ...,
         allow_joins: bool = ...,
         reuse: set[str] | None = ...,
         summarize: bool = ...,
         for_save: bool = ...,
     ) -> F: ...
+    def replace_expressions(self, replacements: Mapping[F, Any]) -> F: ...
     def asc(
         self,
         *,
         descending: bool = ...,
-        nulls_first: bool = ...,
-        nulls_last: bool = ...,
+        nulls_first: bool | None = ...,
+        nulls_last: bool | None = ...,
     ) -> OrderBy: ...
     def desc(
         self,
         *,
-        nulls_first: bool = ...,
-        nulls_last: bool = ...,
+        nulls_first: bool | None = ...,
+        nulls_last: bool | None = ...,
     ) -> OrderBy: ...
-    def deconstruct(self) -> Any: ...  # fake
+    def copy(self) -> F: ...
 
 class ResolvedOuterRef(F): ...
 
 class OuterRef(F):
     def __init__(self, name: str | OuterRef) -> None: ...
     contains_aggregate: bool
     def relabeled_clone(self: Self, relabels: Any) -> Self: ...
@@ -195,16 +199,23 @@
     def __init__(self, refs: str, source: Expression) -> None: ...
 
 class ExpressionList(Func):
     def __init__(self, *expressions: BaseExpression | Combinable, **extra: Any) -> None: ...
 
 class OrderByList(Func): ...
 
-class ExpressionWrapper(Expression):
-    def __init__(self, expression: Q | Combinable, output_field: Field) -> None: ...
+_E = TypeVar("_E", bound=Q | Combinable)
+
+class ExpressionWrapper(Expression, Generic[_E]):
+    def __init__(self, expression: _E, output_field: Field) -> None: ...
+    expression: _E
+
+class NegatedExpression(ExpressionWrapper[_E]):
+    def __init__(self, expression: _E) -> None: ...
+    def __invert__(self) -> _E: ...  # type: ignore[override]
 
 class When(Expression):
     template: str
     condition: Any
     result: Any
     def __init__(self, condition: Any = ..., then: Any = ..., **lookups: Any) -> None: ...
 
@@ -221,43 +232,43 @@
 class Subquery(BaseExpression, Combinable):
     template: str
     query: Query
     extra: dict[Any, Any]
     def __init__(self, queryset: Query | QuerySet, output_field: Field | None = ..., **extra: Any) -> None: ...
 
 class Exists(Subquery):
-    negated: bool
-    def __init__(self, queryset: Query | QuerySet, negated: bool = ..., **kwargs: Any) -> None: ...
-    def __invert__(self) -> Exists: ...
+    def __init__(self, queryset: Query | QuerySet, **kwargs: Any) -> None: ...
 
 class OrderBy(Expression):
     template: str
     nulls_first: bool
     nulls_last: bool
     descending: bool
     expression: Expression | F | Subquery
     def __init__(
         self,
         expression: Expression | F | Subquery,
         descending: bool = ...,
-        nulls_first: bool = ...,
-        nulls_last: bool = ...,
+        nulls_first: bool | None = ...,
+        nulls_last: bool | None = ...,
     ) -> None: ...
+    def asc(self) -> None: ...  # type: ignore[override]
+    def desc(self) -> None: ...  # type: ignore[override]
 
 class Window(SQLiteNumericMixin, Expression):
     template: str
     contains_aggregate: bool
     contains_over_clause: bool
     partition_by: ExpressionList | None
     order_by: ExpressionList | None
     def __init__(
         self,
         expression: BaseExpression,
         partition_by: str | Iterable[BaseExpression | F] | F | BaseExpression | None = ...,
-        order_by: Sequence[BaseExpression | F] | BaseExpression | F | None = ...,
+        order_by: Sequence[BaseExpression | F | str] | BaseExpression | F | str | None = ...,
         frame: WindowFrame | None = ...,
         output_field: Field | None = ...,
     ) -> None: ...
 
 class WindowFrame(Expression):
     template: str
     frame_type: str
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/fields/__init__.pyi` & `django-stubs-4.2.2/django-stubs/db/models/fields/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import decimal
 import uuid
 from collections.abc import Callable, Iterable, Sequence
-from datetime import date
+from datetime import date, time, timedelta
 from datetime import datetime as real_datetime
-from datetime import time, timedelta
 from typing import Any, Generic, Protocol, TypeVar, overload
 
 from django.core import validators  # due to weird mypy.stubtest error
 from django.core.checks import CheckMessage
 from django.core.exceptions import FieldDoesNotExist as FieldDoesNotExist
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Model
 from django.db.models.expressions import Col, Combinable
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from django.db.models.query_utils import Q, RegisterLookupMixin
-from django.forms import Field as FormField
 from django.forms import Widget
 from django.utils.datastructures import DictWrapper
 from django.utils.functional import _Getter, _StrOrPromise
 from typing_extensions import Self, TypeAlias
 
 class Empty: ...
 class NOT_PROVIDED: ...
@@ -146,15 +144,15 @@
     concrete: bool
     default: Any
     error_messages: _ErrorMessagesT
     empty_values: Sequence[Any]
     creation_counter: int
     auto_creation_counter: int
     default_validators: Sequence[validators._ValidatorCallable]
-    default_error_messages: dict[str, str]
+    default_error_messages: _ErrorMessagesT
     hidden: bool
     system_check_removed_details: Any | None
     system_check_deprecated_details: Any | None
     non_db_attrs: tuple[str, ...]
     def __init__(
         self,
         verbose_name: _StrOrPromise | None = ...,
@@ -236,19 +234,19 @@
     _pyi_private_set_type: float | int | str | Combinable
     _pyi_private_get_type: int
     _pyi_lookup_exact_type: str | int
 
 class PositiveIntegerRelDbTypeMixin:
     def rel_db_type(self, connection: BaseDatabaseWrapper) -> str: ...
 
+class SmallIntegerField(IntegerField[_ST, _GT]): ...
+class BigIntegerField(IntegerField[_ST, _GT]): ...
 class PositiveIntegerField(PositiveIntegerRelDbTypeMixin, IntegerField[_ST, _GT]): ...
 class PositiveSmallIntegerField(PositiveIntegerRelDbTypeMixin, SmallIntegerField[_ST, _GT]): ...
 class PositiveBigIntegerField(PositiveIntegerRelDbTypeMixin, BigIntegerField[_ST, _GT]): ...
-class SmallIntegerField(IntegerField[_ST, _GT]): ...
-class BigIntegerField(IntegerField[_ST, _GT]): ...
 
 class FloatField(Field[_ST, _GT]):
     _pyi_private_set_type: float | int | str | Combinable
     _pyi_private_get_type: float
     _pyi_lookup_exact_type: float
 
 class DecimalField(Field[_ST, _GT]):
@@ -425,15 +423,15 @@
     _pyi_private_set_type: str | Combinable
     _pyi_private_get_type: str
 
 class GenericIPAddressField(Field[_ST, _GT]):
     _pyi_private_set_type: str | int | Callable[..., Any] | Combinable
     _pyi_private_get_type: str
 
-    default_error_messages: dict[str, str]
+    default_error_messages: _ErrorMessagesT
     unpack_ipv4: bool
     protocol: str
     def __init__(
         self,
         verbose_name: _StrOrPromise | None = ...,
         name: Any | None = ...,
         protocol: str = ...,
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/fields/files.pyi` & `django-stubs-4.2.2/django-stubs/db/models/fields/files.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/fields/json.pyi` & `django-stubs-4.2.2/django-stubs/db/models/fields/json.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
+from collections.abc import Callable
 from typing import Any
 
+from _typeshed import Self
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import lookups
 from django.db.models.lookups import PostgresOperatorLookup, Transform
 from django.db.models.sql.compiler import SQLCompiler
 from django.utils.functional import _StrOrPromise
 
 from . import Field
@@ -15,51 +17,58 @@
     decoder: type[json.JSONDecoder] | None
     def __init__(
         self,
         verbose_name: _StrOrPromise | None = ...,
         name: str | None = ...,
         encoder: type[json.JSONEncoder] | None = ...,
         decoder: type[json.JSONDecoder] | None = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None: ...
 
 class DataContains(PostgresOperatorLookup): ...
 class ContainedBy(PostgresOperatorLookup): ...
 
 class HasKeyLookup(PostgresOperatorLookup):
     logical_operator: str | None
+    def compile_json_path_final_key(self, key_transform: Any) -> str: ...
 
 class HasKey(HasKeyLookup):
     postgres_operator: str
 
 class HasKeys(HasKeyLookup):
     postgres_operator: str
     logical_operator: str
 
 class HasAnyKeys(HasKeys):
     postgres_operator: str
     logical_operator: str
 
+class HasKeyOrArrayIndex(HasKey): ...
 class JSONExact(lookups.Exact): ...
+class CaseInsensitiveMixin: ...
+class JSONIContains(CaseInsensitiveMixin, lookups.IContains): ...
 
 class KeyTransform(Transform):
     key_name: str
     postgres_operator: str
     postgres_nested_operator: str
     def __init__(self, key_name: Any, *args: Any, **kwargs: Any) -> None: ...
     def preprocess_lhs(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> Any: ...
 
 class KeyTextTransform(KeyTransform):
     postgres_operator: str
     postgres_nested_operator: str
+    @classmethod
+    def from_lookup(cls: type[Self], lookup: str) -> Self: ...
+
+KT: Callable[[str], KeyTextTransform]
 
 class KeyTransformTextLookupMixin:
     def __init__(self, key_transform: Any, *args: Any, **kwargs: Any) -> None: ...
 
-class CaseInsensitiveMixin: ...
 class KeyTransformIsNull(lookups.IsNull): ...
 class KeyTransformIn(lookups.In): ...
 class KeyTransformExact(JSONExact): ...
 class KeyTransformIExact(CaseInsensitiveMixin, KeyTransformTextLookupMixin, lookups.IExact): ...
 class KeyTransformIContains(CaseInsensitiveMixin, KeyTransformTextLookupMixin, lookups.IContains): ...
 class KeyTransformStartsWith(KeyTransformTextLookupMixin, lookups.StartsWith): ...
 class KeyTransformIStartsWith(CaseInsensitiveMixin, KeyTransformTextLookupMixin, lookups.IStartsWith): ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/fields/mixins.pyi` & `django-stubs-4.2.2/django-stubs/db/models/fields/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/fields/related.pyi` & `django-stubs-4.2.2/django-stubs/db/models/fields/related.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Callable, Iterable, Sequence
-from typing import Any, TypeVar, overload
+from typing import Any, Literal, TypeVar, overload
 from uuid import UUID
 
 from django.core import validators  # due to weird mypy.stubtest error
 from django.db.models.base import Model
 from django.db.models.expressions import Combinable
 from django.db.models.fields import Field, _AllLimitChoicesTo, _ErrorMessagesT, _FieldChoices, _LimitChoicesTo
 from django.db.models.fields.mixins import FieldCacheMixin
@@ -17,15 +17,15 @@
 from django.db.models.fields.reverse_related import ForeignObjectRel as ForeignObjectRel  # noqa: F401
 from django.db.models.fields.reverse_related import ManyToManyRel as ManyToManyRel
 from django.db.models.fields.reverse_related import ManyToOneRel as ManyToOneRel
 from django.db.models.fields.reverse_related import OneToOneRel as OneToOneRel
 from django.db.models.manager import RelatedManager
 from django.db.models.query_utils import FilteredRelation, PathInfo, Q
 from django.utils.functional import _StrOrPromise
-from typing_extensions import Literal, Self
+from typing_extensions import Self
 
 RECURSIVE_RELATIONSHIP_CONSTANT: Literal["self"]
 
 def resolve_relation(scope_model: type[Model], relation: str | type[Model]) -> str | type[Model]: ...
 
 # __set__ value type
 _ST = TypeVar("_ST")
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/fields/related_descriptors.pyi` & `django-stubs-4.2.2/django-stubs/db/models/fields/related_descriptors.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from collections.abc import Callable
 from typing import Any, Generic, TypeVar
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models.base import Model
 from django.db.models.fields import Field
-from django.db.models.fields.mixins import FieldCacheMixin
-from django.db.models.fields.related import ForeignKey, ManyToManyField, OneToOneField, RelatedField
+from django.db.models.fields.related import ForeignKey, RelatedField
 from django.db.models.fields.reverse_related import ManyToManyRel, ManyToOneRel, OneToOneRel
 from django.db.models.manager import RelatedManager
 from django.db.models.query import QuerySet
 from django.db.models.query_utils import DeferredAttribute
 
 _T = TypeVar("_T")
 _F = TypeVar("_F", bound=Field)
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/fields/related_lookups.pyi` & `django-stubs-4.2.2/django-stubs/db/models/fields/related_lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/fields/reverse_related.pyi` & `django-stubs-4.2.2/django-stubs/db/models/fields/reverse_related.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from collections.abc import Callable, Sequence
-from typing import Any
+from typing import Any, Literal
 
 from django.db.models.base import Model
 from django.db.models.fields import AutoField, Field, _AllLimitChoicesTo, _ChoicesList, _LimitChoicesTo
 from django.db.models.fields.related import ForeignKey, ForeignObject, ManyToManyField, OneToOneField
 from django.db.models.lookups import Lookup, StartsWith
 from django.db.models.query_utils import FilteredRelation, PathInfo
 from django.db.models.sql.where import WhereNode
-from typing_extensions import Literal
 
 from .mixins import FieldCacheMixin
 
 # Common note: `model` and `through` can be of type `str` when passed to `__init__`.
 # When parent's `contribute_to_class` is called (during startup),
 # strings are resolved to real model classes.
 # Thus `str` is acceptable in __init__, but instance attribute `model` is always
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/functions/__init__.pyi` & `django-stubs-4.2.2/django-stubs/db/models/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/functions/comparison.pyi` & `django-stubs-4.2.2/django-stubs/db/models/functions/comparison.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/functions/datetime.pyi` & `django-stubs-4.2.2/django-stubs/db/models/functions/datetime.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/functions/math.pyi` & `django-stubs-4.2.2/django-stubs/db/models/functions/math.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/functions/text.pyi` & `django-stubs-4.2.2/django-stubs/db/models/functions/text.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/functions/window.pyi` & `django-stubs-4.2.2/django-stubs/db/models/functions/window.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/indexes.pyi` & `django-stubs-4.2.2/django-stubs/db/utils.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,54 @@
-from collections.abc import Sequence
+from collections.abc import Iterable
+from types import TracebackType
 from typing import Any
 
+from django.apps import AppConfig
 from django.db.backends.base.base import BaseDatabaseWrapper
-from django.db.backends.base.schema import BaseDatabaseSchemaEditor
-from django.db.backends.ddl_references import Statement
-from django.db.models.base import Model
-from django.db.models.expressions import BaseExpression, Combinable, Expression, Func
-from django.db.models.query_utils import Q
-from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
-
-class Index:
-    model: type[Model]
-    suffix: str
-    max_name_length: int
-    fields: Sequence[str]
-    fields_orders: Sequence[tuple[str, str]]
-    name: str
-    db_tablespace: str | None
-    opclasses: Sequence[str]
-    condition: Q | None
-    expressions: Sequence[BaseExpression | Combinable]
-    include: Sequence[str]
-    def __init__(
+from django.db.models import Model
+from django.utils.connection import BaseConnectionHandler
+
+DEFAULT_DB_ALIAS: str
+DJANGO_VERSION_PICKLE_KEY: str
+
+class Error(Exception): ...
+class InterfaceError(Error): ...
+class DatabaseError(Error): ...
+class DataError(DatabaseError): ...
+class OperationalError(DatabaseError): ...
+class IntegrityError(DatabaseError): ...
+class InternalError(DatabaseError): ...
+class ProgrammingError(DatabaseError): ...
+class NotSupportedError(DatabaseError): ...
+
+class DatabaseErrorWrapper:
+    def __init__(self, wrapper: Any) -> None: ...
+    def __enter__(self) -> None: ...
+    def __exit__(
         self,
-        *expressions: BaseExpression | Combinable | str,
-        fields: Sequence[str] = ...,
-        name: str | None = ...,
-        db_tablespace: str | None = ...,
-        opclasses: Sequence[str] = ...,
-        condition: Q | None = ...,
-        include: Sequence[str] | None = ...,
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None: ...
+
+def load_backend(backend_name: str) -> Any: ...
+
+class ConnectionHandler(BaseConnectionHandler[BaseDatabaseWrapper]):
     @property
-    def contains_expressions(self) -> bool: ...
-    def create_sql(
-        self, model: type[Model], schema_editor: BaseDatabaseSchemaEditor, using: str = ..., **kwargs: Any
-    ) -> Statement: ...
-    def remove_sql(self, model: type[Model], schema_editor: BaseDatabaseSchemaEditor, **kwargs: Any) -> str: ...
-    def deconstruct(self) -> Any: ...
-    def clone(self) -> Index: ...
-    def set_name_with_model(self, model: type[Model]) -> None: ...
-
-class IndexExpression(Func):
-    template: str
-    wrapper_classes: Sequence[Expression]
-    def set_wrapper_classes(self, connection: Any | None = ...) -> None: ...
-    @classmethod
-    def register_wrappers(cls, *wrapper_classes: Expression) -> None: ...
-    def resolve_expression(
-        self,
-        query: Any | None = ...,
-        allow_joins: bool = ...,
-        reuse: set[str] | None = ...,
-        summarize: bool = ...,
-        for_save: bool = ...,
-    ) -> IndexExpression: ...
-    def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
+    def databases(self) -> dict[str, dict[str, Any]]: ...
+    def ensure_defaults(self, alias: str) -> None: ...
+    def prepare_test_settings(self, alias: str) -> None: ...
+    def create_connection(self, alias: str) -> BaseDatabaseWrapper: ...
+    def close_all(self) -> None: ...
+
+class ConnectionRouter:
+    def __init__(self, routers: Iterable[Any] | None = ...) -> None: ...
+    @property
+    def routers(self) -> list[Any]: ...
+    def db_for_read(self, model: type[Model], **hints: Any) -> str: ...
+    def db_for_write(self, model: type[Model], **hints: Any) -> str: ...
+    def allow_relation(self, obj1: Model, obj2: Model, **hints: Any) -> bool: ...
+    def allow_migrate(self, db: str, app_label: str, **hints: Any) -> bool: ...
+    def allow_migrate_model(self, db: str, model: type[Model]) -> bool: ...
+    def get_migratable_models(
+        self, app_config: AppConfig, db: str, include_auto_created: bool = ...
+    ) -> list[type[Model]]: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/lookups.pyi` & `django-stubs-4.2.2/django-stubs/db/models/lookups.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from collections.abc import Iterable, Mapping
-from typing import Any, Generic, TypeVar
+from typing import Any, Generic, Literal, TypeVar
 
 from _typeshed import Self
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.expressions import Expression, Func
 from django.db.models.query_utils import RegisterLookupMixin
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType, _ParamT
 from django.utils.datastructures import OrderedSet
-from typing_extensions import Literal
 
 _T = TypeVar("_T")
 
 class Lookup(Generic[_T]):
     lookup_name: str
     prepare_rhs: bool
     can_use_none_as_rhs: bool
@@ -29,15 +28,15 @@
     def get_db_prep_lookup(self, value: _ParamT, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def process_lhs(
         self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, lhs: Expression | None = ...
     ) -> _AsSqlType: ...
     def process_rhs(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def rhs_is_direct_value(self) -> bool: ...
     def relabeled_clone(self: Self, relabels: Mapping[str, str]) -> Self: ...
-    def get_group_by_cols(self, alias: str | None = ...) -> list[Expression]: ...
+    def get_group_by_cols(self) -> list[Expression]: ...
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     @property
     def contains_aggregate(self) -> bool: ...
     @property
     def contains_over_clause(self) -> bool: ...
     @property
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/manager.pyi` & `django-stubs-4.2.2/django-stubs/db/models/manager.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/options.pyi` & `django-stubs-4.2.2/django-stubs/db/models/options.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from collections.abc import Iterable, Sequence
-from typing import Any, Generic, TypeVar, Union, overload  # noqa: Y037   # https://github.com/python/mypy/issues/12211
+from typing import (  # noqa: Y037   # https://github.com/python/mypy/issues/12211
+    Any,
+    Generic,
+    Literal,
+    TypeVar,
+    Union,
+    overload,
+)
 
 from django.apps.config import AppConfig
 from django.apps.registry import Apps
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.base import Model
 from django.db.models.constraints import BaseConstraint, UniqueConstraint
 from django.db.models.fields import AutoField, Field
 from django.db.models.fields.related import ManyToManyField, OneToOneField
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from django.db.models.manager import Manager
 from django.db.models.query_utils import PathInfo
 from django.utils.datastructures import ImmutableList, _ListOrTuple
 from django.utils.functional import _StrOrPromise
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import TypeAlias
 
 PROXY_PARENTS: object
 EMPTY_RELATION_TREE: Any
 IMMUTABLE_WARNING: str
 DEFAULT_NAMES: tuple[str, ...]
 
 # https://github.com/python/mypy/issues/12211
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/query.pyi` & `django-stubs-4.2.2/django-stubs/db/models/query.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 class FlatValuesListIterable(BaseIterable[_Row]):
     def __iter__(self) -> Iterator[_Row]: ...
 
 class _QuerySet(Generic[_T, _Row], Collection[_Row], Reversible[_Row], Sized):
     model: type[_T]
     query: Query
     _iterable_class: type[BaseIterable]
+    _result_cache: list[_Row] | None
     def __init__(
         self,
         model: type[Model] | None = ...,
         query: Query | None = ...,
         using: str | None = ...,
         hints: dict[str, Model] | None = ...,
     ) -> None: ...
@@ -167,14 +168,15 @@
     def defer(self: Self, *fields: Any) -> Self: ...
     def only(self: Self, *fields: Any) -> Self: ...
     def using(self: Self, alias: str | None) -> Self: ...
     @property
     def ordered(self) -> bool: ...
     @property
     def db(self) -> str: ...
+    def _fetch_all(self) -> None: ...
     def resolve_expression(self, *args: Any, **kwargs: Any) -> Any: ...
     def __iter__(self) -> Iterator[_Row]: ...
     def __aiter__(self) -> AsyncIterator[_Row]: ...
     def __contains__(self, x: object) -> bool: ...
     @overload
     def __getitem__(self, i: int) -> _Row: ...
     @overload
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/query_utils.pyi` & `django-stubs-4.2.2/django-stubs/db/models/query_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from collections import namedtuple
 from collections.abc import Collection, Iterable, Iterator, Mapping, Sequence
-from typing import Any, TypeVar
+from typing import Any, Literal, TypeVar
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.base import Model
 from django.db.models.expressions import BaseExpression
 from django.db.models.fields import Field
 from django.db.models.fields.mixins import FieldCacheMixin
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
 from django.db.models.sql.query import Query
 from django.db.models.sql.where import WhereNode
 from django.utils import tree
-from typing_extensions import Literal
 
 PathInfo = namedtuple(
     "PathInfo", ["from_opts", "to_opts", "target_fields", "join_field", "m2m", "direct", "filtered_relation"]
 )
 
 class InvalidQuery(Exception): ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/signals.pyi` & `django-stubs-4.2.2/django-stubs/db/models/signals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from collections.abc import Callable
-from typing import Any
 
 from django.apps.registry import Apps
 from django.db.models.base import Model
 from django.dispatch import Signal
 
 class_prepared: Signal
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/sql/compiler.pyi` & `django-stubs-4.2.2/django-stubs/db/models/sql/compiler.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections.abc import Callable, Iterable, Iterator, Sequence
 from datetime import date, datetime
 from decimal import Decimal
-from typing import Any, overload
+from typing import Any, Literal, overload
 from uuid import UUID
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.utils import CursorWrapper
 from django.db.models.base import Model
 from django.db.models.expressions import BaseExpression, Expression
 from django.db.models.sql.query import Query
 from django.db.models.sql.subqueries import AggregateQuery, DeleteQuery, InsertQuery, UpdateQuery
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import TypeAlias
 
 _ParamT: TypeAlias = str | int
 
 _ParamsT: TypeAlias = list[_ParamT]
 _AsSqlType: TypeAlias = tuple[str, _ParamsT]
 
 class SQLCompiler:
@@ -44,14 +44,15 @@
     ) -> list[_AsSqlType]: ...
     def collapse_group_by(
         self, expressions: list[Expression], having: list[Expression] | tuple
     ) -> list[Expression]: ...
     def get_select(
         self,
     ) -> tuple[list[tuple[Expression, _AsSqlType, str | None]], dict[str, Any] | None, dict[str, int]]: ...
+    def _order_by_pairs(self) -> None: ...
     def get_order_by(self) -> list[tuple[Expression, tuple[str, _ParamsT, bool]]]: ...
     def get_extra_select(
         self,
         order_by: list[tuple[Expression, tuple[str, _ParamsT, bool]]],
         select: list[tuple[Expression, _AsSqlType, str | None]],
     ) -> list[tuple[Expression, _AsSqlType, None]]: ...
     def quote_name_unless_alias(self, name: str) -> str: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/sql/datastructures.pyi` & `django-stubs-4.2.2/django-stubs/db/models/sql/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/models/sql/query.pyi` & `django-stubs-4.2.2/django-stubs/db/models/sql/query.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import collections
 from collections import namedtuple
 from collections.abc import Callable, Iterable, Iterator, Sequence
-from typing import Any
+from typing import Any, Literal
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.utils import CursorWrapper
-from django.db.models import Field, FilteredRelation, Model, Q, QuerySet
+from django.db.models import Field, FilteredRelation, Model, Q
 from django.db.models.expressions import BaseExpression, Combinable, Expression, OrderBy
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.options import Options
-from django.db.models.query_utils import PathInfo, RegisterLookupMixin
+from django.db.models.query_utils import PathInfo
 from django.db.models.sql.compiler import SQLCompiler
 from django.db.models.sql.datastructures import BaseTable, Join
 from django.db.models.sql.where import WhereNode
-from typing_extensions import Literal
 
 JoinInfo = namedtuple("JoinInfo", ("final_field", "targets", "opts", "joins", "path", "transform_function"))
 
 class RawQuery:
     high_mark: int | None
     low_mark: int | None
     params: Any
@@ -28,15 +27,15 @@
     cursor: CursorWrapper | None
     def __init__(self, sql: str, using: str, params: Any = ...) -> None: ...
     def chain(self, using: str) -> RawQuery: ...
     def clone(self, using: str) -> RawQuery: ...
     def get_columns(self) -> list[str]: ...
     def __iter__(self) -> Iterator[Any]: ...
     @property
-    def params_type(self) -> None | type[dict] | type[tuple]: ...
+    def params_type(self) -> type[dict | tuple] | None: ...
 
 class Query(BaseExpression):
     related_ids: list[int] | None
     related_updates: dict[type[Model], list[tuple[Field, None, int | str]]]
     values: list[Any]
     alias_prefix: str
     subq_aliases: frozenset[Any]
```

### Comparing `django-stubs-4.2.1/django-stubs/db/models/sql/subqueries.pyi` & `django-stubs-4.2.2/django-stubs/db/models/sql/subqueries.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from collections.abc import Iterable
 from typing import Any
 
 from django.db.models.base import Model
 from django.db.models.expressions import Case
 from django.db.models.fields import Field
-from django.db.models.query import QuerySet
 from django.db.models.sql.query import Query
 from django.db.models.sql.where import WhereNode
 
 class DeleteQuery(Query):
     select: tuple
     where_class: type[WhereNode]
     where: WhereNode
```

### Comparing `django-stubs-4.2.1/django-stubs/db/transaction.pyi` & `django-stubs-4.2.2/django-stubs/db/transaction.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/db/utils.pyi` & `django-stubs-4.2.2/django-stubs/utils/autoreload.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,76 @@
-from collections.abc import Iterable
-from types import TracebackType
+import threading
+import types
+from collections.abc import Callable, Iterable, Iterator
+from logging import Logger
+from pathlib import Path
 from typing import Any
 
-from django.apps import AppConfig
-from django.db.backends.base.base import BaseDatabaseWrapper
-from django.db.models import Model
-from django.utils.connection import BaseConnectionHandler
-
-DEFAULT_DB_ALIAS: str
-DJANGO_VERSION_PICKLE_KEY: str
-
-class Error(Exception): ...
-class InterfaceError(Error): ...
-class DatabaseError(Error): ...
-class DataError(DatabaseError): ...
-class OperationalError(DatabaseError): ...
-class IntegrityError(DatabaseError): ...
-class InternalError(DatabaseError): ...
-class ProgrammingError(DatabaseError): ...
-class NotSupportedError(DatabaseError): ...
-
-class DatabaseErrorWrapper:
-    def __init__(self, wrapper: Any) -> None: ...
-    def __enter__(self) -> None: ...
-    def __exit__(
-        self,
-        exc_type: type[BaseException] | None,
-        exc_value: BaseException | None,
-        exc_tb: TracebackType | None,
-    ) -> None: ...
-
-def load_backend(backend_name: str) -> Any: ...
-
-class ConnectionHandler(BaseConnectionHandler[BaseDatabaseWrapper]):
+from django.apps.registry import Apps
+from django.dispatch import Signal
+from django.utils._os import _PathCompatible
+from typing_extensions import ParamSpec
+
+_P = ParamSpec("_P")
+
+logger: Logger
+autoreload_started: Signal
+file_changed: Signal
+DJANGO_AUTORELOAD_ENV: str
+
+def is_django_module(module: types.ModuleType) -> bool: ...
+def is_django_path(path: _PathCompatible) -> bool: ...
+def check_errors(fn: Callable[_P, Any]) -> Callable[_P, None]: ...
+def raise_last_exception() -> None: ...
+def ensure_echo_on() -> None: ...
+def iter_all_python_module_files() -> set[Path]: ...
+def iter_modules_and_files(
+    modules: Iterable[types.ModuleType], extra_files: Iterable[_PathCompatible]
+) -> frozenset[Path]: ...
+def common_roots(paths: Iterable[Path]) -> Iterable[Path]: ...
+def sys_path_directories() -> Iterator[Path]: ...
+def get_child_arguments() -> list[str]: ...
+def trigger_reload(filename: str) -> None: ...
+def restart_with_reloader() -> int: ...
+
+class BaseReloader:
+    extra_files: set[Path]
+    directory_globs: dict[Path, set[str]]
+    def __init__(self) -> None: ...
+    def watch_dir(self, path: _PathCompatible, glob: str) -> None: ...
+    def watched_files(self, include_globs: bool = ...) -> Iterator[Path]: ...
+    def wait_for_apps_ready(self, app_reg: Apps, django_main_thread: threading.Thread) -> bool: ...
+    def run(self, django_main_thread: threading.Thread) -> None: ...
+    def run_loop(self) -> None: ...
+    def tick(self) -> Iterator[None]: ...
+    @classmethod
+    def check_availability(cls) -> bool | None: ...
+    def notify_file_changed(self, path: _PathCompatible) -> None: ...
     @property
-    def databases(self) -> dict[str, dict[str, Any]]: ...
-    def ensure_defaults(self, alias: str) -> None: ...
-    def prepare_test_settings(self, alias: str) -> None: ...
-    def create_connection(self, alias: str) -> BaseDatabaseWrapper: ...
-    def close_all(self) -> None: ...
+    def should_stop(self) -> bool: ...
+    def stop(self) -> None: ...
 
-class ConnectionRouter:
-    def __init__(self, routers: Iterable[Any] | None = ...) -> None: ...
+class StatReloader(BaseReloader):
+    SLEEP_TIME: int
+    def snapshot_files(self) -> Iterator[tuple[Path, float]]: ...
+    @classmethod
+    def check_availability(cls) -> bool: ...
+
+class WatchmanUnavailable(RuntimeError): ...
+
+class WatchmanReloader(BaseReloader):
+    processed_request: threading.Event
+    client_timeout: int
+    def __init__(self) -> None: ...
     @property
-    def routers(self) -> list[Any]: ...
-    def db_for_read(self, model: type[Model], **hints: Any) -> str: ...
-    def db_for_write(self, model: type[Model], **hints: Any) -> str: ...
-    def allow_relation(self, obj1: Model, obj2: Model, **hints: Any) -> bool: ...
-    def allow_migrate(self, db: str, app_label: str, **hints: Any) -> bool: ...
-    def allow_migrate_model(self, db: str, model: type[Model]) -> bool: ...
-    def get_migratable_models(
-        self, app_config: AppConfig, db: str, include_auto_created: bool = ...
-    ) -> list[type[Model]]: ...
+    def client(self) -> Any: ...
+    def watched_roots(self, watched_files: Iterable[Path]) -> frozenset[Path]: ...
+    def update_watches(self) -> None: ...
+    def request_processed(self, **kwargs: Any) -> None: ...
+    def check_server_status(self, inner_ex: BaseException | None = ...) -> bool: ...
+    @classmethod
+    def check_availability(cls) -> None: ...
+    def stop(self) -> None: ...
+
+def get_reloader() -> BaseReloader: ...
+def start_django(reloader: BaseReloader, main_func: Callable, *args: Any, **kwargs: Any) -> None: ...
+def run_with_reloader(main_func: Callable, *args: Any, **kwargs: Any) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/dispatch/dispatcher.pyi` & `django-stubs-4.2.2/django-stubs/dispatch/dispatcher.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,37 @@
-from collections.abc import Callable
-from typing import Any
+import threading
+from collections.abc import Callable, Hashable, MutableMapping
+from logging import Logger
+from typing import Any, TypeVar
 
-NONE_ID: Any
+NONE_ID: int
 NO_RECEIVERS: Any
 
+logger: Logger
+
 class Signal:
-    receivers: Any
-    providing_args: Any
-    lock: Any
-    use_caching: Any
-    sender_receivers_cache: Any
-    def __init__(self, providing_args: list[str] = ..., use_caching: bool = ...) -> None: ...
+    receivers: list[Any]
+    lock: threading.Lock
+    use_caching: bool
+    sender_receivers_cache: MutableMapping[Any, Any]
+
+    def __init__(self, use_caching: bool = ...) -> None: ...
     def connect(
-        self, receiver: Callable, sender: object | None = ..., weak: bool = ..., dispatch_uid: str | None = ...
+        self, receiver: Callable, sender: object | None = ..., weak: bool = ..., dispatch_uid: Hashable | None = ...
     ) -> None: ...
     def disconnect(
         self, receiver: Callable | None = ..., sender: object | None = ..., dispatch_uid: str | None = ...
     ) -> bool: ...
     def has_listeners(self, sender: Any = ...) -> bool: ...
     def send(self, sender: Any, **named: Any) -> list[tuple[Callable, str | None]]: ...
-    def send_robust(self, sender: Any, **named: Any) -> list[tuple[Callable, Exception | str]]: ...
+    def send_robust(self, sender: Any, **named: Any) -> list[tuple[Callable, Exception | Any]]: ...
+    def _live_receivers(self, sender: Any) -> list[Callable]: ...
+
+_F = TypeVar("_F", bound=Callable[..., Any])
 
-def receiver(signal: list[Signal] | Signal, **kwargs: Any) -> Callable: ...
+def receiver(
+    signal: list[Signal] | tuple[Signal, ...] | Signal,
+    *,
+    sender: object | None = ...,
+    weak: bool = ...,
+    dispatch_uid: Hashable | None = ...,
+) -> Callable[[_F], _F]: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/forms/__init__.pyi` & `django-stubs-4.2.2/django-stubs/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/forms/boundfield.pyi` & `django-stubs-4.2.2/django-stubs/forms/boundfield.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/forms/fields.pyi` & `django-stubs-4.2.2/django-stubs/forms/fields.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from uuid import UUID
 
 from django.core.files import File
 from django.core.validators import _ValidatorCallable
 from django.db.models.fields import _Choice, _ChoiceNamedGroup, _ChoicesCallable, _ErrorMessagesT, _FieldChoices
 from django.forms.boundfield import BoundField
 from django.forms.forms import BaseForm
-from django.forms.widgets import ChoiceWidget, Widget
+from django.forms.widgets import Widget
 from django.utils.datastructures import _PropertyDescriptor
 from django.utils.functional import _StrOrPromise
 from typing_extensions import TypeAlias
 
 # Problem: attribute `widget` is always of type `Widget` after field instantiation.
 # However, on class level it can be set to `Type[Widget]` too.
 # If we annotate it as `Union[Widget, Type[Widget]]`, every code that uses field
```

### Comparing `django-stubs-4.2.1/django-stubs/forms/forms.pyi` & `django-stubs-4.2.2/django-stubs/forms/forms.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/forms/formsets.pyi` & `django-stubs-4.2.2/django-stubs/forms/formsets.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/forms/models.pyi` & `django-stubs-4.2.2/django-stubs/forms/models.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections.abc import Callable, Collection, Container, Iterator, Mapping, Sequence
 from typing import (  # noqa: Y037  # https://github.com/python/mypy/issues/12211
     Any,
     ClassVar,
     Generic,
+    Literal,
     TypeVar,
     Union,
     overload,
 )
 from uuid import UUID
 
 from django.db import models
@@ -19,15 +20,15 @@
 from django.forms.forms import BaseForm, DeclarativeFieldsMetaclass
 from django.forms.formsets import BaseFormSet
 from django.forms.renderers import BaseRenderer
 from django.forms.utils import ErrorList, _DataT, _FilesT
 from django.forms.widgets import Widget
 from django.utils.datastructures import _IndexableCollection, _ListOrTuple, _PropertyDescriptor
 from django.utils.functional import _StrOrPromise
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import TypeAlias
 
 ALL_FIELDS: Literal["__all__"]
 
 # https://github.com/python/mypy/issues/12211
 _Fields: TypeAlias = Union[_ListOrTuple[str], Literal["__all__"]]
 _Widgets: TypeAlias = dict[str, type[Widget] | Widget]
 
@@ -65,14 +66,15 @@
     exclude: _Fields | None
     widgets: _Widgets | None
     localized_fields: _Fields | None
     labels: _Labels | None
     help_texts: _HelpTexts | None
     error_messages: _ErrorMessages | None
     field_classes: dict[str, type[Field]] | None
+    formfield_callback: _FormFieldCallback | None
     def __init__(self, options: type | None = ...) -> None: ...
 
 class ModelFormMetaclass(DeclarativeFieldsMetaclass): ...
 
 class BaseModelForm(Generic[_M], BaseForm):
     instance: _M
     _meta: ModelFormOptions[_M]
@@ -111,14 +113,15 @@
     field_classes: Mapping[str, type[Field]] | None = ...,
 ) -> type[ModelForm[_M]]: ...
 
 _ModelFormT = TypeVar("_ModelFormT", bound=ModelForm)
 
 class BaseModelFormSet(Generic[_M, _ModelFormT], BaseFormSet[_ModelFormT]):
     model: type[_M]
+    edit_only: bool
     unique_fields: Collection[str]
     queryset: QuerySet[_M] | None
     initial_extra: Sequence[dict[str, Any]] | None
     def __init__(
         self,
         data: _DataT | None = ...,
         files: _FilesT | None = ...,
@@ -167,14 +170,16 @@
     help_texts: _HelpTexts | None = ...,
     error_messages: _ErrorMessages | None = ...,
     min_num: int | None = ...,
     validate_min: bool = ...,
     field_classes: Mapping[str, type[Field]] | None = ...,
     absolute_max: int | None = ...,
     can_delete_extra: bool = ...,
+    renderer: BaseRenderer | None = ...,
+    edit_only: bool = ...,
 ) -> type[BaseModelFormSet[_M, _ModelFormT]]: ...
 
 class BaseInlineFormSet(Generic[_M, _ParentM, _ModelFormT], BaseModelFormSet[_M, _ModelFormT]):
     instance: _ParentM
     save_as_new: bool
     unique_fields: Collection[str]
     fk: ForeignKey  # set by inlineformset_set
@@ -215,14 +220,16 @@
     help_texts: _HelpTexts | None = ...,
     error_messages: _ErrorMessages | None = ...,
     min_num: int | None = ...,
     validate_min: bool = ...,
     field_classes: Mapping[str, type[Field]] | None = ...,
     absolute_max: int | None = ...,
     can_delete_extra: bool = ...,
+    renderer: BaseRenderer | None = ...,
+    edit_only: bool = ...,
 ) -> type[BaseInlineFormSet[_M, _ParentM, _ModelFormT]]: ...
 
 class InlineForeignKeyField(Field):
     disabled: bool
     help_text: _StrOrPromise
     required: bool
     show_hidden_initial: bool
```

### Comparing `django-stubs-4.2.1/django-stubs/forms/renderers.pyi` & `django-stubs-4.2.2/django-stubs/forms/renderers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/forms/utils.pyi` & `django-stubs-4.2.2/django-stubs/forms/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/forms/widgets.pyi` & `django-stubs-4.2.2/django-stubs/forms/widgets.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import datetime
 from collections.abc import Iterable, Iterator, Mapping, Sequence
-from typing import Any, Protocol
+from typing import Any, Literal, Protocol
 
 from django.core.files.base import File
 from django.db.models.fields import _FieldChoices
 from django.forms.renderers import BaseRenderer
 from django.forms.utils import _DataT, _FilesT
 from django.utils.datastructures import _ListOrTuple
 from django.utils.functional import _Getter
 from django.utils.safestring import SafeString
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import TypeAlias
 
 _OptAttrs: TypeAlias = dict[str, Any]
 
 class MediaOrderConflictWarning(RuntimeWarning): ...
 
 class Media:
     def __init__(
```

### Comparing `django-stubs-4.2.1/django-stubs/http/__init__.pyi` & `django-stubs-4.2.2/django-stubs/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/http/multipartparser.pyi` & `django-stubs-4.2.2/django-stubs/http/multipartparser.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from collections.abc import Iterator, Mapping
-from typing import IO, Any
+from typing import IO, Any, Literal
 
 from django.http.request import QueryDict
 from django.utils.datastructures import ImmutableList, MultiValueDict
-from typing_extensions import Literal
 
 class MultiPartParserError(Exception): ...
 class InputStreamExhausted(Exception): ...
 
 RAW: Literal["raw"]
 FILE: Literal["file"]
 FIELD: Literal["field"]
@@ -51,9 +50,7 @@
     def __init__(self, stream: LazyStream, boundary: bytes) -> None: ...
     def __iter__(self) -> BoundaryIter: ...
     def __next__(self) -> bytes: ...
 
 class Parser:
     def __init__(self, stream: LazyStream, boundary: bytes) -> None: ...
     def __iter__(self) -> Iterator[tuple[str, dict[str, tuple[str, dict[str, bytes | str]]], LazyStream]]: ...
-
-def parse_header(line: bytes) -> tuple[str, dict[str, bytes]]: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/http/request.pyi` & `django-stubs-4.2.2/django-stubs/http/request.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from collections.abc import Iterable, Mapping
 from io import BytesIO
 from re import Pattern
-from typing import Any, BinaryIO, NoReturn, TypeVar, overload
+from typing import Any, BinaryIO, Literal, NoReturn, TypeVar, overload
 
 from _typeshed import Self
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.auth.models import AnonymousUser
 from django.contrib.sessions.backends.base import SessionBase
 from django.contrib.sites.models import Site
 from django.core.files import uploadedfile, uploadhandler
 from django.urls import ResolverMatch
 from django.utils.datastructures import CaseInsensitiveMapping, ImmutableList, MultiValueDict
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import TypeAlias
 
 RAISE_ERROR: object
 host_validation_re: Pattern[str]
 
 class UnreadablePostError(OSError): ...
 class RawPostDataException(Exception): ...
```

### Comparing `django-stubs-4.2.1/django-stubs/http/response.pyi` & `django-stubs-4.2.2/django-stubs/http/response.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import datetime
 from collections.abc import AsyncIterable, AsyncIterator, Iterable, Iterator
 from io import BytesIO
 from json import JSONEncoder
-from typing import Any, TypeVar, overload, type_check_only
+from typing import Any, Literal, TypeVar, overload, type_check_only
 
 from django.http.cookie import SimpleCookie
 from django.utils.datastructures import CaseInsensitiveMapping, _PropertyDescriptor
-from typing_extensions import Literal
 
 class BadHeaderError(ValueError): ...
 
 _Z = TypeVar("_Z")
 
 class ResponseHeaders(CaseInsensitiveMapping[str]):
     def __init__(self, data: dict[str, str]) -> None: ...
@@ -150,9 +149,9 @@
 class JsonResponse(HttpResponse):
     def __init__(
         self,
         data: Any,
         encoder: type[JSONEncoder] = ...,
         safe: bool = ...,
         json_dumps_params: dict[str, Any] | None = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/middleware/cache.pyi` & `django-stubs-4.2.2/django-stubs/middleware/cache.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,9 +25,9 @@
     cache_timeout: float
     cache: BaseCache
     def __init__(
         self,
         get_response: Callable = ...,
         cache_timeout: float | None = ...,
         page_timeout: float | None = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/middleware/common.pyi` & `django-stubs-4.2.2/django-stubs/middleware/common.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/middleware/csrf.pyi` & `django-stubs-4.2.2/django-stubs/middleware/csrf.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/middleware/security.pyi` & `django-stubs-4.2.2/django-stubs/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/shortcuts.pyi` & `django-stubs-4.2.2/django-stubs/shortcuts.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from collections.abc import Callable, Mapping, Sequence
-from typing import Any, Protocol, TypeVar, overload
+from typing import Any, Literal, Protocol, TypeVar, overload
 
 from django.db.models import Manager, QuerySet
 from django.db.models.base import Model
 from django.http import HttpRequest
 from django.http.response import HttpResponse, HttpResponsePermanentRedirect, HttpResponseRedirect
-from typing_extensions import Literal
 
 def render(
     request: HttpRequest | None,
     template_name: str | Sequence[str],
     context: Mapping[str, Any] | None = ...,
     content_type: str | None = ...,
     status: int | None = ...,
```

### Comparing `django-stubs-4.2.1/django-stubs/template/__init__.pyi` & `django-stubs-4.2.2/django-stubs/template/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/backends/base.pyi` & `django-stubs-4.2.2/django-stubs/template/backends/base.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from collections.abc import Iterator, Mapping
 from typing import Any, Protocol
 
 from django.http.request import HttpRequest
-from django.template import TemplateDoesNotExist
 from django.template.base import Context
 from django.utils.safestring import SafeString
 
 class BaseEngine:
     name: str
     dirs: list[str]
     app_dirs: bool
```

### Comparing `django-stubs-4.2.1/django-stubs/template/backends/django.pyi` & `django-stubs-4.2.2/django-stubs/template/backends/django.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/backends/jinja2.pyi` & `django-stubs-4.2.2/django-stubs/template/backends/jinja2.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/base.pyi` & `django-stubs-4.2.2/django-stubs/template/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 VARIABLE_ATTRIBUTE_SEPARATOR: str
 BLOCK_TAG_START: str
 BLOCK_TAG_END: str
 VARIABLE_TAG_START: str
 VARIABLE_TAG_END: str
 COMMENT_TAG_START: str
 COMMENT_TAG_END: str
-TRANSLATOR_COMMENT_MARK: str
 SINGLE_BRACE_START: str
 SINGLE_BRACE_END: str
 UNKNOWN_SOURCE: str
 tag_re: Pattern[str]
 logger: Logger
 
 class TokenType(Enum):
```

### Comparing `django-stubs-4.2.1/django-stubs/template/context.pyi` & `django-stubs-4.2.2/django-stubs/template/context.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Callable, Iterable, Iterator
 from contextlib import contextmanager
 from types import TracebackType
-from typing import Any, TypeVar
+from typing import Any
 
 from _typeshed import Self
 from django.http.request import HttpRequest
 from django.template.base import Node, Origin, Template
 from django.template.loader_tags import IncludeNode
 from typing_extensions import TypeAlias
```

### Comparing `django-stubs-4.2.1/django-stubs/template/context_processors.pyi` & `django-stubs-4.2.2/django-stubs/template/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/defaultfilters.pyi` & `django-stubs-4.2.2/django-stubs/template/defaultfilters.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/defaulttags.pyi` & `django-stubs-4.2.2/django-stubs/template/defaulttags.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/engine.pyi` & `django-stubs-4.2.2/django-stubs/template/engine.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/library.pyi` & `django-stubs-4.2.2/django-stubs/template/library.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/loader.pyi` & `django-stubs-4.2.2/django-stubs/template/loader.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/loader_tags.pyi` & `django-stubs-4.2.2/django-stubs/template/loader_tags.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     isolated_context: bool
     def __init__(
         self,
         template: FilterExpression,
         *args: Any,
         extra_context: Any | None = ...,
         isolated_context: bool = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None: ...
     def render(self, context: Context) -> SafeString: ...
 
 def do_block(parser: Parser, token: Token) -> BlockNode: ...
 def construct_relative_path(current_template_name: str | None, relative_name: str) -> str: ...
 def do_extends(parser: Parser, token: Token) -> ExtendsNode: ...
 def do_include(parser: Parser, token: Token) -> IncludeNode: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/template/loaders/cached.pyi` & `django-stubs-4.2.2/django-stubs/template/loaders/cached.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/loaders/filesystem.pyi` & `django-stubs-4.2.2/django-stubs/template/loaders/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/response.pyi` & `django-stubs-4.2.2/django-stubs/template/response.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/smartif.pyi` & `django-stubs-4.2.2/django-stubs/template/smartif.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/template/utils.pyi` & `django-stubs-4.2.2/django-stubs/template/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/templatetags/cache.pyi` & `django-stubs-4.2.2/django-stubs/templatetags/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/templatetags/i18n.pyi` & `django-stubs-4.2.2/django-stubs/templatetags/i18n.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/templatetags/static.pyi` & `django-stubs-4.2.2/django-stubs/templatetags/static.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/templatetags/tz.pyi` & `django-stubs-4.2.2/django-stubs/templatetags/tz.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/test/__init__.pyi` & `django-stubs-4.2.2/django-stubs/test/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/test/html.pyi` & `django-stubs-4.2.2/django-stubs/test/html.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/test/runner.pyi` & `django-stubs-4.2.2/django-stubs/test/runner.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import logging
 from argparse import ArgumentParser
 from collections.abc import Iterator, Sequence
 from contextlib import contextmanager
 from io import StringIO
-from typing import Any
+from typing import Any, Literal
 from unittest import TestCase, TestLoader, TestSuite, TextTestResult, TextTestRunner
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.test.testcases import SimpleTestCase
 from django.test.utils import TimeKeeperProtocol
 from django.utils.datastructures import OrderedSet
-from typing_extensions import Literal
 
 class DebugSQLTextTestResult(TextTestResult):
     buffer: bool
     descriptions: bool
     dots: bool
     expectedFailures: list[Any]
     failfast: bool
@@ -129,15 +128,15 @@
         test_name_patterns: list[str] | None = ...,
         pdb: bool = ...,
         buffer: bool = ...,
         enable_faulthandler: bool = ...,
         timing: bool = ...,
         shuffle: int | Literal[False] = ...,
         logger: logging.Logger | None = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None: ...
     @classmethod
     def add_arguments(cls, parser: ArgumentParser) -> None: ...
     @property
     def shuffle_seed(self) -> int | None: ...
     def log(self, msg: str, level: int | None) -> None: ...
     def setup_test_environment(self, **kwargs: Any) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/test/selenium.pyi` & `django-stubs-4.2.2/django-stubs/test/selenium.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/test/signals.pyi` & `django-stubs-4.2.2/django-stubs/test/signals.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/test/testcases.pyi` & `django-stubs-4.2.2/django-stubs/test/testcases.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/test/utils.pyi` & `django-stubs-4.2.2/django-stubs/test/utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import decimal
 from collections.abc import Callable, Iterable, Iterator, Mapping
 from contextlib import AbstractContextManager, contextmanager
 from decimal import Decimal
 from io import StringIO
 from logging import Logger
 from types import TracebackType
-from typing import Any, Protocol, TypeVar
+from typing import Any, Protocol, SupportsIndex, TypeVar
 
 from _typeshed import Self
 from django.apps.registry import Apps
 from django.conf import LazySettings, Settings
 from django.core.checks.registry import CheckRegistry
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.query_utils import RegisterLookupMixin
 from django.test.runner import DiscoverRunner
 from django.test.testcases import SimpleTestCase
-from typing_extensions import SupportsIndex, TypeAlias
+from typing_extensions import TypeAlias
 
 _TestClass: TypeAlias = type[SimpleTestCase]
 
 _DecoratedTest: TypeAlias = Callable | _TestClass
 _DT = TypeVar("_DT", bound=_DecoratedTest)
 _C = TypeVar("_C", bound=Callable)  # Any callable
 
@@ -159,15 +159,15 @@
     interactive: bool,
     *,
     time_keeper: TimeKeeperProtocol | None = ...,
     keepdb: bool = ...,
     debug_sql: bool = ...,
     parallel: int = ...,
     aliases: Mapping[str, Any] | None = ...,
-    **kwargs: Any
+    **kwargs: Any,
 ) -> list[tuple[BaseDatabaseWrapper, str, bool]]: ...
 def teardown_databases(
     old_config: Iterable[tuple[Any, str, bool]], verbosity: int, parallel: int = ..., keepdb: bool = ...
 ) -> None: ...
 def require_jinja2(test_func: _C) -> _C: ...
 @contextmanager
 def register_lookup(
```

### Comparing `django-stubs-4.2.1/django-stubs/urls/__init__.pyi` & `django-stubs-4.2.2/django-stubs/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/urls/base.pyi` & `django-stubs-4.2.2/django-stubs/urls/base.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from collections.abc import Callable, Sequence
-from typing import Any
+from typing import Any, Literal
 
 from django.urls.resolvers import ResolverMatch
-from typing_extensions import Literal
 
 def resolve(path: str, urlconf: str | None = ...) -> ResolverMatch: ...
 def reverse(
     viewname: Callable | str | None,
     urlconf: str | None = ...,
     args: Sequence[Any] | None = ...,
     kwargs: dict[str, Any] | None = ...,
```

### Comparing `django-stubs-4.2.1/django-stubs/urls/conf.pyi` & `django-stubs-4.2.2/django-stubs/urls/conf.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/urls/converters.pyi` & `django-stubs-4.2.2/django-stubs/urls/converters.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/urls/resolvers.pyi` & `django-stubs-4.2.2/django-stubs/urls/resolvers.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from types import ModuleType
 from typing import Any, overload
 
 from django.core.checks.messages import CheckMessage
 from django.urls import _AnyURL
 from django.urls.converters import UUIDConverter
 from django.utils.datastructures import MultiValueDict
+from django.utils.functional import cached_property
 from typing_extensions import TypeAlias
 
 class ResolverMatch:
     func: Callable
     args: tuple[Any, ...]
     kwargs: dict[str, Any]
     url_name: str | None
@@ -28,14 +29,16 @@
         args: tuple[Any, ...],
         kwargs: dict[str, Any],
         url_name: str | None = ...,
         app_names: list[str | None] | None = ...,
         namespaces: list[str | None] | None = ...,
         route: str | None = ...,
         tried: Any | None = ...,
+        captured_kwargs: dict[str, Any] | None = ...,
+        extra_kwargs: dict[str, Any] | None = ...,
     ) -> None: ...
     def __getitem__(self, index: int) -> Any: ...
     # for tuple unpacking
     def __iter__(self) -> Iterator[Any]: ...
 
 def get_resolver(urlconf: str | None = ...) -> URLResolver: ...
 def get_ns_resolver(ns_pattern: str, resolver: URLResolver, converters: tuple) -> URLResolver: ...
@@ -91,15 +94,15 @@
         pattern: _Pattern,
         callback: Callable,
         default_args: dict[str, str] | None = ...,
         name: str | None = ...,
     ) -> None: ...
     def check(self) -> list[CheckMessage]: ...
     def resolve(self, path: str) -> ResolverMatch | None: ...
-    @property
+    @cached_property
     def lookup_str(self) -> str: ...
 
 class URLResolver:
     pattern: _Pattern
     urlconf_name: str | None | Sequence[_AnyURL]
     callback: None
     default_kwargs: dict[str, Any]
@@ -117,16 +120,17 @@
     ) -> None: ...
     @property
     def reverse_dict(self) -> MultiValueDict: ...
     @property
     def namespace_dict(self) -> dict[str, tuple[str, URLResolver]]: ...
     @property
     def app_dict(self) -> dict[str, list[str]]: ...
-    @property
+    @cached_property
     def urlconf_module(self) -> ModuleType | None | Sequence[_AnyURL]: ...
-    @property
+    @cached_property
     def url_patterns(self) -> list[_AnyURL]: ...
     def resolve(self, path: str) -> ResolverMatch: ...
     def resolve_error_handler(self, view_type: int) -> Callable: ...
     def reverse(self, lookup_view: str, *args: Any, **kwargs: Any) -> str: ...
     def _is_callback(self, name: str) -> bool: ...
     def _populate(self) -> None: ...
+    def check(self) -> list[CheckMessage]: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/archive.pyi` & `django-stubs-4.2.2/django-stubs/utils/archive.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/utils/baseconv.pyi` & `django-stubs-4.2.2/django-stubs/utils/baseconv.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/utils/cache.pyi` & `django-stubs-4.2.2/django-stubs/utils/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/utils/connection.pyi` & `django-stubs-4.2.2/django-stubs/utils/connection.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from collections.abc import Iterator, Mapping, Sequence
 from typing import Any, Generic, TypeVar
 
+from django.utils.functional import cached_property
+
 class ConnectionProxy:
     def __init__(self, connections: Mapping[str, Any], alias: str) -> None: ...
     def __getattr__(self, item: str) -> Any: ...
     def __setattr__(self, name: str, value: Any) -> None: ...
     def __delattr__(self, name: str) -> None: ...
     def __contains__(self, key: str) -> bool: ...
     def __eq__(self, other: object) -> bool: ...
@@ -13,17 +15,18 @@
 
 _T = TypeVar("_T")
 
 class BaseConnectionHandler(Generic[_T]):
     settings_name: str | None
     exception_class: type[Exception]
     thread_critical: bool
-    def __init__(self, settings: Any | None = ...) -> None: ...
-    @property
+    @cached_property
     def settings(self) -> dict[str, Any]: ...
+    def __init__(self, settings: Any | None = ...) -> None: ...
     def configure_settings(self, settings: dict[str, Any] | None) -> dict[str, Any]: ...
     def create_connection(self, alias: str) -> _T: ...
     def __getitem__(self, alias: str) -> _T: ...
     def __setitem__(self, key: str, value: _T) -> None: ...
     def __delitem__(self, key: str) -> None: ...
     def __iter__(self) -> Iterator[str]: ...
-    def all(self) -> Sequence[_T]: ...
+    def all(self, initialized_only: bool = ...) -> Sequence[_T]: ...
+    def close_all(self) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/datastructures.pyi` & `django-stubs-4.2.2/django-stubs/utils/datastructures.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from collections.abc import Collection, Iterable, Iterator, Mapping, MutableSet
-from typing import Any, Generic, Protocol, Tuple, TypeVar, overload  # noqa: Y022
+from collections.abc import Collection, Iterable, Iterator, Mapping, MutableMapping, MutableSet
+from typing import Any, Generic, NoReturn, Protocol, Tuple, TypeVar, overload  # noqa: Y022
 
-from _typeshed import Self
-from typing_extensions import TypeAlias
+from _typeshed import Incomplete
+from typing_extensions import Self, TypeAlias
 
 _K = TypeVar("_K")
 _V = TypeVar("_V")
 _Z = TypeVar("_Z")
 _I = TypeVar("_I", covariant=True)
 
 # Unfortunately, there's often check `if isinstance(var, (list, tuple))` in django
@@ -35,21 +35,22 @@
     def __get__(self, instance: Any, owner: Any | None) -> _V: ...
     def __set__(self, instance: Any, value: _K) -> None: ...
 
 class _IndexableCollection(Protocol[_I], Collection[_I]):
     @overload
     def __getitem__(self, index: int) -> _I: ...
     @overload
-    def __getitem__(self: Self, index: slice) -> Self: ...
+    def __getitem__(self, index: slice) -> Self: ...
 
 class OrderedSet(MutableSet[_K]):
     dict: dict[_K, None]
     def __init__(self, iterable: Iterable[_K] | None = ...) -> None: ...
     def __contains__(self, item: object) -> bool: ...
     def __iter__(self) -> Iterator[_K]: ...
+    def __reversed__(self) -> Iterator[_K]: ...
     def __bool__(self) -> bool: ...
     def __len__(self) -> int: ...
     def add(self, item: _K) -> None: ...
     def remove(self, item: _K) -> None: ...
     def discard(self, item: _K) -> None: ...
 
 class MultiValueDictKeyError(KeyError): ...
@@ -70,28 +71,30 @@
     @overload
     def setdefault(self, key: _K, default: _V) -> _V: ...
     def setlistdefault(self, key: _K, default_list: list[_V] | None = ...) -> list[_V]: ...
     def appendlist(self, key: _K, value: _V) -> None: ...
     def items(self) -> Iterator[tuple[_K, _V | list[object]]]: ...  # type: ignore
     def lists(self) -> Iterable[tuple[_K, list[_V]]]: ...
     def dict(self) -> dict[_K, _V | list[object]]: ...
-    def copy(self: Self) -> Self: ...
+    def copy(self) -> Self: ...
     def __getitem__(self, key: _K) -> _V | list[object]: ...  # type: ignore
     def __setitem__(self, key: _K, value: _V) -> None: ...
     # These overrides are needed to convince mypy that this isn't an abstract class
     def __delitem__(self, item: _K) -> None: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[_K]: ...
     # Fake to make `values` work properly
     def values(self) -> Iterator[_V | list[object]]: ...  # type: ignore[override]
+    def __copy__(self) -> Self: ...
+    def __deepcopy__(self, memo: MutableMapping[int, Incomplete]) -> Self: ...
 
 class ImmutableList(tuple[_V, ...]):
     warning: str
-    def __new__(cls: type[Self], *args: Any, warning: str = ..., **kwargs: Any) -> Self: ...
-    def complain(self, *args: Any, **kwargs: Any) -> None: ...
+    def __new__(cls, *args: Any, warning: str = ..., **kwargs: Any) -> Self: ...
+    def complain(self, *args: Any, **kwargs: Any) -> NoReturn: ...
 
 class _ItemCallable(Protocol[_V]):
     """Don't mess with arguments when assigning in class body in stub"""
 
     def __call__(self, __value: _V) -> _V: ...
 
 class DictWrapper(dict[str, _V]):
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/dateformat.pyi` & `django-stubs-4.2.2/django-stubs/utils/dateformat.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from datetime import date
 from datetime import datetime as builtin_datetime
 from datetime import time as builtin_time
 from re import Pattern
-from typing import Any
+from typing import Any, Literal
 
 from django.utils.timezone import _TzInfoT
-from typing_extensions import Literal
 
 re_formatchars: Pattern[str]
 re_escaped: Pattern[str]
 
 class Formatter:
     def format(self, formatstr: str) -> str: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/deprecation.pyi` & `django-stubs-4.2.2/django-stubs/utils/deprecation.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from collections.abc import Callable
+from collections.abc import Awaitable, Callable
 from typing import Any, Protocol
 
 from django.http.request import HttpRequest
 from django.http.response import HttpResponseBase
 from typing_extensions import TypeAlias
 
-class RemovedInDjango40Warning(DeprecationWarning): ...
-class RemovedInDjango41Warning(PendingDeprecationWarning): ...
+class RemovedInDjango50Warning(DeprecationWarning): ...
+class RemovedInDjango51Warning(PendingDeprecationWarning): ...
 
-RemovedInNextVersionWarning: TypeAlias = RemovedInDjango40Warning
+RemovedInNextVersionWarning: TypeAlias = RemovedInDjango50Warning
+RemovedAfterNextVersionWarning: TypeAlias = RemovedInDjango51Warning
 
 class warn_about_renamed_method:
     class_name: str
     old_method_name: str
     new_method_name: str
     deprecation_warning: type[DeprecationWarning]
     def __init__(
@@ -25,14 +26,21 @@
     def __new__(cls, name: Any, bases: Any, attrs: Any) -> type: ...
 
 class DeprecationInstanceCheck(type):
     alternative: str
     deprecation_warning: type[Warning]
     def __instancecheck__(self, instance: Any) -> bool: ...
 
-class GetResponseCallable(Protocol):
+class _GetResponseCallable(Protocol):
     def __call__(self, __request: HttpRequest) -> HttpResponseBase: ...
 
+class _AsyncGetResponseCallable(Protocol):
+    def __call__(self, __request: HttpRequest) -> Awaitable[HttpResponseBase]: ...
+
 class MiddlewareMixin:
-    get_response: GetResponseCallable
-    def __init__(self, get_response: GetResponseCallable = ...) -> None: ...
+    sync_capable: bool
+    async_capable: bool
+
+    get_response: _GetResponseCallable | _AsyncGetResponseCallable
+    def __init__(self, get_response: _GetResponseCallable | _AsyncGetResponseCallable) -> None: ...
     def __call__(self, request: HttpRequest) -> HttpResponseBase: ...
+    async def __acall__(self, request: HttpRequest) -> HttpResponseBase: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/encoding.pyi` & `django-stubs-4.2.2/django-stubs/utils/encoding.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from decimal import Decimal
-from typing import Any, TypeVar, overload
+from typing import Any, Literal, TypeVar, overload
 
 from django.utils.functional import Promise
-from typing_extensions import Literal, TypeGuard
+from typing_extensions import TypeGuard
 
 class DjangoUnicodeDecodeError(UnicodeDecodeError):
     obj: bytes
     def __init__(self, obj: bytes, *args: Any) -> None: ...
 
 _P = TypeVar("_P", bound=Promise)
 _S = TypeVar("_S", bound=str)
@@ -22,31 +22,25 @@
 def smart_str(s: Any, encoding: str = ..., *, errors: str = ...) -> str: ...
 @overload
 def smart_str(s: _PT, encoding: str = ..., strings_only: Literal[True] = ..., errors: str = ...) -> _PT: ...
 @overload
 def smart_str(s: _S, encoding: str = ..., strings_only: bool = ..., errors: str = ...) -> _S: ...
 @overload
 def smart_str(s: Any, encoding: str = ..., strings_only: bool = ..., errors: str = ...) -> str: ...
-
-smart_text = smart_str  # Deprecated
-
 def is_protected_type(obj: Any) -> TypeGuard[_PT]: ...
 @overload
 def force_str(s: _S, encoding: str = ..., *, errors: str = ...) -> _S: ...
 @overload
 def force_str(s: Any, encoding: str = ..., *, errors: str = ...) -> str: ...
 @overload
 def force_str(s: _PT, encoding: str = ..., strings_only: Literal[True] = ..., errors: str = ...) -> _PT: ...
 @overload
 def force_str(s: _S, encoding: str = ..., strings_only: bool = ..., errors: str = ...) -> _S: ...
 @overload
 def force_str(s: Any, encoding: str = ..., strings_only: bool = ..., errors: str = ...) -> str: ...
-
-force_text = force_str  # Deprecated
-
 @overload
 def smart_bytes(s: _P, encoding: str = ..., strings_only: bool = ..., errors: str = ...) -> _P: ...
 @overload
 def smart_bytes(s: _B, encoding: Literal["utf-8"] = ..., *, errors: str = ...) -> _B: ...
 @overload
 def smart_bytes(s: Any, encoding: str = ..., *, errors: str = ...) -> bytes: ...
 @overload
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/feedgenerator.pyi` & `django-stubs-4.2.2/django-stubs/utils/feedgenerator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         author_link: str | None = ...,
         subtitle: str | None = ...,
         categories: tuple[str, str] | None = ...,
         feed_url: str | None = ...,
         feed_copyright: str | None = ...,
         feed_guid: str | None = ...,
         ttl: int | None = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None: ...
     def add_item(
         self,
         title: str,
         link: str,
         description: str,
         author_email: str | None = ...,
@@ -41,15 +41,15 @@
         unique_id: str | None = ...,
         unique_id_is_permalink: bool | None = ...,
         categories: tuple | None = ...,
         item_copyright: str | None = ...,
         ttl: int | None = ...,
         updateddate: datetime.datetime | None = ...,
         enclosures: list[Enclosure] | None = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None: ...
     def num_items(self) -> int: ...
     def root_attributes(self) -> dict[Any, Any]: ...
     def add_root_elements(self, handler: ContentHandler) -> None: ...
     def item_attributes(self, item: dict[str, Any]) -> dict[Any, Any]: ...
     def add_item_elements(self, handler: ContentHandler, item: dict[str, Any]) -> None: ...
     def write(self, outfile: Any, encoding: Any) -> None: ...
@@ -60,14 +60,15 @@
     length: Any
     mime_type: str
     url: str
     def __init__(self, url: str, length: int | str, mime_type: str) -> None: ...
 
 class RssFeed(SyndicationFeed):
     content_type: str
+    def rss_attributes(self) -> dict[str, str]: ...
     def write_items(self, handler: ContentHandler) -> None: ...
     def endChannelElement(self, handler: ContentHandler) -> None: ...
 
 class RssUserland091Feed(RssFeed): ...
 class Rss201rev2Feed(RssFeed): ...
 
 class Atom1Feed(SyndicationFeed):
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/formats.pyi` & `django-stubs-4.2.2/django-stubs/utils/formats.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import types
 from collections.abc import Iterator
-from datetime import date
+from datetime import date, time
 from datetime import datetime as builtin_datetime
-from datetime import time
 from decimal import Decimal
 from typing import Any, TypeVar, overload
 
 ISO_INPUT_FORMATS: dict[str, list[str]]
 FORMAT_SETTINGS: frozenset[str]
 
 def reset_format_cache() -> None: ...
 def iter_format_modules(lang: str, format_module_path: list[str] | str | None = ...) -> Iterator[types.ModuleType]: ...
-def get_format_modules(lang: str | None = ..., reverse: bool = ...) -> list[types.ModuleType]: ...
+def get_format_modules(lang: str | None = ...) -> list[types.ModuleType]: ...
 def get_format(format_type: str, lang: str | None = ..., use_l10n: bool | None = ...) -> Any: ...
 
 get_format_lazy: Any
 
 def date_format(value: date | builtin_datetime | str, format: str | None = ..., use_l10n: bool | None = ...) -> str: ...
 def time_format(value: time | builtin_datetime | str, format: str | None = ..., use_l10n: bool | None = ...) -> str: ...
 def number_format(
@@ -39,7 +38,8 @@
 @overload
 def localize_input(  # type: ignore
     value: builtin_datetime | date | time | Decimal | float | str, default: str | None = ...
 ) -> str: ...
 @overload
 def localize_input(value: _T, default: str | None = ...) -> _T: ...
 def sanitize_separators(value: _T) -> _T: ...
+def sanitize_strftime_format(fmt: str) -> str: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/functional.pyi` & `django-stubs-4.2.2/django-stubs/utils/functional.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from collections.abc import Callable, Sequence
-from typing import Any, Generic, Protocol, TypeVar, overload
+from typing import Any, Generic, Protocol, SupportsIndex, TypeVar, overload
 
 from _typeshed import Self
 from django.db.models.base import Model
-from typing_extensions import SupportsIndex, TypeAlias
+from typing_extensions import TypeAlias
 
 _T = TypeVar("_T")
 
 class cached_property(Generic[_T]):
     func: Callable[..., _T]
-    name: str
-    def __init__(self, func: Callable[..., _T], name: str = ...) -> None: ...
+    name: str | None
+    def __init__(self, func: Callable[..., _T], name: str | None = ...) -> None: ...
     @overload
-    def __get__(self: Self, instance: None, cls: type[Any] = ...) -> Self: ...
+    def __get__(self: Self, instance: None, cls: type[Any] | None = ...) -> Self: ...
     @overload
-    def __get__(self, instance: object, cls: type[Any] = ...) -> _T: ...
+    def __get__(self, instance: object, cls: type[Any] | None = ...) -> _T: ...
+    def __set_name__(self, owner: type[Any], name: str) -> None: ...
 
 # Promise is only subclassed by a proxy class defined in the lazy function
 # so it makes sense for it to have all the methods available in that proxy class
 class Promise:
     def __init__(self, args: Any, kw: Any) -> None: ...
     def __reduce__(self) -> tuple[Any, tuple[Any]]: ...
     def __lt__(self, other: Any) -> bool: ...
@@ -59,44 +60,51 @@
 class LazyObject:
     def __init__(self) -> None: ...
     __getattr__: Callable
     def __setattr__(self, name: str, value: Any) -> None: ...
     def __delattr__(self, name: str) -> None: ...
     def __reduce__(self) -> tuple[Callable, tuple[Model]]: ...
     def __copy__(self) -> LazyObject: ...
+    # TODO: Deepcopy can return a LazyObject or a wrapped object, but we'll need to make LazyObject generic first
+    def __deepcopy__(self, memo: dict[int, Any]) -> Any: ...
     __bytes__: Callable
     __bool__: Callable
     __dir__: Callable
     __ne__: Callable
     __hash__: Callable
     __getitem__: Callable
     __setitem__: Callable
     __delitem__: Callable
     __iter__: Callable
     __len__: Callable
     __contains__: Callable
+    __gt__: Callable
+    __lt__: Callable
+    __add__: Callable
+    __str__: Callable[..., str]
 
 def unpickle_lazyobject(wrapped: Model) -> Model: ...
 
 class SimpleLazyObject(LazyObject):
     def __init__(self, func: Callable[[], Any]) -> None: ...
     def __copy__(self) -> SimpleLazyObject: ...
+    __radd__: Callable
 
 _PartitionMember = TypeVar("_PartitionMember")
 
 def partition(
     predicate: Callable[[_PartitionMember], int | bool], values: list[_PartitionMember]
 ) -> tuple[list[_PartitionMember], list[_PartitionMember]]: ...
 
 _Get = TypeVar("_Get", covariant=True)
 
 class classproperty(Generic[_Get]):
     fget: Callable[[Any], _Get] | None
     def __init__(self, method: Callable[[Any], _Get] | None = ...) -> None: ...
-    def __get__(self, instance: Any | None, cls: type[Any] = ...) -> _Get: ...
+    def __get__(self, instance: Any | None, cls: type[Any] | None = ...) -> _Get: ...
     def getter(self, method: Callable[[Any], _Get]) -> classproperty[_Get]: ...
 
 class _Getter(Protocol[_Get]):
     """Type fake to declare some read-only properties (until `property` builtin is generic)
 
     We can use something like `Union[_Getter[str], str]` in base class to avoid errors
     when redefining attribute with property or property with attribute.
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/http.pyi` & `django-stubs-4.2.2/django-stubs/utils/http.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 MONTHS: list[str]
 RFC1123_DATE: Pattern[str]
 RFC850_DATE: Pattern[str]
 ASCTIME_DATE: Pattern[str]
 RFC3986_GENDELIMS: str
 RFC3986_SUBDELIMS: str
 
-def urlquote(url: str, safe: str = ...) -> str: ...
-def urlquote_plus(url: str, safe: str = ...) -> str: ...
-def urlunquote(quoted_url: str) -> str: ...
-def urlunquote_plus(quoted_url: str) -> str: ...
 def urlencode(
     query: Mapping[str, str | bytes | int | Iterable[str | bytes | int]]
     | Iterable[tuple[str, str | bytes | int | Iterable[str | bytes | int]]]
     | None,
     doseq: bool = ...,
 ) -> str: ...
 def http_date(epoch_seconds: float | None = ...) -> str: ...
@@ -28,19 +24,10 @@
 def urlsafe_base64_decode(s: str) -> bytes: ...
 def parse_etags(etag_str: str) -> list[str]: ...
 def quote_etag(etag_str: str) -> str: ...
 def is_same_domain(host: str, pattern: str) -> bool: ...
 def url_has_allowed_host_and_scheme(
     url: str | None, allowed_hosts: str | Iterable[str] | None, require_https: bool = ...
 ) -> bool: ...
-def is_safe_url(url: str | None, allowed_hosts: str | Iterable[str] | None, require_https: bool = ...) -> bool: ...
-def parse_qsl(
-    qs: str,
-    keep_blank_values: bool = ...,
-    strict_parsing: bool = ...,
-    encoding: str = ...,
-    errors: str = ...,
-    max_num_fields: int | None = ...,
-    separator: str = ...,
-) -> list[tuple[str, str]]: ...
 def escape_leading_slashes(url: str) -> str: ...
 def content_disposition_header(as_attachment: bool, filename: str) -> str | None: ...
+def parse_header_parameters(line: str) -> tuple[str, dict[str, str]]: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/jslex.pyi` & `django-stubs-4.2.2/django-stubs/utils/jslex.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/utils/log.pyi` & `django-stubs-4.2.2/django-stubs/utils/log.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,9 +45,9 @@
 def log_response(
     message: str,
     *args: Any,
     response: HttpResponse | None = ...,
     request: HttpRequest | None = ...,
     logger: Logger = ...,
     level: str | None = ...,
-    exception: BaseException | None = ...
+    exception: BaseException | None = ...,
 ) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/regex_helper.pyi` & `django-stubs-4.2.2/django-stubs/utils/regex_helper.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/utils/safestring.pyi` & `django-stubs-4.2.2/django-stubs/utils/safestring.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/utils/termcolors.pyi` & `django-stubs-4.2.2/django-stubs/utils/termcolors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/utils/text.pyi` & `django-stubs-4.2.2/django-stubs/utils/text.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from collections.abc import Callable, Iterable, Iterator
 from io import BytesIO
 from re import Pattern
 from typing import TypeVar, overload
 
 from django.db.models.base import Model
 from django.utils.functional import SimpleLazyObject, _StrOrPromise
-from django.utils.safestring import SafeString
 
 _StrOrPromiseT = TypeVar("_StrOrPromiseT", bound=_StrOrPromise)
 
 def capfirst(x: _StrOrPromiseT | None) -> _StrOrPromiseT | None: ...
 
 re_words: Pattern[str]
 re_chars: Pattern[str]
@@ -28,24 +27,23 @@
 def get_valid_filename(name: _StrOrPromiseT) -> _StrOrPromiseT: ...
 @overload
 def get_text_list(list_: list[str], last_word: str = ...) -> str: ...
 @overload
 def get_text_list(list_: list[_StrOrPromise], last_word: _StrOrPromise = ...) -> _StrOrPromise: ...
 def normalize_newlines(text: _StrOrPromiseT) -> _StrOrPromiseT: ...
 def phone2numeric(phone: _StrOrPromiseT) -> _StrOrPromiseT: ...
-def compress_string(s: bytes) -> bytes: ...
+def compress_string(s: bytes, *, max_random_bytes: int | None = ...) -> bytes: ...
 
 class StreamingBuffer(BytesIO):
     vals: list[bytes]
     def read(self) -> bytes: ...  # type: ignore
 
-def compress_sequence(sequence: Iterable[bytes]) -> Iterator[bytes]: ...
+def compress_sequence(sequence: Iterable[bytes], *, max_random_bytes: int | None = ...) -> Iterator[bytes]: ...
 
 smart_split_re: Pattern[str]
 
 def smart_split(text: str) -> Iterator[str]: ...
-def unescape_entities(text: _StrOrPromiseT) -> _StrOrPromiseT: ...
 def unescape_string_literal(s: _StrOrPromiseT) -> _StrOrPromiseT: ...
 def slugify(value: _StrOrPromiseT, allow_unicode: bool = ...) -> _StrOrPromiseT: ...
 def camel_case_to_spaces(value: str) -> str: ...
 
 format_lazy: Callable[..., str]
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/timezone.pyi` & `django-stubs-4.2.2/django-stubs/utils/timezone.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from contextlib import ContextDecorator
 from datetime import date, datetime, time, timedelta, timezone, tzinfo
 from types import TracebackType
-from typing import Any, overload
+from typing import Any, Literal, overload
 
 import pytz
 from pytz import BaseTzInfo
-from typing_extensions import Literal, TypeAlias, TypeGuard
+from typing_extensions import TypeAlias, TypeGuard
 
 _PytzTzInfoT: TypeAlias = pytz.tzinfo.BaseTzInfo | pytz._FixedOffset
 
 _TzInfoT: TypeAlias = _PytzTzInfoT | tzinfo
 
 utc: Any
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/translation/__init__.pyi` & `django-stubs-4.2.2/django-stubs/utils/translation/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,27 @@
-import functools
-from collections.abc import Callable
 from contextlib import ContextDecorator
 from types import TracebackType
 from typing import Any
 
 from django.http.request import HttpRequest
 from django.utils.functional import _StrPromise
 
-LANGUAGE_SESSION_KEY: str
-
 class TranslatorCommentWarning(SyntaxWarning): ...
 
-class Trans:
-    activate: Callable
-    check_for_language: functools._lru_cache_wrapper
-    deactivate: Callable
-    deactivate_all: Callable
-    get_language: Callable
-    get_language_bidi: Callable
-    get_language_from_path: Callable
-    get_language_from_request: Callable
-    gettext: Callable
-    gettext_noop: Callable
-    ngettext: Callable
-    npgettext: Callable
-    pgettext: Callable
-    def __getattr__(self, real_name: Any) -> Any: ...
-
 def gettext_noop(message: str) -> str: ...
 def gettext(message: str) -> str: ...
 def ngettext(singular: str, plural: str, number: float) -> str: ...
 def pgettext(context: str, message: str) -> str: ...
 def npgettext(context: str, singular: str, plural: str, number: int) -> str: ...
 
 # lazy evaluated translation functions
 def gettext_lazy(message: str) -> _StrPromise: ...
 def pgettext_lazy(context: str, message: str) -> _StrPromise: ...
 def ngettext_lazy(singular: str, plural: str, number: int | str | None = ...) -> _StrPromise: ...
 def npgettext_lazy(context: str, singular: str, plural: str, number: int | str | None = ...) -> _StrPromise: ...
-
-# NOTE: These translation functions are deprecated and removed in Django 4.0. We should remove them when we drop
-# support for 3.2
-def ugettext_noop(message: str) -> str: ...
-def ugettext(message: str) -> str: ...
-def ungettext(singular: str, plural: str, number: float) -> str: ...
-
-ugettext_lazy = gettext_lazy
-
-ungettext_lazy = ngettext_lazy
-
 def activate(language: str) -> None: ...
 def deactivate() -> None: ...
 
 class override(ContextDecorator):
     language: str | None
     deactivate: bool
     def __init__(self, language: str | None, deactivate: bool = ...) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/translation/trans_null.pyi` & `django-stubs-4.2.2/django-stubs/utils/translation/trans_null.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Any
-
 from django.http.request import HttpRequest
 
 def gettext(message: str) -> str: ...
 
 gettext_noop = gettext
 gettext_lazy = gettext
 _ = gettext
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/translation/trans_real.pyi` & `django-stubs-4.2.2/django-stubs/utils/translation/trans_real.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import gettext as gettext_module
 from collections.abc import Iterator
 from gettext import NullTranslations
 from re import Pattern
 
 # switch to tuple once https://github.com/python/mypy/issues/11098 is fixed
-from typing import Any, Protocol, Tuple, TypeVar  # noqa: Y022
+from typing import Any, Literal, Protocol, Tuple, TypeVar  # noqa: Y022
 
 from django.http.request import HttpRequest
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import TypeAlias
 
 CONTEXT_SEPARATOR: Literal["\x04"]
+ACCEPT_LANGUAGE_HEADER_MAX_LENGTH: int
+
 accept_language_re: Pattern[str]
 language_code_re: Pattern[str]
 language_code_prefix_re: Pattern[str]
 
 class _PluralCallable(Protocol):
     def __call__(self, __n: int) -> int: ...
 
-def reset_cache(**kwargs: Any) -> None: ...
+def reset_cache(*, setting: str, **kwargs: Any) -> None: ...
 
 # switch to tuple once https://github.com/python/mypy/issues/11098 is fixed
 _KeyT: TypeAlias = str | Tuple[str, int]
 
 _Z = TypeVar("_Z")
 
 class TranslationCatalog:
```

### Comparing `django-stubs-4.2.1/django-stubs/utils/tree.pyi` & `django-stubs-4.2.2/django-stubs/utils/tree.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     children: _NodeChildren
     default: str
     connector: str
     negated: bool
     def __init__(
         self, children: _NodeChildren | None = ..., connector: str | None = ..., negated: bool = ...
     ) -> None: ...
+    @classmethod
+    def create(cls, children: _NodeChildren | None = ..., connector: str | None = ..., negated: bool = ...) -> Node: ...
+    def copy(self) -> Node: ...
+    def __copy__(self) -> Node: ...
     def __deepcopy__(self, memodict: dict[Any, Any]) -> Node: ...
     def __len__(self) -> int: ...
     def __bool__(self) -> bool: ...
     def __contains__(self, other: tuple[str, int]) -> bool: ...
     def __hash__(self) -> int: ...
-    def add(self, data: Any, conn_type: str, squash: bool = ...) -> Any: ...
+    def add(self, data: Any, conn_type: str) -> Any: ...
     def negate(self) -> None: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/views/debug.pyi` & `django-stubs-4.2.2/django-stubs/views/debug.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import re
 from collections.abc import Callable, ItemsView, Iterator
-from importlib.abc import SourceLoader
 from pathlib import Path
 from types import TracebackType
 from typing import Any
 
 from django.http.request import HttpRequest, QueryDict
 from django.http.response import Http404, HttpResponse
+from django.template import Engine
 from django.utils.safestring import SafeString
 
-CLEANSED_SUBSTITUTE: str
-CURRENT_DIR: Path
+DEBUG_ENGINE: Engine
 
 class CallableSettingWrapper:
     def __init__(self, callable_setting: Callable | type[Any]) -> None: ...
 
 def technical_500_response(
     request: HttpRequest,
     exc_type: type[BaseException] | None,
@@ -21,14 +21,16 @@
     tb: TracebackType | None,
     status_code: int = ...,
 ) -> HttpResponse: ...
 def get_default_exception_reporter_filter() -> SafeExceptionReporterFilter: ...
 def get_exception_reporter_filter(request: HttpRequest | None) -> SafeExceptionReporterFilter: ...
 
 class SafeExceptionReporterFilter:
+    cleansed_substitute: str
+    hidden_settings: re.Pattern[str]
     def cleanse_setting(self, key: int | str, value: Any) -> Any: ...
     def get_safe_settings(self) -> dict[str, Any]: ...
     def is_active(self, request: HttpRequest | None) -> bool: ...
     def get_cleansed_multivaluedict(self, request: HttpRequest, multivaluedict: QueryDict) -> QueryDict: ...
     def get_post_parameters(self, request: HttpRequest | None) -> dict[str, Any]: ...
     def cleanse_special_types(self, request: HttpRequest | None, value: Any) -> Any: ...
     def get_traceback_frame_variables(self, request: Any, tb_frame: Any) -> ItemsView[str, Any]: ...
```

### Comparing `django-stubs-4.2.1/django-stubs/views/decorators/http.pyi` & `django-stubs-4.2.2/django-stubs/views/decorators/http.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/views/defaults.pyi` & `django-stubs-4.2.2/django-stubs/views/defaults.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/views/generic/__init__.pyi` & `django-stubs-4.2.2/django-stubs/views/generic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/views/generic/base.pyi` & `django-stubs-4.2.2/django-stubs/views/generic/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/views/generic/dates.pyi` & `django-stubs-4.2.2/django-stubs/views/generic/dates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/views/generic/detail.pyi` & `django-stubs-4.2.2/django-stubs/views/generic/detail.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django-stubs/views/generic/edit.pyi` & `django-stubs-4.2.2/django-stubs/views/generic/edit.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import Any, Generic, TypeVar
+from typing import Any, Generic, Literal, TypeVar
 
 from django.db import models
 from django.forms.forms import BaseForm
 from django.forms.models import BaseModelForm
 from django.http import HttpRequest, HttpResponse
 from django.utils.datastructures import _ListOrTuple
 from django.views.generic.base import ContextMixin, TemplateResponseMixin, View
 from django.views.generic.detail import BaseDetailView, SingleObjectMixin, SingleObjectTemplateResponseMixin
-from typing_extensions import Literal
 
 _FormT = TypeVar("_FormT", bound=BaseForm)
 _ModelFormT = TypeVar("_ModelFormT", bound=BaseModelForm)
 _M = TypeVar("_M", bound=models.Model)
 
 class FormMixin(Generic[_FormT], ContextMixin):
     initial: dict[str, Any]
```

### Comparing `django-stubs-4.2.1/django-stubs/views/generic/list.pyi` & `django-stubs-4.2.2/django-stubs/views/generic/list.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def get_paginate_by(self, queryset: _SupportsPagination[_M]) -> int | None: ...
     def get_paginator(
         self,
         queryset: _SupportsPagination[_M],
         per_page: int,
         orphans: int = ...,
         allow_empty_first_page: bool = ...,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> Paginator: ...
     def get_paginate_orphans(self) -> int: ...
     def get_allow_empty(self) -> bool: ...
     def get_context_object_name(self, object_list: _SupportsPagination[_M]) -> str | None: ...
 
 class BaseListView(MultipleObjectMixin[_M], View):
     object_list: _SupportsPagination[_M]
```

### Comparing `django-stubs-4.2.1/django-stubs/views/i18n.pyi` & `django-stubs-4.2.2/django-stubs/views/i18n.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/django_stubs.egg-info/PKG-INFO` & `django-stubs-4.2.2/django_stubs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs
-Version: 4.2.1
+Version: 4.2.2
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -13,17 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: compatible-mypy
 License-File: LICENSE.md
@@ -75,14 +72,15 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
 | 1.16.0         | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.15.0         | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 | 1.14.0         | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 
 ## Features
@@ -102,14 +100,34 @@
     class Meta(TypedModelMeta):
         ordering = ["example"]
         constraints = [
             models.UniqueConstraint(fields=["example"], name="unique_example"),
         ]
 ```
 
+### Other typed base classes
+
+* `django_stubs_ext.db.router.TypedDatabaseRouter` can be used as base when implementing custom database routers.
+
+## Settings
+
+django-stubs has a few settings, which you can list in:
+
+* `pyproject.toml`, under the table `[tool.django-stubs]`
+* `mypy.ini` under the table `[mypy.plugins.django-stubs]`
+
+The supported settings are:
+
+- `django_settings_module`, a string.
+
+  Specify the import path of your settings module, the same as Django’s [`DJANGO_SETTINGS_MODULE` environment variable](https://docs.djangoproject.com/en/stable/topics/settings/#designating-the-settings).
+
+- `strict_settings`, a boolean, default `true`.
+
+  Set to `false` if using dynamic settings, as [described below](https://github.com/typeddjango/django-stubs#how-to-use-a-custom-library-to-handle-django-settings).
 
 ## FAQ
 
 ### Is this an official Django project?
 
 No, it is not. We are independent from Django at the moment.
 There's a [proposal](https://github.com/django/deps/pull/65) to merge our project into the Django itself.
@@ -334,14 +352,61 @@
 
 The lazy translation functions of Django (such as `gettext_lazy`) return a `Promise` instead of `str`. These two types [cannot be used interchangeably](https://github.com/typeddjango/django-stubs/pull/1139#issuecomment-1232167698). The return type of these functions was therefore [changed](https://github.com/typeddjango/django-stubs/pull/689) to reflect that.
 
 If you encounter this error in your own code, you can either cast the `Promise` to `str` (causing the translation to be evaluated), or use the `StrPromise` or `StrOrPromise` types from `django-stubs-ext` in type hints. Which solution to choose depends depends on the particular case. See [working with lazy translation objects](https://docs.djangoproject.com/en/4.1/topics/i18n/translation/#working-with-lazy-translation-objects) in the Django documentation for more information.
 
 If this is reported on Django code, please report an issue or open a pull request to fix the type hints.
 
+### How to use a custom library to handle Django settings?
+
+Using something like [`django-split-settings`](https://github.com/wemake-services/django-split-settings) or [`django-configurations`](https://github.com/jazzband/django-configurations) will make it hard for mypy to infer your settings.
+
+This might also be the case when using something like:
+
+```python
+try:
+    from .local_settings import *
+except Exception:
+    pass
+```
+
+So, mypy would not like this code:
+
+```python
+from django.conf import settings
+
+settings.CUSTOM_VALUE  # E: 'Settings' object has no attribute 'CUSTOM_SETTING'
+```
+
+To handle this corner case we have a special setting `strict_settings` (`True` by default),
+you can switch it to `False` to always return `Any` and not raise any errors if runtime settings module has the given value,
+for example `pyproject.toml`:
+
+```toml
+[tool.django-stubs]
+strict_settings = false
+```
+
+or `mypy.ini`:
+
+```ini
+[mypy.plugins.django-stubs]
+strict_settings = false
+```
+
+And then:
+
+```python
+# Works:
+reveal_type(settings.EXISTS_IN_RUNTIME)  # N: Any
+
+# Errors:
+reveal_type(settings.MISSING)  # E: 'Settings' object has no attribute 'MISSING'
+```
+
 ## Related projects
 
 - [`awesome-python-typing`](https://github.com/typeddjango/awesome-python-typing) - Awesome list of all typing-related things in Python.
 - [`djangorestframework-stubs`](https://github.com/typeddjango/djangorestframework-stubs) - Stubs for Django REST Framework.
 - [`pytest-mypy-plugins`](https://github.com/typeddjango/pytest-mypy-plugins) - `pytest` plugin that we use for testing `mypy` stubs and plugins.
 - [`wemake-django-template`](https://github.com/wemake-services/wemake-django-template) - Create new typed Django projects in seconds.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-stubs-4.2.1/django_stubs.egg-info/SOURCES.txt` & `django-stubs-4.2.2/django_stubs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -296,14 +296,15 @@
 django-stubs/contrib/sitemaps/views.pyi
 django-stubs/contrib/sitemaps/management/__init__.pyi
 django-stubs/contrib/sitemaps/management/commands/__init__.pyi
 django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
 django-stubs/contrib/sites/__init__.pyi
 django-stubs/contrib/sites/admin.pyi
 django-stubs/contrib/sites/apps.pyi
+django-stubs/contrib/sites/checks.pyi
 django-stubs/contrib/sites/management.pyi
 django-stubs/contrib/sites/managers.pyi
 django-stubs/contrib/sites/middleware.pyi
 django-stubs/contrib/sites/models.pyi
 django-stubs/contrib/sites/requests.pyi
 django-stubs/contrib/sites/shortcuts.pyi
 django-stubs/contrib/sites/migrations/__init__.pyi
@@ -342,21 +343,23 @@
 django-stubs/core/cache/backends/filebased.pyi
 django-stubs/core/cache/backends/locmem.pyi
 django-stubs/core/cache/backends/memcached.pyi
 django-stubs/core/checks/__init__.pyi
 django-stubs/core/checks/async_checks.pyi
 django-stubs/core/checks/caches.pyi
 django-stubs/core/checks/database.pyi
+django-stubs/core/checks/files.pyi
 django-stubs/core/checks/messages.pyi
 django-stubs/core/checks/model_checks.pyi
 django-stubs/core/checks/registry.pyi
 django-stubs/core/checks/templates.pyi
 django-stubs/core/checks/translation.pyi
 django-stubs/core/checks/urls.pyi
 django-stubs/core/checks/compatibility/__init__.pyi
+django-stubs/core/checks/compatibility/django_4_0.pyi
 django-stubs/core/checks/security/__init__.pyi
 django-stubs/core/checks/security/base.pyi
 django-stubs/core/checks/security/csrf.pyi
 django-stubs/core/checks/security/sessions.pyi
 django-stubs/core/files/__init__.pyi
 django-stubs/core/files/base.pyi
 django-stubs/core/files/images.pyi
@@ -687,14 +690,15 @@
 django_stubs.egg-info/SOURCES.txt
 django_stubs.egg-info/dependency_links.txt
 django_stubs.egg-info/requires.txt
 django_stubs.egg-info/top_level.txt
 mypy_django_plugin/__init__.py
 mypy_django_plugin/config.py
 mypy_django_plugin/errorcodes.py
+mypy_django_plugin/exceptions.py
 mypy_django_plugin/main.py
 mypy_django_plugin/py.typed
 mypy_django_plugin/django/__init__.py
 mypy_django_plugin/django/context.py
 mypy_django_plugin/lib/__init__.py
 mypy_django_plugin/lib/fullnames.py
 mypy_django_plugin/lib/helpers.py
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/config.py` & `django-stubs-4.2.2/mypy_django_plugin/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,29 +10,31 @@
 else:
     import tomli as tomllib
 
 INI_USAGE = """
 (config)
 ...
 [mypy.plugins.django-stubs]
-    django_settings_module: str (required)
+django_settings_module = str (required)
+strict_settings = bool (default: true)
 ...
 """
 TOML_USAGE = """
 (config)
 ...
 [tool.django-stubs]
 django_settings_module = str (required)
+strict_settings = bool (default: true)
 ...
 """
 INVALID_FILE = "mypy config file is not specified or found"
 COULD_NOT_LOAD_FILE = "could not load configuration file"
-MISSING_SECTION = "no section [{section}] found".format
+MISSING_SECTION = "no section [{section}] found"
 MISSING_DJANGO_SETTINGS = "missing required 'django_settings_module' config"
-INVALID_SETTING = "invalid {key!r}: the setting must be a boolean".format
+INVALID_BOOL_SETTING = "invalid {key!r}: the setting must be a boolean"
 
 
 def exit_with_error(msg: str, is_toml: bool = False) -> NoReturn:
     """Using mypy's argument parser, raise `SystemExit` to fail hard if validation fails.
 
     Considering that the plugin's startup duration is around double as long as mypy's, this aims to
     import and construct objects only when that's required - which happens once and terminates the
@@ -44,16 +46,17 @@
     handler = CapturableArgumentParser(
         prog="(django-stubs) mypy", usage=textwrap.dedent(TOML_USAGE if is_toml else INI_USAGE)
     )
     handler.error(msg)
 
 
 class DjangoPluginConfig:
-    __slots__ = ("django_settings_module",)
+    __slots__ = ("django_settings_module", "strict_settings")
     django_settings_module: str
+    strict_settings: bool
 
     def __init__(self, config_file: Optional[str]) -> None:
         if not config_file:
             exit_with_error(INVALID_FILE)
 
         filepath = Path(config_file)
         if not filepath.is_file():
@@ -71,32 +74,48 @@
                 data = tomllib.load(f)
         except (tomllib.TOMLDecodeError, OSError):
             toml_exit(COULD_NOT_LOAD_FILE)
 
         try:
             config: Dict[str, Any] = data["tool"]["django-stubs"]
         except KeyError:
-            toml_exit(MISSING_SECTION(section="tool.django-stubs"))
+            toml_exit(MISSING_SECTION.format(section="tool.django-stubs"))
 
         if "django_settings_module" not in config:
             toml_exit(MISSING_DJANGO_SETTINGS)
 
         self.django_settings_module = config["django_settings_module"]
         if not isinstance(self.django_settings_module, str):
             toml_exit("invalid 'django_settings_module': the setting must be a string")
 
+        self.strict_settings = config.get("strict_settings", True)
+        if not isinstance(self.strict_settings, bool):
+            toml_exit(INVALID_BOOL_SETTING.format(key="strict_settings"))
+
     def parse_ini_file(self, filepath: Path) -> None:
         parser = configparser.ConfigParser()
         try:
             with filepath.open(encoding="utf-8") as f:
                 parser.read_file(f, source=str(filepath))
         except OSError:
             exit_with_error(COULD_NOT_LOAD_FILE)
 
         section = "mypy.plugins.django-stubs"
         if not parser.has_section(section):
-            exit_with_error(MISSING_SECTION(section=section))
+            exit_with_error(MISSING_SECTION.format(section=section))
 
         if not parser.has_option(section, "django_settings_module"):
             exit_with_error(MISSING_DJANGO_SETTINGS)
 
         self.django_settings_module = parser.get(section, "django_settings_module").strip("'\"")
+
+        try:
+            self.strict_settings = parser.getboolean(section, "strict_settings", fallback=True)
+        except ValueError:
+            exit_with_error(INVALID_BOOL_SETTING.format(key="strict_settings"))
+
+    def to_json(self) -> Dict[str, Any]:
+        """We use this method to reset mypy cache via `report_config_data` hook."""
+        return {
+            "django_settings_module": self.django_settings_module,
+            "strict_settings": self.strict_settings,
+        }
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/django/context.py` & `django-stubs-4.2.2/mypy_django_plugin/django/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from django.db.models.lookups import Exact
 from django.db.models.sql.query import Query
 from django.utils.functional import cached_property
 from mypy.checker import TypeChecker
 from mypy.nodes import TypeInfo
 from mypy.plugin import MethodContext
-from mypy.types import AnyType, Instance
+from mypy.types import AnyType, Instance, TypeOfAny, UnionType
 from mypy.types import Type as MypyType
-from mypy.types import TypeOfAny, UnionType
 
+from mypy_django_plugin.exceptions import UnregisteredModelError
 from mypy_django_plugin.lib import fullnames, helpers
 from mypy_django_plugin.lib.fullnames import WITH_ANNOTATIONS_FULLNAME
 
+# This import fails when `psycopg2` is not installed, avoid crashing the plugin.
 try:
     from django.contrib.postgres.fields import ArrayField
 except ImportError:
 
     class ArrayField:  # type: ignore
         pass
 
@@ -115,24 +116,36 @@
         return None
 
     def get_model_fields(self, model_cls: Type[Model]) -> Iterator["Field[Any, Any]"]:
         for field in model_cls._meta.get_fields():
             if isinstance(field, Field):
                 yield field
 
+    def get_model_foreign_keys(self, model_cls: Type[Model]) -> Iterator["ForeignKey[Any, Any]"]:
+        for field in model_cls._meta.get_fields():
+            if isinstance(field, ForeignKey):
+                yield field
+
+    def get_model_related_fields(self, model_cls: Type[Model]) -> Iterator["RelatedField[Any, Any]"]:
+        """Get model forward relations"""
+        for field in model_cls._meta.get_fields():
+            if isinstance(field, RelatedField):
+                yield field
+
     def get_model_relations(self, model_cls: Type[Model]) -> Iterator[ForeignObjectRel]:
+        """Get model reverse relations"""
         for field in model_cls._meta.get_fields():
             if isinstance(field, ForeignObjectRel):
                 yield field
 
     def get_field_lookup_exact_type(
         self, api: TypeChecker, field: Union["Field[Any, Any]", ForeignObjectRel]
     ) -> MypyType:
         if isinstance(field, (RelatedField, ForeignObjectRel)):
-            related_model_cls = field.related_model
+            related_model_cls = self.get_field_related_model_cls(field)
             primary_key_field = self.get_primary_key_field(related_model_cls)
             primary_key_type = self.get_field_get_type(api, primary_key_field, method="init")
 
             rel_model_info = helpers.lookup_class_typeinfo(api, related_model_cls)
             if rel_model_info is None:
                 return AnyType(TypeOfAny.explicit)
 
@@ -207,17 +220,14 @@
                     foreign_key_info = helpers.lookup_class_typeinfo(api, field.__class__)
                     if foreign_key_info is None:
                         # maybe there's no type annotation for the field
                         expected_types[field_name] = AnyType(TypeOfAny.unannotated)
                         continue
 
                     related_model = self.get_field_related_model_cls(field)
-                    if related_model is None:
-                        expected_types[field_name] = AnyType(TypeOfAny.from_error)
-                        continue
 
                     if related_model._meta.proxy_for_model is not None:
                         related_model = related_model._meta.proxy_for_model
 
                     related_model_info = helpers.lookup_class_typeinfo(api, related_model)
                     if related_model_info is None:
                         expected_types[field_name] = AnyType(TypeOfAny.unannotated)
@@ -309,50 +319,48 @@
         field_info = helpers.lookup_class_typeinfo(api, field.__class__)
         if field_info is None:
             return AnyType(TypeOfAny.unannotated)
 
         is_nullable = self.get_field_nullability(field, method)
         if isinstance(field, RelatedField):
             related_model_cls = self.get_field_related_model_cls(field)
-            if related_model_cls is None:
-                return AnyType(TypeOfAny.from_error)
 
             if method in ("values", "values_list"):
                 primary_key_field = self.get_primary_key_field(related_model_cls)
                 return self.get_field_get_type(api, primary_key_field, method=method)
 
             model_info = helpers.lookup_class_typeinfo(api, related_model_cls)
             if model_info is None:
                 return AnyType(TypeOfAny.unannotated)
 
             return Instance(model_info, [])
         else:
             return helpers.get_private_descriptor_type(field_info, "_pyi_private_get_type", is_nullable=is_nullable)
 
-    def get_field_related_model_cls(
-        self, field: Union["RelatedField[Any, Any]", ForeignObjectRel]
-    ) -> Optional[Type[Model]]:
+    def get_field_related_model_cls(self, field: Union["RelatedField[Any, Any]", ForeignObjectRel]) -> Type[Model]:
         if isinstance(field, RelatedField):
             related_model_cls = field.remote_field.model
         else:
             related_model_cls = field.field.model
 
         if isinstance(related_model_cls, str):
             if related_model_cls == "self":  # type: ignore
                 # same model
                 related_model_cls = field.model
             elif "." not in related_model_cls:
                 # same file model
-                related_model_fullname = field.model.__module__ + "." + related_model_cls
+                related_model_fullname = f"{field.model.__module__}.{related_model_cls}"
                 related_model_cls = self.get_model_class_by_fullname(related_model_fullname)
+                if related_model_cls is None:
+                    raise UnregisteredModelError
             else:
                 try:
                     related_model_cls = self.apps_registry.get_model(related_model_cls)
-                except LookupError:
-                    return None
+                except LookupError as e:
+                    raise UnregisteredModelError from e
 
         return related_model_cls
 
     def _resolve_field_from_parts(
         self, field_parts: Iterable[str], model_cls: Type[Model]
     ) -> Union["Field[Any, Any]", ForeignObjectRel]:
         currently_observed_model = model_cls
@@ -360,21 +368,21 @@
         for field_part in field_parts:
             if field_part == "pk":
                 field = self.get_primary_key_field(currently_observed_model)
                 continue
 
             field = currently_observed_model._meta.get_field(field_part)
             if isinstance(field, RelatedField):
-                currently_observed_model = field.related_model
+                currently_observed_model = self.get_field_related_model_cls(field)
                 model_name = currently_observed_model._meta.model_name
                 if model_name is not None and field_part == (model_name + "_id"):
                     field = self.get_primary_key_field(currently_observed_model)
 
             if isinstance(field, ForeignObjectRel):
-                currently_observed_model = field.related_model
+                currently_observed_model = self.get_field_related_model_cls(field)
 
         # Guaranteed by `query.solve_lookup_type` before.
         assert isinstance(field, (Field, ForeignObjectRel))
         return field
 
     def solve_lookup_type(
         self, model_cls: Type[Model], lookup: str
@@ -394,17 +402,23 @@
         except AttributeError:
             pass
         query_parts = lookup.split("__")
         try:
             field = query.get_meta().get_field(query_parts[0])
         except FieldDoesNotExist:
             return None
+
         if len(query_parts) == 1:
             return [], [query_parts[0]], False
-        sub_query = Query(field.related_model).solve_lookup_type("__")
+
+        if not isinstance(field, (RelatedField, ForeignObjectRel)):
+            return None
+
+        related_model = self.get_field_related_model_cls(field)
+        sub_query = Query(related_model).solve_lookup_type("__".join(query_parts[1:]))
         entire_query_parts = [query_parts[0], *sub_query[1]]
         return sub_query[0], entire_query_parts, sub_query[2]
 
     def resolve_lookup_into_field(
         self, model_cls: Type[Model], lookup: str
     ) -> Union["Field[Any, Any]", ForeignObjectRel, None]:
         solved_lookup = self.solve_lookup_type(model_cls, lookup)
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/lib/fullnames.py` & `django-stubs-4.2.2/mypy_django_plugin/lib/fullnames.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/mypy_django_plugin/lib/helpers.py` & `django-stubs-4.2.2/mypy_django_plugin/lib/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import OrderedDict
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Iterator, List, Optional, Set, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Iterator, List, Literal, Optional, Set, Union, cast
 
 from django.db.models.fields import Field
 from django.db.models.fields.related import RelatedField
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from mypy import checker
 from mypy.checker import TypeChecker
 from mypy.mro import calculate_mro
@@ -29,27 +29,42 @@
     ClassDefContext,
     DynamicClassDefContext,
     FunctionContext,
     MethodContext,
     SemanticAnalyzerPluginInterface,
 )
 from mypy.semanal import SemanticAnalyzer
-from mypy.types import AnyType, Instance, NoneTyp, TupleType
+from mypy.types import AnyType, Instance, NoneTyp, TupleType, TypedDictType, TypeOfAny, UnionType
 from mypy.types import Type as MypyType
-from mypy.types import TypedDictType, TypeOfAny, UnionType
+from typing_extensions import TypedDict
 
 from mypy_django_plugin.lib import fullnames
 from mypy_django_plugin.lib.fullnames import WITH_ANNOTATIONS_FULLNAME
 
 if TYPE_CHECKING:
     from mypy_django_plugin.django.context import DjangoContext
 
 
-def get_django_metadata(model_info: TypeInfo) -> Dict[str, Any]:
-    return model_info.metadata.setdefault("django", {})
+class DjangoTypeMetadata(TypedDict, total=False):
+    from_queryset_manager: str
+    reverse_managers: Dict[str, str]
+    baseform_bases: Dict[str, int]
+    manager_bases: Dict[str, int]
+    model_bases: Dict[str, int]
+    queryset_bases: Dict[str, int]
+
+
+def get_django_metadata(model_info: TypeInfo) -> DjangoTypeMetadata:
+    return cast(DjangoTypeMetadata, model_info.metadata.setdefault("django", {}))
+
+
+def get_django_metadata_bases(
+    model_info: TypeInfo, key: Literal["baseform_bases", "manager_bases", "model_bases", "queryset_bases"]
+) -> Dict[str, int]:
+    return get_django_metadata(model_info).setdefault(key, cast(Dict[str, int], {}))
 
 
 class IncompleteDefnException(Exception):
     pass
 
 
 def is_toml(filename: str) -> bool:
@@ -316,29 +331,29 @@
 
     return typ
 
 
 def make_typeddict(
     api: CheckerPluginInterface, fields: "OrderedDict[str, MypyType]", required_keys: Set[str]
 ) -> TypedDictType:
-    object_type = api.named_generic_type("mypy_extensions._TypedDict", [])
-    typed_dict_type = TypedDictType(fields, required_keys=required_keys, fallback=object_type)
+    fallback_type = api.named_generic_type("typing._TypedDict", [])
+    typed_dict_type = TypedDictType(fields, required_keys=required_keys, fallback=fallback_type)
     return typed_dict_type
 
 
 def resolve_string_attribute_value(attr_expr: Expression, django_context: "DjangoContext") -> Optional[str]:
     if isinstance(attr_expr, StrExpr):
         return attr_expr.value
 
     # support extracting from settings, in general case it's unresolvable yet
     if isinstance(attr_expr, MemberExpr):
         member_name = attr_expr.name
         if isinstance(attr_expr.expr, NameExpr) and attr_expr.expr.fullname == "django.conf.settings":
             if hasattr(django_context.settings, member_name):
-                return getattr(django_context.settings, member_name)  # type: ignore
+                return getattr(django_context.settings, member_name)  # type: ignore[no-any-return]
     return None
 
 
 def get_semanal_api(ctx: Union[ClassDefContext, DynamicClassDefContext]) -> SemanticAnalyzer:
     if not isinstance(ctx.api, SemanticAnalyzer):
         raise ValueError("Not a SemanticAnalyzer")
     return ctx.api
@@ -373,8 +388,9 @@
     var.is_inferred = True
     info.names[name] = SymbolTableNode(MDEF, var, plugin_generated=True, no_serialize=no_serialize)
 
 
 def add_new_manager_base(api: SemanticAnalyzerPluginInterface, fullname: str) -> None:
     sym = api.lookup_fully_qualified_or_none(fullnames.MANAGER_CLASS_FULLNAME)
     if sym is not None and isinstance(sym.node, TypeInfo):
-        get_django_metadata(sym.node)["manager_bases"][fullname] = 1
+        bases = get_django_metadata_bases(sym.node, "manager_bases")
+        bases[fullname] = 1
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/main.py` & `django-stubs-4.2.2/mypy_django_plugin/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+import itertools
 import sys
 from functools import partial
-from typing import Callable, Dict, List, Optional, Tuple, Type
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type
 
-from django.db.models.fields.related import RelatedField
 from mypy.modulefinder import mypy_path
 from mypy.nodes import MypyFile, TypeInfo
 from mypy.options import Options
 from mypy.plugin import (
     AnalyzeTypeContext,
     AttributeContext,
     ClassDefContext,
     DynamicClassDefContext,
     FunctionContext,
     MethodContext,
     Plugin,
+    ReportConfigContext,
 )
 from mypy.types import Type as MypyType
 
 import mypy_django_plugin.transformers.orm_lookups
 from mypy_django_plugin.config import DjangoPluginConfig
 from mypy_django_plugin.django.context import DjangoContext
+from mypy_django_plugin.exceptions import UnregisteredModelError
 from mypy_django_plugin.lib import fullnames, helpers
 from mypy_django_plugin.transformers import fields, forms, init_create, meta, querysets, request, settings
 from mypy_django_plugin.transformers.functional import resolve_str_promise_attribute
 from mypy_django_plugin.transformers.managers import (
     create_new_manager_class_from_as_manager_method,
     create_new_manager_class_from_from_queryset_method,
     reparametrize_any_manager_hook,
@@ -37,27 +39,29 @@
 from mypy_django_plugin.transformers.request import check_querydict_is_mutable
 
 
 def transform_model_class(ctx: ClassDefContext, django_context: DjangoContext) -> None:
     sym = ctx.api.lookup_fully_qualified_or_none(fullnames.MODEL_CLASS_FULLNAME)
 
     if sym is not None and isinstance(sym.node, TypeInfo):
-        helpers.get_django_metadata(sym.node)["model_bases"][ctx.cls.fullname] = 1
+        bases = helpers.get_django_metadata_bases(sym.node, "model_bases")
+        bases[ctx.cls.fullname] = 1
     else:
         if not ctx.api.final_iteration:
             ctx.api.defer()
             return
 
     process_model_class(ctx, django_context)
 
 
 def transform_form_class(ctx: ClassDefContext) -> None:
     sym = ctx.api.lookup_fully_qualified_or_none(fullnames.BASEFORM_CLASS_FULLNAME)
     if sym is not None and isinstance(sym.node, TypeInfo):
-        helpers.get_django_metadata(sym.node)["baseform_bases"][ctx.cls.fullname] = 1
+        bases = helpers.get_django_metadata_bases(sym.node, "baseform_bases")
+        bases[ctx.cls.fullname] = 1
 
     forms.make_meta_nested_class_inherit_from_any(ctx)
 
 
 def add_new_manager_base_hook(ctx: ClassDefContext) -> None:
     helpers.add_new_manager_base(ctx.api, ctx.cls.fullname)
 
@@ -71,49 +75,46 @@
         # Add paths from mypy_path config option
         sys.path.extend(options.mypy_path)
         self.django_context = DjangoContext(self.plugin_config.django_settings_module)
 
     def _get_current_queryset_bases(self) -> Dict[str, int]:
         model_sym = self.lookup_fully_qualified(fullnames.QUERYSET_CLASS_FULLNAME)
         if model_sym is not None and isinstance(model_sym.node, TypeInfo):
-            return helpers.get_django_metadata(model_sym.node).setdefault(  # type: ignore[no-any-return]
-                "queryset_bases", {fullnames.QUERYSET_CLASS_FULLNAME: 1}
-            )
+            bases = helpers.get_django_metadata_bases(model_sym.node, "queryset_bases")
+            bases[fullnames.QUERYSET_CLASS_FULLNAME] = 1
+            return bases
         else:
             return {}
 
     def _get_current_manager_bases(self) -> Dict[str, int]:
         model_sym = self.lookup_fully_qualified(fullnames.MANAGER_CLASS_FULLNAME)
         if model_sym is not None and isinstance(model_sym.node, TypeInfo):
-            return helpers.get_django_metadata(model_sym.node).setdefault(  # type: ignore[no-any-return]
-                "manager_bases", {fullnames.MANAGER_CLASS_FULLNAME: 1}
-            )
+            bases = helpers.get_django_metadata_bases(model_sym.node, "manager_bases")
+            bases[fullnames.MANAGER_CLASS_FULLNAME] = 1
+            return bases
         else:
             return {}
 
     def _get_current_model_bases(self) -> Dict[str, int]:
         model_sym = self.lookup_fully_qualified(fullnames.MODEL_CLASS_FULLNAME)
         if model_sym is not None and isinstance(model_sym.node, TypeInfo):
-            return helpers.get_django_metadata(model_sym.node).setdefault(  # type: ignore[no-any-return]
-                "model_bases", {fullnames.MODEL_CLASS_FULLNAME: 1}
-            )
+            bases = helpers.get_django_metadata_bases(model_sym.node, "model_bases")
+            bases[fullnames.MODEL_CLASS_FULLNAME] = 1
+            return bases
         else:
             return {}
 
     def _get_current_form_bases(self) -> Dict[str, int]:
         model_sym = self.lookup_fully_qualified(fullnames.BASEFORM_CLASS_FULLNAME)
         if model_sym is not None and isinstance(model_sym.node, TypeInfo):
-            return helpers.get_django_metadata(model_sym.node).setdefault(  # type: ignore[no-any-return]
-                "baseform_bases",
-                {
-                    fullnames.BASEFORM_CLASS_FULLNAME: 1,
-                    fullnames.FORM_CLASS_FULLNAME: 1,
-                    fullnames.MODELFORM_CLASS_FULLNAME: 1,
-                },
-            )
+            bases = helpers.get_django_metadata_bases(model_sym.node, "baseform_bases")
+            bases[fullnames.BASEFORM_CLASS_FULLNAME] = 1
+            bases[fullnames.FORM_CLASS_FULLNAME] = 1
+            bases[fullnames.MODELFORM_CLASS_FULLNAME] = 1
+            return bases
         else:
             return {}
 
     def _get_typeinfo_or_none(self, class_name: str) -> Optional[TypeInfo]:
         sym = self.lookup_fully_qualified(class_name)
         if sym is not None and isinstance(sym.node, TypeInfo):
             return sym.node
@@ -125,15 +126,15 @@
     def get_additional_deps(self, file: MypyFile) -> List[Tuple[int, str, int]]:
         # for settings
         if file.fullname == "django.conf" and self.django_context.django_settings_module:
             return [self._new_dependency(self.django_context.django_settings_module)]
 
         # for values / values_list
         if file.fullname == "django.db.models":
-            return [self._new_dependency("mypy_extensions"), self._new_dependency("typing")]
+            return [self._new_dependency("typing")]
 
         # for `get_user_model()`
         if self.django_context.settings:
             if file.fullname == "django.contrib.auth" or file.fullname in {"django.http", "django.http.request"}:
                 auth_user_model_name = self.django_context.settings.AUTH_USER_MODEL
                 try:
                     auth_user_module = self.django_context.apps_registry.get_model(auth_user_model_name).__module__
@@ -143,31 +144,30 @@
                 return [self._new_dependency(auth_user_module)]
 
         # ensure that all mentioned to='someapp.SomeModel' are loaded with corresponding related Fields
         defined_model_classes = self.django_context.model_modules.get(file.fullname)
         if not defined_model_classes:
             return []
         deps = set()
+
         for model_class in defined_model_classes:
-            # forward relations
-            for field in self.django_context.get_model_fields(model_class):
-                if isinstance(field, RelatedField):
+            for field in itertools.chain(
+                # forward relations
+                self.django_context.get_model_related_fields(model_class),
+                # reverse relations - `related_objects` is private API (according to docstring)
+                model_class._meta.related_objects,  # type: ignore[attr-defined]
+            ):
+                try:
                     related_model_cls = self.django_context.get_field_related_model_cls(field)
-                    if related_model_cls is None:
-                        continue
-                    related_model_module = related_model_cls.__module__
-                    if related_model_module != file.fullname:
-                        deps.add(self._new_dependency(related_model_module))
-            # reverse relations
-            # `related_objects` is private API (according to docstring)
-            for relation in model_class._meta.related_objects:  # type: ignore[attr-defined]
-                related_model_cls = self.django_context.get_field_related_model_cls(relation)
+                except UnregisteredModelError:
+                    continue
                 related_model_module = related_model_cls.__module__
                 if related_model_module != file.fullname:
                     deps.add(self._new_dependency(related_model_module))
+
         return list(deps) + [
             # for QuerySet.annotate
             self._new_dependency("django_stubs_ext"),
             # For BaseManager.from_queryset
             self._new_dependency("django.db.models.query"),
         ]
 
@@ -270,15 +270,19 @@
         return None
 
     def get_attribute_hook(self, fullname: str) -> Optional[Callable[[AttributeContext], MypyType]]:
         class_name, _, attr_name = fullname.rpartition(".")
 
         # Lookup of a settings variable
         if class_name == fullnames.DUMMY_SETTINGS_BASE_CLASS:
-            return partial(settings.get_type_of_settings_attribute, django_context=self.django_context)
+            return partial(
+                settings.get_type_of_settings_attribute,
+                django_context=self.django_context,
+                plugin_config=self.plugin_config,
+            )
 
         info = self._get_typeinfo_or_none(class_name)
 
         # Lookup of the '.is_superuser' attribute
         if info and info.has_base(fullnames.PERMISSION_MIXIN_CLASS_FULLNAME) and attr_name == "is_superuser":
             return partial(set_auth_user_model_boolean_fields, django_context=self.django_context)
 
@@ -323,10 +327,14 @@
                 return create_new_manager_class_from_from_queryset_method
         elif method_name == "as_manager":
             info = self._get_typeinfo_or_none(class_name)
             if info and info.has_base(fullnames.QUERYSET_CLASS_FULLNAME):
                 return create_new_manager_class_from_as_manager_method
         return None
 
+    def report_config_data(self, ctx: ReportConfigContext) -> Dict[str, Any]:
+        # Cache would be cleared if any settings do change.
+        return self.plugin_config.to_json()
+
 
 def plugin(version: str) -> Type[NewSemanalDjangoPlugin]:
     return NewSemanalDjangoPlugin
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/fields.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from django.core.exceptions import FieldDoesNotExist
 from django.db.models.fields import AutoField, Field
 from django.db.models.fields.related import RelatedField
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from mypy.nodes import AssignmentStmt, NameExpr, TypeInfo
 from mypy.plugin import FunctionContext
-from mypy.types import AnyType, Instance
+from mypy.types import AnyType, Instance, TypeOfAny, UnionType
 from mypy.types import Type as MypyType
-from mypy.types import TypeOfAny, UnionType
 
 from mypy_django_plugin.django.context import DjangoContext
+from mypy_django_plugin.exceptions import UnregisteredModelError
 from mypy_django_plugin.lib import fullnames, helpers
 
 if TYPE_CHECKING:
     from django.contrib.contenttypes.fields import GenericForeignKey
 
 
 def _get_current_field_from_assignment(
@@ -56,16 +56,17 @@
 def fill_descriptor_types_for_related_field(ctx: FunctionContext, django_context: DjangoContext) -> MypyType:
     current_field = _get_current_field_from_assignment(ctx, django_context)
     if current_field is None:
         return AnyType(TypeOfAny.from_error)
 
     assert isinstance(current_field, RelatedField)
 
-    related_model_cls = django_context.get_field_related_model_cls(current_field)
-    if related_model_cls is None:
+    try:
+        related_model_cls = django_context.get_field_related_model_cls(current_field)
+    except UnregisteredModelError:
         return AnyType(TypeOfAny.from_error)
 
     default_related_field_type = set_descriptor_types_for_field(ctx)
 
     # self reference with abstract=True on the model where ForeignKey is defined
     current_model_cls = current_field.model
     if current_model_cls._meta.abstract and current_model_cls == related_model_cls:
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/forms.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Optional
 
 from mypy.plugin import ClassDefContext, MethodContext
-from mypy.types import CallableType, Instance, NoneTyp
+from mypy.types import CallableType, Instance, NoneTyp, TypeType
 from mypy.types import Type as MypyType
-from mypy.types import TypeType
 
 from mypy_django_plugin.lib import helpers
 
 
 def make_meta_nested_class_inherit_from_any(ctx: ClassDefContext) -> None:
     meta_node = helpers.get_nested_meta_node_for_current_class(ctx.cls.info)
     if meta_node is None:
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/functional.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from mypy.checkmember import analyze_member_access
 from mypy.errorcodes import ATTR_DEFINED
 from mypy.nodes import CallExpr, MemberExpr
 from mypy.plugin import AttributeContext
-from mypy.types import AnyType, Instance
+from mypy.types import AnyType, Instance, TypeOfAny
 from mypy.types import Type as MypyType
-from mypy.types import TypeOfAny
 
 from mypy_django_plugin.lib import helpers
 
 
 def resolve_str_promise_attribute(ctx: AttributeContext) -> MypyType:
     if isinstance(ctx.context, MemberExpr):
         method_name = ctx.context.name
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/init_create.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/init_create.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/managers.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,16 @@
     SymbolTableNode,
     TypeInfo,
     Var,
 )
 from mypy.plugin import AttributeContext, ClassDefContext, DynamicClassDefContext
 from mypy.semanal import SemanticAnalyzer
 from mypy.semanal_shared import has_placeholder
-from mypy.types import AnyType, CallableType, Instance, ProperType
+from mypy.types import AnyType, CallableType, Instance, ProperType, TypeOfAny
 from mypy.types import Type as MypyType
-from mypy.types import TypeOfAny
 from mypy.typevars import fill_typevars
 
 from mypy_django_plugin.lib import fullnames, helpers
 
 MANAGER_METHODS_RETURNING_QUERYSET: Final = frozenset(
     (
         "alias",
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/meta.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.core.exceptions import FieldDoesNotExist
 from mypy.plugin import MethodContext
-from mypy.types import AnyType, Instance
+from mypy.types import AnyType, Instance, TypeOfAny
 from mypy.types import Type as MypyType
-from mypy.types import TypeOfAny
 
 from mypy_django_plugin.django.context import DjangoContext
 from mypy_django_plugin.lib import helpers
 
 
 def _get_field_instance(ctx: MethodContext, field_fullname: str) -> MypyType:
     field_info = helpers.lookup_fully_qualified_typeinfo(helpers.get_typechecker_api(ctx), field_fullname)
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/models.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from typing import Any, Dict, List, Optional, Type, Union, cast
 
 from django.db.models import Manager, Model
 from django.db.models.fields import DateField, DateTimeField, Field
-from django.db.models.fields.related import ForeignKey
 from django.db.models.fields.reverse_related import ForeignObjectRel, OneToOneRel
 from mypy.checker import TypeChecker
 from mypy.nodes import ARG_STAR2, Argument, AssignmentStmt, CallExpr, Context, NameExpr, TypeInfo, Var
 from mypy.plugin import AnalyzeTypeContext, AttributeContext, CheckerPluginInterface, ClassDefContext
 from mypy.plugins import common
 from mypy.semanal import SemanticAnalyzer
-from mypy.types import AnyType, Instance
+from mypy.types import AnyType, Instance, TypedDictType, TypeOfAny, get_proper_type
 from mypy.types import Type as MypyType
-from mypy.types import TypedDictType, TypeOfAny, get_proper_type
 from mypy.typevars import fill_typevars
 
 from mypy_django_plugin.django.context import DjangoContext
 from mypy_django_plugin.errorcodes import MANAGER_MISSING
+from mypy_django_plugin.exceptions import UnregisteredModelError
 from mypy_django_plugin.lib import fullnames, helpers
 from mypy_django_plugin.lib.fullnames import ANNOTATIONS_FULLNAME, ANY_ATTR_ALLOWED_CLASS_FULLNAME, MODEL_CLASS_FULLNAME
 from mypy_django_plugin.transformers import fields
 from mypy_django_plugin.transformers.fields import get_field_descriptor_types
 from mypy_django_plugin.transformers.managers import (
     MANAGER_METHODS_RETURNING_QUERYSET,
     create_manager_info_from_from_queryset_call,
@@ -231,49 +230,49 @@
                 dest_name="pk",
                 existing_field=self.model_classdef.info.has_readable_member(auto_field.name),
             )
 
 
 class AddRelatedModelsId(ModelClassInitializer):
     def run_with_model_cls(self, model_cls: Type[Model]) -> None:
-        for field in model_cls._meta.get_fields():
-            if isinstance(field, ForeignKey):
+        for field in self.django_context.get_model_foreign_keys(model_cls):
+            try:
                 related_model_cls = self.django_context.get_field_related_model_cls(field)
-                if related_model_cls is None:
-                    error_context: Context = self.ctx.cls
-                    field_sym = self.ctx.cls.info.get(field.name)
-                    if field_sym is not None and field_sym.node is not None:
-                        error_context = field_sym.node
-                    self.api.fail(
-                        f"Cannot find model {field.related_model!r} referenced in field {field.name!r}",
-                        ctx=error_context,
-                    )
-                    self.add_new_node_to_model_class(field.attname, AnyType(TypeOfAny.explicit))
-                    continue
+            except UnregisteredModelError:
+                error_context: Context = self.ctx.cls
+                field_sym = self.ctx.cls.info.get(field.name)
+                if field_sym is not None and field_sym.node is not None:
+                    error_context = field_sym.node
+                self.api.fail(
+                    f"Cannot find model {field.related_model!r} referenced in field {field.name!r}",
+                    ctx=error_context,
+                )
+                self.add_new_node_to_model_class(field.attname, AnyType(TypeOfAny.explicit))
+                continue
 
-                if related_model_cls._meta.abstract:
-                    continue
+            if related_model_cls._meta.abstract:
+                continue
+
+            rel_target_field = self.django_context.get_related_target_field(related_model_cls, field)
+            if not rel_target_field:
+                continue
 
-                rel_target_field = self.django_context.get_related_target_field(related_model_cls, field)
-                if not rel_target_field:
+            try:
+                field_info = self.lookup_class_typeinfo_or_incomplete_defn_error(rel_target_field.__class__)
+            except helpers.IncompleteDefnException as exc:
+                if not self.api.final_iteration:
+                    raise exc
+                else:
                     continue
 
-                try:
-                    field_info = self.lookup_class_typeinfo_or_incomplete_defn_error(rel_target_field.__class__)
-                except helpers.IncompleteDefnException as exc:
-                    if not self.api.final_iteration:
-                        raise exc
-                    else:
-                        continue
-
-                is_nullable = self.django_context.get_field_nullability(field, None)
-                set_type, get_type = get_field_descriptor_types(
-                    field_info, is_set_nullable=is_nullable, is_get_nullable=is_nullable
-                )
-                self.add_new_node_to_model_class(field.attname, Instance(field_info, [set_type, get_type]))
+            is_nullable = self.django_context.get_field_nullability(field, None)
+            set_type, get_type = get_field_descriptor_types(
+                field_info, is_set_nullable=is_nullable, is_get_nullable=is_nullable
+            )
+            self.add_new_node_to_model_class(field.attname, Instance(field_info, [set_type, get_type]))
 
 
 class AddManagers(ModelClassInitializer):
     def has_any_parametrized_manager_as_base(self, info: TypeInfo) -> bool:
         for base in helpers.iter_bases(info):
             if self.is_any_parametrized_manager(base):
                 return True
@@ -445,16 +444,14 @@
             attname = relation.get_accessor_name()
             if attname is None or attname in self.model_classdef.info.names:
                 # No reverse accessor or already declared. Note that this would also leave any
                 # explicitly declared(i.e. non-inferred) reverse accessors alone
                 continue
 
             related_model_cls = self.django_context.get_field_related_model_cls(relation)
-            if related_model_cls is None:
-                continue
 
             try:
                 related_model_info = self.lookup_class_typeinfo_or_incomplete_defn_error(related_model_cls)
             except helpers.IncompleteDefnException as exc:
                 if not self.api.final_iteration:
                     raise exc
                 else:
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/orm_lookups.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/orm_lookups.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from mypy.plugin import MethodContext
-from mypy.types import AnyType, Instance
+from mypy.types import AnyType, Instance, TypeOfAny
 from mypy.types import Type as MypyType
-from mypy.types import TypeOfAny
 
 from mypy_django_plugin.django.context import DjangoContext
+from mypy_django_plugin.exceptions import UnregisteredModelError
 from mypy_django_plugin.lib import fullnames, helpers
 from mypy_django_plugin.lib.helpers import is_annotated_model_fullname
 
 
 def typecheck_queryset_filter(ctx: MethodContext, django_context: DjangoContext) -> MypyType:
     # Expected formal arguments for filter methods are `*args` and `**kwargs`. We'll only typecheck
     # `**kwargs`, which means that `arg_names[1]` is what we're interested in.
@@ -33,15 +33,18 @@
         ):
             provided_type = resolve_combinable_type(provided_type, django_context)
 
         lookup_type: MypyType
         if is_annotated_model_fullname(model_cls_fullname):
             lookup_type = AnyType(TypeOfAny.implementation_artifact)
         else:
-            lookup_type = django_context.resolve_lookup_expected_type(ctx, model_cls, lookup_kwarg)
+            try:
+                lookup_type = django_context.resolve_lookup_expected_type(ctx, model_cls, lookup_kwarg)
+            except UnregisteredModelError:
+                lookup_type = AnyType(TypeOfAny.from_error)
         # Managers as provided_type is not supported yet
         if isinstance(provided_type, Instance) and helpers.has_any_of_bases(
             provided_type.type, (fullnames.MANAGER_CLASS_FULLNAME, fullnames.QUERYSET_CLASS_FULLNAME)
         ):
             return ctx.default_return_type
 
         helpers.check_types_compatible(
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/querysets.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/querysets.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
 from django.core.exceptions import FieldError
 from django.db.models.base import Model
 from django.db.models.fields.related import RelatedField
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from mypy.nodes import ARG_NAMED, ARG_NAMED_OPT, Expression, NameExpr
 from mypy.plugin import FunctionContext, MethodContext
-from mypy.types import AnyType, Instance, TupleType
+from mypy.types import AnyType, Instance, TupleType, TypedDictType, TypeOfAny, get_proper_type
 from mypy.types import Type as MypyType
-from mypy.types import TypedDictType, TypeOfAny, get_proper_type
 
 from mypy_django_plugin.django.context import DjangoContext, LookupsAreUnsupported
 from mypy_django_plugin.lib import fullnames, helpers
 from mypy_django_plugin.lib.fullnames import ANY_ATTR_ALLOWED_CLASS_FULLNAME
 from mypy_django_plugin.lib.helpers import is_annotated_model_fullname
 from mypy_django_plugin.transformers.models import get_or_create_annotated_type
 
@@ -60,16 +59,14 @@
 
     if lookup_field is None:
         return AnyType(TypeOfAny.implementation_artifact)
     elif (isinstance(lookup_field, RelatedField) and lookup_field.column == lookup) or isinstance(
         lookup_field, ForeignObjectRel
     ):
         related_model_cls = django_context.get_field_related_model_cls(lookup_field)
-        if related_model_cls is None:
-            return AnyType(TypeOfAny.from_error)
         lookup_field = django_context.get_primary_key_field(related_model_cls)
 
     field_get_type = django_context.get_field_get_type(helpers.get_typechecker_api(ctx), lookup_field, method=method)
     return field_get_type
 
 
 def get_values_list_row_type(
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/request.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from mypy.plugin import AttributeContext, MethodContext
-from mypy.types import Instance
+from mypy.types import Instance, UninhabitedType, UnionType
 from mypy.types import Type as MypyType
-from mypy.types import UninhabitedType, UnionType
 
 from mypy_django_plugin.django.context import DjangoContext
 from mypy_django_plugin.lib import helpers
 
 
 def set_auth_user_model_as_type_for_request_user(ctx: AttributeContext, django_context: DjangoContext) -> MypyType:
     if not django_context.apps_registry.is_installed("django.contrib.auth"):
```

### Comparing `django-stubs-4.2.1/mypy_django_plugin/transformers/settings.py` & `django-stubs-4.2.2/mypy_django_plugin/transformers/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from mypy.nodes import MemberExpr
 from mypy.plugin import AttributeContext, FunctionContext
-from mypy.types import AnyType, Instance
+from mypy.types import AnyType, Instance, TypeOfAny, TypeType
 from mypy.types import Type as MypyType
-from mypy.types import TypeOfAny, TypeType
 
+from mypy_django_plugin.config import DjangoPluginConfig
 from mypy_django_plugin.django.context import DjangoContext
 from mypy_django_plugin.lib import helpers
 
 
 def get_user_model_hook(ctx: FunctionContext, django_context: DjangoContext) -> MypyType:
     auth_user_model = django_context.settings.AUTH_USER_MODEL
     model_cls = django_context.apps_registry.get_model(auth_user_model)
@@ -16,15 +16,17 @@
     model_info = helpers.lookup_fully_qualified_typeinfo(helpers.get_typechecker_api(ctx), model_cls_fullname)
     if model_info is None:
         return AnyType(TypeOfAny.unannotated)
 
     return TypeType(Instance(model_info, []))
 
 
-def get_type_of_settings_attribute(ctx: AttributeContext, django_context: DjangoContext) -> MypyType:
+def get_type_of_settings_attribute(
+    ctx: AttributeContext, django_context: DjangoContext, plugin_config: DjangoPluginConfig
+) -> MypyType:
     if not isinstance(ctx.context, MemberExpr):
         return ctx.default_attr_type
 
     setting_name = ctx.context.name
 
     typechecker_api = helpers.get_typechecker_api(ctx)
 
@@ -39,9 +41,16 @@
                     ctx.api.fail(
                         f"Import cycle from Django settings module prevents type inference for {setting_name!r}",
                         ctx.context,
                     )
                     return ctx.default_attr_type
                 return sym.type
 
+    # Now, we want to check if this setting really exist in runtime.
+    # If it does, we just return `Any`, not to raise any false-positives.
+    # But, we cannot reconstruct the exact runtime type.
+    # See https://github.com/typeddjango/django-stubs/pull/1163
+    if not plugin_config.strict_settings and hasattr(django_context.settings, setting_name):
+        return AnyType(TypeOfAny.implementation_artifact)
+
     ctx.api.fail(f"'Settings' object has no attribute {setting_name!r}", ctx.context)
     return ctx.default_attr_type
```

### Comparing `django-stubs-4.2.1/setup.py` & `django-stubs-4.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 
 with open("README.md") as f:
     readme = f.read()
 
 dependencies = [
     "mypy>=1.0.0",
     "django",
-    "django-stubs-ext>=4.2.1",
+    "django-stubs-ext>=4.2.2",
     "tomli; python_version < '3.11'",
     # Types:
     "typing-extensions",
     "types-pytz",
     "types-PyYAML",
 ]
 
+# Keep compatible-mypy major.minor version pinned to what we use in CI (requirements.txt)
 extras_require = {
-    "compatible-mypy": ["mypy>=1.3.0,<1.4"],
+    "compatible-mypy": ["mypy==1.4.*"],
 }
 
 setup(
     name="django-stubs",
-    version="4.2.1",
+    version="4.2.2",
     description="Mypy stubs for Django",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Maksim Kurnikov",
@@ -62,17 +63,14 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
     ],
     project_urls={
         "Release notes": "https://github.com/typeddjango/django-stubs/releases",
     },
```

### Comparing `django-stubs-4.2.1/tests/test_error_handling.py` & `django-stubs-4.2.2/tests/test_error_handling.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 
 from mypy_django_plugin.config import DjangoPluginConfig
 
 TEMPLATE = """
 (config)
 ...
 [mypy.plugins.django-stubs]
-    django_settings_module: str (required)
+django_settings_module = str (required)
+strict_settings = bool (default: true)
 ...
 (django-stubs) mypy: error: {}
 """
 
 TEMPLATE_TOML = """
 (config)
 ...
 [tool.django-stubs]
 django_settings_module = str (required)
+strict_settings = bool (default: true)
 ...
 (django-stubs) mypy: error: {}
 """
 
 
 @contextmanager
 def write_to_file(file_contents: str, suffix: Optional[str] = None) -> Generator[str, None, None]:
@@ -48,14 +50,19 @@
             id="missing-settings-module",
         ),
         pytest.param(
             ["[mypy.plugins.django-stubs]"],
             "missing required 'django_settings_module' config",
             id="no-settings-given",
         ),
+        pytest.param(
+            ["[mypy.plugins.django-stubs]", "django_settings_module = some.module", "strict_settings = bad"],
+            "invalid 'strict_settings': the setting must be a boolean",
+            id="missing-settings-module",
+        ),
     ],
 )
 def test_misconfiguration_handling(capsys: Any, config_file_contents: List[str], message_part: str) -> None:
     """Invalid configuration raises `SystemExit` with a precise error message."""
     contents = "\n".join(config_file_contents).expandtabs(4)
     with write_to_file(contents) as filename:
         with pytest.raises(SystemExit, match="2"):
@@ -109,44 +116,61 @@
             id="missing django_settings_module",
         ),
         pytest.param(
             "tool.django-stubs]",
             "could not load configuration file",
             id="invalid toml",
         ),
+        pytest.param(
+            """
+            [tool.django-stubs]
+            django_settings_module = "some.module"
+            strict_settings = "a"
+            """,
+            "invalid 'strict_settings': the setting must be a boolean",
+            id="invalid strict_settings type",
+        ),
     ],
 )
 def test_toml_misconfiguration_handling(capsys: Any, config_file_contents, message_part) -> None:
     with write_to_file(config_file_contents, suffix=".toml") as filename:
         with pytest.raises(SystemExit, match="2"):
             DjangoPluginConfig(filename)
 
     error_message = "usage: " + TEMPLATE_TOML.format(message_part)
     assert error_message == capsys.readouterr().err
 
 
-def test_correct_toml_configuration() -> None:
+@pytest.mark.parametrize("boolean_value", ["true", "false"])
+def test_correct_toml_configuration(boolean_value: str) -> None:
     config_file_contents = """
     [tool.django-stubs]
     some_other_setting = "setting"
     django_settings_module = "my.module"
-    """
+    strict_settings = {}
+    """.format(
+        boolean_value
+    )
 
     with write_to_file(config_file_contents, suffix=".toml") as filename:
         config = DjangoPluginConfig(filename)
 
     assert config.django_settings_module == "my.module"
+    assert config.strict_settings is (boolean_value == "true")
 
 
-def test_correct_configuration() -> None:
+@pytest.mark.parametrize("boolean_value", ["true", "True", "false", "False"])
+def test_correct_configuration(boolean_value) -> None:
     """Django settings module gets extracted given valid configuration."""
     config_file_contents = "\n".join(
         [
             "[mypy.plugins.django-stubs]",
-            "\tsome_other_setting = setting",
-            "\tdjango_settings_module = my.module",
+            "some_other_setting = setting",
+            "django_settings_module = my.module",
+            f"strict_settings = {boolean_value}",
         ]
-    ).expandtabs(4)
+    )
     with write_to_file(config_file_contents) as filename:
         config = DjangoPluginConfig(filename)
 
     assert config.django_settings_module == "my.module"
+    assert config.strict_settings is (boolean_value.lower() == "true")
```

