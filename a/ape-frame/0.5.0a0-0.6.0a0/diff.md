# Comparing `tmp/ape-frame-0.5.0a0.tar.gz` & `tmp/ape-frame-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-frame-0.5.0a0.tar", last modified: Sun Dec  4 15:58:54 2022, max compression
+gzip compressed data, was "ape-frame-0.6.0a0.tar", last modified: Tue Jun 27 13:59:53 2023, max compression
```

## Comparing `ape-frame-0.5.0a0.tar` & `ape-frame-0.6.0a0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:58:54.678831 ape-frame-0.5.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:58:54.670831 ape-frame-0.5.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:58:54.674831 ape-frame-0.5.0a0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      473 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:58:54.674831 ape-frame-0.5.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.github/workflows/title.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      625 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2022-12-04 15:58:54.678831 ape-frame-0.5.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:58:54.674831 ape-frame-0.5.0a0/ape_frame/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/ape_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/ape_frame/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-04 15:58:54.000000 ape-frame-0.5.0a0/ape_frame/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:58:54.678831 ape-frame-0.5.0a0/ape_frame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2022-12-04 15:58:54.000000 ape-frame-0.5.0a0/ape_frame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2022-12-04 15:58:54.000000 ape-frame-0.5.0a0/ape_frame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 15:58:54.000000 ape-frame-0.5.0a0/ape_frame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 15:58:54.000000 ape-frame-0.5.0a0/ape_frame.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      412 2022-12-04 15:58:54.000000 ape-frame-0.5.0a0/ape_frame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-04 15:58:54.000000 ape-frame-0.5.0a0/ape_frame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-04 15:58:54.678831 ape-frame-0.5.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 15:58:54.678831 ape-frame-0.5.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-04 15:58:00.000000 ape-frame-0.5.0a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/ape_frame/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/ape_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/ape_frame/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/ape_frame/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/ape_frame/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/ape_frame/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-27 13:59:52.000000 ape-frame-0.6.0a0/ape_frame/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/ape_frame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 13:59:53.000000 ape-frame-0.6.0a0/ape_frame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 13:59:53.336301 ape-frame-0.6.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:53.332301 ape-frame-0.6.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:58:32.000000 ape-frame-0.6.0a0/tests/__init__.py
```

### Comparing `ape-frame-0.5.0a0/.github/ISSUE_TEMPLATE/bug.md` & `ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/.github/ISSUE_TEMPLATE/feature.md` & `ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-frame-0.6.0a0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/.github/release-drafter.yml` & `ape-frame-0.6.0a0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/.github/workflows/commitlint.yaml` & `ape-frame-0.6.0a0/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/.github/workflows/publish.yaml` & `ape-frame-0.6.0a0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/.github/workflows/test.yaml` & `ape-frame-0.6.0a0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/.github/workflows/title.yaml` & `ape-frame-0.6.0a0/.github/workflows/title.yaml`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/.gitignore` & `ape-frame-0.6.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/.pre-commit-config.yaml` & `ape-frame-0.6.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/CONTRIBUTING.md` & `ape-frame-0.6.0a0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/LICENSE` & `ape-frame-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/PKG-INFO` & `ape-frame-0.6.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-frame
-Version: 0.5.0a0
+Version: 0.6.0a0
 Summary: ape-frame: Frame (https://frame.sh) account plugin for Ape
 Home-page: https://github.com/ApeWorX/ape-frame
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-frame-0.5.0a0/README.md` & `ape-frame-0.6.0a0/README.md`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/ape_frame.egg-info/PKG-INFO` & `ape-frame-0.6.0a0/ape_frame.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-frame
-Version: 0.5.0a0
+Version: 0.6.0a0
 Summary: ape-frame: Frame (https://frame.sh) account plugin for Ape
 Home-page: https://github.com/ApeWorX/ape-frame
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-frame-0.5.0a0/ape_frame.egg-info/SOURCES.txt` & `ape-frame-0.6.0a0/ape_frame.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 .github/ISSUE_TEMPLATE/work-item.md
 .github/workflows/commitlint.yaml
 .github/workflows/draft.yaml
 .github/workflows/publish.yaml
 .github/workflows/test.yaml
 .github/workflows/title.yaml
 ape_frame/__init__.py
+ape_frame/accounts.py
+ape_frame/exceptions.py
+ape_frame/providers.py
 ape_frame/py.typed
 ape_frame/version.py
 ape_frame.egg-info/PKG-INFO
 ape_frame.egg-info/SOURCES.txt
 ape_frame.egg-info/dependency_links.txt
 ape_frame.egg-info/not-zip-safe
 ape_frame.egg-info/requires.txt
```

### Comparing `ape-frame-0.5.0a0/pyproject.toml` & `ape-frame-0.6.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-frame-0.5.0a0/setup.py` & `ape-frame-0.6.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-frame",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.5.7,<0.6.0",
+        "eth-ape>=0.6.0,<0.7.0",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_frame"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
```

