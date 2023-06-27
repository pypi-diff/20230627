# Comparing `tmp/lumacli-0.0.1.tar.gz` & `tmp/lumacli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumacli-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lumacli-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lumacli-0.0.1.tar` & `lumacli-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      821 2023-06-26 15:49:44.283720 lumacli-0.0.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     3145 2023-06-26 15:49:44.283720 lumacli-0.0.1/.gitignore
--rw-r--r--   0        0        0     1064 2023-06-26 15:49:44.283720 lumacli-0.0.1/LICENSE
--rw-r--r--   0        0        0     2338 2023-06-26 15:49:44.283720 lumacli-0.0.1/README.md
--rw-r--r--   0        0        0     1916 2023-06-26 15:49:44.283720 lumacli-0.0.1/lumaCLI/README.md
--rw-r--r--   0        0        0      502 2023-06-26 15:49:44.283720 lumacli-0.0.1/lumaCLI/__init__.py
--rw-r--r--   0        0        0     2367 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/common.py
--rw-r--r--   0        0        0     4449 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/dbt.py
--rw-r--r--   0        0        0      239 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/luma.py
--rw-r--r--   0        0        0        0 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/tests/__init__.py
--rw-r--r--   0        0        0     8087 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/tests/catalog.json
--rw-r--r--   0        0        0   173474 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/tests/manifest.json
--rw-r--r--   0        0        0    10271 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/tests/run_results.json
--rw-r--r--   0        0        0     9716 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/tests/sources.json
--rw-r--r--   0        0        0      330 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/tests/test_common.py
--rw-r--r--   0        0        0      396 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/tests/test_dbt.py
--rw-r--r--   0        0        0      150 2023-06-26 15:49:44.287720 lumacli-0.0.1/lumaCLI/tests/utils.py
--rw-r--r--   0        0        0     1057 2023-06-26 15:49:44.287720 lumacli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 lumacli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-06-27 12:31:36.748239 lumacli-0.0.2/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     3145 2023-06-27 12:31:36.748239 lumacli-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1064 2023-06-27 12:31:36.748239 lumacli-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2338 2023-06-27 12:31:36.748239 lumacli-0.0.2/README.md
+-rw-r--r--   0        0        0     1916 2023-06-27 12:31:36.748239 lumacli-0.0.2/lumaCLI/README.md
+-rw-r--r--   0        0        0      502 2023-06-27 12:31:36.748239 lumacli-0.0.2/lumaCLI/__init__.py
+-rw-r--r--   0        0        0     2367 2023-06-27 12:31:36.748239 lumacli-0.0.2/lumaCLI/common.py
+-rw-r--r--   0        0        0     6050 2023-06-27 12:31:36.748239 lumacli-0.0.2/lumaCLI/dbt.py
+-rw-r--r--   0        0        0      239 2023-06-27 12:31:36.748239 lumacli-0.0.2/lumaCLI/luma.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:31:36.748239 lumacli-0.0.2/lumaCLI/tests/__init__.py
+-rw-r--r--   0        0        0     8087 2023-06-27 12:31:36.748239 lumacli-0.0.2/lumaCLI/tests/catalog.json
+-rw-r--r--   0        0        0   173474 2023-06-27 12:31:36.752239 lumacli-0.0.2/lumaCLI/tests/manifest.json
+-rw-r--r--   0        0        0    10271 2023-06-27 12:31:36.752239 lumacli-0.0.2/lumaCLI/tests/run_results.json
+-rw-r--r--   0        0        0     9716 2023-06-27 12:31:36.752239 lumacli-0.0.2/lumaCLI/tests/sources.json
+-rw-r--r--   0        0        0      330 2023-06-27 12:31:36.752239 lumacli-0.0.2/lumaCLI/tests/test_common.py
+-rw-r--r--   0        0        0      396 2023-06-27 12:31:36.752239 lumacli-0.0.2/lumaCLI/tests/test_dbt.py
+-rw-r--r--   0        0        0      150 2023-06-27 12:31:36.752239 lumacli-0.0.2/lumaCLI/tests/utils.py
+-rw-r--r--   0        0        0     1057 2023-06-27 12:31:36.752239 lumacli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 lumacli-0.0.2/PKG-INFO
```

### Comparing `lumacli-0.0.1/.github/workflows/publish_to_pypi.yml` & `lumacli-0.0.2/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.1/.gitignore` & `lumacli-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.1/LICENSE` & `lumacli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.1/README.md` & `lumacli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.1/lumaCLI/README.md` & `lumacli-0.0.2/lumaCLI/README.md`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.1/lumaCLI/common.py` & `lumacli-0.0.2/lumaCLI/common.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.1/lumaCLI/dbt.py` & `lumacli-0.0.2/lumaCLI/dbt.py`

 * *Files 25% similar despite different names*

