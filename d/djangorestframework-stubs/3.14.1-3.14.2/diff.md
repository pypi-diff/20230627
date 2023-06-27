# Comparing `tmp/djangorestframework-stubs-3.14.1.tar.gz` & `tmp/djangorestframework-stubs-3.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-stubs-3.14.1.tar", last modified: Fri Jun  2 14:19:49 2023, max compression
+gzip compressed data, was "djangorestframework-stubs-3.14.2.tar", last modified: Tue Jun 27 17:54:14 2023, max compression
```

## Comparing `djangorestframework-stubs-3.14.1.tar` & `djangorestframework-stubs-3.14.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:49.000298 djangorestframework-stubs-3.14.1/
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/LICENSE.txt
--rw-r--r--   0 marti     (1000) marti      (121)     2444 2023-06-02 14:19:49.000298 djangorestframework-stubs-3.14.1/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)     1495 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.986965 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)     2444 2023-06-02 14:19:48.000000 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)     3237 2023-06-02 14:19:48.000000 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-02 14:19:48.000000 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)      213 2023-06-02 14:19:48.000000 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       37 2023-06-02 14:19:48.000000 djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.986965 djangorestframework-stubs-3.14.1/mypy_drf_plugin/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/__init__.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.986965 djangorestframework-stubs-3.14.1/mypy_drf_plugin/lib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/lib/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     2714 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/lib/fullnames.py
--rw-r--r--   0 marti     (1000) marti      (121)      167 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/lib/helpers.py
--rw-r--r--   0 marti     (1000) marti      (121)     1880 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/main.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.986965 djangorestframework-stubs-3.14.1/mypy_drf_plugin/transformers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/transformers/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)      355 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/mypy_drf_plugin/transformers/serializers.py
--rw-r--r--   0 marti     (1000) marti      (121)      207 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/pyproject.toml
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.993631 djangorestframework-stubs-3.14.1/rest_framework-stubs/
--rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       77 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1115 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authentication.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/
--rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       74 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       73 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      394 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/management/commands/drf_create_token.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/serializers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/authtoken/views.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1985 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/compat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3273 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1560 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/documentation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3052 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    23541 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2002 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/filters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4415 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/generics.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      384 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/management/commands/generateschema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      726 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/metadata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1260 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/negotiation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4964 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/pagination.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1794 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/parsers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3062 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/permissions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6983 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/relations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4382 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/renderers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3202 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/request.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1128 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/response.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      671 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/reverse.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/routers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/
--rw-r--r--   0 marti     (1000) marti      (121)      973 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2794 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/coreapi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2044 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/generators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      528 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/inspectors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3250 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/openapi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      261 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/views.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    12294 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/serializers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4150 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/settings.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2642 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/status.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:48.996965 djangorestframework-stubs-3.14.1/rest_framework-stubs/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1658 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/templatetags/rest_framework.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5592 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/test.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1126 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/throttling.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      565 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/urlpatterns.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       89 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/urls.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:19:49.000298 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/breadcrumbs.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       54 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/encoders.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/field_mapping.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      404 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/formatting.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      183 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/humanize_datetime.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/mediatypes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      703 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/model_meta.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/representation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1774 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/serializer_helpers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      145 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1169 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/versioning.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4716 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/views.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1792 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.1/rest_framework-stubs/viewsets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      434 2023-06-02 14:19:49.000298 djangorestframework-stubs-3.14.1/setup.cfg
--rw-r--r--   0 marti     (1000) marti      (121)     2041 2023-06-02 14:19:36.000000 djangorestframework-stubs-3.14.1/setup.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.252280 djangorestframework-stubs-3.14.2/
+-rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/LICENSE.txt
+-rw-r--r--   0 marti     (1000) marti      (121)     2444 2023-06-27 17:54:14.252280 djangorestframework-stubs-3.14.2/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)     1495 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.2/README.md
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.235613 djangorestframework-stubs-3.14.2/djangorestframework_stubs.egg-info/
+-rw-r--r--   0 marti     (1000) marti      (121)     2444 2023-06-27 17:54:14.000000 djangorestframework-stubs-3.14.2/djangorestframework_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)     3237 2023-06-27 17:54:14.000000 djangorestframework-stubs-3.14.2/djangorestframework_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-27 17:54:14.000000 djangorestframework-stubs-3.14.2/djangorestframework_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti      (121)      208 2023-06-27 17:54:14.000000 djangorestframework-stubs-3.14.2/djangorestframework_stubs.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       37 2023-06-27 17:54:14.000000 djangorestframework-stubs-3.14.2/djangorestframework_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.235613 djangorestframework-stubs-3.14.2/mypy_drf_plugin/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/mypy_drf_plugin/__init__.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.235613 djangorestframework-stubs-3.14.2/mypy_drf_plugin/lib/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/mypy_drf_plugin/lib/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2714 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/mypy_drf_plugin/lib/fullnames.py
+-rw-r--r--   0 marti     (1000) marti      (121)      167 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/mypy_drf_plugin/lib/helpers.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1480 2023-06-27 17:53:54.000000 djangorestframework-stubs-3.14.2/mypy_drf_plugin/main.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.238947 djangorestframework-stubs-3.14.2/mypy_drf_plugin/transformers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/mypy_drf_plugin/transformers/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)      355 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/mypy_drf_plugin/transformers/serializers.py
+-rw-r--r--   0 marti     (1000) marti      (121)      429 2023-06-27 17:53:54.000000 djangorestframework-stubs-3.14.2/pyproject.toml
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.245613 djangorestframework-stubs-3.14.2/rest_framework-stubs/
+-rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       77 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1115 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/authentication.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.245613 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/
+-rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       74 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       73 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.245613 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.245613 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      394 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/management/commands/drf_create_token.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/authtoken/views.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1985 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/compat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3273 2023-06-27 17:53:54.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1560 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/documentation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3065 2023-06-27 17:53:54.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    23541 2023-06-27 17:53:54.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2002 2023-04-27 14:17:42.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/filters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4415 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/generics.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.245613 djangorestframework-stubs-3.14.2/rest_framework-stubs/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.245613 djangorestframework-stubs-3.14.2/rest_framework-stubs/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      384 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/management/commands/generateschema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      726 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/metadata.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1260 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/negotiation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4964 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/pagination.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1794 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/parsers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3062 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/permissions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6983 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/relations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4382 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/renderers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3202 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/request.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1128 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/response.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      671 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/reverse.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/routers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.248947 djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/
+-rw-r--r--   0 marti     (1000) marti      (121)      973 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2794 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/coreapi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2044 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/generators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      528 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/inspectors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3250 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/openapi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      261 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/views.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    12006 2023-06-27 17:53:54.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4150 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/settings.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2631 2023-06-27 17:53:54.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/status.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.248947 djangorestframework-stubs-3.14.2/rest_framework-stubs/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1658 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/templatetags/rest_framework.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5592 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/test.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1126 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/throttling.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      565 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/urlpatterns.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       89 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/urls.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-27 17:54:14.248947 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/breadcrumbs.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       54 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/encoders.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/field_mapping.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      404 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/formatting.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/html.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      183 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/humanize_datetime.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/json.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/mediatypes.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      703 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/model_meta.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/representation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1774 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/serializer_helpers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      145 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/validators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1169 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/versioning.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4716 2023-03-15 16:53:40.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/views.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1792 2023-06-02 14:08:55.000000 djangorestframework-stubs-3.14.2/rest_framework-stubs/viewsets.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      434 2023-06-27 17:54:14.252280 djangorestframework-stubs-3.14.2/setup.cfg
+-rw-r--r--   0 marti     (1000) marti      (121)     2126 2023-06-27 17:53:54.000000 djangorestframework-stubs-3.14.2/setup.py
```

### Comparing `djangorestframework-stubs-3.14.1/LICENSE.txt` & `djangorestframework-stubs-3.14.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/PKG-INFO` & `djangorestframework-stubs-3.14.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-stubs
-Version: 3.14.1
+Version: 3.14.2
 Summary: PEP-484 stubs for django-rest-framework
 Home-page: https://github.com/typeddjango/djangorestframework-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
