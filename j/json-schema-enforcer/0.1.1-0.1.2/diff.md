# Comparing `tmp/json_schema_enforcer-0.1.1.tar.gz` & `tmp/json_schema_enforcer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_schema_enforcer-0.1.1.tar", max compression
+gzip compressed data, was "json_schema_enforcer-0.1.2.tar", max compression
```

## Comparing `json_schema_enforcer-0.1.1.tar` & `json_schema_enforcer-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2650 2023-06-27 19:15:35.843509 json_schema_enforcer-0.1.1/README.md
--rw-r--r--   0        0        0      100 2023-06-25 20:01:54.278748 json_schema_enforcer-0.1.1/json_schema_enforcer/__init__.py
--rw-r--r--   0        0        0    29552 2023-06-26 12:22:06.870156 json_schema_enforcer-0.1.1/json_schema_enforcer/schema.py
--rw-r--r--   0        0        0      382 2023-06-27 19:16:10.658304 json_schema_enforcer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 json_schema_enforcer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2650 2023-06-27 19:15:35.843509 json_schema_enforcer-0.1.2/README.md
+-rw-r--r--   0        0        0      138 2023-06-27 19:29:56.058279 json_schema_enforcer-0.1.2/json_schema_enforcer/__init__.py
+-rw-r--r--   0        0        0    29552 2023-06-26 12:22:06.870156 json_schema_enforcer-0.1.2/json_schema_enforcer/schema.py
+-rw-r--r--   0        0        0      382 2023-06-27 19:30:09.818194 json_schema_enforcer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 json_schema_enforcer-0.1.2/PKG-INFO
```

### Comparing `json_schema_enforcer-0.1.1/README.md` & `json_schema_enforcer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `json_schema_enforcer-0.1.1/json_schema_enforcer/schema.py` & `json_schema_enforcer-0.1.2/json_schema_enforcer/schema.py`

 * *Files identical despite different names*

### Comparing `json_schema_enforcer-0.1.1/PKG-INFO` & `json_schema_enforcer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-schema-enforcer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A progressive JSON schema validator
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

