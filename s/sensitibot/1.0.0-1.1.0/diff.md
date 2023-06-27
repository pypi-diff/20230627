# Comparing `tmp/sensitibot-1.0.0.tar.gz` & `tmp/sensitibot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensitibot-1.0.0.tar", max compression
+gzip compressed data, was "sensitibot-1.1.0.tar", max compression
```

## Comparing `sensitibot-1.0.0.tar` & `sensitibot-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0        0 2023-04-21 02:12:15.225562 sensitibot-1.0.0/cleaner/__init__.py
--rw-r--r--   0        0        0     2392 2023-05-29 16:21:53.061005 sensitibot-1.0.0/cleaner/access_cleaner.py
--rw-r--r--   0        0        0     3783 2023-06-07 16:27:09.150277 sensitibot-1.0.0/cleaner/cleaner.py
--rw-r--r--   0        0        0     1176 2023-05-28 17:57:03.644191 sensitibot-1.0.0/cleaner/csv_cleaner.py
--rw-r--r--   0        0        0     1691 2023-05-28 17:57:03.651175 sensitibot-1.0.0/cleaner/excel_cleaner.py
--rw-r--r--   0        0        0     1343 2023-06-07 17:21:47.954890 sensitibot-1.0.0/cleaner/json_cleaner.py
--rw-r--r--   0        0        0     1948 2023-06-07 16:07:22.689625 sensitibot-1.0.0/cleaner/show_matches.py
--rw-r--r--   0        0        0     1177 2023-05-28 17:57:03.659153 sensitibot-1.0.0/cleaner/tsv_cleaner.py
--rw-r--r--   0        0        0        0 2023-04-21 02:12:15.225562 sensitibot-1.0.0/github/__init__.py
--rw-r--r--   0        0        0     8928 2023-06-06 18:30:15.703957 sensitibot-1.0.0/github/github.py
--rw-r--r--   0        0        0        0 2023-04-21 02:12:15.228547 sensitibot-1.0.0/local/__init__.py
--rw-r--r--   0        0        0     1783 2023-06-06 17:27:19.895672 sensitibot-1.0.0/local/local.py
--rw-r--r--   0        0        0      996 2023-06-08 13:07:12.584645 sensitibot-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 02:12:15.232535 sensitibot-1.0.0/reader/__init__.py
--rw-r--r--   0        0        0     4355 2023-05-29 23:21:40.469735 sensitibot-1.0.0/reader/access_reader.py
--rw-r--r--   0        0        0     1701 2023-05-31 13:33:36.329605 sensitibot-1.0.0/reader/columns_reader.py
--rw-r--r--   0        0        0     1286 2023-05-29 21:39:14.941841 sensitibot-1.0.0/reader/csv_reader.py
--rw-r--r--   0        0        0     3038 2023-06-06 18:47:19.887583 sensitibot-1.0.0/reader/excel_reader.py
--rw-r--r--   0        0        0     1272 2023-05-29 22:50:04.921218 sensitibot-1.0.0/reader/headers_reader.py
--rw-r--r--   0        0        0     1329 2023-06-06 18:43:24.200256 sensitibot-1.0.0/reader/json_reader.py
--rw-r--r--   0        0        0     3628 2023-06-06 18:57:14.728022 sensitibot-1.0.0/reader/reader.py
--rw-r--r--   0        0        0     1286 2023-05-29 21:39:19.588222 sensitibot-1.0.0/reader/tsv_reader.py
--rw-r--r--   0        0        0      628 2023-06-07 16:22:07.034962 sensitibot-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-04-21 02:12:15.234530 sensitibot-1.0.0/renderer/__init__.py
--rw-r--r--   0        0        0     1602 2023-06-06 15:52:11.486925 sensitibot-1.0.0/renderer/renderer.py
--rw-r--r--   0        0        0        0 2023-04-21 02:12:15.238520 sensitibot-1.0.0/sensitibot/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 02:12:15.239516 sensitibot-1.0.0/sensitibot/__main__.py
--rw-r--r--   0        0        0     1084 2023-05-31 23:15:28.194785 sensitibot-1.0.0/sensitibot/custom_formatters.py
--rw-r--r--   0        0        0     3302 2023-06-06 16:03:52.940836 sensitibot-1.0.0/sensitibot/sensitibot.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 sensitibot-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.779840 sensitibot-1.1.0/cleaner/__init__.py
+-rw-r--r--   0        0        0     2466 2023-06-12 19:54:58.518829 sensitibot-1.1.0/cleaner/access_cleaner.py
+-rw-r--r--   0        0        0     3396 2023-06-25 16:06:00.250762 sensitibot-1.1.0/cleaner/cleaner.py
+-rw-r--r--   0        0        0     1176 2023-06-12 19:53:18.780838 sensitibot-1.1.0/cleaner/csv_cleaner.py
+-rw-r--r--   0        0        0     1691 2023-06-12 19:53:18.781837 sensitibot-1.1.0/cleaner/excel_cleaner.py
+-rw-r--r--   0        0        0     1343 2023-06-12 19:54:58.519830 sensitibot-1.1.0/cleaner/json_cleaner.py
+-rw-r--r--   0        0        0     1948 2023-06-12 19:54:58.519830 sensitibot-1.1.0/cleaner/show_matches.py
+-rw-r--r--   0        0        0     1177 2023-06-12 19:53:18.782840 sensitibot-1.1.0/cleaner/tsv_cleaner.py
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.782840 sensitibot-1.1.0/github/__init__.py
+-rw-r--r--   0        0        0     8713 2023-06-25 15:30:27.861844 sensitibot-1.1.0/github/github.py
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.783839 sensitibot-1.1.0/local/__init__.py
+-rw-r--r--   0        0        0     1383 2023-06-25 15:30:40.284141 sensitibot-1.1.0/local/local.py
+-rw-r--r--   0        0        0      997 2023-06-27 15:38:05.601306 sensitibot-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.787841 sensitibot-1.1.0/reader/__init__.py
+-rw-r--r--   0        0        0     4365 2023-06-12 19:54:58.523829 sensitibot-1.1.0/reader/access_reader.py
+-rw-r--r--   0        0        0     1701 2023-06-12 19:53:18.788840 sensitibot-1.1.0/reader/columns_reader.py
+-rw-r--r--   0        0        0     1286 2023-06-12 19:53:18.789839 sensitibot-1.1.0/reader/csv_reader.py
+-rw-r--r--   0        0        0     3038 2023-06-12 19:53:18.790878 sensitibot-1.1.0/reader/excel_reader.py
+-rw-r--r--   0        0        0     1272 2023-06-12 19:53:18.790878 sensitibot-1.1.0/reader/headers_reader.py
+-rw-r--r--   0        0        0     1333 2023-06-12 19:54:58.523829 sensitibot-1.1.0/reader/json_reader.py
+-rw-r--r--   0        0        0     3458 2023-06-25 16:06:25.804932 sensitibot-1.1.0/reader/reader.py
+-rw-r--r--   0        0        0     1286 2023-06-12 19:53:18.791838 sensitibot-1.1.0/reader/tsv_reader.py
+-rw-r--r--   0        0        0      628 2023-06-22 19:08:34.082525 sensitibot-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.792844 sensitibot-1.1.0/renderer/__init__.py
+-rw-r--r--   0        0        0     1584 2023-06-22 19:19:21.522620 sensitibot-1.1.0/renderer/renderer.py
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.794840 sensitibot-1.1.0/sensitibot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 19:53:18.794840 sensitibot-1.1.0/sensitibot/__main__.py
+-rw-r--r--   0        0        0     1084 2023-06-12 19:54:58.527831 sensitibot-1.1.0/sensitibot/custom_formatters.py
+-rw-r--r--   0        0        0     2595 2023-06-22 19:08:34.146146 sensitibot-1.1.0/sensitibot/parser.py
+-rw-r--r--   0        0        0     1211 2023-06-22 19:08:34.160161 sensitibot-1.1.0/sensitibot/sensitibot.py
+-rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 sensitibot-1.1.0/PKG-INFO
```

### Comparing `sensitibot-1.0.0/cleaner/access_cleaner.py` & `sensitibot-1.1.0/cleaner/access_cleaner.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
     try:
         connection_string = (
             r"DRIVER={Microsoft Access Driver (*.mdb, *.accdb)};" +
             r"DBQ={};".format(new_filename) +
             r"ExtendedAnsiSQL=1;"
         )
