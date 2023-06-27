# Comparing `tmp/latviastreetify-0.0.1.tar.gz` & `tmp/latviastreetify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latviastreetify-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "latviastreetify-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `latviastreetify-0.0.1.tar` & `latviastreetify-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,27 @@
--rw-r--r--   0        0        0      422 2023-06-23 09:01:05.632000 latviastreetify-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      912 2023-06-23 09:01:05.632000 latviastreetify-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1062 2023-06-23 09:01:05.632000 latviastreetify-0.0.1/LICENSE
--rw-r--r--   0        0        0       33 2023-06-23 09:01:05.632000 latviastreetify-0.0.1/README.md
--rw-r--r--   0        0        0     2145 2023-06-23 09:01:05.632000 latviastreetify-0.0.1/cliff.toml
--rw-r--r--   0        0        0       99 2023-06-23 09:01:05.632000 latviastreetify-0.0.1/latviastreetify/__init__.py
--rw-r--r--   0        0        0      672 2023-06-23 09:01:05.632000 latviastreetify-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 latviastreetify-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       84 2023-06-27 06:07:26.192000 latviastreetify-0.0.2/.gitattributes
+-rw-r--r--   0        0        0       44 2023-06-27 09:06:25.632000 latviastreetify-0.0.2/.gitignore
+-rw-r--r--   0        0        0      538 2023-06-27 09:06:25.632000 latviastreetify-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1001 2023-06-27 08:25:15.616000 latviastreetify-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4534 2023-06-27 13:19:17.308000 latviastreetify-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1062 2023-06-27 06:07:26.192000 latviastreetify-0.0.2/LICENSE
+-rw-r--r--   0        0        0       31 2023-06-27 06:07:26.192000 latviastreetify-0.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     3268 2023-06-27 12:55:57.164000 latviastreetify-0.0.2/README.md
+-rw-r--r--   0        0        0     2145 2023-06-27 06:07:26.192000 latviastreetify-0.0.2/cliff.toml
+-rw-r--r--   0        0        0      265 2023-06-27 12:55:57.164000 latviastreetify-0.0.2/examples/head.py
+-rw-r--r--   0        0        0       99 2023-06-27 13:19:17.308000 latviastreetify-0.0.2/latviastreetify/__init__.py
+-rw-r--r--   0        0        0     2181 2023-06-27 12:46:17.000000 latviastreetify-0.0.2/latviastreetify/cli.py
+-rw-r--r--   0        0        0        6 2023-06-27 06:07:26.196000 latviastreetify-0.0.2/latviastreetify/data/Apkaimes.cpg
+-rw-r--r--   0        0        0     2563 2023-06-27 06:07:26.492000 latviastreetify-0.0.2/latviastreetify/data/Apkaimes.dbf
+-rw-r--r--   0        0        0      409 2023-06-27 06:07:26.216000 latviastreetify-0.0.2/latviastreetify/data/Apkaimes.prj
+-rw-r--r--   0        0        0   131180 2023-06-27 06:07:26.460000 latviastreetify-0.0.2/latviastreetify/data/Apkaimes.shp
+-rw-r--r--   0        0        0      780 2023-06-27 06:07:26.216000 latviastreetify-0.0.2/latviastreetify/data/Apkaimes.shx
+-rw-r--r--   0        0        0        6 2023-06-27 06:07:26.216000 latviastreetify-0.0.2/latviastreetify/data/adreses.cpg
+-rw-r--r--   0        0        0 36400307 2023-06-27 06:07:27.080000 latviastreetify-0.0.2/latviastreetify/data/adreses.dbf
+-rw-r--r--   0        0        0      144 2023-06-27 06:07:26.216000 latviastreetify-0.0.2/latviastreetify/data/adreses.prj
+-rw-r--r--   0        0        0      257 2023-06-27 06:07:26.216000 latviastreetify-0.0.2/latviastreetify/data/adreses.qpj
+-rw-r--r--   0        0        0  1256824 2023-06-27 06:07:26.524000 latviastreetify-0.0.2/latviastreetify/data/adreses.shp
+-rw-r--r--   0        0        0   359164 2023-06-27 06:07:26.220000 latviastreetify-0.0.2/latviastreetify/data/adreses.shx
+-rw-r--r--   0        0        0     2765 2023-06-27 08:40:25.080000 latviastreetify-0.0.2/latviastreetify/resolvers.py
+-rw-r--r--   0        0        0     1704 2023-06-27 08:57:35.204000 latviastreetify-0.0.2/latviastreetify/tests/test_resolver.py
+-rw-r--r--   0        0        0      738 2023-06-27 06:07:26.220000 latviastreetify-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4107 1970-01-01 00:00:00.000000 latviastreetify-0.0.2/PKG-INFO
```

### Comparing `latviastreetify-0.0.1/.pre-commit-config.yaml` & `latviastreetify-0.0.2/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 default_stages: [commit]
 repos:
-    - repo: https://github.com/pycqa/isort
-      rev: 5.12.0
-      hooks:
-          - id: isort
+  - repo: https://github.com/pycqa/isort
+    rev: 5.12.0
+    hooks:
+      - id: isort
+        args: ["--profile", "black"]
 
-    - repo: https://github.com/psf/black
-      rev: 22.6.0
-      hooks:
-          - id: black
+  - repo: https://github.com/psf/black
+    rev: 22.6.0
+    hooks:
+      - id: black
 
-    - repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.4.0
-      hooks:
-          - id: trailing-whitespace
-          - id: end-of-file-fixer
-          - id: check-json
-          - id: pretty-format-json
-            args:
-                - "--autofix"
-          - id: check-toml
-          - id: check-merge-conflict
-          - id: check-added-large-files
-    - repo: https://github.com/compilerla/conventional-pre-commit
-      rev: 7e1ceac2d5967f5428f0b1900cb7fe26da724bb1
-      hooks:
-          - id: conventional-pre-commit
-            stages: [commit-msg]
-            args: [feat, fix, docs, chore, ci, build] # optional: list of Conventional Commits types to allow
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.4.0
+    hooks:
+      - id: trailing-whitespace
+      - id: end-of-file-fixer
+      - id: check-json
+      - id: pretty-format-json
+        args:
+          - "--autofix"
+      - id: check-toml
+      - id: check-merge-conflict
+      - id: check-added-large-files
+  - repo: https://github.com/compilerla/conventional-pre-commit
+    rev: 7e1ceac2d5967f5428f0b1900cb7fe26da724bb1
+    hooks:
+      - id: conventional-pre-commit
+        stages: [commit-msg]
+        args: [feat, fix, docs, chore, ci, build] # optional: list of Conventional Commits types to allow
+
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: "6e63c9e9c65e1df04465cdcda0f2490e89291f58"
+    hooks:
+      - id: mypy
```

### Comparing `latviastreetify-0.0.1/LICENSE` & `latviastreetify-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `latviastreetify-0.0.1/cliff.toml` & `latviastreetify-0.0.2/cliff.toml`

 * *Files identical despite different names*

### Comparing `latviastreetify-0.0.1/pyproject.toml` & `latviastreetify-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 [project]
 name = "latviastreetify"
 authors = [{ name = "William Droz", email = "william.droz@idiap.ch" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
-dependencies = []
+dependencies = ["geopandas >= 0.13.2,<1.0.0"]
 [project.urls]
 Home = "https://gitlab.idiap.ch/socialcomputing/Icarus/latvian_streets_neighborhoods"
 
 [project.optional-dependencies]
 dev = [
     "black == 22.3.0",
     "coverage >= 6.4.2,<7.0.0",
     "flake8 >=3.8.3,<4.0.0",
     "mypy >=0.971,<1.0",
     "pre-commit >=3.3.3,<4.0.0",
     "pytest >=7.1.2,<8.0.0",
 ]
+
+cli = ["typer[all] >= 0.9.0,<1.0.0"]
```

