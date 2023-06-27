# Comparing `tmp/how_fake_accounts-0.1.0.tar.gz` & `tmp/how_fake_accounts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "how_fake_accounts-0.1.0.tar", last modified: Tue Jun 27 10:54:12 2023, max compression
+gzip compressed data, was "how_fake_accounts-0.2.0.tar", last modified: Tue Jun 27 10:58:45 2023, max compression
```

## Comparing `how_fake_accounts-0.1.0.tar` & `how_fake_accounts-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 10:54:12.977187 how_fake_accounts-0.1.0/
--rw-r--r--   0 joaonogueira   (501) staff       (20)      220 2023-06-27 10:54:12.977014 how_fake_accounts-0.1.0/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      135 2023-06-27 10:49:30.000000 how_fake_accounts-0.1.0/README.md
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 10:54:12.975303 how_fake_accounts-0.1.0/how_fake_accounts/
--rw-r--r--   0 joaonogueira   (501) staff       (20)       50 2023-06-27 10:33:16.000000 how_fake_accounts-0.1.0/how_fake_accounts/__init__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      881 2023-06-27 10:40:42.000000 how_fake_accounts-0.1.0/how_fake_accounts/__main__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      837 2023-06-27 10:41:12.000000 how_fake_accounts-0.1.0/how_fake_accounts/core.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 10:54:12.976791 how_fake_accounts-0.1.0/how_fake_accounts.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)      220 2023-06-27 10:54:12.000000 how_fake_accounts-0.1.0/how_fake_accounts.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      352 2023-06-27 10:54:12.000000 how_fake_accounts-0.1.0/how_fake_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-06-27 10:54:12.000000 how_fake_accounts-0.1.0/how_fake_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       70 2023-06-27 10:54:12.000000 how_fake_accounts-0.1.0/how_fake_accounts.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        6 2023-06-27 10:54:12.000000 how_fake_accounts-0.1.0/how_fake_accounts.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       18 2023-06-27 10:54:12.000000 how_fake_accounts-0.1.0/how_fake_accounts.egg-info/top_level.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-06-27 10:54:12.977234 how_fake_accounts-0.1.0/setup.cfg
--rw-r--r--   0 joaonogueira   (501) staff       (20)      413 2023-06-27 10:52:15.000000 how_fake_accounts-0.1.0/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 10:58:45.111998 how_fake_accounts-0.2.0/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      260 2023-06-27 10:58:45.111836 how_fake_accounts-0.2.0/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      135 2023-06-27 10:49:30.000000 how_fake_accounts-0.2.0/README.md
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 10:58:45.110192 how_fake_accounts-0.2.0/how_fake_accounts/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       50 2023-06-27 10:33:16.000000 how_fake_accounts-0.2.0/how_fake_accounts/__init__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      881 2023-06-27 10:40:42.000000 how_fake_accounts-0.2.0/how_fake_accounts/__main__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      837 2023-06-27 10:41:12.000000 how_fake_accounts-0.2.0/how_fake_accounts/core.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 10:58:45.111604 how_fake_accounts-0.2.0/how_fake_accounts.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      260 2023-06-27 10:58:45.000000 how_fake_accounts-0.2.0/how_fake_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      352 2023-06-27 10:58:45.000000 how_fake_accounts-0.2.0/how_fake_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-06-27 10:58:45.000000 how_fake_accounts-0.2.0/how_fake_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       70 2023-06-27 10:58:45.000000 how_fake_accounts-0.2.0/how_fake_accounts.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        6 2023-06-27 10:58:45.000000 how_fake_accounts-0.2.0/how_fake_accounts.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       18 2023-06-27 10:58:45.000000 how_fake_accounts-0.2.0/how_fake_accounts.egg-info/top_level.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-06-27 10:58:45.112048 how_fake_accounts-0.2.0/setup.cfg
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      421 2023-06-27 10:58:29.000000 how_fake_accounts-0.2.0/setup.py
```

### Comparing `how_fake_accounts-0.1.0/how_fake_accounts/__main__.py` & `how_fake_accounts-0.2.0/how_fake_accounts/__main__.py`

 * *Files identical despite different names*

### Comparing `how_fake_accounts-0.1.0/how_fake_accounts/core.py` & `how_fake_accounts-0.2.0/how_fake_accounts/core.py`

 * *Files identical despite different names*

