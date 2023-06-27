# Comparing `tmp/tee_cli-0.1.0.tar.gz` & `tmp/tee_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tee_cli-0.1.0.tar", max compression
+gzip compressed data, was "tee_cli-0.2.0.tar", max compression
```

## Comparing `tee_cli-0.1.0.tar` & `tee_cli-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1063 2023-03-27 15:34:00.744993 tee_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0        9 2023-03-27 15:34:00.744993 tee_cli-0.1.0/README.md
--rw-r--r--   0        0        0      429 2023-03-27 15:34:00.744993 tee_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1306 2023-03-27 15:34:00.748993 tee_cli-0.1.0/src/tee_cli/__main__.py
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 tee_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-27 15:22:24.570790 tee_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0      455 2023-06-27 15:22:24.570790 tee_cli-0.2.0/README.md
+-rw-r--r--   0        0        0      429 2023-06-27 15:22:24.570790 tee_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1264 2023-06-27 15:22:24.570790 tee_cli-0.2.0/src/tee_cli/__main__.py
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 tee_cli-0.2.0/PKG-INFO
```

### Comparing `tee_cli-0.1.0/LICENSE` & `tee_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

