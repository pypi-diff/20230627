# Comparing `tmp/flask-rest-jsonapi-next-0.34.5.tar.gz` & `tmp/flask-rest-jsonapi-next-0.34.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-rest-jsonapi-next-0.34.5.tar", last modified: Mon Feb 13 10:55:27 2023, max compression
+gzip compressed data, was "flask-rest-jsonapi-next-0.34.6.tar", last modified: Tue Jun 27 11:33:02 2023, max compression
```

## Comparing `flask-rest-jsonapi-next-0.34.5.tar` & `flask-rest-jsonapi-next-0.34.6.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.127259 flask-rest-jsonapi-next-0.34.5/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      314 2023-02-13 10:54:55.000000 flask-rest-jsonapi-next-0.34.5/.bumpversion.cfg
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      427 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/.readthedocs.yaml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4327 2023-02-13 10:54:55.000000 flask-rest-jsonapi-next-0.34.5/CHANGELOG.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1071 2021-12-28 11:36:30.000000 flask-rest-jsonapi-next-0.34.5/LICENSE
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      254 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4860 2023-02-13 10:55:27.127259 flask-rest-jsonapi-next-0.34.5/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3719 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/README.md
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.119258 flask-rest-jsonapi-next-0.34.5/docs/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     7634 2021-12-28 11:36:30.000000 flask-rest-jsonapi-next-0.34.5/docs/Makefile
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      295 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/api.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1298 2023-02-13 10:54:55.000000 flask-rest-jsonapi-next-0.34.5/docs/conf.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      485 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/configuration.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5591 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/data_layer.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2854 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/errors.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5512 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/features.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5160 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/filtering.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2265 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/flask-rest-jsonapi-next.rst
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.119258 flask-rest-jsonapi-next-0.34.5/docs/img/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    60801 2021-12-28 11:36:30.000000 flask-rest-jsonapi-next-0.34.5/docs/img/schema.png
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4119 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/include_related_objects.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2841 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/index.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      609 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/installation.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4453 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/logical_data_abstraction.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      800 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/make.bat
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      106 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/modules.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2362 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/oauth.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1034 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/pagination.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2783 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/permission.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    25491 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/quickstart.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     6990 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/resource_manager.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      882 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/routing.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      896 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/sorting.rst
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1686 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/docs/sparse_fieldsets.rst
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.123258 flask-rest-jsonapi-next-0.34.5/examples/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     5717 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/examples/api.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     7316 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/examples/api_nested.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.123258 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      376 2023-02-13 10:54:55.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     7840 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/api.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.123258 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/data_layers/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/data_layers/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    32059 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/data_layers/alchemy.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    14136 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/data_layers/base.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.123258 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/data_layers/filtering/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/data_layers/filtering/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     6158 2023-02-13 10:54:45.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2654 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/decorators.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.123258 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      209 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2331 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/error_formatters.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2504 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.123258 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exception_converters/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      290 2023-02-11 07:54:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exception_converters/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2859 2023-02-11 07:54:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exception_converters/base.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      541 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exception_converters/flask_rest_jsonapi.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1448 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     8242 2023-02-11 07:54:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      375 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exception_converters/werkzeug.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      617 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exceptions.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      478 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/errors.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3072 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/exceptions.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1994 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/pagination.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     7678 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/querystring.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    21925 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/resource.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     7386 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/schema.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.123258 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4860 2023-02-13 10:55:27.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2233 2023-02-13 10:55:27.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-02-13 10:55:27.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2022-09-15 06:59:45.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      278 2023-02-13 10:55:27.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       43 2023-02-13 10:55:27.000000 flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next.egg-info/top_level.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2130 2023-02-13 10:54:55.000000 flask-rest-jsonapi-next-0.34.5/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-02-13 10:55:27.127259 flask-rest-jsonapi-next-0.34.5/setup.cfg
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       69 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/setup.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-02-13 10:55:27.127259 flask-rest-jsonapi-next-0.34.5/tests/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        0 2022-03-15 15:14:27.000000 flask-rest-jsonapi-next-0.34.5/tests/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      171 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/tests/conftest.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    69985 2023-02-03 10:30:16.000000 flask-rest-jsonapi-next-0.34.5/tests/test_sqlalchemy_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.482515 flask-rest-jsonapi-next-0.34.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-27 11:33:02.482515 flask-rest-jsonapi-next-0.34.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.478515 flask-rest-jsonapi-next-0.34.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/data_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/filtering.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/flask-rest-jsonapi-next.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.478515 flask-rest-jsonapi-next-0.34.6/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    60801 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/img/schema.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/include_related_objects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/logical_data_abstraction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/pagination.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/permission.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/resource_manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/sorting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/docs/sparse_fieldsets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.478515 flask-rest-jsonapi-next-0.34.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/examples/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/examples/api_nested.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.478515 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.478515 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/data_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/data_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32059 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/data_layers/alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/data_layers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.478515 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/data_layers/filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/data_layers/filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.478515 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/error_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.482515 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/flask_rest_jsonapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/werkzeug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21925 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.478515 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-27 11:33:02.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-27 11:33:02.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:33:02.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:33:02.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-27 11:33:02.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 11:33:02.000000 flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:33:02.482515 flask-rest-jsonapi-next-0.34.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:33:02.482515 flask-rest-jsonapi-next-0.34.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69985 2023-06-27 11:32:52.000000 flask-rest-jsonapi-next-0.34.6/tests/test_sqlalchemy_data_layer.py
```

### Comparing `flask-rest-jsonapi-next-0.34.5/CHANGELOG.md` & `flask-rest-jsonapi-next-0.34.6/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG
 