```diff
@@ -83,15 +83,32 @@
     bundle_dict = {
         "manifest_json": manifest_dict,
         "catalog_json": catalog_dict,
         "sources_json": sources_dict,
         "run_results_json": run_results_dict,
     }
 
-    response = requests.post(endpoint, json=bundle_dict, verify=False)
+    try:
+        response = requests.post(
+            endpoint, json=bundle_dict, verify=False, timeout=(3.05, 60 * 30)
+        )
+    except (requests.exceptions.Timeout, requests.exceptions.ConnectionError) as e:
+        error_message = (
+            "[red]The request has failed. Please check your connection and try again."
+        )
+        if isinstance(e, requests.exceptions.Timeout):
+            error_message += " If you're using a VPN, ensure it's properly connected or try disabling it temporarily."
+        elif isinstance(e, requests.exceptions.ConnectionError):
+            error_message += (
+                " This could be due to maximum retries being exceeded or failure to establish a new connection. "
+                "Please check your network configuration."
+            )
+        print(Panel(error_message + "[/red]"))
+        raise typer.Exit(1)
+
     print_response(response)
     return response
 
 
 @app.command()
 def send_test_results(
     metadata_dir: str = typer.Argument(
@@ -124,14 +141,32 @@
         )
     run_results_path = Path(metadata_dir) / "run_results.json"
     is_run_results_json_valid = validate_json(run_results_path, "run_results.json")
     if not is_run_results_json_valid:
         raise typer.Exit(1)
 
     run_results_dict = json_to_dict(json_path=run_results_path)
-    response = requests.post(endpoint, json=run_results_dict, verify=False)
+
+    try:
+        response = requests.post(
+            endpoint, json=run_results_dict, verify=False, timeout=(3.05, 60 * 30)
+        )
+    except (requests.exceptions.Timeout, requests.exceptions.ConnectionError) as e:
+        error_message = (
+            "[red]The request has failed. Please check your connection and try again."
+        )
+        if isinstance(e, requests.exceptions.Timeout):
+            error_message += " If you're using a VPN, ensure it's properly connected or try disabling it temporarily."
+        elif isinstance(e, requests.exceptions.ConnectionError):
+            error_message += (
+                " This could be due to maximum retries being exceeded or failure to establish a new connection. "
+                "Please check your network configuration."
+            )
+        print(Panel(error_message + "[/red]"))
+        raise typer.Exit(1)
+
     print_response(response)
     return response
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `lumacli-0.0.1/lumaCLI/tests/catalog.json` & `lumacli-0.0.2/lumaCLI/tests/catalog.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.1/lumaCLI/tests/manifest.json` & `lumacli-0.0.2/lumaCLI/tests/manifest.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.1/lumaCLI/tests/run_results.json` & `lumacli-0.0.2/lumaCLI/tests/run_results.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.1/lumaCLI/tests/sources.json` & `lumacli-0.0.2/lumaCLI/tests/sources.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.1/pyproject.toml` & `lumacli-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "lumaCLI"
 description = "A CLI tool for managing the data catalog platform."
 readme = "README.md"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name="Facundo Goiriz", email="fgoiriz@dyvenia.com" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
 ]
```

### Comparing `lumacli-0.0.1/PKG-INFO` & `lumacli-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumaCLI
-Version: 0.0.1
+Version: 0.0.2
 Summary: A CLI tool for managing the data catalog platform.
 Keywords: cli,dbt,luma,data,catalog
 Author-email: Facundo Goiriz <fgoiriz@dyvenia.com>
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