-        connection_url = sa.engine.URL.create("access+pyodbc", query={"odbc_connect": connection_string})
+        connection_url = sa.engine.URL.create(
+            "access+pyodbc", query={"odbc_connect": connection_string})
         engine = sa.create_engine(connection_url)
     except Exception as e:
         error = {"file": new_filename, "error": str(e)}
 
     for positive_table in positive_tables:
         positive_name = positive_table["name"] if "name" in positive_table else ""
         positive_headers = positive_table["positive_headers"] if "positive_headers" in positive_table else [
@@ -48,21 +49,25 @@
         positive_columns = positive_table["positive_columns"] if "positive_columns" in positive_table else dict(
         )
 
         deleted_columns = []
 
         for positive_header in positive_headers:
             if positive_header not in deleted_columns:
-                delete_column(new_filename, positive_table["name"], positive_header, engine)
+                delete_column(
+                    new_filename, positive_table["name"], positive_header, engine)
                 deleted_columns.append(positive_header)
 
         for positive_column in positive_columns.keys():
             if positive_column not in deleted_columns:
-                delete_column(new_filename, positive_table["name"], positive_column, engine)
+                delete_column(
+                    new_filename, positive_table["name"], positive_column, engine)
                 deleted_columns.append(positive_column)
 
     engine.dispose()
 
+
 def delete_column(filename, table_name, column_name, engine):
     # If the column exists, remove it from the table
     with engine.begin() as connection:
-        connection.execute(sa.text(f'ALTER TABLE "{table_name}" DROP COLUMN "{column_name}"'))
+        connection.execute(
+            sa.text(f'ALTER TABLE "{table_name}" DROP COLUMN "{column_name}"'))
```

### Comparing `sensitibot-1.0.0/cleaner/cleaner.py` & `sensitibot-1.1.0/cleaner/cleaner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from tqdm import tqdm
-
-from cleaner import access_cleaner, csv_cleaner, excel_cleaner, json_cleaner, show_matches, tsv_cleaner
+from cleaner import (csv_cleaner, excel_cleaner, json_cleaner, show_matches,
+                     tsv_cleaner)
 
 
 def process_cleaner(files):
     generate_clean_files = input(
         "\nDo you want to generate clean files? (yes/no): ")
     while generate_clean_files.lower() not in ("yes", "no"):
         generate_clean_files = input("Please enter either 'yes' or 'no': ")
@@ -21,18 +20,15 @@
         replace_files (bool): If true, the files will be replaced by the clean ones.
 
     Returns:
         None.
     """
     repository = files["repositories"][0]
 
-    # pbar = tqdm(repository["files"],
-    #             desc="Cleaning files", ncols=300, unit=" repo", bar_format="\tCleaning file {n_fmt}/{total_fmt} |{bar:20}| f:{desc}")
     for file in repository["files"]:
-        # pbar.set_description(file["name"][-50:])
         clean_file(file)
 
 
 def clean_file(file):
     """
     Cleans the file.
 
@@ -67,17 +63,14 @@
         if file["name"].endswith('.tsv'):
             tsv_cleaner.clean_tsv_file(file, replace)
 
         excel_extensions = [".xlsx", ".xlsm", ".xltx", ".xltm"]
         if any(file["name"].endswith(ext) for ext in excel_extensions):
             excel_cleaner.clean_excel_file(file, replace)
 
-        if file["name"].endswith('.mdb') or file["name"].endswith('.accdb'):
-            access_cleaner.clean_access_file(file, replace)
-
         if file["name"].endswith('.json') or file["name"].endswith('.jsonl'):
             json_cleaner.clean_json_file(file, replace)
 
 
 def ask_clean_file():
     """
     Asks the user if he wants to clean the file.
```

### Comparing `sensitibot-1.0.0/cleaner/csv_cleaner.py` & `sensitibot-1.1.0/cleaner/csv_cleaner.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/cleaner/excel_cleaner.py` & `sensitibot-1.1.0/cleaner/excel_cleaner.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/cleaner/json_cleaner.py` & `sensitibot-1.1.0/cleaner/json_cleaner.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/cleaner/show_matches.py` & `sensitibot-1.1.0/cleaner/show_matches.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/cleaner/tsv_cleaner.py` & `sensitibot-1.1.0/cleaner/tsv_cleaner.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/github/github.py` & `sensitibot-1.1.0/github/github.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 import os
-import sys
 import urllib
 
 import requests
 from tqdm import tqdm
 
-from reader import reader
-
 api_url = 'https://api.github.com'
 raw_url = 'https://raw.githubusercontent.com'
 headers = {}
 multipleRepositories = False
 
 
-def process_github(owner, repository=None, branch=None, token=None, deep_search=False, wide_search=False):
+class GitHubAPIException(Exception):
+    def __init__(self, message):
+        self.message = message
+
+    def __str__(self):
+        return self.message
+
+
+def process_github(owner, repository=None, branch=None, token=None):
     """
     Initiates the process of getting the files from GitHub.
 
     Args:
         owner (str): The GitHub user.
         repository (str): The repository to search.
         branch (str): The branch to search.
         token (str): The GitHub token.
-        deep_search (bool): If true, the content of the files will be analyzed.
-        wide_search (bool): If true, all the tables or sheets will be analyzed.
 
     Returns:
         dict: The result of getting the files.
     """
     global multipleRepositories
     TOKEN = os.getenv("GITHUB_TOKEN", default=None)
     if token != None:
         TOKEN = token
 
     if TOKEN != None:
         headers['Authorization'] = f'Bearer {TOKEN}'
 
     files = {}
-    result = {}
     if repository == None:
         multipleRepositories = True
         files = get_files_from_repositories(owner)
     else:
-        print(f'Searching repositoriy {owner}/{repository}:')
+        print(f'Searching repository {owner}/{repository}:')
         files = get_files_from_repository(owner, repository, branch)
         if files != None:
             files = {"repositories": [files]}
 
     if files == None:
         print("\nNo dataset files found")
         return None
 
-    result = reader.process_files(files, deep_search, wide_search)
-    if result == None:
-        print("\nYour files are clean!")
-        return None
-
-    return result
+    return files
 
 
 def get_files_from_repositories(owner):
     """
     Gets the files from all repositories of the GitHub user.
 
     Args:
@@ -79,14 +76,15 @@
 
     result = {"repositories": []}
 
     number_of_repos = len(json_repos)
     remaining = get_rate_limit()
     if remaining <= number_of_repos:
         number_of_repos = remaining
+        json_repos = json_repos[:number_of_repos]
         print(
             f'Warning: Only {number_of_repos} repositories will be analyzed, because the GitHub API rate limit has been exceeded.')
 
     pbar = tqdm(json_repos,
                 desc="Reading repositories", ncols=200, unit=" repo", ascii=' █', bar_format="Reading repository {n_fmt}/{total_fmt} |{bar:20}| r:{desc}")
     for repository in pbar:
         pbar.set_description(repository["name"])
@@ -121,19 +119,18 @@
     while count == per_page:
         response = requests.get(
             f'{api_url}/users/{owner}/repos?page={page}&per_page={per_page}', headers=headers)
         if not response.ok:
             error = response.json()
             error_message = error.get('message')
             if error_message == "Not Found":
-                print(f'Error: Github User or Organization {error_message}\n')
-                sys.exit(1)  # exit with non-zero exit code
+                raise GitHubAPIException(
+                    f'Error: Github User or Organization {error_message}')
             elif error_message == "Bad credentials":
-                print("Error: Bad credentials\n")
-                sys.exit(1)  # exit with non-zero exit code
+                raise GitHubAPIException("Error: Bad credentials")
             elif "API rate limit exceeded" in error_message:
                 if page == 1:   # If the first request has already exceeded the rate limit, we can't continue
                     print(
                         "API rate limit exceeded, could not analyze GitHub user or organization.")
                     return None
                 else:           # If the rate limit has been exceeded after the first request, we can continue with the repositories already found
                     print(
@@ -154,14 +151,20 @@
     """
     Gets the rate limit from the GitHub API.
 
     Returns:
         int: The rate limit from the GitHub API.
     """
     response = requests.get(f'{api_url}/rate_limit', headers=headers)
+    if not response.ok:
+        error = response.json()
+        error_message = error.get('message')
+        if error_message == "Bad credentials":
+            raise GitHubAPIException("Error: Bad credentials")
+
     json_data = response.json()
     return json_data["rate"]["remaining"]
 
 
 def get_files_from_repository(owner, repository, branch=None):
     """
     Gets the files from the GitHub repository.
@@ -183,19 +186,17 @@
     if not response.ok:
         error = response.json()
         error_message = error.get('message')
         if error_message == "Not Found":
             if multipleRepositories:
                 return None
             else:
-                print(f'Error: Repository {error_message}\n')
-                sys.exit(1)  # exit with non-zero exit code
+                raise GitHubAPIException(f'Error: Repository {error_message}')
         elif error_message == "Bad credentials":
-            print("Error: Bad credentials\n")
-            sys.exit(1)  # exit with non-zero exit code
+            raise GitHubAPIException("Error: Bad credentials")
         elif error_message == "Git Repository is empty.":
             return None
         elif "API rate limit exceeded" in error_message:
             print("API rate limit exceeded")
             return None
 
     json_files = response.json()
@@ -221,19 +222,18 @@
     if not response.ok:
         error = response.json()
         error_message = error.get('message')
         if error_message == "Not Found":
             if multipleRepositories:
                 return None
             else:
-                print(f'Error: Repository {error_message}\n')
-                sys.exit(1)  # exit with non-zero exit code
+                raise GitHubAPIException(
+                    f'Error: Repository {error_message}')
         elif error_message == "Bad credentials":
-            print("Error: Bad credentials\n")
-            sys.exit(1)  # exit with non-zero exit code
+            raise GitHubAPIException("Error: Bad credentials")
         elif "API rate limit exceeded" in error_message:
             print(
                 "API rate limit exceeded, not all repositories have been analyzed.")
             return None
 
     json_repo = response.json()
     return json_repo["default_branch"]
@@ -250,15 +250,15 @@
 
     Returns:
         dict: The data sets files from the GitHub repository.
     """
     result_repository = {"name": repository, "files": []}
 
     extensions = [".csv", ".tsv", ".xlsx", "xlsm", "xltx",
-                  "xltm", ".mdb", ".accdb", ".json", ".jsonl"]
+                  "xltm", ".json", ".jsonl"]
 
     for file in json_files["tree"]:
         if (file["type"] == "blob"):
 
             if any(file["path"].endswith(ext) for ext in extensions):
                 result_repository["files"].append(
                     urllib.parse.quote(f'{raw_url}/{owner}/{repository}/master/{file["path"]}', safe=':/.'))
```

### Comparing `sensitibot-1.0.0/local/local.py` & `sensitibot-1.1.0/local/local.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 import os
 
-from reader import reader
 
-
-def process_local(directory=None, deep_search=False, wide_search=False):
+def process_local(directory=None):
     """
     Initiates the process of getting the files from the local repository.
 
     Args:
         directory (str): The directory to search.
-        deep_search (bool): If true, the content of the files will be analyzed.
-        wide_search (bool): If true, all the tables or sheets will be analyzed.
 
     Returns:
         dict: The result of getting the files.
     """
     files = get_files_recursively(directory)
 
     if files == None:
         print("\nNo dataset files found")
         return None
 
-    result = reader.process_files(files, deep_search, wide_search)
-    if result == None:
-        print("\nYour files are clean!")
-        return None
-
-    return result
+    return files
 
 
-def get_files_recursively(directory):
+def get_files_recursively(directory=None):
     """
     Gets the files from the local directory.
 
     Args:
         directory (str): The directory to search.
 
     Returns:
@@ -41,15 +32,15 @@
     """
     if directory == None:
         directory = "./"
 
     result = {"repositories": [{"name": "local", "files": []}]}
 
     extensions = [".csv", ".tsv", ".xlsx", "xlsm", "xltx",
-                  "xltm", ".mdb", ".accdb", ".json", ".jsonl"]
+                  "xltm", ".json", ".jsonl"]
 
     print(f'Searching directory {directory}:')
 
     for root, _, files in os.walk(directory):
         for filename in files:
 
             if any(filename.endswith(ext) for ext in extensions):
