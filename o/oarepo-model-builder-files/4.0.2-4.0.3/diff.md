# Comparing `tmp/oarepo-model-builder-files-4.0.2.tar.gz` & `tmp/oarepo-model-builder-files-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-files-4.0.2.tar", last modified: Mon Jun 12 08:05:29 2023, max compression
+gzip compressed data, was "oarepo-model-builder-files-4.0.3.tar", last modified: Tue Jun 27 09:01:25 2023, max compression
```

## Comparing `oarepo-model-builder-files-4.0.2.tar` & `oarepo-model-builder-files-4.0.3.tar`

### file list

```diff
@@ -1,62 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.712492 oarepo-model-builder-files-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-12 08:05:29.712492 oarepo-model-builder-files-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.704492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.708492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.708492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/invenio_files_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/invenio_files_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/invenio_files_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/invenio_files_record_service_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.708492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_service_config.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.708492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio_parent/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio_parent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.708492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio_parent/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/parent_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.708492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/invenio_files_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/invenio_files_conftest_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.708492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.708492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builtin_models/invenio_files.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.708492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.712492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/datatypes/components/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/datatypes/components/parent_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/datatypes/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.712492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/profiles/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:05:29.708492 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-12 08:05:29.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-12 08:05:29.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:05:29.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-12 08:05:29.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 08:05:29.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 08:05:29.000000 oarepo-model-builder-files-4.0.2/oarepo_model_builder_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-12 08:05:29.712492 oarepo-model-builder-files-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:01:28.000000 oarepo-model-builder-files-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/invenio_files_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/invenio_files_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/invenio_files_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/invenio_files_record_service_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_service_config.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/parent_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/invenio_files_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/invenio_files_conftest_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builtin_models/invenio_files.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/ext_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/files_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/profiles/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/setup.py
```

### Comparing `oarepo-model-builder-files-4.0.2/PKG-INFO` & `oarepo-model-builder-files-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 4.0.2
+Version: 4.0.3
 Description-Content-Type: text/markdown
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
```

### Comparing `oarepo-model-builder-files-4.0.2/README.md` & `oarepo-model-builder-files-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/__init__.py` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2`

 * *Files 8% similar despite different names*