```

### Comparing `djangorestframework-stubs-3.14.1/README.md` & `djangorestframework-stubs-3.14.2/README.md`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/PKG-INFO` & `djangorestframework-stubs-3.14.2/djangorestframework_stubs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-stubs
-Version: 3.14.1
+Version: 3.14.2
 Summary: PEP-484 stubs for django-rest-framework
 Home-page: https://github.com/typeddjango/djangorestframework-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
```

### Comparing `djangorestframework-stubs-3.14.1/djangorestframework_stubs.egg-info/SOURCES.txt` & `djangorestframework-stubs-3.14.2/djangorestframework_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/mypy_drf_plugin/lib/fullnames.py` & `djangorestframework-stubs-3.14.2/mypy_drf_plugin/lib/fullnames.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/authentication.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/authentication.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/compat.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/decorators.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/decorators.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from collections.abc import Callable, Mapping, Sequence
-from typing import Any, Protocol, TypeVar
+from typing import Any, Literal, Protocol, TypeVar
 
 from django.http import HttpRequest
 from django.http.response import HttpResponseBase
 from rest_framework.authentication import BaseAuthentication
 from rest_framework.parsers import BaseParser
 from rest_framework.permissions import _PermissionClass
 from rest_framework.renderers import BaseRenderer
 from rest_framework.request import Request
 from rest_framework.schemas.inspectors import ViewInspector
 from rest_framework.throttling import BaseThrottle
 from rest_framework.views import APIView, AsView  # noqa: F401
