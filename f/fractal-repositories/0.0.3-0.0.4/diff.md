# Comparing `tmp/fractal_repositories-0.0.3.tar.gz` & `tmp/fractal_repositories-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_repositories-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fractal_repositories-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractal_repositories-0.0.3.tar` & `fractal_repositories-0.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      187 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.coveragerc
--rw-r--r--   0        0        0      100 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.flake8
--rw-r--r--   0        0        0      945 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.gitignore
--rw-r--r--   0        0        0      161 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.isort.cfg
--rw-r--r--   0        0        0       43 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.mypy.ini
--rw-r--r--   0        0        0     1691 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/LICENSE
--rw-r--r--   0        0        0     1557 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/Makefile
--rw-r--r--   0        0        0     2276 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/README.md
--rw-r--r--   0        0        0      780 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/align_version.py
--rw-r--r--   0        0        0      182 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/django/__init__.py
--rw-r--r--   0        0        0     3291 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/django/mixins.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/elastic/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0     5318 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/gcp/firestore/mixins.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     3253 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/mongo/mixins.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    11960 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/contrib/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/core/__init__.py
--rw-r--r--   0        0        0     1466 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/core/entity.py
--rw-r--r--   0        0        0     2434 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/core/repositories.py
--rw-r--r--   0        0        0      343 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/mixins/__init__.py
--rw-r--r--   0        0        0     1219 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0     2965 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/mixins/file_repository_mixin.py
--rw-r--r--   0        0        0      957 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/mixins/filter_repository_mixin.py
--rw-r--r--   0        0        0     3044 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/mixins/inmemory_repository_mixin.py
--rw-r--r--   0        0        0       77 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/py.typed
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/utils/__init__.py
--rw-r--r--   0        0        0     2299 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/utils/cached_repository.py
--rw-r--r--   0        0        0     2381 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/utils/distributed_read_repository.py
--rw-r--r--   0        0        0      636 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/utils/json_encoder.py
--rw-r--r--   0        0        0      235 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/poetry.lock
--rw-r--r--   0        0        0     1667 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       69 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/setup.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/contrib/__init__.py
--rw-r--r--   0        0        0     4177 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/contrib/test_django.py
--rw-r--r--   0        0        0     4438 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/contrib/test_firestore.py
--rw-r--r--   0        0        0     4100 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/contrib/test_mongo.py
--rw-r--r--   0        0        0    12220 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/contrib/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/core/__init__.py
--rw-r--r--   0        0        0     3168 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/core/test_models.py
--rw-r--r--   0        0        0     1046 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/core/test_repositories.py
--rw-r--r--   0        0        0      232 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2164 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/django/__init__.py
--rw-r--r--   0        0        0      643 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/django/models.py
--rw-r--r--   0        0        0     1144 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/firestore.py
--rw-r--r--   0        0        0      898 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/mongo.py
--rw-r--r--   0        0        0     6786 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/repositories.py
--rw-r--r--   0        0        0     7674 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0      601 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_file_file_repository_mixin.py
--rw-r--r--   0        0        0     3764 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_file_repository_mixin.py
--rw-r--r--   0        0        0     3542 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_filter_repository_mixin.py
--rw-r--r--   0        0        0      827 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_inmemory_file_repository_mixin.py
--rw-r--r--   0        0        0     3150 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_inmemory_repository_mixin.py
--rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/utils/__init__.py
--rw-r--r--   0        0        0     4025 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/utils/test_cached_repository.py
--rw-r--r--   0        0        0     2381 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/utils/test_distributed_read_repository.py
--rw-r--r--   0        0        0      996 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/utils/test_json_encoder.py
--rw-r--r--   0        0        0      826 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tox.ini
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.coveragerc
+-rw-r--r--   0        0        0      100 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.flake8
+-rw-r--r--   0        0        0      945 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.gitignore
+-rw-r--r--   0        0        0      161 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.isort.cfg
+-rw-r--r--   0        0        0       43 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.mypy.ini
+-rw-r--r--   0        0        0     1691 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1557 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/Makefile
+-rw-r--r--   0        0        0     2276 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/README.md
+-rw-r--r--   0        0        0      780 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/align_version.py
+-rw-r--r--   0        0        0      182 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/django/__init__.py
+-rw-r--r--   0        0        0     3291 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/django/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/elastic/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0     5318 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/gcp/firestore/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     3253 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/mongo/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11960 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/contrib/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/core/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/core/entity.py
+-rw-r--r--   0        0        0     2434 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/core/repositories.py
+-rw-r--r--   0        0        0      343 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/mixins/__init__.py
+-rw-r--r--   0        0        0     1219 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0     2965 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/mixins/file_repository_mixin.py
+-rw-r--r--   0        0        0      957 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/mixins/filter_repository_mixin.py
+-rw-r--r--   0        0        0     3088 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/mixins/inmemory_repository_mixin.py
+-rw-r--r--   0        0        0       77 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/py.typed
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/utils/__init__.py
+-rw-r--r--   0        0        0     2299 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/utils/cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/utils/distributed_read_repository.py
+-rw-r--r--   0        0        0      636 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/fractal_repositories/utils/json_encoder.py
+-rw-r--r--   0        0        0      235 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/poetry.lock
+-rw-r--r--   0        0        0     1667 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/setup.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/contrib/__init__.py
+-rw-r--r--   0        0        0     4177 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/contrib/test_django.py
+-rw-r--r--   0        0        0     4438 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/contrib/test_firestore.py
+-rw-r--r--   0        0        0     4100 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/contrib/test_mongo.py
+-rw-r--r--   0        0        0    12220 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/contrib/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/core/__init__.py
+-rw-r--r--   0        0        0     3168 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/core/test_models.py
+-rw-r--r--   0        0        0     1046 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/core/test_repositories.py
+-rw-r--r--   0        0        0      232 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2164 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/fixtures/django/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/fixtures/django/models.py
+-rw-r--r--   0        0        0     1144 2023-06-27 11:43:15.526687 fractal_repositories-0.0.4/tests/fixtures/firestore.py
+-rw-r--r--   0        0        0      898 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/fixtures/mongo.py
+-rw-r--r--   0        0        0     6786 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/fixtures/repositories.py
+-rw-r--r--   0        0        0     7674 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/fixtures/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/__init__.py
+-rw-r--r--   0        0        0     1154 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0      601 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_file_file_repository_mixin.py
+-rw-r--r--   0        0        0     3764 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_file_repository_mixin.py
+-rw-r--r--   0        0        0     3542 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_filter_repository_mixin.py
+-rw-r--r--   0        0        0      827 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_inmemory_file_repository_mixin.py
+-rw-r--r--   0        0        0     3150 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/mixins/test_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/utils/__init__.py
+-rw-r--r--   0        0        0     4025 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/utils/test_cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/utils/test_distributed_read_repository.py
+-rw-r--r--   0        0        0      996 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tests/utils/test_json_encoder.py
+-rw-r--r--   0        0        0      826 2023-06-27 11:43:15.530687 fractal_repositories-0.0.4/tox.ini
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.4/PKG-INFO
```

### Comparing `fractal_repositories-0.0.3/.github/workflows/build.yml` & `fractal_repositories-0.0.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/.github/workflows/publish.yml` & `fractal_repositories-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/.gitignore` & `fractal_repositories-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/.pre-commit-config.yaml` & `fractal_repositories-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/LICENSE` & `fractal_repositories-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/Makefile` & `fractal_repositories-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/README.md` & `fractal_repositories-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/align_version.py` & `fractal_repositories-0.0.4/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/contrib/django/mixins.py` & `fractal_repositories-0.0.4/fractal_repositories/contrib/django/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/contrib/gcp/firestore/mixins.py` & `fractal_repositories-0.0.4/fractal_repositories/contrib/gcp/firestore/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/contrib/mongo/mixins.py` & `fractal_repositories-0.0.4/fractal_repositories/contrib/mongo/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/contrib/sqlalchemy/mixins.py` & `fractal_repositories-0.0.4/fractal_repositories/contrib/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/core/entity.py` & `fractal_repositories-0.0.4/fractal_repositories/core/entity.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/core/repositories.py` & `fractal_repositories-0.0.4/fractal_repositories/core/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.4/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/mixins/file_repository_mixin.py` & `fractal_repositories-0.0.4/fractal_repositories/mixins/file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/mixins/filter_repository_mixin.py` & `fractal_repositories-0.0.4/fractal_repositories/mixins/filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/mixins/inmemory_repository_mixin.py` & `fractal_repositories-0.0.4/fractal_repositories/mixins/inmemory_repository_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     def update(self, entity: EntityType, *, upsert=False) -> EntityType:
         if entity.id in self.entities or upsert:
             return self.add(entity)
         raise self._object_not_found()
 
     def remove_one(self, specification: Specification):
         if obj := self.find_one(specification):
