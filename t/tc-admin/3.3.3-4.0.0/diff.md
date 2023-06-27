# Comparing `tmp/tc-admin-3.3.3.tar.gz` & `tmp/tc-admin-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-admin-3.3.3.tar", last modified: Tue May  9 19:26:45 2023, max compression
+gzip compressed data, was "tc-admin-4.0.0.tar", last modified: Tue Jun 27 14:59:18 2023, max compression
```

## Comparing `tc-admin-3.3.3.tar` & `tc-admin-4.0.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-05-09 19:26:45.848726 tc-admin-3.3.3/
--rw-r--r--   0 mboris     (501) staff       (20)    16725 2023-05-09 19:09:53.000000 tc-admin-3.3.3/LICENSE
--rw-r--r--   0 mboris     (501) staff       (20)    20004 2023-05-09 19:26:45.848821 tc-admin-3.3.3/PKG-INFO
--rw-r--r--   0 mboris     (501) staff       (20)    19672 2022-10-27 20:38:34.000000 tc-admin-3.3.3/README.md
--rw-r--r--   0 mboris     (501) staff       (20)       39 2022-10-27 20:38:15.000000 tc-admin-3.3.3/pyproject.toml
--rw-r--r--   0 mboris     (501) staff       (20)      105 2023-05-09 19:26:45.849134 tc-admin-3.3.3/setup.cfg
--rw-r--r--   0 mboris     (501) staff       (20)     1063 2023-05-09 19:26:08.000000 tc-admin-3.3.3/setup.py
-drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-05-09 19:26:45.841472 tc-admin-3.3.3/tc_admin.egg-info/
--rw-r--r--   0 mboris     (501) staff       (20)    20004 2023-05-09 19:26:45.000000 tc-admin-3.3.3/tc_admin.egg-info/PKG-INFO
--rw-r--r--   0 mboris     (501) staff       (20)     1094 2023-05-09 19:26:45.000000 tc-admin-3.3.3/tc_admin.egg-info/SOURCES.txt
--rw-r--r--   0 mboris     (501) staff       (20)        1 2023-05-09 19:26:45.000000 tc-admin-3.3.3/tc_admin.egg-info/dependency_links.txt
--rw-r--r--   0 mboris     (501) staff       (20)       47 2023-05-09 19:26:45.000000 tc-admin-3.3.3/tc_admin.egg-info/entry_points.txt
--rw-r--r--   0 mboris     (501) staff       (20)      149 2023-05-09 19:26:45.000000 tc-admin-3.3.3/tc_admin.egg-info/requires.txt
--rw-r--r--   0 mboris     (501) staff       (20)        8 2023-05-09 19:26:45.000000 tc-admin-3.3.3/tc_admin.egg-info/top_level.txt
-drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-05-09 19:26:45.844313 tc-admin-3.3.3/tcadmin/
--rw-r--r--   0 mboris     (501) staff       (20)        0 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/__init__.py
--rw-r--r--   0 mboris     (501) staff       (20)     4817 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/appconfig.py
--rw-r--r--   0 mboris     (501) staff       (20)     1017 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/apply.py
--rw-r--r--   0 mboris     (501) staff       (20)     1853 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/boot.py
--rw-r--r--   0 mboris     (501) staff       (20)     2448 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/callbacks.py
--rw-r--r--   0 mboris     (501) staff       (20)      726 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/check.py
--rw-r--r--   0 mboris     (501) staff       (20)      416 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/constants.py
-drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-05-09 19:26:45.845466 tc-admin-3.3.3/tcadmin/current/
--rw-r--r--   0 mboris     (501) staff       (20)      758 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/current/__init__.py
--rw-r--r--   0 mboris     (501) staff       (20)      877 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/current/clients.py
--rw-r--r--   0 mboris     (501) staff       (20)     1042 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/current/hooks.py
--rw-r--r--   0 mboris     (501) staff       (20)      632 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/current/roles.py
--rw-r--r--   0 mboris     (501) staff       (20)     1229 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/current/secrets.py
--rw-r--r--   0 mboris     (501) staff       (20)     1392 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/current/worker_pools.py
--rw-r--r--   0 mboris     (501) staff       (20)     4869 2022-10-28 12:39:23.000000 tc-admin-3.3.3/tcadmin/diff.py
--rw-r--r--   0 mboris     (501) staff       (20)      741 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/generate.py
--rw-r--r--   0 mboris     (501) staff       (20)     4327 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/main.py
--rw-r--r--   0 mboris     (501) staff       (20)     1964 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/options.py
--rw-r--r--   0 mboris     (501) staff       (20)      695 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/output.py
-drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-05-09 19:26:45.846951 tc-admin-3.3.3/tcadmin/resources/
--rw-r--r--   0 mboris     (501) staff       (20)      489 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/resources/__init__.py
--rw-r--r--   0 mboris     (501) staff       (20)     2006 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/resources/client.py
--rw-r--r--   0 mboris     (501) staff       (20)     3435 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/resources/hook.py
--rw-r--r--   0 mboris     (501) staff       (20)     6620 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/resources/resources.py
--rw-r--r--   0 mboris     (501) staff       (20)     1487 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/resources/role.py
--rw-r--r--   0 mboris     (501) staff       (20)     2308 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/resources/secret.py
--rw-r--r--   0 mboris     (501) staff       (20)      962 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/resources/util.py
--rw-r--r--   0 mboris     (501) staff       (20)     1513 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/resources/worker_pool.py
--rw-r--r--   0 mboris     (501) staff       (20)     5644 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/update.py
-drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-05-09 19:26:45.848546 tc-admin-3.3.3/tcadmin/util/
--rw-r--r--   0 mboris     (501) staff       (20)        0 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/util/__init__.py
--rw-r--r--   0 mboris     (501) staff       (20)      545 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/util/ansi.py
--rw-r--r--   0 mboris     (501) staff       (20)     2050 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/util/config.py
--rw-r--r--   0 mboris     (501) staff       (20)      342 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/util/json.py
--rw-r--r--   0 mboris     (501) staff       (20)     1046 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/util/matchlist.py
--rw-r--r--   0 mboris     (501) staff       (20)     1402 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/util/root_url.py
--rw-r--r--   0 mboris     (501) staff       (20)     4317 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/util/scopes.py
--rw-r--r--   0 mboris     (501) staff       (20)      813 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/util/sessions.py
--rw-r--r--   0 mboris     (501) staff       (20)      682 2022-10-27 20:38:15.000000 tc-admin-3.3.3/tcadmin/util/taskcluster.py
+drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-06-27 14:59:18.476276 tc-admin-4.0.0/
+-rw-r--r--   0 mboris     (501) staff       (20)    16725 2023-05-09 19:09:53.000000 tc-admin-4.0.0/LICENSE
+-rw-r--r--   0 mboris     (501) staff       (20)    20158 2023-06-27 14:59:18.476375 tc-admin-4.0.0/PKG-INFO
+-rw-r--r--   0 mboris     (501) staff       (20)    19672 2022-10-27 20:38:34.000000 tc-admin-4.0.0/README.md
+-rw-r--r--   0 mboris     (501) staff       (20)       39 2022-10-27 20:38:15.000000 tc-admin-4.0.0/pyproject.toml
+-rw-r--r--   0 mboris     (501) staff       (20)      105 2023-06-27 14:59:18.476812 tc-admin-4.0.0/setup.cfg
+-rw-r--r--   0 mboris     (501) staff       (20)     1214 2023-06-27 14:57:08.000000 tc-admin-4.0.0/setup.py
+drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-06-27 14:59:18.470622 tc-admin-4.0.0/tc_admin.egg-info/
+-rw-r--r--   0 mboris     (501) staff       (20)    20158 2023-06-27 14:59:18.000000 tc-admin-4.0.0/tc_admin.egg-info/PKG-INFO
+-rw-r--r--   0 mboris     (501) staff       (20)     1094 2023-06-27 14:59:18.000000 tc-admin-4.0.0/tc_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 mboris     (501) staff       (20)        1 2023-06-27 14:59:18.000000 tc-admin-4.0.0/tc_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 mboris     (501) staff       (20)       47 2023-06-27 14:59:18.000000 tc-admin-4.0.0/tc_admin.egg-info/entry_points.txt
+-rw-r--r--   0 mboris     (501) staff       (20)      149 2023-06-27 14:59:18.000000 tc-admin-4.0.0/tc_admin.egg-info/requires.txt
+-rw-r--r--   0 mboris     (501) staff       (20)        8 2023-06-27 14:59:18.000000 tc-admin-4.0.0/tc_admin.egg-info/top_level.txt
+drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-06-27 14:59:18.472737 tc-admin-4.0.0/tcadmin/
+-rw-r--r--   0 mboris     (501) staff       (20)        0 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/__init__.py
+-rw-r--r--   0 mboris     (501) staff       (20)     4817 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/appconfig.py
+-rw-r--r--   0 mboris     (501) staff       (20)     1017 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/apply.py
+-rw-r--r--   0 mboris     (501) staff       (20)     1853 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/boot.py
+-rw-r--r--   0 mboris     (501) staff       (20)     2448 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/callbacks.py
+-rw-r--r--   0 mboris     (501) staff       (20)      726 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/check.py
+-rw-r--r--   0 mboris     (501) staff       (20)      416 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/constants.py
+drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-06-27 14:59:18.473622 tc-admin-4.0.0/tcadmin/current/
+-rw-r--r--   0 mboris     (501) staff       (20)      758 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/current/__init__.py
+-rw-r--r--   0 mboris     (501) staff       (20)      877 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/current/clients.py
+-rw-r--r--   0 mboris     (501) staff       (20)     1042 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/current/hooks.py
+-rw-r--r--   0 mboris     (501) staff       (20)      632 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/current/roles.py
+-rw-r--r--   0 mboris     (501) staff       (20)     1229 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/current/secrets.py
+-rw-r--r--   0 mboris     (501) staff       (20)     1392 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/current/worker_pools.py
+-rw-r--r--   0 mboris     (501) staff       (20)     4869 2022-10-28 12:39:23.000000 tc-admin-4.0.0/tcadmin/diff.py
+-rw-r--r--   0 mboris     (501) staff       (20)      741 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/generate.py
+-rw-r--r--   0 mboris     (501) staff       (20)     4327 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/main.py
+-rw-r--r--   0 mboris     (501) staff       (20)     1964 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/options.py
+-rw-r--r--   0 mboris     (501) staff       (20)      695 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/output.py
+drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-06-27 14:59:18.474828 tc-admin-4.0.0/tcadmin/resources/
+-rw-r--r--   0 mboris     (501) staff       (20)      489 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/resources/__init__.py
+-rw-r--r--   0 mboris     (501) staff       (20)     2006 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/resources/client.py
+-rw-r--r--   0 mboris     (501) staff       (20)     3435 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/resources/hook.py
+-rw-r--r--   0 mboris     (501) staff       (20)     6620 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/resources/resources.py
+-rw-r--r--   0 mboris     (501) staff       (20)     1487 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/resources/role.py
+-rw-r--r--   0 mboris     (501) staff       (20)     2308 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/resources/secret.py
+-rw-r--r--   0 mboris     (501) staff       (20)      962 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/resources/util.py
+-rw-r--r--   0 mboris     (501) staff       (20)     1513 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/resources/worker_pool.py
+-rw-r--r--   0 mboris     (501) staff       (20)     5644 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/update.py
+drwxr-xr-x   0 mboris     (501) staff       (20)        0 2023-06-27 14:59:18.476125 tc-admin-4.0.0/tcadmin/util/
+-rw-r--r--   0 mboris     (501) staff       (20)        0 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/util/__init__.py
+-rw-r--r--   0 mboris     (501) staff       (20)      545 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/util/ansi.py
+-rw-r--r--   0 mboris     (501) staff       (20)     2050 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/util/config.py
+-rw-r--r--   0 mboris     (501) staff       (20)      342 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/util/json.py
+-rw-r--r--   0 mboris     (501) staff       (20)     1046 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/util/matchlist.py
+-rw-r--r--   0 mboris     (501) staff       (20)     1402 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/util/root_url.py
+-rw-r--r--   0 mboris     (501) staff       (20)     4317 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/util/scopes.py
+-rw-r--r--   0 mboris     (501) staff       (20)      813 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/util/sessions.py
+-rw-r--r--   0 mboris     (501) staff       (20)      682 2022-10-27 20:38:15.000000 tc-admin-4.0.0/tcadmin/util/taskcluster.py
```

### Comparing `tc-admin-3.3.3/LICENSE` & `tc-admin-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/PKG-INFO` & `tc-admin-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: tc-admin
-Version: 3.3.3
+Version: 4.0.0
 Summary: Administration of Taskcluster runtime configuration
 Home-page: https://github.com/taskcluster/tc-admin
 Author: Dustin Mitchell
 Author-email: dustin@mozilla.com
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 The `tc-admin` library supports administration of the runtime configuration of a Taskcluster deployment.
 This means creation and maintenance of resources such as roles, hooks, and worker pools, based on version-controlled specifications..
 
 # Usage
