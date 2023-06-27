# Comparing `tmp/btgitserver-1.0.1.tar.gz` & `tmp/btgitserver-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btgitserver-1.0.1.tar", last modified: Mon Jun 26 20:33:55 2023, max compression
+gzip compressed data, was "btgitserver-1.0.2.tar", last modified: Tue Jun 27 17:46:02 2023, max compression
```

## Comparing `btgitserver-1.0.1.tar` & `btgitserver-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-26 20:33:55.482574 btgitserver-1.0.1/
--rwx------   0 etejeda    (501) staff       (20)     1442 2023-06-25 15:47:07.000000 btgitserver-1.0.1/.gitignore
--rwx------   0 etejeda    (501) staff       (20)      445 2019-11-19 14:59:57.000000 btgitserver-1.0.1/Dockerfile
--rw-r--r--   0 etejeda    (501) staff       (20)     2031 2023-06-26 20:33:55.482772 btgitserver-1.0.1/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     1398 2023-06-26 20:33:40.000000 btgitserver-1.0.1/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-06-26 20:33:53.000000 btgitserver-1.0.1/VERSION.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-26 20:33:55.479697 btgitserver-1.0.1/btgitserver/
--rw-r--r--   0 etejeda    (501) staff       (20)      214 2023-06-25 19:24:10.000000 btgitserver-1.0.1/btgitserver/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5860 2023-06-26 02:28:43.000000 btgitserver-1.0.1/btgitserver/app.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2192 2023-06-25 21:21:58.000000 btgitserver-1.0.1/btgitserver/args.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1004 2023-06-25 15:50:24.000000 btgitserver-1.0.1/btgitserver/config.py
--rw-r--r--   0 etejeda    (501) staff       (20)      591 2023-06-25 19:54:41.000000 btgitserver-1.0.1/btgitserver/defaults.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-25 19:36:10.000000 btgitserver-1.0.1/btgitserver/logger.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-26 20:33:55.481985 btgitserver-1.0.1/btgitserver.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     2031 2023-06-26 20:33:55.000000 btgitserver-1.0.1/btgitserver.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      455 2023-06-26 20:33:55.000000 btgitserver-1.0.1/btgitserver.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-26 20:33:55.000000 btgitserver-1.0.1/btgitserver.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       52 2023-06-26 20:33:55.000000 btgitserver-1.0.1/btgitserver.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-25 19:26:41.000000 btgitserver-1.0.1/btgitserver.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)      173 2023-06-26 20:33:55.000000 btgitserver-1.0.1/btgitserver.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       12 2023-06-26 20:33:55.000000 btgitserver-1.0.1/btgitserver.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-26 20:33:55.482297 btgitserver-1.0.1/etc/
--rwx------   0 etejeda    (501) staff       (20)      135 2023-06-25 19:20:14.000000 btgitserver-1.0.1/etc/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)     1236 2023-06-26 20:33:55.483584 btgitserver-1.0.1/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)      780 2023-06-26 00:48:02.000000 btgitserver-1.0.1/setup.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:46:02.628337 btgitserver-1.0.2/
+-rwx------   0 etejeda    (501) staff       (20)     1442 2023-06-25 15:47:07.000000 btgitserver-1.0.2/.gitignore
+-rwx------   0 etejeda    (501) staff       (20)      445 2019-11-19 14:59:57.000000 btgitserver-1.0.2/Dockerfile
+-rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-06-27 17:46:02.628572 btgitserver-1.0.2/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     1730 2023-06-27 12:45:34.000000 btgitserver-1.0.2/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-06-27 17:45:04.000000 btgitserver-1.0.2/VERSION.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:46:02.625369 btgitserver-1.0.2/btgitserver/
+-rw-r--r--   0 etejeda    (501) staff       (20)      214 2023-06-25 19:24:10.000000 btgitserver-1.0.2/btgitserver/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     6145 2023-06-27 17:44:53.000000 btgitserver-1.0.2/btgitserver/app.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2206 2023-06-27 12:46:04.000000 btgitserver-1.0.2/btgitserver/args.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1004 2023-06-25 15:50:24.000000 btgitserver-1.0.2/btgitserver/config.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      595 2023-06-27 12:39:08.000000 btgitserver-1.0.2/btgitserver/defaults.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-25 19:36:10.000000 btgitserver-1.0.2/btgitserver/logger.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:46:02.627679 btgitserver-1.0.2/btgitserver.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-06-27 17:46:02.000000 btgitserver-1.0.2/btgitserver.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      455 2023-06-27 17:46:02.000000 btgitserver-1.0.2/btgitserver.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-27 17:46:02.000000 btgitserver-1.0.2/btgitserver.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       52 2023-06-27 17:46:02.000000 btgitserver-1.0.2/btgitserver.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-25 19:26:41.000000 btgitserver-1.0.2/btgitserver.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)      173 2023-06-27 17:46:02.000000 btgitserver-1.0.2/btgitserver.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       12 2023-06-27 17:46:02.000000 btgitserver-1.0.2/btgitserver.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:46:02.628007 btgitserver-1.0.2/etc/
+-rwx------   0 etejeda    (501) staff       (20)      162 2023-06-27 17:44:31.000000 btgitserver-1.0.2/etc/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)     1236 2023-06-27 17:46:02.629519 btgitserver-1.0.2/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)      780 2023-06-26 00:48:02.000000 btgitserver-1.0.2/setup.py
```

### Comparing `btgitserver-1.0.1/.gitignore` & `btgitserver-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.1/PKG-INFO` & `btgitserver-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,15 @@
-Metadata-Version: 2.1
-Name: btgitserver
-Version: 1.0.1
-Summary: Python-based Git Server
-Home-page: https://github.com/berttejeda/bert.git-server
-Author: Engelbert Tejeda
-Author-email: berttejeda@gmail.com
-Keywords: yaml,configuration,config,file,python,settings
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-
 ## Overview
 
 A git server implementation written in python.
 
