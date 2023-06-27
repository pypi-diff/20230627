# Comparing `tmp/polywrap_client_config_builder-0.1.0a33.tar.gz` & `tmp/polywrap_client_config_builder-0.1.0a34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_client_config_builder-0.1.0a33.tar", max compression
+gzip compressed data, was "polywrap_client_config_builder-0.1.0a34.tar", max compression
```

## Comparing `polywrap_client_config_builder-0.1.0a33.tar` & `polywrap_client_config_builder-0.1.0a34.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1410 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/README.md
--rw-r--r--   0        0        0      138 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/__init__.py
--rw-r--r--   0        0        0      309 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/__init__.py
--rw-r--r--   0        0        0      995 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/base_configure.py
--rw-r--r--   0        0        0     2702 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/env_configure.py
--rw-r--r--   0        0        0     2120 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/interface_configure.py
--rw-r--r--   0        0        0     1628 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/package_configure.py
--rw-r--r--   0        0        0     1645 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/redirect_configure.py
--rw-r--r--   0        0        0      965 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/resolver_configure.py
--rw-r--r--   0        0        0     1607 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/wrapper_configure.py
--rw-r--r--   0        0        0     4240 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/polywrap_client_config_builder.py
--rw-r--r--   0        0        0        0 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/py.typed
--rw-r--r--   0        0        0      164 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/types/__init__.py
--rw-r--r--   0        0        0      613 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/types/build_options.py
--rw-r--r--   0        0        0     1154 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/types/builder_config.py
--rw-r--r--   0        0        0     6256 2023-06-19 13:35:11.334121 polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/types/client_config_builder.py
--rw-r--r--   0        0        0     1108 2023-06-19 13:45:57.337015 polywrap_client_config_builder-0.1.0a33/pyproject.toml
--rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 polywrap_client_config_builder-0.1.0a33/PKG-INFO
+-rw-r--r--   0        0        0     1410 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/README.md
+-rw-r--r--   0        0        0      138 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/__init__.py
+-rw-r--r--   0        0        0      309 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/__init__.py
+-rw-r--r--   0        0        0      995 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/base_configure.py
+-rw-r--r--   0        0        0     2702 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/env_configure.py
+-rw-r--r--   0        0        0     2120 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/interface_configure.py
+-rw-r--r--   0        0        0     1628 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/package_configure.py
+-rw-r--r--   0        0        0     1645 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/redirect_configure.py
+-rw-r--r--   0        0        0      965 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/resolver_configure.py
+-rw-r--r--   0        0        0     1607 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/wrapper_configure.py
+-rw-r--r--   0        0        0     4240 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/polywrap_client_config_builder.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/py.typed
+-rw-r--r--   0        0        0      164 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/types/__init__.py
+-rw-r--r--   0        0        0      613 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/types/build_options.py
+-rw-r--r--   0        0        0     1154 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/types/builder_config.py
+-rw-r--r--   0        0        0     6256 2023-06-27 11:59:05.052871 polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/types/client_config_builder.py
+-rw-r--r--   0        0        0     1108 2023-06-27 12:08:25.284041 polywrap_client_config_builder-0.1.0a34/pyproject.toml
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 polywrap_client_config_builder-0.1.0a34/PKG-INFO
```

### Comparing `polywrap_client_config_builder-0.1.0a33/README.md` & `polywrap_client_config_builder-0.1.0a34/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/base_configure.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/base_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/env_configure.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/env_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/interface_configure.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/interface_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/package_configure.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/package_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/redirect_configure.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/redirect_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/resolver_configure.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/resolver_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/configures/wrapper_configure.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/configures/wrapper_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/polywrap_client_config_builder.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/polywrap_client_config_builder.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/types/build_options.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/types/build_options.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/types/builder_config.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/types/builder_config.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/polywrap_client_config_builder/types/client_config_builder.py` & `polywrap_client_config_builder-0.1.0a34/polywrap_client_config_builder/types/client_config_builder.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a33/pyproject.toml` & `polywrap_client_config_builder-0.1.0a34/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-client-config-builder"
-version = "0.1.0a33"
+version = "0.1.0a34"
 description = ""
 authors = ["Media <media@polywrap.io>", "Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-uri-resolvers = "^0.1.0a33"
-polywrap-core = "^0.1.0a33"
+polywrap-uri-resolvers = "^0.1.0a34"
+polywrap-core = "^0.1.0a34"
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
```

### Comparing `polywrap_client_config_builder-0.1.0a33/PKG-INFO` & `polywrap_client_config_builder-0.1.0a34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: polywrap-client-config-builder
-Version: 0.1.0a33
+Version: 0.1.0a34
 Summary: 
 Author: Media
 Author-email: media@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-core (>=0.1.0a33,<0.2.0)
-Requires-Dist: polywrap-uri-resolvers (>=0.1.0a33,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0a34,<0.2.0)
+Requires-Dist: polywrap-uri-resolvers (>=0.1.0a34,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-client-config-builder
 
 A utility class for building the PolywrapClient config. 
 
 Supports building configs using method chaining or imperatively.
```

