# Comparing `tmp/microsoft_kiota_serialization_json-0.3.5.tar.gz` & `tmp/microsoft_kiota_serialization_json-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_serialization_json-0.3.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_serialization_json-0.3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_serialization_json-0.3.5.tar` & `microsoft_kiota_serialization_json-0.3.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       82 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1874 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.gitignore
--rw-r--r--   0        0        0    15976 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.pylintrc
--rw-r--r--   0        0        0     1126 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/LICENSE
--rw-r--r--   0        0        0     1146 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/Pipfile
--rw-r--r--   0        0        0    71082 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/Pipfile.lock
--rw-r--r--   0        0        0     2545 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/README.md
--rw-r--r--   0        0        0     2757 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/__init__.py
--rw-r--r--   0        0        0       23 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/_version.py
--rw-r--r--   0        0        0    11570 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_parse_node.py
--rw-r--r--   0        0        0     1445 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_parse_node_factory.py
--rw-r--r--   0        0        0    16605 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_serialization_writer.py
--rw-r--r--   0        0        0     1297 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_serialization_writer_factory.py
--rw-r--r--   0        0        0     1344 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      909 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/__init__.py
--rw-r--r--   0        0        0      119 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1569 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/entity.py
--rw-r--r--   0        0        0     2692 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/intersection_type.py
--rw-r--r--   0        0        0       94 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/office_location.py
--rw-r--r--   0        0        0     3077 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/union_type.py
--rw-r--r--   0        0        0     3133 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/user.py
--rw-r--r--   0        0        0     2151 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/user2.py
--rw-r--r--   0        0        0        0 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/__init__.py
--rw-r--r--   0        0        0     1554 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/conftest.py
--rw-r--r--   0        0        0     5236 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_intersection_wrapper.py
--rw-r--r--   0        0        0     4123 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_parse_node.py
--rw-r--r--   0        0        0     1686 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_parse_node_factory.py
--rw-r--r--   0        0        0     7188 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_serialization_writer.py
--rw-r--r--   0        0        0     1018 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_serialization_writer_factory.py
--rw-r--r--   0        0        0     5873 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_union_wrapper.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-06-27 09:36:19.290674 microsoft_kiota_serialization_json-0.3.6/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1874 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.gitignore
+-rw-r--r--   0        0        0    15976 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/.pylintrc
+-rw-r--r--   0        0        0     1250 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1146 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/Pipfile
+-rw-r--r--   0        0        0    71082 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/Pipfile.lock
+-rw-r--r--   0        0        0     2545 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/README.md
+-rw-r--r--   0        0        0     2757 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/_version.py
+-rw-r--r--   0        0        0    11570 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_parse_node.py
+-rw-r--r--   0        0        0     1433 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_parse_node_factory.py
+-rw-r--r--   0        0        0    16605 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_serialization_writer.py
+-rw-r--r--   0        0        0     1297 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     1344 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      909 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0      119 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1569 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/entity.py
+-rw-r--r--   0        0        0     2692 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/intersection_type.py
+-rw-r--r--   0        0        0       94 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/office_location.py
+-rw-r--r--   0        0        0     3077 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/union_type.py
+-rw-r--r--   0        0        0     3133 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/user.py
+-rw-r--r--   0        0        0     2151 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/helpers/user2.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1554 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/conftest.py
+-rw-r--r--   0        0        0     5236 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_intersection_wrapper.py
+-rw-r--r--   0        0        0     4123 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_parse_node.py
+-rw-r--r--   0        0        0     1679 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_parse_node_factory.py
+-rw-r--r--   0        0        0     7188 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_serialization_writer.py
+-rw-r--r--   0        0        0     1018 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     5873 2023-06-27 09:36:19.294674 microsoft_kiota_serialization_json-0.3.6/tests/unit/test_union_wrapper.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-0.3.6/PKG-INFO
```

### Comparing `microsoft_kiota_serialization_json-0.3.5/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_serialization_json-0.3.6/.github/workflows/auto-merge-dependabot.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/.github/workflows/build_publish.yml` & `microsoft_kiota_serialization_json-0.3.6/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_serialization_json-0.3.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_serialization_json-0.3.6/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/.gitignore` & `microsoft_kiota_serialization_json-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/.pylintrc` & `microsoft_kiota_serialization_json-0.3.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/CHANGELOG.md` & `microsoft_kiota_serialization_json-0.3.6/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.6] - 2023-06-27
+
+### Added
+
+### Changed
+- Fixed a bug with loading json response in method to get root parse node.
+
 ## [0.3.5] - 2023-06-14
 
 ### Added
 
 - Added support for composed types (de)serialization.
 
 ### Changed
