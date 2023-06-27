# Comparing `tmp/iamactionhunter-1.0.1.tar.gz` & `tmp/iamactionhunter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamactionhunter-1.0.1.tar", max compression
+gzip compressed data, was "iamactionhunter-1.0.2.tar", max compression
```

## Comparing `iamactionhunter-1.0.1.tar` & `iamactionhunter-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11179 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/IAMActionHunter/IAMActionHunter.py
--rw-r--r--   0        0        0        0 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/IAMActionHunter/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/IAMActionHunter/configs/__init.py__
--rw-r--r--   0        0        0     5970 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/IAMActionHunter/configs/all.py
--rw-r--r--   0        0        0        0 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/IAMActionHunter/lib/__init__.py
--rw-r--r--   0        0        0     1973 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/IAMActionHunter/lib/create_csv.py
--rw-r--r--   0        0        0     6108 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/IAMActionHunter/lib/data_collection.py
--rw-r--r--   0        0        0     5220 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/IAMActionHunter/lib/statement_parser.py
--rw-r--r--   0        0        0      433 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/IAMActionHunter/lib/text_formatter.py
--rw-r--r--   0        0        0    11357 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/LICENSE
--rw-r--r--   0        0        0     4111 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/README.md
--rw-r--r--   0        0        0      882 2023-06-23 16:43:04.215251 iamactionhunter-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 iamactionhunter-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11430 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/IAMActionHunter/IAMActionHunter.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/IAMActionHunter/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/IAMActionHunter/configs/__init.py__
+-rw-r--r--   0        0        0     5970 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/IAMActionHunter/configs/all.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/IAMActionHunter/lib/__init__.py
+-rw-r--r--   0        0        0     1973 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/IAMActionHunter/lib/create_csv.py
+-rw-r--r--   0        0        0     6108 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/IAMActionHunter/lib/data_collection.py
+-rw-r--r--   0        0        0     5220 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/IAMActionHunter/lib/statement_parser.py
+-rw-r--r--   0        0        0      433 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/IAMActionHunter/lib/text_formatter.py
+-rw-r--r--   0        0        0    11357 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4183 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/README.md
+-rw-r--r--   0        0        0      882 2023-06-27 16:11:11.566816 iamactionhunter-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 iamactionhunter-1.0.2/PKG-INFO
```

### Comparing `iamactionhunter-1.0.1/IAMActionHunter/IAMActionHunter.py` & `iamactionhunter-1.0.2/IAMActionHunter/IAMActionHunter.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,22 +165,30 @@
     output to the console and CSV file if specified
     Args: policy_file (string): file name to process
     Args: cli_args (object): command line arguments
     returns: None
     """
     query_results = {}
     query = config["ActionsNeeded"]
+    all_or_none = config["AllOrNone"]
 
     # Expand the actions for the query actions to a list
     query = Statement({"Action": query}).actions_expanded
 
     for action in query:
         if permissions_json.get(action):
             query_results.update({action: permissions_json.get(action)})
 
+    # If the AllOrNone is true, check if all actions are allowed
+    if all_or_none:
+        if all(item in query_results for item in query):
+            pass
+        else:
+            query_results = {}
+
     # Write CSV file if specified
     if cli_args.csv:
         process_json_and_append_to_csv(query_results, cli_args.csv, principal_type_name)
 
     if query_results:
         print(f"{color.green('[+]')} {color.green(principal_type_name)} vulnerable to {color.green(config['Name'])}:")
         for action in query_results:
```

### Comparing `iamactionhunter-1.0.1/IAMActionHunter/configs/all.py` & `iamactionhunter-1.0.2/IAMActionHunter/configs/all.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.1/IAMActionHunter/lib/create_csv.py` & `iamactionhunter-1.0.2/IAMActionHunter/lib/create_csv.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.1/IAMActionHunter/lib/data_collection.py` & `iamactionhunter-1.0.2/IAMActionHunter/lib/data_collection.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.1/IAMActionHunter/lib/statement_parser.py` & `iamactionhunter-1.0.2/IAMActionHunter/lib/statement_parser.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.1/LICENSE` & `iamactionhunter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.1/README.md` & `iamactionhunter-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,30 @@
 
 ## Blue Team Use
 This tool also offers the ability to output and save query results in a CSV format, which is beneficial for security teams seeking a high-level overview of principal permissions and resources within an AWS account. For instance, you may want to identify users and roles with `iam:put*` permissions in an account. By executing a query and generating a CSV, you can easily review all users and roles with these permissions, along with the resources they have access to.
 
 # Installation
 Much of this functionality has also been implemented into https://github.com/RhinoSecurityLabs/pacu as a module, `iam__enum_action_query` if you prefer that.
 
-Suggested Setup:
+Suggested:
+```
+pip3 install iamactionhunter
+```
+
+
+Clone and use Poetry:
 ```
 git clone https://github.com/RhinoSecurityLabs/IAMActionHunter.git
 cd IAMActionHunter
 poetry install
 iamactionhunter --help
 iamactionhunter --collect --profile <some-aws-profile>
 ```
 
-Or pip:
+Clone and use Pip:
 ```
 git clone https://github.com/RhinoSecurityLabs/IAMActionHunter.git
 cd IAMActionHunter
 pip install .
 iamactionhunter --help
 iamactionhunter --collect --profile <some-aws-profile>
 ```
```

### Comparing `iamactionhunter-1.0.1/pyproject.toml` & `iamactionhunter-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "IAMActionHunter"
-version = "1.0.1"
+version = "1.0.2"
 description = "A query tool for AWS IAM policy statements."
 authors = ["Dave Yesland with Rhino Security Labs"]
 readme = "README.md"
 packages = [{include = "IAMActionHunter"},{include="lib", from="IAMActionHunter"},{include="configs", from="IAMActionHunter"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `iamactionhunter-1.0.1/PKG-INFO` & `iamactionhunter-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamactionhunter
-Version: 1.0.1
+Version: 1.0.2
 Summary: A query tool for AWS IAM policy statements.
 Author: Dave Yesland with Rhino Security Labs
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -22,24 +22,30 @@
 
 ## Blue Team Use
 This tool also offers the ability to output and save query results in a CSV format, which is beneficial for security teams seeking a high-level overview of principal permissions and resources within an AWS account. For instance, you may want to identify users and roles with `iam:put*` permissions in an account. By executing a query and generating a CSV, you can easily review all users and roles with these permissions, along with the resources they have access to.
 
 # Installation
 Much of this functionality has also been implemented into https://github.com/RhinoSecurityLabs/pacu as a module, `iam__enum_action_query` if you prefer that.
 
-Suggested Setup:
+Suggested:
+```
+pip3 install iamactionhunter
+```
+
+
+Clone and use Poetry:
 ```
 git clone https://github.com/RhinoSecurityLabs/IAMActionHunter.git
 cd IAMActionHunter
 poetry install
 iamactionhunter --help
 iamactionhunter --collect --profile <some-aws-profile>
 ```
 
-Or pip:
+Clone and use Pip:
 ```
 git clone https://github.com/RhinoSecurityLabs/IAMActionHunter.git
 cd IAMActionHunter
 pip install .
 iamactionhunter --help
 iamactionhunter --collect --profile <some-aws-profile>
 ```
```