```

### Comparing `sensitibot-1.0.0/pyproject.toml` & `sensitibot-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SensitiBot"
-version = "1.0.0"
+version = "1.1.0"
 description = "A Python bot to detect data leaks on public repositories"
 readme = "README.md"
 authors = ["José Manuel Martín Luque <josemanuelmartinluque@outlook.com>"]
 packages = [
     { include = "sensitibot" },
     { include = "local" },
     { include = "github" },
@@ -17,15 +17,15 @@
 python = "^3.11"
 requests = "^2.28.2"
 python-dotenv = "^1.0.0"
 pandas = "^2.0.2"
 tqdm = "^4.62.3"
 openpyxl = "^3.1.2"
 XlsxWriter = "^3.1.0"
-sqlalchemy-access = "^2.0.2"
+#sqlalchemy-access = "^2.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 sensitibot = "sensitibot.sensitibot:main"
```

### Comparing `sensitibot-1.0.0/reader/access_reader.py` & `sensitibot-1.1.0/reader/access_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import shutil
 import tempfile
+
 import pandas as pd
 import requests
 import sqlalchemy as sa
 
 from reader import columns_reader, headers_reader
 
 
@@ -26,34 +27,35 @@
     try:
         # Establish a connection to the Access database
         connection_string = (
             r"DRIVER={Microsoft Access Driver (*.mdb, *.accdb)};" +
             r"DBQ={};".format(new_file) +
             r"ExtendedAnsiSQL=1;"
         )
-        connection_url = sa.engine.URL.create("access+pyodbc", query={"odbc_connect": connection_string})
+        connection_url = sa.engine.URL.create(
+            "access+pyodbc", query={"odbc_connect": connection_string})
         engine = sa.create_engine(connection_url)
     except Exception as e:
         error = {"file": file, "error": str(e)}
         return None, error
 
     try:
         # Query to retrieve table names
         inspector = sa.inspect(engine)
         table_names = inspector.get_table_names()
     except Exception as e:
         error = {"file": file, "error": str(e)}
         return None, error
-    
+
     tables_to_read = table_names
     if not wide_search and len(table_names) > 1:
         read_all_sheets = ask_read_all_tables(len(table_names))
         if not read_all_sheets:
             tables_to_read = ask_which_tables(table_names)
-    
+
     result_file = {"name": file}
 
     result_tables = []
     for table_name in tables_to_read:
 
         # Query to retrieve all records from the table
         query = f"SELECT * FROM {table_name}"
@@ -122,14 +124,15 @@
                 "\t\t\tPlease enter either 'yes' or 'no': ")
 
         if ask_table.lower() == "yes":
             tables_to_read.append(table_name)
 
     return tables_to_read
 