```

### Comparing `microsoft_kiota_serialization_json-0.3.5/LICENSE` & `microsoft_kiota_serialization_json-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/Pipfile` & `microsoft_kiota_serialization_json-0.3.6/Pipfile`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [[source]]
 url = "https://pypi.org/simple"
 verify_ssl = true
 name = "pypi"
 
 [packages]
-microsoft-kiota-abstractions = "==0.5.1"
+microsoft-kiota-abstractions = "==0.5.4"
 python-dateutil = "==2.8.2"
 astroid = "==2.15.5"
 certifi = "==2023.5.7"
 charset-normalizer = "==3.1.0"
 colorama = "==0.4.6"
 coverage = {version = "==7.2.7", extras = ["toml"]}
 dill = "==0.3.6"
@@ -17,38 +17,38 @@
 flit = "==3.9.0"
 flit-core = "==3.9.0"
 idna = "==3.4"
 iniconfig = "==2.0.0"
 isort = "==5.12.0"
 lazy-object-proxy = "==1.9.0"
 mccabe = "==0.7.0"
-mypy = "==1.3.0"
+mypy = "==1.4.1"
 mypy-extensions = "==1.0.0"
 packaging = "==23.1"
-platformdirs = "==3.5.3"
-pluggy = "==1.0.0"
+platformdirs = "==3.8.0"
+pluggy = "==1.2.0"
 pylint = "==2.17.4"
-pytest = "==7.3.2"
+pytest = "==7.4.0"
 pytest-cov = "==4.1.0"
 requests = "==2.31.0"
 toml = "==0.10.2"
 tomli = "==2.0.1"
 tomli-w = "==1.0.0"
 tomlkit = "==0.11.8"
 types-python-dateutil = "==2.8.19.13"
 typing-extensions = "==4.6.3"
 urllib3 = "==2.0.3"
 wrapt = "==1.15.0"
-yapf = "==0.40.0"
+yapf = "==0.40.1"
 six = "==1.16.0"
 uritemplate = "==4.1.1"
 
 [dev-packages]
 flit = "==3.9.0"
 pylint = "==2.17.4"
-mypy = "==1.3.0"
-yapf = "==0.40.0"
+mypy = "==1.4.1"
+yapf = "==0.40.1"
 isort = "==5.12.0"
-pytest = "==7.3.2"
+pytest = "==7.4.0"
 pytest-cov = "==4.1.0"
 types-python-dateutil = "*"
 toml = "==0.10.2"
```

### Comparing `microsoft_kiota_serialization_json-0.3.5/Pipfile.lock` & `microsoft_kiota_serialization_json-0.3.6/Pipfile.lock`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9795470732970734%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'7da2b2b5b7679b9c55cc180ba16d69712289937c2ad5426a767c095584712661'}}",*

 * * "'default'": "{'importlib-metadata': {'hashes': "*

 * *              "['sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4', "*

 * *              "'sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5'], "*

 * *              "'version': '==6.7.0'}, 'microsoft-kiota-abstractions': {'hashes': "*

 * *              "['sha256:27152023d0a4c3ad2dba52240f5fd3c7276942c7f85f4bab3 […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "ea102596802a4b66275e5b6806f841a2c801f5f3cec56b310aaf69c7efc01ae4"
+            "sha256": "7da2b2b5b7679b9c55cc180ba16d69712289937c2ad5426a767c095584712661"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -234,19 +234,19 @@
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "index": "pypi",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
-                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
+                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
+                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==6.6.0"
+            "version": "==6.7.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "index": "pypi",
@@ -308,51 +308,51 @@
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "index": "pypi",
             "version": "==0.7.0"
         },
         "microsoft-kiota-abstractions": {
             "hashes": [
-                "sha256:1e9e3696b2414e6a6787e756eb69c658743f8db2b9eef8ecc415e03f6bc8b9c9",
-                "sha256:3ff7a0ba5d0476d7b6765d71fa3153b4198cb5507d367640d20d8e5107efd64c"
+                "sha256:27152023d0a4c3ad2dba52240f5fd3c7276942c7f85f4bab34f16dac4bb71dc4",
+                "sha256:590e3f3f2c8e1d7c525c107bece4afa48faedcf02409f2fc828456cb35fa19fe"
             ],
             "index": "pypi",
-            "version": "==0.5.1"
+            "version": "==0.5.4"
         },
         "mypy": {
             "hashes": [
-                "sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703",
-                "sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf",
-                "sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4",
-                "sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85",
-                "sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd",
-                "sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae",
-                "sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd",
-                "sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca",
-                "sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305",
-                "sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409",
-                "sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c",
-                "sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb",
-                "sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee",
-                "sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a",
-                "sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228",
-                "sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897",
-                "sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d",
-                "sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f",
-                "sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152",
-                "sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf",
-                "sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8",
-                "sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11",
-                "sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017",
-                "sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929",
-                "sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e",
-                "sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a"
+                "sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042",
+                "sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd",
+                "sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2",
+                "sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01",
+                "sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7",
+                "sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3",
+                "sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816",
+                "sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3",
+                "sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc",
+                "sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4",
+                "sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b",
+                "sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8",
+                "sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c",
+                "sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462",
+                "sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7",
+                "sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc",
+                "sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258",
+                "sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b",
+                "sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9",
+                "sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6",
+                "sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f",
+                "sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1",
+                "sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828",
+                "sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878",
+                "sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f",
+                "sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b"
             ],
             "index": "pypi",
-            "version": "==1.3.0"
+            "version": "==1.4.1"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "index": "pypi",
@@ -364,43 +364,43 @@
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "index": "pypi",
             "version": "==23.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed",
-                "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"
+                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
+                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
             ],
             "index": "pypi",
