# Comparing `tmp/eiffel_framework-0.1.1.tar.gz` & `tmp/eiffel_framework-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eiffel_framework-0.1.1.tar", max compression
+gzip compressed data, was "eiffel_framework-0.1.2.tar", max compression
```

## Comparing `eiffel_framework-0.1.1.tar` & `eiffel_framework-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1061 2023-06-23 15:46:58.922074 eiffel_framework-0.1.1/LICENSE
--rw-r--r--   0        0        0       77 2023-06-23 15:46:58.922074 eiffel_framework-0.1.1/README.md
--rw-r--r--   0        0        0      962 2023-06-23 15:46:58.922074 eiffel_framework-0.1.1/eiffel/__init__.py
--rw-r--r--   0        0        0      146 2023-06-23 15:46:58.922074 eiffel_framework-0.1.1/eiffel/__main__.py
--rw-r--r--   0        0        0      173 2023-06-23 15:46:58.922074 eiffel_framework-0.1.1/eiffel/module.py
--rw-r--r--   0        0        0     1255 2023-06-26 16:18:43.225597 eiffel_framework-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 eiffel_framework-0.1.1/setup.py
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 eiffel_framework-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-23 15:27:52.569113 eiffel_framework-0.1.2/LICENSE
+-rw-r--r--   0        0        0       77 2023-06-23 15:27:52.569233 eiffel_framework-0.1.2/README.md
+-rw-r--r--   0        0        0      962 2023-06-23 15:30:11.612153 eiffel_framework-0.1.2/eiffel/__init__.py
+-rw-r--r--   0        0        0      146 2023-06-23 15:30:11.612748 eiffel_framework-0.1.2/eiffel/__main__.py
+-rw-r--r--   0        0        0      173 2023-06-23 15:30:11.614450 eiffel_framework-0.1.2/eiffel/module.py
+-rw-r--r--   0        0        0     1357 2023-06-27 09:40:40.687424 eiffel_framework-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 eiffel_framework-0.1.2/setup.py
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 eiffel_framework-0.1.2/PKG-INFO
```

### Comparing `eiffel_framework-0.1.1/LICENSE` & `eiffel_framework-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eiffel_framework-0.1.1/eiffel/__init__.py` & `eiffel_framework-0.1.2/eiffel/__init__.py`

 * *Files identical despite different names*

### Comparing `eiffel_framework-0.1.1/pyproject.toml` & `eiffel_framework-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 [tool.poetry]
 name = "eiffel-framework"
-version = "0.1.1"
+version = "0.1.2"
 description = "Evaluation Framework for FL-based intrusion detection using Flower."
 authors = ["phdcybersec <82591009+phdcybersec@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "eiffel", from = "." }]
 
 [tool.poetry.dependencies]
 python = "~3.10"
 
-# macos
-tensorflow-metal = { version = "~0.6.0", markers = "sys_platform == 'darwin'", optional = true}
-tensorflow-macos = { version = "~2.10.0", markers = "sys_platform == 'darwin'", optional = true}
-grpcio = { version = ">=1.37.0,<2.0", optional = true }
-h5py = { version = ">=3.6.0,<3.7", optional = true }
-numpy = { version = ">=1.23.2,<1.23.3", optional = true }
-protobuf = { version = ">=3.19.1,<3.20", optional = true }
-
-# linux
-tensorflow = { version = "~2.10.0", markers = "sys_platform != 'darwin'", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 isort = "^5.12.0"
 autoflake = "^2.1.1"
 
+
+[tool.poetry.group.darwin.dependencies]
+tensorflow-metal = { platform = "darwin", version = "~0.6.0", optional = true }
+tensorflow-macos = { platform = "darwin", version = "~2.10.0", optional = true }
+grpcio = { platform = "darwin", version = ">=1.37.0,<2.0", optional = true }
+h5py = { platform = "darwin", version = ">=3.6.0,<3.7", optional = true }
+numpy = { platform = "darwin", version = ">=1.23.2,<1.23.3", optional = true }
+protobuf = { platform = "darwin", version = ">=3.19.1,<3.20", optional = true }
+
+[tool.poetry.group.linux.dependencies]
+#tensorflow = { platform = "linux", version = "~2.10.0", optional = true }
+
 [tool.poetry.extras]
-macos = ["tensorflow-metal", "tensorflow-macos", "grpcio", "h5py", "numpy", "protobuf"]
+darwin = ["tensorflow-metal", "tensorflow-macos", "grpcio", "h5py", "numpy", "protobuf"]
 linux = ["tensorflow"]
 
 
 [tool.poetry.scripts]
 # eiffel = "eiffel:main"
 
 [build-system]
```