```

### Comparing `tc-admin-3.3.3/README.md` & `tc-admin-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/setup.py` & `tc-admin-4.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="tc-admin",
-    version="3.3.3",
+    version="4.0.0",
     description="Administration of Taskcluster runtime configuration",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Dustin Mitchell",
     author_email="dustin@mozilla.com",
     url="https://github.com/taskcluster/tc-admin",
     packages=find_packages("."),
     install_requires=[
-        "taskcluster>=44.0.0,<50.1",
+        "taskcluster>=44.0.0,<53.1",
         "click>=8.0.0,<8.2",
         "blessings~=1.7",
         "attrs>=21.4.0,<23.2",
         "sortedcontainers~=2.4.0",
         "aiohttp~=3.8.0",
-        "pytest>=7.0.0,<7.4",
+        "pytest>=7.0.0,<7.5",
         "pyyaml~=6.0",
     ],
     setup_requires=["pytest-runner", "flake8"],
     tests_require=["pytest", "pytest-mock", "pytest-asyncio>=0.18.0,<0.22", "flake8", "asyncmock"],
     classifiers=[
-        "Programming Language :: Python :: 3",
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     entry_points={
         "console_scripts": [
             "tc-admin = tcadmin.boot:boot",
         ]},
 )
```

### Comparing `tc-admin-3.3.3/tc_admin.egg-info/PKG-INFO` & `tc-admin-4.0.0/tc_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: tc-admin
-Version: 3.3.3
+Version: 4.0.0
 Summary: Administration of Taskcluster runtime configuration
 Home-page: https://github.com/taskcluster/tc-admin
 Author: Dustin Mitchell
 Author-email: dustin@mozilla.com
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 The `tc-admin` library supports administration of the runtime configuration of a Taskcluster deployment.
 This means creation and maintenance of resources such as roles, hooks, and worker pools, based on version-controlled specifications..
 
 # Usage