-            "version": "==3.5.3"
+            "version": "==3.8.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "index": "pypi",
-            "version": "==1.0.0"
+            "version": "==1.2.0"
         },
         "pylint": {
             "hashes": [
                 "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
                 "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
             "index": "pypi",
             "version": "==2.17.4"
         },
         "pytest": {
             "hashes": [
-                "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295",
-                "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
-            "version": "==7.3.2"
+            "version": "==7.4.0"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
                 "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
             ],
             "index": "pypi",
@@ -573,19 +573,19 @@
                 "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
             "index": "pypi",
             "version": "==1.15.0"
         },
         "yapf": {
             "hashes": [
-                "sha256:63386557876c2686cb29d8c422b2d1e484f29f7a278821f91515b5c5adf569a7",
-                "sha256:7eeb8c404e386f16e24cbd785103dbc573f51cbb68e65a35f4392e0233f3d7bc"
+                "sha256:958587eb5c8ec6c860119a9c25d02addf30a44f75aa152a4220d30e56a98037c",
+                "sha256:b8bfc1f280949153e795181768ca14ef43d7312629a06c43e7abd279323af313"
             ],
             "index": "pypi",
-            "version": "==0.40.0"
+            "version": "==0.40.1"
         },
         "zipp": {
             "hashes": [
                 "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
                 "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
@@ -797,19 +797,19 @@
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "index": "pypi",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
-                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
+                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
+                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==6.6.0"
+            "version": "==6.7.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "index": "pypi",
@@ -871,43 +871,43 @@
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "index": "pypi",
             "version": "==0.7.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703",
-                "sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf",
-                "sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4",
-                "sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85",
-                "sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd",
-                "sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae",
-                "sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd",
-                "sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca",
-                "sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305",
-                "sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409",
-                "sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c",
-                "sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb",
-                "sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee",
-                "sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a",
-                "sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228",
-                "sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897",
-                "sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d",
-                "sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f",
-                "sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152",
-                "sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf",
-                "sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8",
-                "sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11",
-                "sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017",
-                "sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929",
-                "sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e",
-                "sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a"
+                "sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042",
+                "sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd",
+                "sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2",
+                "sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01",
+                "sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7",
+                "sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3",
+                "sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816",
+                "sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3",
+                "sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc",
+                "sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4",
+                "sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b",
+                "sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8",
+                "sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c",
+                "sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462",
+                "sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7",
+                "sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc",
+                "sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258",
+                "sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b",
+                "sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9",
+                "sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6",
+                "sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f",
+                "sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1",
+                "sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828",
+                "sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878",
+                "sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f",
+                "sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b"
             ],
             "index": "pypi",
-            "version": "==1.3.0"
+            "version": "==1.4.1"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "index": "pypi",
@@ -919,43 +919,43 @@
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "index": "pypi",
             "version": "==23.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed",
-                "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"
+                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
+                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
             ],
             "index": "pypi",
-            "version": "==3.5.3"
+            "version": "==3.8.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "index": "pypi",
-            "version": "==1.0.0"
+            "version": "==1.2.0"
         },
         "pylint": {
             "hashes": [
                 "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
                 "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
             "index": "pypi",
             "version": "==2.17.4"
         },
         "pytest": {
             "hashes": [
-                "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295",
-                "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
-            "version": "==7.3.2"
+            "version": "==7.4.0"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
                 "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
             ],
             "index": "pypi",
@@ -1104,19 +1104,19 @@
                 "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
             "index": "pypi",
             "version": "==1.15.0"
         },
         "yapf": {
             "hashes": [
-                "sha256:63386557876c2686cb29d8c422b2d1e484f29f7a278821f91515b5c5adf569a7",
-                "sha256:7eeb8c404e386f16e24cbd785103dbc573f51cbb68e65a35f4392e0233f3d7bc"
+                "sha256:958587eb5c8ec6c860119a9c25d02addf30a44f75aa152a4220d30e56a98037c",
+                "sha256:b8bfc1f280949153e795181768ca14ef43d7312629a06c43e7abd279323af313"
             ],
             "index": "pypi",
-            "version": "==0.40.0"
+            "version": "==0.40.1"
         },
         "zipp": {
             "hashes": [
                 "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
                 "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `microsoft_kiota_serialization_json-0.3.5/README.md` & `microsoft_kiota_serialization_json-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/SECURITY.md` & `microsoft_kiota_serialization_json-0.3.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/SUPPORT.md` & `microsoft_kiota_serialization_json-0.3.6/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_parse_node.py` & `microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_parse_node_factory.py` & `microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_parse_node_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         if valid_content_type.casefold() != content_type.casefold():
             raise TypeError(f"Expected {valid_content_type} as content type")
 
         if not content:
             raise TypeError("Content cannot be null")
 
         content_as_str = content.decode('utf-8')
-        content_dict = json.loads(json.dumps(content_as_str))
+        content_dict = json.loads(content_as_str)
         return JsonParseNode(content_dict)
```

### Comparing `microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_serialization_writer.py` & `microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-0.3.6/kiota_serialization_json/json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/pyproject.toml` & `microsoft_kiota_serialization_json-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/requirements-dev.txt` & `microsoft_kiota_serialization_json-0.3.6/requirements-dev.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,35 +13,35 @@
 coverage[toml]==7.2.7
 dill==0.3.6
 docutils==0.20.1
 exceptiongroup==1.1.1
 flit-core==3.9.0
 flit==3.9.0
 idna==3.4
-importlib-metadata==6.6.0; python_version >= '3.7'
+importlib-metadata==6.7.0; python_version >= '3.7'
 iniconfig==2.0.0
 isort==5.12.0
 lazy-object-proxy==1.9.0
 mccabe==0.7.0
-microsoft-kiota-abstractions==0.5.3
+microsoft-kiota-abstractions==0.5.4
 mypy-extensions==1.0.0
-mypy==1.3.0
+mypy==1.4.1
 packaging==23.1
-platformdirs==3.5.3
-pluggy==1.0.0
+platformdirs==3.8.0
+pluggy==1.2.0
 pylint==2.17.4
 pytest-cov==4.1.0
-pytest==7.3.2
+pytest==7.4.0
 python-dateutil==2.8.2
 requests==2.31.0
 six==1.16.0
 toml==0.10.2
 tomli-w==1.0.0
 tomli==2.0.1
 tomlkit==0.11.8
 types-python-dateutil==2.8.19.13
 typing-extensions==4.6.3
 uritemplate==4.1.1
 urllib3==2.0.3
 wrapt==1.15.0
-yapf==0.40.0
+yapf==0.40.1
 zipp==3.15.0; python_version >= '3.7'
```

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/helpers/entity.py` & `microsoft_kiota_serialization_json-0.3.6/tests/helpers/entity.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/helpers/intersection_type.py` & `microsoft_kiota_serialization_json-0.3.6/tests/helpers/intersection_type.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/helpers/union_type.py` & `microsoft_kiota_serialization_json-0.3.6/tests/helpers/union_type.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/helpers/user.py` & `microsoft_kiota_serialization_json-0.3.6/tests/helpers/user.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/helpers/user2.py` & `microsoft_kiota_serialization_json-0.3.6/tests/helpers/user2.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/unit/conftest.py` & `microsoft_kiota_serialization_json-0.3.6/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/unit/test_intersection_wrapper.py` & `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_intersection_wrapper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_parse_node.py` & `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_parse_node_factory.py` & `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_parse_node_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 
 def test_get_root_parse_node(sample_json_string):
     factory = JsonParseNodeFactory()
     sample_json_string_bytes = sample_json_string.encode('utf-8')
     root = factory.get_root_parse_node('application/json', sample_json_string_bytes)
     assert isinstance(root, JsonParseNode)
-    assert str(root.get_bytes_value(), "utf-8") == sample_json_string
-
+    assert root._json_node == json.loads(sample_json_string)
 
+  
 def test_get_root_parse_node_no_content_type(sample_json_string):
     with pytest.raises(Exception) as e_info:
         factory = JsonParseNodeFactory()
         sample_json_string_bytes = sample_json_string.encode('utf-8')
         root = factory.get_root_parse_node('', sample_json_string_bytes)
```

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_serialization_writer.py` & `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/tests/unit/test_union_wrapper.py` & `microsoft_kiota_serialization_json-0.3.6/tests/unit/test_union_wrapper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.5/PKG-INFO` & `microsoft_kiota_serialization_json-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-serialization-json
-Version: 0.3.5
+Version: 0.3.6
 Summary: Implementation of Kiota Serialization interfaces for JSON
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