+
 def download_file(file):
     # Create a temporary file to save the downloaded Access file
     temp_file = tempfile.NamedTemporaryFile(delete=False)
     temp_file_path = temp_file.name
 
     # Download the Access file from GitHub
     response = requests.get(file, stream=True)
```

### Comparing `sensitibot-1.0.0/reader/columns_reader.py` & `sensitibot-1.1.0/reader/columns_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/reader/csv_reader.py` & `sensitibot-1.1.0/reader/csv_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/reader/excel_reader.py` & `sensitibot-1.1.0/reader/excel_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/reader/headers_reader.py` & `sensitibot-1.1.0/reader/headers_reader.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/reader/json_reader.py` & `sensitibot-1.1.0/reader/tsv_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-from reader import columns_reader, headers_reader
 import pandas as pd
 
-# Ignore warnings
-import warnings
-warnings.simplefilter(action='ignore', category=FutureWarning)
+from reader import columns_reader, headers_reader
 
 
-def read_json_file(file, deep_search=False):
+def read_tsv_file(file, deep_search=False):
     """
-    Analyzes the json file.
+    Analyzes the tsv file.
 
     Args:
         files (str): The file to analyze.
         deep_search (bool): If true, the content of the files will be analyzed.
 
     Returns:
-        dict: The result of analyzing the json file.
+        dict: The result of analyzing the tsv file.
     """
     try:
-        data = pd.read_json(file, lines=file.endswith(".jsonl"), dtype=str)
+        data = pd.read_csv(file, comment='#', sep='\t',
+                           engine='python', skip_blank_lines=True, dtype=str)
     except Exception as e:
         error = {"file": file, "error": str(e)}
-        return None, None
+        return None, error
 
     result_file = {"name": file}
 
     headers = data.columns.values
     result_headers = headers_reader.analize_headers(headers)
 
     # Only show headers that have errors
```

### Comparing `sensitibot-1.0.0/reader/reader.py` & `sensitibot-1.1.0/reader/reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from tqdm import tqdm
 
-from reader import access_reader, csv_reader, excel_reader, json_reader, tsv_reader
+from reader import csv_reader, excel_reader, json_reader, tsv_reader
 
 
 def process_files(files, deep_search=False, wide_search=False):
     """
     Initiates the process of analyzing the files.
 
     Args:
@@ -54,15 +54,19 @@
         if len(result_errors) != 0:
             result_repository["errors"] = result_errors
 
         # Only add repository if it has files with errors
         if len(result_repository) != 1:
             result["repositories"].append(result_repository)
 
-    return result if len(result['repositories']) != 0 else None
+    if len(result['repositories']) == 0:
+        print("\nYour files are clean!")
+        return None
+
+    return result
 
 
 def read_file(file, deep_search=False, wide_search=False):
     """
     Analyzes the file.
 
     Args:
@@ -83,18 +87,13 @@
 
     excel_extensions = [".xlsx", "xlsm", "xltx", "xltm"]
     if any(file.endswith(ext) for ext in excel_extensions):
         result_file, result_error = excel_reader.read_excel_file(
             file, deep_search, wide_search)
         return result_file, result_error
 
-    if file.endswith('.mdb') or file.endswith('.accdb'):
-        result_file, result_error = access_reader.read_access_file(
-            file, deep_search, wide_search)
-        return result_file, result_error
-
     if file.endswith('.json') or file.endswith('.jsonl'):
         result_file, result_error = json_reader.read_json_file(
             file, deep_search)
         return result_file, result_error
 
     return None, None
```

### Comparing `sensitibot-1.0.0/reader/tsv_reader.py` & `sensitibot-1.1.0/reader/json_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+# Ignore warnings
+import warnings
+
 import pandas as pd
 
 from reader import columns_reader, headers_reader
 
+warnings.simplefilter(action='ignore', category=FutureWarning)
+
 
-def read_tsv_file(file, deep_search=False):
+def read_json_file(file, deep_search=False):
     """
-    Analyzes the tsv file.
+    Analyzes the json file.
 
     Args:
         files (str): The file to analyze.
         deep_search (bool): If true, the content of the files will be analyzed.
 
     Returns:
-        dict: The result of analyzing the tsv file.
+        dict: The result of analyzing the json file.
     """
     try:
-        data = pd.read_csv(file, comment='#', sep='\t',
-                           engine='python', skip_blank_lines=True, dtype=str)
+        data = pd.read_json(file, lines=file.endswith(".jsonl"), dtype=str)
     except Exception as e:
         error = {"file": file, "error": str(e)}
-        return None, error
+        return None, None
 
     result_file = {"name": file}
 
     headers = data.columns.values
     result_headers = headers_reader.analize_headers(headers)
 
     # Only show headers that have errors
```

### Comparing `sensitibot-1.0.0/README.md` & `sensitibot-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/renderer/renderer.py` & `sensitibot-1.1.0/renderer/renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import datetime
-import webbrowser
+import json
 import os
 import subprocess
 import sys
 import tempfile
-import json
 
 
 def show_result_as_text(data, name, deep_search=False):
     """
     Shows the result as text.
 
     Args:
@@ -29,15 +28,15 @@
         f.write(data)
         f.close()
 
     if os.name == 'nt':  # For Windows
         subprocess.Popen(["notepad.exe", f.name])
     elif os.name == 'posix':  # For Linux and macOS
         opener = 'open' if sys.platform == 'darwin' else 'xdg-open'
-        subprocess.call([opener, f.name])
+        subprocess.Popen([opener, f.name])
     else:
         raise OSError('Unsupported operating system')
 
 
 def ask_generate_report():
     """
     Asks the user if he wants to generate a report.