-            del self.entities[obj.id]
+            if obj.id in self.entities:
+                del self.entities[obj.id]
 
     @property
     def _get_entities(self) -> Iterator[EntityType]:
         for value in self.entities.values():
             yield value
 
     def find_one(self, specification: Specification) -> EntityType:
```

### Comparing `fractal_repositories-0.0.3/fractal_repositories/utils/cached_repository.py` & `fractal_repositories-0.0.4/fractal_repositories/utils/cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/utils/distributed_read_repository.py` & `fractal_repositories-0.0.4/fractal_repositories/utils/distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/fractal_repositories/utils/json_encoder.py` & `fractal_repositories-0.0.4/fractal_repositories/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/pyproject.toml` & `fractal_repositories-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-repositories"
-version = "0.0.3"
+version = "0.0.4"
 description = "Fractal Repositories is an implementation of the repository pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal_repositories-0.0.3/tests/contrib/test_django.py` & `fractal_repositories-0.0.4/tests/contrib/test_django.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/contrib/test_firestore.py` & `fractal_repositories-0.0.4/tests/contrib/test_firestore.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/contrib/test_mongo.py` & `fractal_repositories-0.0.4/tests/contrib/test_mongo.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/contrib/test_sqlalchemy.py` & `fractal_repositories-0.0.4/tests/contrib/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/core/test_models.py` & `fractal_repositories-0.0.4/tests/core/test_models.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/core/test_repositories.py` & `fractal_repositories-0.0.4/tests/core/test_repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/fixtures/django/__init__.py` & `fractal_repositories-0.0.4/tests/fixtures/django/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/fixtures/django/models.py` & `fractal_repositories-0.0.4/tests/fixtures/django/models.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/fixtures/firestore.py` & `fractal_repositories-0.0.4/tests/fixtures/firestore.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/fixtures/mongo.py` & `fractal_repositories-0.0.4/tests/fixtures/mongo.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/fixtures/repositories.py` & `fractal_repositories-0.0.4/tests/fixtures/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/fixtures/sqlalchemy.py` & `fractal_repositories-0.0.4/tests/fixtures/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/mixins/test_external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.4/tests/mixins/test_external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/mixins/test_file_file_repository_mixin.py` & `fractal_repositories-0.0.4/tests/mixins/test_file_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/mixins/test_file_repository_mixin.py` & `fractal_repositories-0.0.4/tests/mixins/test_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/mixins/test_filter_repository_mixin.py` & `fractal_repositories-0.0.4/tests/mixins/test_filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/mixins/test_inmemory_file_repository_mixin.py` & `fractal_repositories-0.0.4/tests/mixins/test_inmemory_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/mixins/test_inmemory_repository_mixin.py` & `fractal_repositories-0.0.4/tests/mixins/test_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/utils/test_cached_repository.py` & `fractal_repositories-0.0.4/tests/utils/test_cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/utils/test_distributed_read_repository.py` & `fractal_repositories-0.0.4/tests/utils/test_distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tests/utils/test_json_encoder.py` & `fractal_repositories-0.0.4/tests/utils/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/tox.ini` & `fractal_repositories-0.0.4/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.3/PKG-INFO` & `fractal_repositories-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-repositories
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fractal Repositories is an implementation of the repository pattern of Domain Driven Design (DDD) for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-repositories
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