-from typing_extensions import Concatenate, Literal, ParamSpec, TypeAlias
+from typing_extensions import Concatenate, ParamSpec, TypeAlias
 
 _View = TypeVar("_View", bound=Callable[..., HttpResponseBase])
 _P = ParamSpec("_P")
 _RESP = TypeVar("_RESP", bound=HttpResponseBase)
 
 class MethodMapper(dict):
     def __init__(self, action: _View, methods: Sequence[str]) -> None: ...
```

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/documentation.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/documentation.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/exceptions.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/exceptions.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 from rest_framework.request import Request
 from typing_extensions import TypeAlias, TypedDict
 
 class ErrorDetail(str):
     code: str | None
     def __new__(cls, string: str, code: str | None = ...): ...
 
-_Detail: TypeAlias = ErrorDetail | list[ErrorDetail] | dict[str, ErrorDetail]
+_Detail: TypeAlias = ErrorDetail | list[_Detail] | dict[str, _Detail]
 # NB! _APIExceptionInput doesn't technically handle Sequence/Mapping, but only list/tuple/dict.
 # But since list/tuple are non-covariant types, we run into issues with union type compatibility for input params.
 # So use the more relaxed Sequence/Mapping for now.
 _APIExceptionInput: TypeAlias = (
     _Detail | StrOrPromise | Sequence[_APIExceptionInput] | Mapping[str, _APIExceptionInput] | None
 )
 _ErrorCodes: TypeAlias = str | None | list[_ErrorCodes] | dict[str, _ErrorCodes]
 
 class _FullDetailDict(TypedDict):
     message: ErrorDetail
     code: str | None
 
-_ErrorFullDetails: TypeAlias = _FullDetailDict | list[_FullDetailDict] | dict[str, _FullDetailDict]
+_ErrorFullDetails: TypeAlias = _FullDetailDict | list[_ErrorFullDetails] | dict[str, _ErrorFullDetails]
 
 def _get_error_details(data: _APIExceptionInput, default_code: str | None = ...) -> _Detail: ...
 def _get_codes(detail: _Detail) -> _ErrorCodes: ...
 def _get_full_details(detail: _Detail) -> _ErrorFullDetails: ...
 
 class APIException(Exception):
     status_code: int
@@ -37,16 +37,16 @@
 
     detail: _Detail
     def __init__(self, detail: _APIExceptionInput = ..., code: str | None = ...) -> None: ...
     def get_codes(self) -> _ErrorCodes: ...
     def get_full_details(self) -> _ErrorFullDetails: ...
 
 class ValidationError(APIException):
-    # ValidationError always wraps `detail` in a list.
-    detail: list[ErrorDetail] | dict[str, ErrorDetail]
+    # ValidationError wraps `detail` in a list if it's not already a list/dict.
+    detail: list[_Detail] | dict[str, _Detail]
 
 class ParseError(APIException): ...
 class AuthenticationFailed(APIException): ...
 class NotAuthenticated(APIException): ...
 class PermissionDenied(APIException): ...
 class NotFound(APIException): ...
```

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/fields.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/fields.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
 import uuid
 from collections.abc import Callable, Generator, Iterable, Mapping, MutableMapping, Sequence
 from decimal import Decimal
 from enum import Enum
 from json import JSONDecoder, JSONEncoder
 from re import Pattern
-from typing import Any, Generic, NoReturn, Protocol, TypeVar
+from typing import Any, Final, Generic, NoReturn, Protocol, TypeVar
 
 from _typeshed import Self
 from django.core.files.base import File
 from django.db import models
 from django.forms import ImageField as DjangoImageField  # noqa: F401
 from django_stubs_ext import StrOrPromise
 from rest_framework.serializers import BaseSerializer
 from rest_framework.validators import Validator
-from typing_extensions import Final, TypeAlias
+from typing_extensions import TypeAlias
 
 class _Empty(Enum):
     sentinel = 0  # noqa: Y015
 
 empty: Final = _Empty.sentinel
 
 class BuiltinSignatureError(Exception): ...
