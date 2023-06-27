# Comparing `tmp/types-tree-sitter-languages-1.5.0.2.tar.gz` & `tmp/types-tree-sitter-languages-1.6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tree-sitter-languages-1.5.0.2.tar", last modified: Tue Feb 21 01:34:07 2023, max compression
+gzip compressed data, was "types-tree-sitter-languages-1.6.0.0.tar", last modified: Tue Jun 27 01:43:00 2023, max compression
```

## Comparing `types-tree-sitter-languages-1.5.0.2.tar` & `types-tree-sitter-languages-1.6.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:34:07.976412 types-tree-sitter-languages-1.5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-21 01:34:07.000000 types-tree-sitter-languages-1.5.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:34:07.000000 types-tree-sitter-languages-1.5.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-21 01:34:07.976412 types-tree-sitter-languages-1.5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:34:07.976412 types-tree-sitter-languages-1.5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-21 01:34:07.000000 types-tree-sitter-languages-1.5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:34:07.976412 types-tree-sitter-languages-1.5.0.2/tree_sitter_languages-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-21 01:34:07.000000 types-tree-sitter-languages-1.5.0.2/tree_sitter_languages-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-21 01:26:21.000000 types-tree-sitter-languages-1.5.0.2/tree_sitter_languages-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-21 01:26:21.000000 types-tree-sitter-languages-1.5.0.2/tree_sitter_languages-stubs/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:34:07.976412 types-tree-sitter-languages-1.5.0.2/types_tree_sitter_languages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-21 01:34:07.000000 types-tree-sitter-languages-1.5.0.2/types_tree_sitter_languages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-21 01:34:07.000000 types-tree-sitter-languages-1.5.0.2/types_tree_sitter_languages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:34:07.000000 types-tree-sitter-languages-1.5.0.2/types_tree_sitter_languages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-21 01:34:07.000000 types-tree-sitter-languages-1.5.0.2/types_tree_sitter_languages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-21 01:34:07.000000 types-tree-sitter-languages-1.5.0.2/types_tree_sitter_languages.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:43:00.261959 types-tree-sitter-languages-1.6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-27 01:42:59.000000 types-tree-sitter-languages-1.6.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 01:42:59.000000 types-tree-sitter-languages-1.6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-27 01:43:00.261959 types-tree-sitter-languages-1.6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 01:43:00.261959 types-tree-sitter-languages-1.6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-27 01:42:59.000000 types-tree-sitter-languages-1.6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:43:00.257959 types-tree-sitter-languages-1.6.0.0/tree_sitter_languages-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 01:42:59.000000 types-tree-sitter-languages-1.6.0.0/tree_sitter_languages-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-27 01:42:44.000000 types-tree-sitter-languages-1.6.0.0/tree_sitter_languages-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 01:42:44.000000 types-tree-sitter-languages-1.6.0.0/tree_sitter_languages-stubs/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:43:00.261959 types-tree-sitter-languages-1.6.0.0/types_tree_sitter_languages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-27 01:43:00.000000 types-tree-sitter-languages-1.6.0.0/types_tree_sitter_languages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-27 01:43:00.000000 types-tree-sitter-languages-1.6.0.0/types_tree_sitter_languages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 01:43:00.000000 types-tree-sitter-languages-1.6.0.0/types_tree_sitter_languages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 01:43:00.000000 types-tree-sitter-languages-1.6.0.0/types_tree_sitter_languages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 01:43:00.000000 types-tree-sitter-languages-1.6.0.0/types_tree_sitter_languages.egg-info/top_level.txt
```

### Comparing `types-tree-sitter-languages-1.5.0.2/CHANGELOG.md` & `types-tree-sitter-languages-1.6.0.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+## 1.6.0.0 (2023-06-27)
+
+[stubsabot] Bump tree-sitter-languages to 1.6.* (#10364)
+
+Release: https://pypi.org/pypi/tree-sitter-languages/1.6.1
+Homepage: https://github.com/grantjenks/py-tree-sitter-languages
+Diff: https://github.com/grantjenks/py-tree-sitter-languages/compare/v1.5.0...v1.6.1
+
+Stubsabot analysis of the diff between the two releases:
+ - 0 public Python files have been added.
+ - 0 files included in typeshed's stubs have been deleted.
+ - 1 file included in typeshed's stubs has been modified or renamed: `tree_sitter_languages/__init__.py`.
+ - Total lines of Python code added: 68.
+ - Total lines of Python code deleted: 5.
+
 ## 1.5.0.2 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
 
 If you're reading about this commit from an autogenerated changelog entry, this should have no user-visible impact on how the stubs are interpreted by a type checker; it's just an internal change to how typeshed's tests work.
 
 ## 1.5.0.1 (2023-01-13)
```

### Comparing `types-tree-sitter-languages-1.5.0.2/PKG-INFO` & `types-tree-sitter-languages-1.6.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tree-sitter-languages
-Version: 1.5.0.2
+Version: 1.6.0.0
 Summary: Typing stubs for tree-sitter-languages
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tree-sitter-languages.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tree-sitter-languages`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tree-sitter-languages. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `b8ab395d4bafd6352560e74b636744d49a9bcd6e` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
+pytype 2023.6.2.
```

### Comparing `types-tree-sitter-languages-1.5.0.2/setup.py` & `types-tree-sitter-languages-1.6.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tree-sitter-languages`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tree-sitter-languages. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `b8ab395d4bafd6352560e74b636744d49a9bcd6e` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
+pytype 2023.6.2.
 '''.lstrip()
 
 setup(name=name,
-      version="1.5.0.2",
+      version="1.6.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tree-sitter-languages.md",
```

### Comparing `types-tree-sitter-languages-1.5.0.2/types_tree_sitter_languages.egg-info/PKG-INFO` & `types-tree-sitter-languages-1.6.0.0/types_tree_sitter_languages.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tree-sitter-languages
-Version: 1.5.0.2
+Version: 1.6.0.0
 Summary: Typing stubs for tree-sitter-languages
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tree-sitter-languages.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tree-sitter-languages`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tree-sitter-languages. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `b8ab395d4bafd6352560e74b636744d49a9bcd6e` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
+pytype 2023.6.2.
```

