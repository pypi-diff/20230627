# Comparing `tmp/gpt_code_search-0.0.6.tar.gz` & `tmp/gpt_code_search-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_search-0.0.6.tar", max compression
+gzip compressed data, was "gpt_code_search-0.0.7.tar", max compression
```

## Comparing `gpt_code_search-0.0.6.tar` & `gpt_code_search-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.6/LICENSE
--rw-r--r--   0        0        0     7511 2023-06-26 14:56:05.849955 gpt_code_search-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.6/core/__init__.py
--rw-r--r--   0        0        0     6035 2023-06-26 02:41:46.649895 gpt_code_search-0.0.6/core/ai.py
--rw-r--r--   0        0        0     1104 2023-06-25 22:07:30.429077 gpt_code_search-0.0.6/core/analytics.py
--rw-r--r--   0        0        0     2911 2023-06-25 19:52:46.261474 gpt_code_search-0.0.6/core/config.py
--rw-r--r--   0        0        0     7637 2023-06-26 02:43:17.380254 gpt_code_search-0.0.6/core/functions.py
--rw-r--r--   0        0        0     3072 2023-06-25 22:44:27.362555 gpt_code_search-0.0.6/core/main.py
--rw-r--r--   0        0        0        0 2023-06-26 01:55:02.493714 gpt_code_search-0.0.6/core/tests/__init__.py
--rw-r--r--   0        0        0      968 2023-06-26 14:44:25.615029 gpt_code_search-0.0.6/core/tests/test_truncate_text.py
--rw-r--r--   0        0        0     1258 2023-06-26 15:49:06.690608 gpt_code_search-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     8870 1970-01-01 00:00:00.000000 gpt_code_search-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.7/LICENSE
+-rw-r--r--   0        0        0     7511 2023-06-26 14:56:05.849955 gpt_code_search-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.7/core/__init__.py
+-rw-r--r--   0        0        0     6035 2023-06-26 02:41:46.649895 gpt_code_search-0.0.7/core/ai.py
+-rw-r--r--   0        0        0     1104 2023-06-25 22:07:30.429077 gpt_code_search-0.0.7/core/analytics.py
+-rw-r--r--   0        0        0     2911 2023-06-25 19:52:46.261474 gpt_code_search-0.0.7/core/config.py
+-rw-r--r--   0        0        0     7637 2023-06-26 02:43:17.380254 gpt_code_search-0.0.7/core/functions.py
+-rw-r--r--   0        0        0     3207 2023-06-26 16:06:16.220339 gpt_code_search-0.0.7/core/main.py
+-rw-r--r--   0        0        0        0 2023-06-26 01:55:02.493714 gpt_code_search-0.0.7/core/tests/__init__.py
+-rw-r--r--   0        0        0      968 2023-06-26 14:44:25.615029 gpt_code_search-0.0.7/core/tests/test_truncate_text.py
+-rw-r--r--   0        0        0     1292 2023-06-26 16:07:58.890001 gpt_code_search-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8870 1970-01-01 00:00:00.000000 gpt_code_search-0.0.7/PKG-INFO
```

### Comparing `gpt_code_search-0.0.6/LICENSE` & `gpt_code_search-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.6/README.md` & `gpt_code_search-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.6/core/ai.py` & `gpt_code_search-0.0.7/core/ai.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.6/core/analytics.py` & `gpt_code_search-0.0.7/core/analytics.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.6/core/config.py` & `gpt_code_search-0.0.7/core/config.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.6/core/functions.py` & `gpt_code_search-0.0.7/core/functions.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.6/core/main.py` & `gpt_code_search-0.0.7/core/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,24 +84,27 @@
     """
     Opt out of anonymous usage analytics and crash reports.
     """
     save_opt_out_of_analytics()
     console.print("You have opted out of anonymous usage analytics and crash reports.")
 
 
-@app.callback()
-def callback():
+@app.callback(invoke_without_command=True)
+def callback(ctx: typer.Context):
     if not os.path.exists(CONFIG_FILE_PATH):
         logging.info("Creating default config file...")
         create_or_update_with_default_config()
 
     console.print(
         "\nTip: Mention specific file names in your query for the best results. "
         "Run this CLI closer to the directory or file for more accurate answers. The max depth is 5 levels.\n",
         style="bold yellow",
     )
     if not os.getenv("LOCAL_DEV"):
         configure_deps()
 
+    if ctx.invoked_subcommand is None:
+        typer.main.get_command(app).get_help(ctx)
+
 
 if __name__ == "__main__":
     app()
```

### Comparing `gpt_code_search-0.0.6/core/tests/test_truncate_text.py` & `gpt_code_search-0.0.7/core/tests/test_truncate_text.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.6/pyproject.toml` & `gpt_code_search-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-code-search"
-version = "0.0.6"
+version = "0.0.7"
 description = "gpt-code-search enables you to search your codebase with natural language."
 authors = ["narenmanoharan <narenkmanoharan@gmail.com>", "skovy <smiskoviak@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "core"}]
 homepage = "https://wolfia.com"
 repository = "https://github.com/wolfia-app/gpt-code-search"
@@ -12,14 +12,15 @@
 
 [tool.poetry.urls]
 issues = "https://github.com/wolfia-app/gpt-code-search/issues"
 discussions = "https://github.com/wolfia-app/gpt-code-search/discussions"
 wiki = "https://github.com/wolfia-app/gpt-code-search/wiki"
 
 [tool.poetry.scripts]
+gpt-code-search = "core.main:app"
 gcs = "core.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.8.17"
 typer = {extras = ["all"], version = "^0.9.0"}
 rich = "^13.4.2"
 tiktoken = "^0.4.0"
```

### Comparing `gpt_code_search-0.0.6/PKG-INFO` & `gpt_code_search-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-code-search
-Version: 0.0.6
+Version: 0.0.7
 Summary: gpt-code-search enables you to search your codebase with natural language.
 Home-page: https://wolfia.com
 License: Apache-2.0
 Keywords: gpt,code,search,wolfia,gpt4,llm
 Author: narenmanoharan
 Author-email: narenkmanoharan@gmail.com
 Requires-Python: >=3.8.17,<4.0.0
```