```

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/filters.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/filters.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/generics.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/generics.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/metadata.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/metadata.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/mixins.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/mixins.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/negotiation.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/negotiation.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/pagination.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/pagination.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/parsers.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/permissions.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/permissions.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/relations.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/relations.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/renderers.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/renderers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/request.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/request.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/response.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/reverse.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/reverse.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/routers.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/routers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/__init__.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/coreapi.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/coreapi.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/generators.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/generators.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/inspectors.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/inspectors.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/schemas/openapi.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/schemas/openapi.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/serializers.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/serializers.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from collections.abc import Callable, Iterable, Iterator, Mapping, MutableMapping, Sequence
-from typing import Any, Generic, NoReturn, TypeVar
+from typing import Any, Generic, Literal, NoReturn, TypeVar
 
 from _typeshed import Self
-from django.core.exceptions import ValidationError as DjangoValidationError
 from django.db import models
-from django.db.models import DurationField as ModelDurationField
 from django.db.models import Manager, Model, QuerySet
-from django.db.models.fields import Field as DjangoModelField
 from django.utils.functional import cached_property
-from django.utils.translation import ugettext_lazy as _
 from django_stubs_ext import StrOrPromise
 from rest_framework.exceptions import APIException as APIException
 from rest_framework.exceptions import AuthenticationFailed as AuthenticationFailed
 from rest_framework.exceptions import ErrorDetail as ErrorDetail
 from rest_framework.exceptions import MethodNotAllowed as MethodNotAllowed
 from rest_framework.exceptions import NotAcceptable as NotAcceptable
 from rest_framework.exceptions import NotAuthenticated as NotAuthenticated
@@ -63,15 +59,14 @@
 from rest_framework.relations import PrimaryKeyRelatedField as PrimaryKeyRelatedField
 from rest_framework.relations import RelatedField as RelatedField
 from rest_framework.relations import SlugRelatedField as SlugRelatedField
 from rest_framework.relations import StringRelatedField as StringRelatedField
 from rest_framework.utils.model_meta import FieldInfo, RelationInfo
 from rest_framework.utils.serializer_helpers import BindingDict, BoundField, ReturnDict, ReturnList
 from rest_framework.validators import BaseUniqueForValidator, UniqueTogetherValidator, Validator
-from typing_extensions import Literal
 
 LIST_SERIALIZER_KWARGS: Sequence[str]
 ALL_FIELDS: str
 
 _MT = TypeVar("_MT", bound=Model)  # Model Type
 _IN = TypeVar("_IN")  # Instance Type
```

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/settings.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/settings.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/status.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/status.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing_extensions import Literal
+from typing import Literal
 
 def is_informational(code: int) -> bool: ...
 def is_success(code: int) -> bool: ...
 def is_redirect(code: int) -> bool: ...
 def is_client_error(code: int) -> bool: ...
 def is_server_error(code: int) -> bool: ...
```

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/templatetags/rest_framework.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/templatetags/rest_framework.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/test.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/test.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/throttling.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/throttling.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/urlpatterns.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/urlpatterns.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/field_mapping.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/field_mapping.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/model_meta.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/model_meta.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/utils/serializer_helpers.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/utils/serializer_helpers.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/validators.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/validators.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/versioning.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/versioning.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/views.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/views.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/rest_framework-stubs/viewsets.pyi` & `djangorestframework-stubs-3.14.2/rest_framework-stubs/viewsets.pyi`

 * *Files identical despite different names*

### Comparing `djangorestframework-stubs-3.14.1/setup.py` & `djangorestframework-stubs-3.14.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,30 +17,31 @@
 
 
 with open("README.md") as f:
     readme = f.read()
 
 dependencies = [
     "mypy>=0.991",
-    "django-stubs>=4.2.1",
+    "django-stubs>=4.2.2",
     "typing-extensions>=3.10.0",
     "requests>=2.0.0",
     "types-requests>=0.1.12",
     "types-PyYAML>=5.4.3",
 ]
 
+# Keep compatible-mypy major.minor version pinned to what we use in CI (requirements.txt)
 extras_require = {
-    "compatible-mypy": ["mypy>=1.3.0,<1.4"],
+    "compatible-mypy": ["mypy==1.4.*"],
     "coreapi": ["coreapi>=2.0.0"],
     "markdown": ["types-Markdown>=0.1.5"],
 }
 
 setup(
     name="djangorestframework-stubs",
-    version="3.14.1",
+    version="3.14.2",
     description="PEP-484 stubs for django-rest-framework",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/typeddjango/djangorestframework-stubs",
     author="Maksim Kurnikov",
     author_email="maxim.kurnikov@gmail.com",
     maintainer="Marti Raudsepp",
```