-The app services any git repository lying below the _search\_path_ 
-available for cloning via HTTP using basic authentication.
+Based off the amazing work by Stewart Park in this gist: [https://gist.github.com/stewartpark/1b079dc0481c6213def9](https://gist.github.com/stewartpark/1b079dc0481c6213def9).
+
+The app makes any git repository lying below the _search\_paths_ 
+available for `git clone` via HTTP using basic authentication.
 
 Application defaults can be overridden by specifying a configuration file.
 
 Review [etc/config.yaml](etc/config.yaml) for a sample data structure.
 
 ## Installation
 
@@ -61,26 +45,29 @@
 git init .
 touch test_file.txt
 git add .
 git commit -m 'Initial Commit'
 git-server -r /tmp/repos
 ```
 
+**Note**: The `--repo-search-paths/-r` cli option allows specifying 
+multiple, space-delimitted search paths, e.g. `git-server -r /tmp/repos /tmp/repos2`
+
 * Launch the standalone git server
 
 `git-server`
 
 You should see output similar to:
 ```
 Running on http://0.0.0.0:5000/	
 ```
 
-* On client:
+* On client-side:
 
-Try cloning the repo you just created via the three supported routes:
+Try cloning the repo you just created via the supported routes:
 
 e.g.
 	
 ```bash
 git clone http://127.0.0.1:5000/test.git
 git clone http://127.0.0.1:5000/example/test.git
 ```
```

### Comparing `btgitserver-1.0.1/btgitserver/app.py` & `btgitserver-1.0.2/btgitserver/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from btgitserver.args import parse_args
 from btgitserver.config import AppConfig
 from btgitserver.defaults import default_app_port, \
 default_app_host_address, \
-default_repo_search_path, \
+default_repo_search_paths, \
 default_verify_tls
 from btgitserver.logger import Logger
 
 from dulwich.pack import PackStreamReader
 import subprocess
 from flask_httpauth import HTTPBasicAuth
 from flask import Flask, make_response, request, abort
@@ -15,58 +15,61 @@
 if sys.version_info[0] == 2:
     from StringIO import StringIO
 if sys.version_info[0] >= 3:
     from io import StringIO
 
 # Private variables
 __author__ = 'berttejeda'
+__original_author = 'stewartpark'
 
 # Read command-line args
 args = parse_args()
 # Initialize logging facility
 logger_obj = Logger(
     logfile_path=args.logfile_path,
     logfile_write_mode=args.logfile_write_mode)
 logger = logger_obj.init_logger('app')
 
-verify_tls = args.no_verify_tls or default_verify_tls
+verify_tls = args.no_verify_tls or app_config.get('verify_tls', default_verify_tls)
 
 # Flask
 app = Flask(__name__)
 auth = HTTPBasicAuth()
 
 # Initialize Config Readers
 app_config = AppConfig().initialize(
   args=vars(args),
   verify_tls=verify_tls
 )
 
-git_search_path = Path(args.repo_search_path or default_repo_search_path).expanduser()
+git_search_paths = args.repo_search_paths or app_config.get('search_paths', default_repo_search_paths)
 git_repo_map = {}
 
-logger.info(f'Searching for git repos under {git_search_path}')
-for p in Path(git_search_path).rglob("*"):
-    if p.is_dir() and p.name == '.git':
-      git_directory = p.parent.as_posix()
-      git_directory_name = p.parent.name
-      if git_directory_name:
-        git_repo_map[git_directory_name] = git_directory
+for git_search_path in git_search_paths:
+  fq_git_search_path = Path(git_search_path).expanduser()
+  logger.info(f'Building git repo map ...')
+  logger.info(f'Adding git repos under {fq_git_search_path}')
+  for p in Path(fq_git_search_path).rglob("*"):
+      if p.is_dir() and p.name == '.git':
+        git_directory = p.parent.as_posix()
+        git_directory_name = p.parent.name
+        if git_directory_name:
+          git_repo_map[git_directory_name] = git_directory
+  logger.info(f'Finished building git repo map!')
 
 numrepos = len(list(git_repo_map.keys()))
 logger.info(f'Found {numrepos} repo(s)')
 
 authorized_users = app_config.auth.users
 users = [u[0] for u in authorized_users.items()]
 available_repos = list(git_repo_map.keys())
 
 def start_api():
   """API functions.
-
   This function defines the API routes and starts the API Process.
-
   """
 
   @auth.get_password
   def get_pw(username):
       if username in users:
           credential = authorized_users.get(username).password
           return credential
```

### Comparing `btgitserver-1.0.1/btgitserver/args.py` & `btgitserver-1.0.2/btgitserver/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,16 @@
             username2:
               password: password2
         
         app:
           debug: false
           listen: "0.0.0.0"
           port: 5000
-          basedir: ~/git
-          workers: 4
-
+          search_paths: 
+            - ~/repos
         """,
         fromfile_prefix_chars='@')
     parser.add_argument(
         "-host",
         "--host-address",
         help="Override listening address",
         metavar="ARG", required=False)
@@ -43,15 +42,15 @@
     parser.add_argument(
         "-w",
         "--workers",
         help="Override number of gunicorn workers",
         metavar="ARG", required=False)    
     parser.add_argument('--no-verify-tls', '-notls',action='store_true', help='Verify SSL cert when downloading web content')
     parser.add_argument('--config-file', '-f', help="Path to config file override")
-    parser.add_argument('--repo-search-path', '-r', help="Path to directory containing git repositories")
+    parser.add_argument('--repo-search-paths', '-r', nargs='+', help="List of directories containing git repositories")
     parser.add_argument('--logfile-path', '-L', help="Path to logfile")
     parser.add_argument('--logfile-write-mode', '-Lw', default='w', choices=['a', 'w'], help="File mode when writing to log file, 'a' to append, 'w' to overwrite")    
     parser.add_argument('--debug', action='store_true')
     parser.add_argument(
         "-v",
         "--verbose",
         help="increase output verbosity",
```

### Comparing `btgitserver-1.0.1/btgitserver/config.py` & `btgitserver-1.0.2/btgitserver/config.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.1/btgitserver/logger.py` & `btgitserver-1.0.2/btgitserver/logger.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.1/btgitserver.egg-info/PKG-INFO` & `btgitserver-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgitserver
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python-based Git Server
 Home-page: https://github.com/berttejeda/bert.git-server
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,18 @@
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 ## Overview
 
 A git server implementation written in python.
 
-The app services any git repository lying below the _search\_path_ 
-available for cloning via HTTP using basic authentication.
+Based off the amazing work by Stewart Park in this gist: [https://gist.github.com/stewartpark/1b079dc0481c6213def9](https://gist.github.com/stewartpark/1b079dc0481c6213def9).
+
+The app makes any git repository lying below the _search\_paths_ 
+available for `git clone` via HTTP using basic authentication.
 
 Application defaults can be overridden by specifying a configuration file.
 
 Review [etc/config.yaml](etc/config.yaml) for a sample data structure.
 
 ## Installation
 
@@ -61,26 +63,29 @@
 git init .
 touch test_file.txt
 git add .
 git commit -m 'Initial Commit'
 git-server -r /tmp/repos
 ```
 
+**Note**: The `--repo-search-paths/-r` cli option allows specifying 
+multiple, space-delimitted search paths, e.g. `git-server -r /tmp/repos /tmp/repos2`
+
 * Launch the standalone git server
 
 `git-server`
 
 You should see output similar to:
 ```
 Running on http://0.0.0.0:5000/	
 ```
 
-* On client:
+* On client-side:
 
-Try cloning the repo you just created via the three supported routes:
+Try cloning the repo you just created via the supported routes:
 
 e.g.
 	
 ```bash
 git clone http://127.0.0.1:5000/test.git
 git clone http://127.0.0.1:5000/example/test.git
 ```
```

### Comparing `btgitserver-1.0.1/setup.cfg` & `btgitserver-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.1/setup.py` & `btgitserver-1.0.2/setup.py`

 * *Files identical despite different names*

