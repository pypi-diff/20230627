# Comparing `tmp/tableau-helpers-2.0.5.dev3.tar.gz` & `tmp/tableau-helpers-2.0.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau-helpers-2.0.5.dev3.tar", last modified: Tue Jun 20 14:29:08 2023, max compression
+gzip compressed data, was "tableau-helpers-2.0.5.dev4.tar", last modified: Tue Jun 27 17:52:14 2023, max compression
```

## Comparing `tableau-helpers-2.0.5.dev3.tar` & `tableau-helpers-2.0.5.dev4.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.260014 tableau-helpers-2.0.5.dev3/
--rw-rw-rw-   0        0        0      122 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/.env.sample
--rw-rw-rw-   0        0        0       54 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/.flake8
--rw-rw-rw-   0        0        0      376 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/.gitignore
--rw-rw-rw-   0        0        0      463 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1088 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/LICENSE
--rw-rw-rw-   0        0        0     1893 2023-06-20 14:29:08.260014 tableau-helpers-2.0.5.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/README.md
--rw-rw-rw-   0        0        0     1053 2023-06-20 12:54:09.000000 tableau-helpers-2.0.5.dev3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 14:29:08.260014 tableau-helpers-2.0.5.dev3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.049145 tableau-helpers-2.0.5.dev3/tableau_helpers/
--rw-rw-rw-   0        0        0      191 2023-06-20 14:25:15.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.117853 tableau-helpers-2.0.5.dev3/tableau_helpers/cli/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/cli/__init__.py
--rw-rw-rw-   0        0        0     2559 2023-06-20 14:27:44.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/cli/csv_to_hyper.py
--rw-rw-rw-   0        0        0     1141 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/cli/upload_hyper.py
--rw-rw-rw-   0        0        0     7726 2023-06-19 14:05:36.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/hyper.py
--rw-rw-rw-   0        0        0     8008 2023-06-06 16:49:39.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/server.py
--rw-rw-rw-   0        0        0     1146 2023-06-20 14:25:19.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.102228 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/
--rw-rw-rw-   0        0        0     1893 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      146 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.149105 tableau-helpers-2.0.5.dev3/tests/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.180601 tableau-helpers-2.0.5.dev3/tests/cli/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev3/tests/cli/__init__.py
--rw-rw-rw-   0        0        0      880 2023-06-06 16:03:33.000000 tableau-helpers-2.0.5.dev3/tests/cli/test_csv_to_hyper.py
--rw-rw-rw-   0        0        0      730 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev3/tests/cli/test_upload_hyper.py
--rw-rw-rw-   0        0        0     1836 2023-06-12 12:44:15.000000 tableau-helpers-2.0.5.dev3/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.260014 tableau-helpers-2.0.5.dev3/tests/resources/
--rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_default_format.csv
--rw-rw-rw-   0        0        0    65536 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_default_format.hyper
--rw-rw-rw-   0        0        0       34 2023-06-06 15:42:19.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_default_format.tab
--rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_default_format2.csv
--rw-rw-rw-   0        0        0      378 2023-06-09 15:46:22.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_default_format_table_def.json
--rw-rw-rw-   0        0        0      887 2023-06-12 12:33:02.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_join_table_def.json
--rw-rw-rw-   0        0        0       52 2023-06-12 10:42:48.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_left.csv
--rw-rw-rw-   0        0        0       56 2023-06-12 10:43:02.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_right.csv
--rw-rw-rw-   0        0        0    65536 2023-06-12 12:41:14.000000 tableau-helpers-2.0.5.dev3/tests/resources/joined.hyper
--rw-rw-rw-   0        0        0     3886 2023-06-12 12:44:37.000000 tableau-helpers-2.0.5.dev3/tests/test_hyper.py
--rw-rw-rw-   0        0        0     1128 2023-06-12 12:43:43.000000 tableau-helpers-2.0.5.dev3/tests/test_server.py
--rw-rw-rw-   0        0        0      591 2023-06-12 09:09:36.000000 tableau-helpers-2.0.5.dev3/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.509108 tableau-helpers-2.0.5.dev4/
+-rw-rw-rw-   0        0        0      122 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev4/.env.sample
+-rw-rw-rw-   0        0        0      376 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev4/.gitignore
+-rw-rw-rw-   0        0        0     1088 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev4/LICENSE
+-rw-rw-rw-   0        0        0     1914 2023-06-27 17:52:14.509108 tableau-helpers-2.0.5.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     1617 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev4/README.md
+-rw-rw-rw-   0        0        0     1237 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:52:14.509108 tableau-helpers-2.0.5.dev4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.248654 tableau-helpers-2.0.5.dev4/tableau_helpers/
+-rw-rw-rw-   0        0        0      191 2023-06-27 17:51:43.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.342637 tableau-helpers-2.0.5.dev4/tableau_helpers/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/cli/__init__.py
+-rw-rw-rw-   0        0        0     2533 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/cli/csv_to_hyper.py
+-rw-rw-rw-   0        0        0     1114 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/cli/upload_hyper.py
+-rw-rw-rw-   0        0        0     7794 2023-06-27 17:51:06.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/hyper.py
+-rw-rw-rw-   0        0        0     7998 2023-06-27 17:51:06.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/server.py
+-rw-rw-rw-   0        0        0     1142 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.310814 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/
+-rw-rw-rw-   0        0        0     1914 2023-06-27 17:52:13.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2023-06-27 17:52:14.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:52:13.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-06-27 17:52:13.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      183 2023-06-27 17:52:13.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 17:52:13.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.373904 tableau-helpers-2.0.5.dev4/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.405573 tableau-helpers-2.0.5.dev4/tests/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/cli/__init__.py
+-rw-rw-rw-   0        0        0      881 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/cli/test_csv_to_hyper.py
+-rw-rw-rw-   0        0        0      696 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/cli/test_upload_hyper.py
+-rw-rw-rw-   0        0        0     1838 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.488824 tableau-helpers-2.0.5.dev4/tests/resources/
+-rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_default_format.csv
+-rw-rw-rw-   0        0        0    65536 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_default_format.hyper
+-rw-rw-rw-   0        0        0       34 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_default_format.tab
+-rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_default_format2.csv
+-rw-rw-rw-   0        0        0      378 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_default_format_table_def.json
+-rw-rw-rw-   0        0        0      887 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_join_table_def.json
+-rw-rw-rw-   0        0        0       52 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_left.csv
+-rw-rw-rw-   0        0        0       56 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_right.csv
+-rw-rw-rw-   0        0        0    65536 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/joined.hyper
+-rw-rw-rw-   0        0        0     3902 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/test_hyper.py
+-rw-rw-rw-   0        0        0     1128 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/test_server.py
+-rw-rw-rw-   0        0        0      564 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tox.ini
```

### Comparing `tableau-helpers-2.0.5.dev3/LICENSE` & `tableau-helpers-2.0.5.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev3/PKG-INFO` & `tableau-helpers-2.0.5.dev4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tableau-helpers
-Version: 2.0.5.dev3
+Version: 2.0.5.dev4
 Summary: A collection of helpers to reduce boilerplate with Tableau APIs.
 License: MIT License
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 # tableau_helpers
 
 A wrapper for the tableau-server-client and hyper-api which abstracts away
 boilerplate and in some cases provides a CLI which works without admin privileges.