```

### Comparing `sensitibot-1.0.0/sensitibot/custom_formatters.py` & `sensitibot-1.1.0/sensitibot/custom_formatters.py`

 * *Files identical despite different names*

### Comparing `sensitibot-1.0.0/sensitibot/sensitibot.py` & `sensitibot-1.1.0/sensitibot/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-import argparse
 import sys
 from importlib.metadata import version
+
 from sensitibot import custom_formatters
-from cleaner import cleaner
-from github import github
-from local import local
-from renderer import renderer
 
 
-def main():
+def parse_args(args=None):
     parser = custom_formatters.CustomArgumentParser(
         prog='sensitibot',
         description='SensitiBot is a tool to analyze datasets for sensitive information.',
         formatter_class=custom_formatters.CustomHelpFormatter
     )
 
     subparsers = parser.add_subparsers(dest='command')
@@ -45,36 +41,14 @@
     local_parser.add_argument('--wide-search', action='store_true',
                               help='analyze all tables or sheets in Office files')
 
     parser._optionals.title = "optional arguments"
     github_parser._optionals.title = "optional arguments"
     local_parser._optionals.title = "optional arguments"
 
-    args = parser.parse_args()
-
-    result = ""
-    name = ""
+    result = parser.parse_args(args)
 
-    if args.command == None:
+    if result.command == None:
         parser.print_help()
-        sys.exit(1)
-
-    if args.command == 'github':
-        name = args.user
-        result = github.process_github(
-            args.user, args.repository, args.branch, args.token, args.deep_search, args.wide_search)
-
-    if args.command == 'local':
-        name = "local"
-        result = local.process_local(
-            args.path, args.deep_search, args.wide_search)
-
-    if result == None:
-        print("")
         sys.exit(1)  # exit with non-zero exit code
 
-    renderer.show_result_as_text(result, name, args.deep_search)
-
-    if args.command == 'local':
-        cleaner.process_cleaner(result)
-
-    print("")
+    return result
```

### Comparing `sensitibot-1.0.0/PKG-INFO` & `sensitibot-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: sensitibot
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python bot to detect data leaks on public repositories
 Author: José Manuel Martín Luque
 Author-email: josemanuelmartinluque@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: XlsxWriter (>=3.1.0,<4.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: sqlalchemy-access (>=2.0.2,<3.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Documentation, https://github.com/TFG-SensitiBot/SensitiBot/wiki
 Project-URL: Homepage, https://pypi.org/project/sensitibot/
 Project-URL: Source, https://github.com/TFG-SensitiBot/SensitiBot
 Description-Content-Type: text/markdown
 
 ## Introduction
```