```diff
@@ -10,111 +10,111 @@
 
 def test_files_api_flow(client_with_credentials, search_clear, headers, input_data):
     """Test record creation."""
     # Initialize a draft
     res = client_with_credentials.post("{{ parent_record.resource_config.base_url }}", headers=headers, json=input_data)
     assert res.status_code == 201
     id_ = res.json["id"]
-    assert res.json["links"]["files"].endswith(f"{id_}/files")
+    assert res.json["links"]["files"].endswith(f"{id_}{{ test_constants.read_url }}/files")
 
     # Initialize files upload
     res = client_with_credentials.post(
-        f"{{ parent_record.resource_config.base_url }}{id_}/files", # todo - this won't work if the url is specified differently
+        f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files",
         headers=headers,
         json=[
             {"key": "test.pdf", "title": "Test file"},
         ],
     )
     assert res.status_code == 201
     res_file = res.json["entries"][0]
     assert res_file["key"] == "test.pdf"
     assert res_file["status"] == "pending"
     assert res_file["metadata"] == {"title": "Test file"}
-    assert res_file["links"]["self"].endswith(f"{id_}/files/test.pdf")
+    assert res_file["links"]["self"].endswith(f"{id_}{{ test_constants.read_url }}/files/test.pdf")
     assert res_file["links"]["content"].endswith(
-        f"files/test.pdf/content"
+        f"{{ test_constants.read_url }}/files/test.pdf/content"
     )
     assert res_file["links"]["commit"].endswith(
-        f"files/test.pdf/commit"
+        f"{{ test_constants.read_url }}/files/test.pdf/commit"
     )
 
     # Get the file metadata
-    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}/files/test.pdf", headers=headers)
+    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files/test.pdf", headers=headers)
     assert res.status_code == 200
     assert res.json["key"] == "test.pdf"
     assert res.json["status"] == "pending"
     assert res.json["metadata"] == {"title": "Test file"}
 
     # Upload a file
     res = client_with_credentials.put(
-        f"{{ parent_record.resource_config.base_url }}{id_}/files/test.pdf/content",
+        f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}/files/test.pdf/content",
         headers={
             "content-type": "application/octet-stream",
             "accept": "application/json",
         },
         data=BytesIO(b"testfile"),
     )
     assert res.status_code == 200
     assert res.json["status"] == "pending"
 
     # Commit the uploaded file
-    res = client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}/files/test.pdf/commit", headers=headers)
+    res = client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files/test.pdf/commit", headers=headers)
     assert res.status_code == 200
     assert res.json["status"] == "completed"
 
     # Get the file metadata
-    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}/files/test.pdf", headers=headers)
+    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files/test.pdf", headers=headers)
     assert res.status_code == 200
     assert res.json["key"] == "test.pdf"
     assert res.json["status"] == "completed"
     assert res.json["metadata"] == {"title": "Test file"}
     file_size = str(res.json["size"])
     assert isinstance(res.json["size"], int), "File size not integer"
 
     # Read a file's content
-    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}/files/test.pdf/content", headers=headers)
+    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files/test.pdf/content", headers=headers)
     assert res.status_code == 200
     assert res.data == b"testfile"
 
     # Update file metadata
     res = client_with_credentials.put(
-        f"{{ parent_record.resource_config.base_url }}{id_}/files/test.pdf", headers=headers, json={"title": "New title"}
+        f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}/files/test.pdf", headers=headers, json={"title": "New title"}
     )
     assert res.status_code == 200
     assert res.json["key"] == "test.pdf"
     assert res.json["status"] == "completed"
     assert res.json["metadata"] == {"title": "New title"}
 
     # Get all files
-    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}/files", headers=headers)
+    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files", headers=headers)
     assert res.status_code == 200
     assert len(res.json["entries"]) == 1
     assert res.json["entries"][0]["key"] == "test.pdf"
     assert res.json["entries"][0]["status"] == "completed"
     assert res.json["entries"][0]["metadata"] == {"title": "New title"}
 
     # Delete a file
-    res = client_with_credentials.delete(f"{{ parent_record.resource_config.base_url }}{id_}/files/test.pdf", headers=headers)
+    res = client_with_credentials.delete(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.delete_url }}/files/test.pdf", headers=headers)
     assert res.status_code == 204
 
     # Get all files
-    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}/files", headers=headers)
+    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files", headers=headers)
     assert res.status_code == 200
     assert len(res.json["entries"]) == 0
 
 def test_default_preview_file(app, client_with_credentials, search_clear, headers, input_data):
     # Initialize a draft
     res = client_with_credentials.post("{{ parent_record.resource_config.base_url }}", headers=headers, json=input_data)
     assert res.status_code == 201
     id_ = res.json["id"]
-    assert res.json["links"]["files"].endswith(f"{id_}/files")
+    assert res.json["links"]["files"].endswith(f"{id_}{{ test_constants.read_url }}/files")
 
     # Initialize 3 file uploads
     res = client_with_credentials.post(
-        f"{{ parent_record.resource_config.base_url }}{id_}/files",
+        f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files",
         headers=headers,
         json=[
             {"key": "f1.pdf"},
             {"key": "f2.pdf"},
             {"key": "f3.pdf"},
         ],
     )
@@ -127,145 +127,147 @@
         ("f3.pdf", "pending"),
     }
     assert res.json["default_preview"] is None
 
     # Upload and commit the 3 files
     for f in file_entries:
         res = client_with_credentials.put(
-            f"{{ parent_record.resource_config.base_url }}{id_}/files/{f['key']}/content",
+            f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}/files/{f['key']}/content",
             headers={
                 "content-type": "application/octet-stream",
                 "accept": "application/json",
             },
             data=BytesIO(b"testfile"),
         )
         assert res.status_code == 200
         assert res.json["status"] == "pending"
 
-        res = client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}/files/{f['key']}/commit", headers=headers)
+        res = client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files/{f['key']}/commit", headers=headers)
         assert res.status_code == 200
         assert res.json["status"] == "completed"
 
     # Set the default preview file
     input_data["files"]["default_preview"] = "f1.pdf"
-    res = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}", headers=headers, json=input_data)
+    res = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}", headers=headers, json=input_data)
     assert res.status_code == 200
     assert res.json["files"]["default_preview"] == "f1.pdf"
 
     # Change the default preview file
     input_data["files"]["default_preview"] = "f2.pdf"
-    res = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}", headers=headers, json=input_data)
+    res = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}", headers=headers, json=input_data)
     assert res.status_code == 200
     assert res.json["files"]["default_preview"] == "f2.pdf"
 
     # Unset the default preview file
     input_data["files"]["default_preview"] = None
-    res = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}", headers=headers, json=input_data)
+    res = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}", headers=headers, json=input_data)
     assert res.status_code == 200
     assert res.json["files"].get("default_preview") is None
 
     # Empty string the default preview file
     input_data["files"]["default_preview"] = ""
-    res = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}", headers=headers, json=input_data)
+    res = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}", headers=headers, json=input_data)
     assert res.status_code == 200
     assert res.json["files"].get("default_preview") is None
 
     # Set the default preview file
     input_data["files"]["default_preview"] = "f3.pdf"
-    res = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}", headers=headers, json=input_data)
+    res = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}", headers=headers, json=input_data)
     assert res.status_code == 200
     assert res.json["files"]["default_preview"] == "f3.pdf"
 
     # Delete the default preview file
-    res = client_with_credentials.delete(f"{{ parent_record.resource_config.base_url }}{id_}/files/f3.pdf", headers=headers)
+    res = client_with_credentials.delete(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.delete_url }}/files/f3.pdf", headers=headers)
     assert res.status_code == 204
 
     # Get all files and check default preview
-    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}/files", headers=headers)
+    res = client_with_credentials.get(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files", headers=headers)
     assert res.status_code == 200
     assert len(res.json["entries"]) == 2
     assert res.json["default_preview"] is None
 
 def test_file_api_errors(client_with_credentials, search_clear, headers, input_data,):
     """Test REST API errors for file management."""
     h = headers
 
     # Initialize a draft
     res = client_with_credentials.post("{{ parent_record.resource_config.base_url }}", headers=headers, json=input_data)
     assert res.status_code == 201
     id_ = res.json["id"]
-    assert res.json["links"]["files"].endswith(f"{id_}/files")
+    assert res.json["links"]["files"].endswith(f"{id_}{{ test_constants.read_url }}/files")
 
     # Initialize files upload
     # Pass an object instead of an array
-    res = client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}/files", headers=headers, json={"key": "test.pdf"})
+    res = client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files", headers=headers, json={"key": "test.pdf"})
     assert res.status_code == 400
 
     res = client_with_credentials.post(
-        f"{{ parent_record.resource_config.base_url }}{id_}/files",
+        f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files",
         headers=headers,
         json=[
             {"key": "test.pdf", "title": "Test file"},
         ],
     )
     assert res.status_code == 201
 
     # Upload a file
     res = client_with_credentials.put(
-        f"{{ parent_record.resource_config.base_url }}{id_}/files/test.pdf/content",
+        f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}/files/test.pdf/content",
         headers={
             "content-type": "application/octet-stream",
             "accept": "application/json",
         },
         data=BytesIO(b"testfile"),
     )
     assert res.status_code == 200
     assert res.json["status"] == "pending"
 
     # Commit the uploaded file
-    res = client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}/files/test.pdf/commit", headers=headers)
+    res = client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files/test.pdf/commit", headers=headers)
     assert res.status_code == 200
     assert res.json["status"] == "completed"
 
     # Initialize same file upload again
     res = client_with_credentials.post(
-        f"{{ parent_record.resource_config.base_url }}{id_}/files",
+        f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files",
         headers=headers,
         json=[
             {"key": "test.pdf", "title": "Test file"},
         ],
     )
     assert res.status_code == 400
 
+{% if not test_constants.skip_continous_disable_files_test %}
 def test_disable_files_when_files_already_present_should_error(
     app, client_with_credentials, search_clear, headers, input_data
 ):
     # Initialize a record
     response = client_with_credentials.post("{{ parent_record.resource_config.base_url }}", headers=headers, json=input_data)
     id_ = response.json["id"]
     # Add file
     file_id = "f1.pdf"
-    client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}/files", headers=headers, json=[{"key": file_id}])
+    client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files", headers=headers, json=[{"key": file_id}])
     client_with_credentials.put(
-        f"{{ parent_record.resource_config.base_url }}{id_}/files/{file_id}/content",
+        f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}/files/{file_id}/content",
         headers={
             "content-type": "application/octet-stream",
             "accept": "application/json",
         },
         data=BytesIO(b"testfile"),
     )
-    client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}/files/{file_id}/commit", headers=headers)
+    client_with_credentials.post(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.read_url }}/files/{file_id}/commit", headers=headers)
     # Disable files
     input_data["files"] = {"enabled": False}
 
-    response = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}", headers=headers, json=input_data)
+    response = client_with_credentials.put(f"{{ parent_record.resource_config.base_url }}{id_}{{ test_constants.update_url }}", headers=headers, json=input_data)
 
     assert response.status_code == 400
     assert response.json["errors"] == [
         {
             "field": "files.enabled",
             "messages": [
                 "You must first delete all files to set the record to be "
                 "metadata-only."
             ],
         }
-    ]
+    ]
+{% endif %}
```

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/builtin_models/invenio_files.json` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builtin_models/invenio_files.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/datatypes/components/parent_record.py` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/parent_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     depends_on = [
         DefaultsModelComponent,
         RecordMetadataModelComponent,
         ServiceModelComponent,
     ]
 
     def before_model_prepare(self, datatype, *, context, **kwargs):