+## 0.34.6 (fork-0.34.6) (2023-06-27)
+
+- fix: filtering operator `between` was not correctly implemented for SQLAlchemy
+  data layer
+
 ## 0.34.5 (fork-0.34.5) (2023-02-13)
 
 - fix: filtering operator `between` was not correctly implemented for SQLAlchemy
   data layer
 
 ## 0.34.4 (fork-0.34.4) (2023-02-03)
```

### Comparing `flask-rest-jsonapi-next-0.34.5/LICENSE` & `flask-rest-jsonapi-next-0.34.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/PKG-INFO` & `flask-rest-jsonapi-next-0.34.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rest-jsonapi-next
-Version: 0.34.5
+Version: 0.34.6
 Summary: Flask extension to create REST web api according to JSONAPI 1.0 specification with Flask, Marshmallow and data provider of your choice (SQLAlchemy, MongoDB, ...)
 Author: original miLibris/flask-rest-jsonapi contributors
 Maintainer-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-rest-jsonapi-next
 Project-URL: Documentation, https://flask-rest-jsonapi-next.readthedocs.io/en/latest/
 Keywords: web,api,rest,jsonapi,flask,sqlalchemy,marshmallow
```

### Comparing `flask-rest-jsonapi-next-0.34.5/README.md` & `flask-rest-jsonapi-next-0.34.6/README.md`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/Makefile` & `flask-rest-jsonapi-next-0.34.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/conf.py` & `flask-rest-jsonapi-next-0.34.6/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "flask-rest-jsonapi-next"
 copyright = "2016-2021 miLibris; 2021-... miLibris, tadams42"
 author = "tadams42"
-release = "0.34.5"
+release = "0.34.6"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
```

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/data_layer.rst` & `flask-rest-jsonapi-next-0.34.6/docs/data_layer.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/errors.rst` & `flask-rest-jsonapi-next-0.34.6/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/features.rst` & `flask-rest-jsonapi-next-0.34.6/docs/features.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/filtering.rst` & `flask-rest-jsonapi-next-0.34.6/docs/filtering.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/flask-rest-jsonapi-next.rst` & `flask-rest-jsonapi-next-0.34.6/docs/flask-rest-jsonapi-next.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/img/schema.png` & `flask-rest-jsonapi-next-0.34.6/docs/img/schema.png`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/include_related_objects.rst` & `flask-rest-jsonapi-next-0.34.6/docs/include_related_objects.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/index.rst` & `flask-rest-jsonapi-next-0.34.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/installation.rst` & `flask-rest-jsonapi-next-0.34.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/logical_data_abstraction.rst` & `flask-rest-jsonapi-next-0.34.6/docs/logical_data_abstraction.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/make.bat` & `flask-rest-jsonapi-next-0.34.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/oauth.rst` & `flask-rest-jsonapi-next-0.34.6/docs/oauth.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/pagination.rst` & `flask-rest-jsonapi-next-0.34.6/docs/pagination.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/permission.rst` & `flask-rest-jsonapi-next-0.34.6/docs/permission.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/quickstart.rst` & `flask-rest-jsonapi-next-0.34.6/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/resource_manager.rst` & `flask-rest-jsonapi-next-0.34.6/docs/resource_manager.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/routing.rst` & `flask-rest-jsonapi-next-0.34.6/docs/routing.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/sorting.rst` & `flask-rest-jsonapi-next-0.34.6/docs/sorting.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/docs/sparse_fieldsets.rst` & `flask-rest-jsonapi-next-0.34.6/docs/sparse_fieldsets.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/examples/api.py` & `flask-rest-jsonapi-next-0.34.6/examples/api.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/examples/api_nested.py` & `flask-rest-jsonapi-next-0.34.6/examples/api_nested.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/api.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/api.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/data_layers/alchemy.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/data_layers/alchemy.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/data_layers/base.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/data_layers/base.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/decorators.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/error_formatters.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/error_formatters.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exception_converters/base.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,22 @@
 import abc
 from typing import List, Union
 
 import flask
-import sqlalchemy
-
-CONVERTERS_REGISTRY = set()
-
-
-class ConvertersRegistry:
-    @classmethod
-    def register(cls, klass):
-        CONVERTERS_REGISTRY.add(klass)
-
-    @classmethod
-    def get_converted_data(cls, err):
-        from .sqlalchemy import GenericSQLAlchemyErrorConverter
-
-        data = None
-
-        for klass in CONVERTERS_REGISTRY:
-            try:
-                data = klass.convert(err)
-            except ValueError:
-                pass
-
-            if data:
-                break
-
-        if not data:
-            try:
-                data = GenericSQLAlchemyErrorConverter.convert(err)
-            except ValueError:
-                pass
-
-        if not data:
-            data = GenericErrorConverter.convert(err)
-
-        return data
 
 
 class ExceptionConverter(abc.ABC):
     @abc.abstractclassmethod
     def convert(cls, exc: Exception) -> Union[List[dict], dict]:
         raise NotImplementedError()
 
     @classmethod
     def register(cls):
+        from .registry import ConvertersRegistry
+
         ConvertersRegistry.register(cls)
 
 
 class GenericErrorConverter(ExceptionConverter):
     @classmethod
     def convert(cls, exc):
         title = type(exc).__name__
@@ -62,15 +29,15 @@
         if not detail:
             if flask.current_app.debug:
                 detail = str(exc)
             else:
                 detail = """
                     ************************** Congratulations!!!! **************************
                     You have just discovered new, unknown species of backend bug! Play
-                    it nice and report the issue (together with complete contenets of
+                    it nice and report the issue (together with complete contents of
                     this error response) to backend maintainers."
                 """
 
         meta = {}
         if hasattr(exc, "payload") and exc.payload:
             meta = {"payload": exc.payload}
         elif hasattr(exc, "response") and exc.response:
```

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,11 +41,7 @@
 
         return dict(
             title="IncorrectTypeError",
             detail=exc.detail,
             source={"pointer": exc.pointer},
             http_status=requests.codes["conflict"],
         )