```

### Comparing `tc-admin-3.3.3/tc_admin.egg-info/SOURCES.txt` & `tc-admin-4.0.0/tc_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/appconfig.py` & `tc-admin-4.0.0/tcadmin/appconfig.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/apply.py` & `tc-admin-4.0.0/tcadmin/apply.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/boot.py` & `tc-admin-4.0.0/tcadmin/boot.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/callbacks.py` & `tc-admin-4.0.0/tcadmin/callbacks.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/check.py` & `tc-admin-4.0.0/tcadmin/check.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/current/__init__.py` & `tc-admin-4.0.0/tcadmin/current/__init__.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/current/clients.py` & `tc-admin-4.0.0/tcadmin/current/clients.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/current/hooks.py` & `tc-admin-4.0.0/tcadmin/current/hooks.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/current/roles.py` & `tc-admin-4.0.0/tcadmin/current/roles.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/current/secrets.py` & `tc-admin-4.0.0/tcadmin/current/secrets.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/current/worker_pools.py` & `tc-admin-4.0.0/tcadmin/current/worker_pools.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/diff.py` & `tc-admin-4.0.0/tcadmin/diff.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/generate.py` & `tc-admin-4.0.0/tcadmin/generate.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/main.py` & `tc-admin-4.0.0/tcadmin/main.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/options.py` & `tc-admin-4.0.0/tcadmin/options.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/output.py` & `tc-admin-4.0.0/tcadmin/output.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/resources/client.py` & `tc-admin-4.0.0/tcadmin/resources/client.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/resources/hook.py` & `tc-admin-4.0.0/tcadmin/resources/hook.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/resources/resources.py` & `tc-admin-4.0.0/tcadmin/resources/resources.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/resources/role.py` & `tc-admin-4.0.0/tcadmin/resources/role.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/resources/secret.py` & `tc-admin-4.0.0/tcadmin/resources/secret.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/resources/util.py` & `tc-admin-4.0.0/tcadmin/resources/util.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/resources/worker_pool.py` & `tc-admin-4.0.0/tcadmin/resources/worker_pool.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/update.py` & `tc-admin-4.0.0/tcadmin/update.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/util/ansi.py` & `tc-admin-4.0.0/tcadmin/util/ansi.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/util/config.py` & `tc-admin-4.0.0/tcadmin/util/config.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/util/matchlist.py` & `tc-admin-4.0.0/tcadmin/util/matchlist.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/util/root_url.py` & `tc-admin-4.0.0/tcadmin/util/root_url.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/util/scopes.py` & `tc-admin-4.0.0/tcadmin/util/scopes.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/util/sessions.py` & `tc-admin-4.0.0/tcadmin/util/sessions.py`

 * *Files identical despite different names*

### Comparing `tc-admin-3.3.3/tcadmin/util/taskcluster.py` & `tc-admin-4.0.0/tcadmin/util/taskcluster.py`

 * *Files identical despite different names*

