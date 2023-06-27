# Comparing `tmp/cstore-0.6.1.tar.gz` & `tmp/cstore-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cstore-0.6.1.tar", last modified: Sun Jun 25 23:20:08 2023, max compression
+gzip compressed data, was "cstore-0.6.2.tar", last modified: Tue Jun 27 12:09:30 2023, max compression
```

## Comparing `cstore-0.6.1.tar` & `cstore-0.6.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:20:08.144957 cstore-0.6.1/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.6.1/LICENSE
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-25 23:20:08.144957 cstore-0.6.1/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      115 2023-06-14 08:22:10.000000 cstore-0.6.1/README.md
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:20:08.144957 cstore-0.6.1/cstore/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:12:45.000000 cstore-0.6.1/cstore/__init__.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)    15243 2023-06-25 23:19:03.000000 cstore-0.6.1/cstore/cli.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      180 2023-06-25 12:51:24.000000 cstore-0.6.1/cstore/constants.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      393 2023-06-21 10:01:53.000000 cstore-0.6.1/cstore/database.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1007 2023-06-25 23:16:51.000000 cstore-0.6.1/cstore/models.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:20:08.144957 cstore-0.6.1/cstore/repo/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-20 15:21:29.000000 cstore-0.6.1/cstore/repo/__init__.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     2908 2023-06-25 23:16:32.000000 cstore-0.6.1/cstore/repo/repo_command.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1322 2023-06-25 23:16:39.000000 cstore-0.6.1/cstore/repo/repo_tag.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1757 2023-06-25 23:16:56.000000 cstore-0.6.1/cstore/schemes.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      529 2023-06-25 14:04:16.000000 cstore-0.6.1/cstore/verbose.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-25 23:20:08.144957 cstore-0.6.1/cstore.egg-info/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      415 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/SOURCES.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/dependency_links.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/entry_points.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       74 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/requires.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-06-25 23:20:08.000000 cstore-0.6.1/cstore.egg-info/top_level.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      821 2023-06-25 23:19:11.000000 cstore-0.6.1/pyproject.toml
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-25 23:20:08.144957 cstore-0.6.1/setup.cfg
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-27 12:09:30.151234 cstore-0.6.2/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.6.2/LICENSE
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-27 12:09:30.151234 cstore-0.6.2/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      115 2023-06-14 08:22:10.000000 cstore-0.6.2/README.md
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-27 12:09:30.147234 cstore-0.6.2/cstore/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-14 11:12:45.000000 cstore-0.6.2/cstore/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)    15373 2023-06-27 12:07:33.000000 cstore-0.6.2/cstore/cli.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      180 2023-06-25 12:51:24.000000 cstore-0.6.2/cstore/constants.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      481 2023-06-27 12:02:50.000000 cstore-0.6.2/cstore/database.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1007 2023-06-25 23:16:51.000000 cstore-0.6.2/cstore/models.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-27 12:09:30.147234 cstore-0.6.2/cstore/repo/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-20 15:21:29.000000 cstore-0.6.2/cstore/repo/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     2908 2023-06-25 23:16:32.000000 cstore-0.6.2/cstore/repo/repo_command.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1322 2023-06-25 23:16:39.000000 cstore-0.6.2/cstore/repo/repo_tag.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1757 2023-06-25 23:16:56.000000 cstore-0.6.2/cstore/schemes.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      529 2023-06-25 14:04:16.000000 cstore-0.6.2/cstore/verbose.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-27 12:09:30.147234 cstore-0.6.2/cstore.egg-info/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      676 2023-06-27 12:09:30.000000 cstore-0.6.2/cstore.egg-info/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      415 2023-06-27 12:09:30.000000 cstore-0.6.2/cstore.egg-info/SOURCES.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-27 12:09:30.000000 cstore-0.6.2/cstore.egg-info/dependency_links.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-06-27 12:09:30.000000 cstore-0.6.2/cstore.egg-info/entry_points.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       74 2023-06-27 12:09:30.000000 cstore-0.6.2/cstore.egg-info/requires.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-06-27 12:09:30.000000 cstore-0.6.2/cstore.egg-info/top_level.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      821 2023-06-27 12:09:22.000000 cstore-0.6.2/pyproject.toml
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-27 12:09:30.151234 cstore-0.6.2/setup.cfg
```

### Comparing `cstore-0.6.1/LICENSE` & `cstore-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cstore-0.6.1/PKG-INFO` & `cstore-0.6.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cstore-0.6.1/cstore/cli.py` & `cstore-0.6.2/cstore/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,22 @@
 from typer import Typer, Option, Exit, Context, confirm, Abort, prompt
 from simple_term_menu import TerminalMenu
 import cryptocode
 
 
 import cstore.schemes as schemes
 from cstore.models import DcBase, Command, Tag
-from cstore.database import engine
+from cstore.database import engine, db_path
 from cstore.constants import actions_enum, ActionsEnum
 from cstore.repo.repo_command import RepoCommand
 from cstore.repo.repo_tag import RepoTag
 from cstore.verbose import Verbose
 
 
-__version__ = "0.6.1"
-db_path = "cstore_sqlite.db"
+__version__ = "0.6.2"
 state = {"verbose": False}
 defult_action = actions_enum.filter
 app = Typer()
 console = Console()
 verbose_manager = Verbose()
 
 
@@ -308,22 +307,31 @@
             os.remove(db_path)
             print("Database flushed.")
 
 
 @app.command("tags")
 def show_all_tags():
     all_tags = RepoTag().get_all()
+    if len(all_tags) == 0:
+        print("No tags found!")
+        raise Exit()
+    
     menu_list = []
     for tag_item in all_tags:
         menu_list.append(tag_item.name)
+        
     terminal_menu = TerminalMenu(menu_list, title="tags list")
     selected_index = terminal_menu.show()
-    if selected_index >= 0:
-        selected_tag = all_tags[selected_index].name
-        os.system(f"cstore --tag {selected_tag}")
+    
+    if not selected_index:
+        print("No tag selected.")
+        raise Exit()
+    
+    selected_tag = all_tags[selected_index].name
+    os.system(f"cstore --tag {selected_tag}")
 
 
 @app.callback(invoke_without_command=True)
 def main(
     ctx: Context,
     verbose: bool = False,
     version: Annotated[
```

### Comparing `cstore-0.6.1/cstore/models.py` & `cstore-0.6.2/cstore/models.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.1/cstore/repo/repo_command.py` & `cstore-0.6.2/cstore/repo/repo_command.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.1/cstore/repo/repo_tag.py` & `cstore-0.6.2/cstore/repo/repo_tag.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.1/cstore/schemes.py` & `cstore-0.6.2/cstore/schemes.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.1/cstore/verbose.py` & `cstore-0.6.2/cstore/verbose.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.1/cstore.egg-info/PKG-INFO` & `cstore-0.6.2/cstore.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cstore-0.6.1/pyproject.toml` & `cstore-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cstore"
-version = "0.6.1"
+version = "0.6.2"
 dependencies = [
     "pydantic",
     "typer[all]",
     "rich",
     "simple_term_menu",
     "SQLAlchemy",
     "pyperclip",
```