-
-
-MarshmallowJsonapiIncorrectTypeErrorConverter.register()
-MarshmallowValidationErrorConverter.register()
```

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,69 +27,59 @@
                 "for typos and virtual attributes."
             ),
             http_status=requests.codes["unprocessable"],
             meta={"sql_exception": str(exc)} if flask.current_app.debug else None,
         )
 
 
-ArgumentErrorConverter.register()
-
-
 class NoResultFoundConverter(ExceptionConverter):
     @classmethod
     def convert(cls, exc):
         if not isinstance(exc, orm.exc.NoResultFound):
             raise ValueError()
 
         return dict(
             title="SQLNoResultFound",
             detail="Object not found!",
             http_status=requests.codes["not_found"],
             meta={"sql_exception": str(exc)} if flask.current_app.debug else None,
         )
 
 
-NoResultFoundConverter.register()
-
-
 class MultipleResultsFoundConverter(ExceptionConverter):
     @classmethod
     def convert(cls, exc):
         if not isinstance(exc, orm.exc.MultipleResultsFound):
             raise ValueError()
 
         return dict(
             title="SQLMulitpleResultsFound",
             detail="Query was supposed to return one, but many found!",
             http_status=requests.codes["unprocessable"],
             meta={"sql_exception": str(exc)} if flask.current_app.debug else None,
         )
 
 
-MultipleResultsFoundConverter.register()
-
-
-class UniqueViolationConverter(ExceptionConverter):
-    @classmethod
-    def convert(cls, exc):
-        if not isinstance(exc, psycopg2.errors.UniqueViolation):
-            raise ValueError()
-
-        return dict(
-            title="SQLUniqueViolation",
-            detail=(
-                "Unique constraint violated! "
-                + (getattr(getattr(exc, "diag", None), "message_detail", ""))
-            ),
-            http_status=requests.codes["conflict"],
-            meta={"psql_exception": str(exc)} if flask.current_app.debug else None,
-        )
+if _HAS_PSYCOPG2:
+    class UniqueViolationConverter(ExceptionConverter):
+        @classmethod
+        def convert(cls, exc):
+            if not isinstance(exc, psycopg2.errors.UniqueViolation):
+                raise ValueError()
 
+            return dict(
+                title="SQLUniqueViolation",
+                detail=(
+                    "Unique constraint violated! "
+                    + (getattr(getattr(exc, "diag", None), "message_detail", ""))
+                ),
+                http_status=requests.codes["conflict"],
+                meta={"psql_exception": str(exc)} if flask.current_app.debug else None,
+            )
 
-if _HAS_PSYCOPG2:
 
     class CheckViolationConverter(ExceptionConverter):
         @classmethod
         def convert(cls, exc):
             if not isinstance(exc, psycopg2.errors.CheckViolation):
                 raise ValueError()
 
@@ -101,15 +91,14 @@
                     "psql_exception": str(exc),
                     "psql_diag": f"{getattr(getattr(exc, 'diag', None), 'constraint_name', '')}",
                 }
                 if flask.current_app.debug
                 else None,
             )
 
-    CheckViolationConverter.register()
 
     class ForeignKeyViolationConverter(ExceptionConverter):
         @classmethod
         def convert(cls, exc):
             if not isinstance(exc, psycopg2.errors.ForeignKeyViolation):
                 raise ValueError()
 
@@ -125,15 +114,14 @@
                     "psql_exception": str(exc),
                     "psql_diag": f"{getattr(getattr(exc, 'diag', None), 'constraint_name', '')}",
                 }
                 if flask.current_app.debug
                 else None,
             )
 
-    CheckViolationConverter.register()
 
     class NotNullViolationConverter(ExceptionConverter):
         @classmethod
         def convert(cls, exc):
             if not isinstance(exc, psycopg2.errors.NotNullViolation):
                 raise ValueError()
 
@@ -154,15 +142,14 @@
                     "psql_exception": str(exc),
                     "psql_diag": f" [{getattr(getattr(exc, 'diag', None), 'message_primary', '')}]",
                 }
                 if flask.current_app.debug
                 else None,
             )
 
-    NotNullViolationConverter.register()
 
     class IntegrityErrorConverter(ExceptionConverter):
         @classmethod
         def convert(cls, exc):
             if not isinstance(exc, sqlalchemy.exc.IntegrityError):
                 raise ValueError()
 
@@ -185,16 +172,14 @@
 
             if flask.current_app.debug:
                 retv["meta"] = retv.get("meta", dict())
                 retv["meta"]["exc"] = str(exc)
 
             return retv
 
-    IntegrityErrorConverter.register()
-
 
 class InvalidRequestErrorConverter(ExceptionConverter):
     @classmethod
     def convert(cls, exc):
         if not isinstance(exc, sqlalchemy.exc.InvalidRequestError):
             raise ValueError()
 
@@ -205,17 +190,14 @@
                 http_status=requests.codes["unprocessable"],
                 source={"parameter": "filter"},
             )
 
         raise ValueError()
 
 
-InvalidRequestErrorConverter.register()
-
-
 class DataErrorConverter(ExceptionConverter):
     @classmethod
     def convert(cls, exc):
         if not isinstance(exc, sqlalchemy.exc.DataError):
             raise ValueError()
 
         if hasattr(exc, "orig"):
@@ -237,15 +219,33 @@
                 http_status=requests.codes["unprocessable"],
                 source={"pointer": "body"},
             )
 
         raise ValueError()
 
 
-DataErrorConverter.register()
+class SQLStatementErrorConverter(ExceptionConverter):
+    @classmethod
+    def convert(cls, exc):
+        if not isinstance(exc, sqlalchemy.exc.StatementError):
+            raise ValueError()
+
+        detail = ""
+
+        if hasattr(exc, "orig"):
+            detail = ";".join(exc.orig.args)
+        else:
+            detail = ";".join(exc.args)
+
+        return dict(
+            title="SQLStatementError",
+            detail=detail,
+            http_status=requests.codes["unprocessable"],
+            source={"pointer": "filter"},
+        )
 
 
 class GenericSQLAlchemyErrorConverter(ExceptionConverter):
     @classmethod
     def convert(cls, exc):
         if not isinstance(exc, sqlalchemy.exc.SQLAlchemyError):
             raise ValueError()
```

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/error_responses/exceptions.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/error_responses/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/exceptions.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/pagination.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/pagination.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/querystring.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/querystring.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/resource.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/resource.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next/schema.py` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next/schema.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next.egg-info/PKG-INFO` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rest-jsonapi-next
-Version: 0.34.5
+Version: 0.34.6
 Summary: Flask extension to create REST web api according to JSONAPI 1.0 specification with Flask, Marshmallow and data provider of your choice (SQLAlchemy, MongoDB, ...)
 Author: original miLibris/flask-rest-jsonapi contributors
 Maintainer-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-rest-jsonapi-next
 Project-URL: Documentation, https://flask-rest-jsonapi-next.readthedocs.io/en/latest/
 Keywords: web,api,rest,jsonapi,flask,sqlalchemy,marshmallow