-        if context["profile"] == "files":
+        if context["profile"] != "record":
             return
         prepend_array(datatype, "record-metadata", "base-classes", "RecordMetadataBase")
         prepend_array(datatype, "record-metadata", "base-classes", "db.Model")
 
         append_array(
             datatype,
             "record-metadata",
```

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files/profiles/file.py` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/profiles/file.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files.egg-info/PKG-INFO` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 4.0.2
+Version: 4.0.3
 Description-Content-Type: text/markdown
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
```

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files.egg-info/SOURCES.txt` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -38,10 +38,21 @@
 oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2
 oarepo_model_builder_files/builtin_models/__init__.py
 oarepo_model_builder_files/builtin_models/invenio_files.json
 oarepo_model_builder_files/datatypes/__init__.py
 oarepo_model_builder_files/datatypes/file.py
 oarepo_model_builder_files/datatypes/components/__init__.py
 oarepo_model_builder_files/datatypes/components/file.py
+oarepo_model_builder_files/datatypes/components/files_tests.py
 oarepo_model_builder_files/datatypes/components/parent_record.py
+oarepo_model_builder_files/datatypes/components/files_model/__init__.py
+oarepo_model_builder_files/datatypes/components/files_model/defaults.py
+oarepo_model_builder_files/datatypes/components/files_model/ext_resource.py
+oarepo_model_builder_files/datatypes/components/files_model/files_field.py
+oarepo_model_builder_files/datatypes/components/files_model/permissions.py
+oarepo_model_builder_files/datatypes/components/files_model/pid.py
+oarepo_model_builder_files/datatypes/components/files_model/record.py
+oarepo_model_builder_files/datatypes/components/files_model/record_metadata.py
+oarepo_model_builder_files/datatypes/components/files_model/resource.py
+oarepo_model_builder_files/datatypes/components/files_model/service.py
 oarepo_model_builder_files/profiles/__init__.py
 oarepo_model_builder_files/profiles/file.py
```

### Comparing `oarepo-model-builder-files-4.0.2/oarepo_model_builder_files.egg-info/entry_points.txt` & `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.2/setup.cfg` & `oarepo-model-builder-files-4.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-files
-version = 4.0.2
+version = 4.0.3
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