```

### Comparing `tableau-helpers-2.0.5.dev3/README.md` & `tableau-helpers-2.0.5.dev4/README.md`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev3/pyproject.toml` & `tableau-helpers-2.0.5.dev4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -16,27 +16,37 @@
 ]
 dynamic = ["version"]
 
 [project.scripts]
 csv-to-hyper = "tableau_helpers.cli.csv_to_hyper:entry_point"
 upload-hyper = "tableau_helpers.cli.upload_hyper:entry_point"
 
-[tool.setuptools.dynamic]
-version ={attr = "tableau_helpers.__version__"}
-
 [tool.setuptools.packages.find]
 include = ["tableau_helpers*"]
 exclude = ["tableau_helpers.tests*"]
 
 [project.optional-dependencies]
-test = [
-    "pytest",
-    "pylint"
+test = ["pytest"]
+dev = [
+    "pre-commit",
+    "black",
+    "ruff",
+    "pylint",
+    "pyright"
 ]
 
-[tool.isort]
-profile = "black"
+[tool.setuptools.dynamic]
+version ={attr = "tableau_helpers.__version__"}
+
+[tool.pyright]
+files="tableau_helpers"
+ignore_missing_imports=true
 
-[tool.pytest.ini_options]
+[tools.pytest.ini_options]
 markers = [
+    "development: Development tests",
     "integration: integration tests which require a tableau-server",
 ]
+
+
+[tool.ruff]
+target-version = "py39"
```

