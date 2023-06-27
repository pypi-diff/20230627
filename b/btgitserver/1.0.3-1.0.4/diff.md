# Comparing `tmp/btgitserver-1.0.3.tar.gz` & `tmp/btgitserver-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btgitserver-1.0.3.tar", last modified: Tue Jun 27 17:48:27 2023, max compression
+gzip compressed data, was "btgitserver-1.0.4.tar", last modified: Tue Jun 27 17:51:57 2023, max compression
```

## Comparing `btgitserver-1.0.3.tar` & `btgitserver-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:48:27.352830 btgitserver-1.0.3/
--rwx------   0 etejeda    (501) staff       (20)     1442 2023-06-25 15:47:07.000000 btgitserver-1.0.3/.gitignore
--rwx------   0 etejeda    (501) staff       (20)      445 2019-11-19 14:59:57.000000 btgitserver-1.0.3/Dockerfile
--rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-06-27 17:48:27.353039 btgitserver-1.0.3/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     1730 2023-06-27 12:45:34.000000 btgitserver-1.0.3/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-06-27 17:48:11.000000 btgitserver-1.0.3/VERSION.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:48:27.349146 btgitserver-1.0.3/btgitserver/
--rw-r--r--   0 etejeda    (501) staff       (20)      214 2023-06-25 19:24:10.000000 btgitserver-1.0.3/btgitserver/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     6115 2023-06-27 17:47:53.000000 btgitserver-1.0.3/btgitserver/app.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2206 2023-06-27 12:46:04.000000 btgitserver-1.0.3/btgitserver/args.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1004 2023-06-25 15:50:24.000000 btgitserver-1.0.3/btgitserver/config.py
--rw-r--r--   0 etejeda    (501) staff       (20)      595 2023-06-27 12:39:08.000000 btgitserver-1.0.3/btgitserver/defaults.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-25 19:36:10.000000 btgitserver-1.0.3/btgitserver/logger.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:48:27.351975 btgitserver-1.0.3/btgitserver.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-06-27 17:48:27.000000 btgitserver-1.0.3/btgitserver.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      455 2023-06-27 17:48:27.000000 btgitserver-1.0.3/btgitserver.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-27 17:48:27.000000 btgitserver-1.0.3/btgitserver.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       52 2023-06-27 17:48:27.000000 btgitserver-1.0.3/btgitserver.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-25 19:26:41.000000 btgitserver-1.0.3/btgitserver.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)      173 2023-06-27 17:48:27.000000 btgitserver-1.0.3/btgitserver.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       12 2023-06-27 17:48:27.000000 btgitserver-1.0.3/btgitserver.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:48:27.352279 btgitserver-1.0.3/etc/
--rwx------   0 etejeda    (501) staff       (20)      162 2023-06-27 17:44:31.000000 btgitserver-1.0.3/etc/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)     1236 2023-06-27 17:48:27.353914 btgitserver-1.0.3/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)      780 2023-06-26 00:48:02.000000 btgitserver-1.0.3/setup.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:51:57.307683 btgitserver-1.0.4/
+-rwx------   0 etejeda    (501) staff       (20)     1442 2023-06-25 15:47:07.000000 btgitserver-1.0.4/.gitignore
+-rwx------   0 etejeda    (501) staff       (20)      445 2019-11-19 14:59:57.000000 btgitserver-1.0.4/Dockerfile
+-rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-06-27 17:51:57.307903 btgitserver-1.0.4/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     1730 2023-06-27 12:45:34.000000 btgitserver-1.0.4/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-06-27 17:51:39.000000 btgitserver-1.0.4/VERSION.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:51:57.303810 btgitserver-1.0.4/btgitserver/
+-rw-r--r--   0 etejeda    (501) staff       (20)      214 2023-06-25 19:24:10.000000 btgitserver-1.0.4/btgitserver/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     6119 2023-06-27 17:51:03.000000 btgitserver-1.0.4/btgitserver/app.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2206 2023-06-27 12:46:04.000000 btgitserver-1.0.4/btgitserver/args.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1004 2023-06-25 15:50:24.000000 btgitserver-1.0.4/btgitserver/config.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      595 2023-06-27 12:39:08.000000 btgitserver-1.0.4/btgitserver/defaults.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-25 19:36:10.000000 btgitserver-1.0.4/btgitserver/logger.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:51:57.306786 btgitserver-1.0.4/btgitserver.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      455 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       52 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-25 19:26:41.000000 btgitserver-1.0.4/btgitserver.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)      173 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       12 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:51:57.307098 btgitserver-1.0.4/etc/
+-rwx------   0 etejeda    (501) staff       (20)      162 2023-06-27 17:44:31.000000 btgitserver-1.0.4/etc/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)     1236 2023-06-27 17:51:57.308911 btgitserver-1.0.4/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)      780 2023-06-26 00:48:02.000000 btgitserver-1.0.4/setup.py
```

### Comparing `btgitserver-1.0.3/.gitignore` & `btgitserver-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.3/PKG-INFO` & `btgitserver-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgitserver
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python-based Git Server
 Home-page: https://github.com/berttejeda/bert.git-server
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btgitserver-1.0.3/README.md` & `btgitserver-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.3/btgitserver/app.py` & `btgitserver-1.0.4/btgitserver/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 # Initialize Config Readers
 app_config = AppConfig().initialize(
   args=vars(args),
   verify_tls=verify_tls
 )
 
-git_search_paths = args.repo_search_paths or app_config.get('search_paths', default_repo_search_paths)
+git_search_paths = args.repo_search_paths or app_config.get('app.search_paths', default_repo_search_paths)
 git_repo_map = {}
 
 for git_search_path in git_search_paths:
   fq_git_search_path = Path(git_search_path).expanduser()
   logger.info(f'Building git repo map ...')
   logger.info(f'Adding git repos under {fq_git_search_path}')
   for p in Path(fq_git_search_path).rglob("*"):
```

### Comparing `btgitserver-1.0.3/btgitserver/args.py` & `btgitserver-1.0.4/btgitserver/args.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.3/btgitserver/config.py` & `btgitserver-1.0.4/btgitserver/config.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.3/btgitserver/defaults.py` & `btgitserver-1.0.4/btgitserver/defaults.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.3/btgitserver/logger.py` & `btgitserver-1.0.4/btgitserver/logger.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.3/btgitserver.egg-info/PKG-INFO` & `btgitserver-1.0.4/btgitserver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgitserver
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python-based Git Server
 Home-page: https://github.com/berttejeda/bert.git-server
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btgitserver-1.0.3/setup.cfg` & `btgitserver-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.3/setup.py` & `btgitserver-1.0.4/setup.py`

 * *Files identical despite different names*

