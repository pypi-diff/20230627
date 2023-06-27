# Comparing `tmp/robocorp-0.0.1.tar.gz` & `tmp/robocorp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp-0.0.1.tar", last modified: Wed Dec  9 13:27:48 2020, max compression
+gzip compressed data, was "robocorp-0.1.0.tar", max compression
```

## Comparing `robocorp-0.0.1.tar` & `robocorp-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2020-12-09 13:26:16.674542 robocorp-0.0.1/README.md
--rw-r--r--   0        0        0      326 2020-12-09 13:27:17.243634 robocorp-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2020-12-09 13:26:41.402182 robocorp-0.0.1/robocorp/__init__.py
--rw-r--r--   0        0        0      494 2020-12-09 13:27:48.065220 robocorp-0.0.1/setup.py
--rw-r--r--   0        0        0      399 2020-12-09 13:27:48.065469 robocorp-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-06-27 09:39:26.547654 robocorp-0.1.0/README.md
+-rw-r--r--   0        0        0      776 2023-06-27 09:39:26.547654 robocorp-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-06-27 09:39:26.547654 robocorp-0.1.0/src/robocorp/_meta/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:39:26.547654 robocorp-0.1.0/src/robocorp/_meta/py.typed
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 robocorp-0.1.0/PKG-INFO
```