### Comparing `tableau-helpers-2.0.5.dev3/tableau_helpers/cli/csv_to_hyper.py` & `tableau-helpers-2.0.5.dev4/tableau_helpers/cli/csv_to_hyper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 import sys
 from pathlib import Path
 import tempfile
-from typing import Union
 
 from tableau_helpers import hyper, utils
 
 tempdir = tempfile.TemporaryDirectory()
 
 
 def literal(value: str) -> str:
```

### Comparing `tableau-helpers-2.0.5.dev3/tableau_helpers/cli/upload_hyper.py` & `tableau-helpers-2.0.5.dev4/tableau_helpers/cli/upload_hyper.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,38 +5,41 @@
 from tableau_helpers import server
 
 
 def _parse_args(args) -> argparse.Namespace:
     description = "Upload or overwrite a hyperfile on tableau-server"
     parser = argparse.ArgumentParser(description=description)
     parser.add_argument(
-            "--hyperfile",
-            type=Path,
-            required=True,
-            help="The path to the hyperfile to be uploaded.")
+        "--hyperfile",
+        type=Path,
+        required=True,
+        help="The path to the hyperfile to be uploaded.",
+    )
     parser.add_argument(
-            "--dest",
-            type=str,
-            required=True,
-            help="The destination project string from root folder")
+        "--dest",
+        type=str,
+        required=True,
+        help="The destination project string from root folder",
+    )
     parser.add_argument(
-            "--new-name",
-            type=str,
-            required=False,
-            default=None,
-            help="A name for the datasource (if desired different from hyperfile)")
+        "--new-name",
+        type=str,
+        required=False,
+        default=None,
+        help="A name for the datasource (if desired different from hyperfile)",
+    )
     return parser.parse_args(args)
 
 
 def main(args):
     args = _parse_args(args)
-    server.create_or_replace_hyper_file(project=args.dest, hyperfile_path=args.hyperfile, name=args.new_name)
+    server.create_or_replace_hyper_file(
+        project=args.dest, hyperfile_path=args.hyperfile, name=args.new_name
+    )
 
 
 def entry_point():
     main(sys.argv[1:])
 
 
 if __name__ == "__main__":
     entry_point()
-        
-
```

### Comparing `tableau-helpers-2.0.5.dev3/tableau_helpers/hyper.py` & `tableau-helpers-2.0.5.dev4/tableau_helpers/hyper.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 ):
     sql_with: str = "WITH ("
     sql_with += "FORMAT csv"
     sql_with += f", NULL {escape_string_literal(null)}"
     sql_with += f", DELIMITER {escape_string_literal(delimiter)}"
     sql_with += f", ENCODING {escape_string_literal(encoding)}"
     sql_with += f", ON_CAST_FAILURE {escape_string_literal(on_cast_failure)}"
-    sql_with += f", HEADER {str(header).capitalize()}"
+    if header:
+        sql_with += f", HEADER"
     sql_with += f", QUOTE {escape_string_literal(quote)}"
     if escape is not None:
         sql_with += f", ESCAPE {escape_string_literal(escape)}"
     if force_not_null is not None:
         sql_with += f", FORCE_NOT_NULL ({','.join(force_not_null)})"
     if force_null is not None:
         sql_with += f", FORCE_NULL ({','.join(force_null)})"
@@ -84,15 +85,17 @@
     columns = tableconf.get("columns", [])
     columns = parse_columns(columns)
     table_def = TableDefinition(TableName(table_name), columns)
     constraints = tableconf.get("constraints")
     if constraints is not None:
         if isinstance(constraints, str):
             constraints = [constraints]
-        table_def.th_alterations = [f"ALTER TABLE \"{table_name}\" ADD {x}" for x in constraints]
+        table_def.th_alterations = [
+            f'ALTER TABLE "{table_name}" ADD {x}' for x in constraints
+        ]
     return table_def
 
 
 def copy_csv_to_hyper(
     save_path: Path,
     csv: Union[Path, list[Path]],
     schema: Union[TableDefinition, list[TableDefinition]],
@@ -162,18 +165,18 @@
             force_not_null=force_not_null,
             force_null=force_null,
         )
         sql_commands.append(f"{sql_from} {sql_with}")
         try:
             if s.th_alterations is not None:
                 [alterations.append(x) for x in s.th_alterations]
