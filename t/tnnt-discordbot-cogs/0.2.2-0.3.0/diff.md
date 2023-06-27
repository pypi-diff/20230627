# Comparing `tmp/tnnt_discordbot_cogs-0.2.2.tar.gz` & `tmp/tnnt_discordbot_cogs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tnnt_discordbot_cogs-0.2.2.tar", last modified: Thu Jun  2 15:23:03 2022, max compression
+gzip compressed data, was "tnnt_discordbot_cogs-0.3.0.tar", last modified: Thu Jun 16 18:29:55 2022, max compression
```

## Comparing `tnnt_discordbot_cogs-0.2.2.tar` & `tnnt_discordbot_cogs-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 15:23:03.893476 tnnt_discordbot_cogs-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-06-02 15:23:03.893476 tnnt_discordbot_cogs-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-06-02 15:23:03.893476 tnnt_discordbot_cogs-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 15:23:03.889476 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 15:23:03.893476 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6937 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/about.py
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     9717 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/members.py
--rw-r--r--   0 runner    (1001) docker     (121)     5849 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/price_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     3623 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     4558 2022-06-02 15:22:45.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/timers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 15:23:03.893476 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-06-02 15:23:03.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-06-02 15:23:03.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 15:23:03.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 15:23:02.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-06-02 15:23:03.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-02 15:23:03.000000 tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 18:29:55.608399 tnnt_discordbot_cogs-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-06-16 18:29:55.608399 tnnt_discordbot_cogs-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-06-16 18:29:55.612399 tnnt_discordbot_cogs-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 18:29:55.608399 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/auth_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 18:29:55.608399 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6937 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/about.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4140 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9717 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/members.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5849 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/price_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4558 2022-06-16 18:29:38.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/timers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 18:29:55.608399 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-06-16 18:29:55.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-06-16 18:29:55.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 18:29:55.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 18:29:53.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-06-16 18:29:55.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-16 18:29:55.000000 tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs.egg-info/top_level.txt
```

### Comparing `tnnt_discordbot_cogs-0.2.2/LICENSE` & `tnnt_discordbot_cogs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.2.2/PKG-INFO` & `tnnt_discordbot_cogs-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tnnt_discordbot_cogs
-Version: 0.2.2
+Version: 0.3.0
 Summary: TN-NT customized cogs for aa-discordbot
 Home-page: https://github.com/terra-nanotech/tn-nt-discordbot-cogs
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GPL-3.0
```

### Comparing `tnnt_discordbot_cogs-0.2.2/setup.cfg` & `tnnt_discordbot_cogs-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/about.py` & `tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/about.py`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/auth.py` & `tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/members.py` & `tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/members.py`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/price_check.py` & `tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/price_check.py`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs/cogs/timers.py` & `tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs/cogs/timers.py`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs.egg-info/PKG-INFO` & `tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tnnt-discordbot-cogs
-Version: 0.2.2
+Version: 0.3.0
 Summary: TN-NT customized cogs for aa-discordbot
 Home-page: https://github.com/terra-nanotech/tn-nt-discordbot-cogs
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: development@ppfeufer.de
 License: GPL-3.0
```

### Comparing `tnnt_discordbot_cogs-0.2.2/tnnt_discordbot_cogs.egg-info/SOURCES.txt` & `tnnt_discordbot_cogs-0.3.0/tnnt_discordbot_cogs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,9 +14,8 @@
 tnnt_discordbot_cogs.egg-info/requires.txt
 tnnt_discordbot_cogs.egg-info/top_level.txt
 tnnt_discordbot_cogs/cogs/__init__.py
 tnnt_discordbot_cogs/cogs/about.py
 tnnt_discordbot_cogs/cogs/auth.py
 tnnt_discordbot_cogs/cogs/members.py
 tnnt_discordbot_cogs/cogs/price_check.py
-tnnt_discordbot_cogs/cogs/time.py
 tnnt_discordbot_cogs/cogs/timers.py
```