```

### Comparing `flask-rest-jsonapi-next-0.34.5/flask_rest_jsonapi_next.egg-info/SOURCES.txt` & `flask-rest-jsonapi-next-0.34.6/flask_rest_jsonapi_next.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,12 +56,13 @@
 flask_rest_jsonapi_next/error_responses/error_formatters.py
 flask_rest_jsonapi_next/error_responses/errors_as_json_api.py
 flask_rest_jsonapi_next/error_responses/exceptions.py
 flask_rest_jsonapi_next/error_responses/exception_converters/__init__.py
 flask_rest_jsonapi_next/error_responses/exception_converters/base.py
 flask_rest_jsonapi_next/error_responses/exception_converters/flask_rest_jsonapi.py
 flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py
+flask_rest_jsonapi_next/error_responses/exception_converters/registry.py
 flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py
 flask_rest_jsonapi_next/error_responses/exception_converters/werkzeug.py
 tests/__init__.py
 tests/conftest.py
 tests/test_sqlalchemy_data_layer.py
```

### Comparing `flask-rest-jsonapi-next-0.34.5/pyproject.toml` & `flask-rest-jsonapi-next-0.34.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # setuptools v64 was first to support `pip install -e` for packages defined using
 # pyproject.toml (older versions support this, but only for setup.py projects)
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flask-rest-jsonapi-next"
-version = "0.34.5"
+version = "0.34.6"
 description = "Flask extension to create REST web api according to JSONAPI 1.0 specification with Flask, Marshmallow and data provider of your choice (SQLAlchemy, MongoDB, ...)"
 readme = "README.md"
 classifiers = [
 	"Framework :: Flask",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
@@ -55,15 +55,15 @@
 	"furo",
 	"ipython",
 	"isort",
 	"myst-parser",
 	"pytest",
 	"sphinx-copybutton",
 	"sphinx",
-	"twine",
+	"psycopg2-binary",
 ]
 docs = ["furo", "myst-parser", "sphinx", "sphinx-copybutton"]
 tests = ["check-manifest", "pytest", "coverage"]
 
 
 [tool.setuptools]
 zip-safe = false
```

### Comparing `flask-rest-jsonapi-next-0.34.5/tests/test_sqlalchemy_data_layer.py` & `flask-rest-jsonapi-next-0.34.6/tests/test_sqlalchemy_data_layer.py`

 * *Files identical despite different names*