-        except:
+        except AttributeError:
+            # alterations are optional
             pass
 
-
     process_parameters = {}
     log_file_max_count = os.getenv("TABLEAU_HYPERAPI_LOG_FILE_MAX_COUNT", "3")
     process_parameters["log_file_max_count"] = log_file_max_count
     log_file_size_limit = os.getenv("TABLEAU_HYPERAPI_LOG_FILE_SIZE_LIMIT", "100M")
     process_parameters["log_file_size_limit"] = log_file_size_limit
     log_dir = os.getenv("TABLEAU_HYPERAPI_LOG_DIR", None)
     if log_dir is not None:
```

### Comparing `tableau-helpers-2.0.5.dev3/tableau_helpers/server.py` & `tableau-helpers-2.0.5.dev4/tableau_helpers/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             server.use_server_version()
         else:
             server.version = tableau_api_version
 
         auth = TSC.PersonalAccessTokenAuth(
             token_name=token_name,
             personal_access_token=personal_access_token,
-            site_id="",
+            site_id=os.getenv("TABLEAU_SITE", "")
         )
         server.auth.sign_in_with_personal_access_token(auth)
         return server
 
     def get_project_id(
         self,
         project_name: str,
@@ -93,23 +93,22 @@
         project_name_remainder = None
         if project_name.find("/") > 0:
             project_name_parts = project_name.split("/", 1)
             project_name = project_name_parts[0]
             project_name_remainder = project_name_parts[1]
         req_option = TSC.RequestOptions()
         proj_filter = TSC.Filter(
-                TSC.RequestOptions.Field.Name,
-                TSC.RequestOptions.Operator.Equals,
-                project_name,)
+            TSC.RequestOptions.Field.Name,
+            TSC.RequestOptions.Operator.Equals,
+            project_name,
+        )
         req_option.filter.add(proj_filter)
         projects, _ = server.projects.get(req_option)
         if parent_id is not None:
-            projects = [
-                x for x in projects if x.parent_id == parent_id
-            ]
+            projects = [x for x in projects if x.parent_id == parent_id]
         # it isn't clear if tableau can return multiple projects with the same name
         # we should avoid unintentional writing to the wrong project
         if len(projects) > 1:
             raise MultipleProjectsShareNameException(project_name, projects)
         elif len(projects) < 1:
             # try finding a matching id instead of name as a backup
             projects = [x for x in projects if x.id == project_name]
@@ -126,17 +125,18 @@
         return self.get_project_id(project_name_remainder, project_id)
 
     def get_flow(self, project_name, flow_name) -> Optional[TSC.FlowItem]:
         project_id: str = self.get_project_id(project_name)
         flows: list[TSC.FlowItem]
         req_option = TSC.RequestOptions()
         flow_filter = TSC.Filter(
-                TSC.RequestOptions.Field.Name,
-                TSC.RequestOptions.Operator.Equals,
-                flow_name,)
+            TSC.RequestOptions.Field.Name,
+            TSC.RequestOptions.Operator.Equals,
+            flow_name,
+        )
         req_option.filter.add(flow_filter)
         flows, _ = self.server.flows.get(req_option)
         for flow in flows:
             if flow.project_id == project_id:
                 return flow
         return None
```

### Comparing `tableau-helpers-2.0.5.dev3/tableau_helpers/utils.py` & `tableau-helpers-2.0.5.dev4/tableau_helpers/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,9 +37,7 @@
             result = download_file(url=arg)
         else:
             result = Path(arg)
     else:
         raise TypeError
 
     return result
-
-
```

### Comparing `tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/PKG-INFO` & `tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tableau-helpers
-Version: 2.0.5.dev3
+Version: 2.0.5.dev4
 Summary: A collection of helpers to reduce boilerplate with Tableau APIs.
 License: MIT License
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 # tableau_helpers
 
 A wrapper for the tableau-server-client and hyper-api which abstracts away
 boilerplate and in some cases provides a CLI which works without admin privileges.
