# Comparing `tmp/json_schema_enforcer-0.1.0.tar.gz` & `tmp/json_schema_enforcer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_schema_enforcer-0.1.0.tar", max compression
+gzip compressed data, was "json_schema_enforcer-0.1.1.tar", max compression
```

## Comparing `json_schema_enforcer-0.1.0.tar` & `json_schema_enforcer-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      974 2023-06-25 18:56:14.071575 json_schema_enforcer-0.1.0/README.md
--rw-r--r--   0        0        0      100 2023-06-25 20:01:54.278748 json_schema_enforcer-0.1.0/json_schema_enforcer/__init__.py
--rw-r--r--   0        0        0      943 2023-06-25 12:20:00.029072 json_schema_enforcer-0.1.0/json_schema_enforcer/__main__.py
--rw-r--r--   0        0        0    29552 2023-06-26 12:22:06.870156 json_schema_enforcer-0.1.0/json_schema_enforcer/schema.py
--rw-r--r--   0        0        0      382 2023-06-26 00:14:40.432264 json_schema_enforcer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 json_schema_enforcer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2650 2023-06-27 19:15:35.843509 json_schema_enforcer-0.1.1/README.md
+-rw-r--r--   0        0        0      100 2023-06-25 20:01:54.278748 json_schema_enforcer-0.1.1/json_schema_enforcer/__init__.py
+-rw-r--r--   0        0        0    29552 2023-06-26 12:22:06.870156 json_schema_enforcer-0.1.1/json_schema_enforcer/schema.py
+-rw-r--r--   0        0        0      382 2023-06-27 19:16:10.658304 json_schema_enforcer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 json_schema_enforcer-0.1.1/PKG-INFO
```

### Comparing `json_schema_enforcer-0.1.0/json_schema_enforcer/schema.py` & `json_schema_enforcer-0.1.1/json_schema_enforcer/schema.py`

 * *Files identical despite different names*