```

### Comparing `tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/SOURCES.txt` & `tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 .env.sample
-.flake8
 .gitignore
-.pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 tox.ini
 tableau_helpers/__init__.py
 tableau_helpers/hyper.py
 tableau_helpers/server.py
```

### Comparing `tableau-helpers-2.0.5.dev3/tests/cli/test_csv_to_hyper.py` & `tableau-helpers-2.0.5.dev4/tests/cli/test_csv_to_hyper.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,10 +29,10 @@
         "--csv",
         tsv,
         "--table-def",
         table_def,
         "--dest",
         Path(tmp_path, "tmp.hyper").absolute().as_posix(),
         "--delimiter",
-        '\t'
+        "\t",
     ]
     main(args)
```

### Comparing `tableau-helpers-2.0.5.dev3/tests/cli/test_upload_hyper.py` & `tableau-helpers-2.0.5.dev4/tests/cli/test_upload_hyper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from pathlib import Path
-
 import pytest
 
 from tableau_helpers.cli.upload_hyper import main
 from tests import conftest
 
 
-@pytest.mark.parametrize(
-    "hyperfile,project", [(conftest.good_hyper_path(), "ApiTest")]
-)
+@pytest.mark.parametrize("hyperfile,project", [(conftest.good_hyper_path(), "ApiTest")])
 def test_upload_hyper(hyperfile, project):
     args = [
         "--hyperfile",
         hyperfile,
         "--dest",
         project,
     ]
     main(args)
 
+
 @pytest.mark.parametrize(
     "hyperfile,project,new_name", [(conftest.good_hyper_path(), "ApiTest", "new-name")]
 )
 def test_upload_hyper_rename(hyperfile, project, new_name):
     args = [
         "--hyperfile",
         hyperfile,
```

### Comparing `tableau-helpers-2.0.5.dev3/tests/conftest.py` & `tableau-helpers-2.0.5.dev4/tests/conftest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     load_dotenv()
 
 
 def good_csv_path():
     return os.path.abspath("tests/resources/good_default_format.csv")
 
 
-
 def good_csv2_path():
     return os.path.abspath("tests/resources/good_default_format2.csv")
 
+
 def good_left_path():
     return os.path.abspath("tests/resources/good_left.csv")
 
 
 def good_right_path():
     return os.path.abspath("tests/resources/good_left.csv")
 
@@ -65,8 +65,8 @@
 
 
 def good_hyper_path():
     return os.path.abspath("tests/resources/good_default_format.hyper")
 
 
 def joined_hyper_path():
-    return os.path.abspath("tests/resources/joined.hyper")
+    return os.path.abspath("tests/resources/joined.hyper")
```

### Comparing `tableau-helpers-2.0.5.dev3/tests/resources/good_default_format.hyper` & `tableau-helpers-2.0.5.dev4/tests/resources/good_default_format.hyper`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev3/tests/resources/good_join_table_def.json` & `tableau-helpers-2.0.5.dev4/tests/resources/good_join_table_def.json`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev3/tests/resources/joined.hyper` & `tableau-helpers-2.0.5.dev4/tests/resources/joined.hyper`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev3/tests/test_hyper.py` & `tableau-helpers-2.0.5.dev4/tests/test_hyper.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     assert linecount == 2
 
 
 def test_create_hyper_from_default_tab_path_str(
     tmp_path, csv_path=ct.good_tab_path(), csv_schema=ct.good_csv_schema()
 ):
     tmp_hyper_file = Path(tmp_path, "tmp.hyper")
-    linecount = hyper.copy_csv_to_hyper(tmp_hyper_file, Path(csv_path), csv_schema, delimiter='\t')
+    linecount = hyper.copy_csv_to_hyper(
+        tmp_hyper_file, Path(csv_path), csv_schema, delimiter="\t"
+    )
     assert linecount == 2
 
 
 def test_fail_create_hyper_from_default_tab_path_str(
     tmp_path, csv_path=ct.good_tab_path(), csv_schema=ct.good_csv_schema()
 ):
     tmp_hyper_file = Path(tmp_path, "tmp.hyper")
```

### Comparing `tableau-helpers-2.0.5.dev3/tests/test_server.py` & `tableau-helpers-2.0.5.dev4/tests/test_server.py`

 * *Files identical despite different names*

