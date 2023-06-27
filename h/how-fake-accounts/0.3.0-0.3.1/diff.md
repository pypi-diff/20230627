# Comparing `tmp/how_fake_accounts-0.3.0.tar.gz` & `tmp/how_fake_accounts-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "how_fake_accounts-0.3.0.tar", last modified: Tue Jun 27 11:10:01 2023, max compression
+gzip compressed data, was "how_fake_accounts-0.3.1.tar", last modified: Tue Jun 27 11:17:17 2023, max compression
```

## Comparing `how_fake_accounts-0.3.0.tar` & `how_fake_accounts-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 11:10:01.202526 how_fake_accounts-0.3.0/
--rw-r--r--   0 joaonogueira   (501) staff       (20)      523 2023-06-27 11:10:01.202350 how_fake_accounts-0.3.0/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      375 2023-06-27 11:09:39.000000 how_fake_accounts-0.3.0/README.md
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 11:10:01.200197 how_fake_accounts-0.3.0/how_fake_accounts/
--rw-r--r--   0 joaonogueira   (501) staff       (20)       50 2023-06-27 10:33:16.000000 how_fake_accounts-0.3.0/how_fake_accounts/__init__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      881 2023-06-27 11:07:55.000000 how_fake_accounts-0.3.0/how_fake_accounts/__main__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      837 2023-06-27 10:41:12.000000 how_fake_accounts-0.3.0/how_fake_accounts/core.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 11:10:01.201978 how_fake_accounts-0.3.0/how_fake_accounts.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)      523 2023-06-27 11:10:01.000000 how_fake_accounts-0.3.0/how_fake_accounts.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      352 2023-06-27 11:10:01.000000 how_fake_accounts-0.3.0/how_fake_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-06-27 11:10:01.000000 how_fake_accounts-0.3.0/how_fake_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       70 2023-06-27 11:10:01.000000 how_fake_accounts-0.3.0/how_fake_accounts.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        6 2023-06-27 11:10:01.000000 how_fake_accounts-0.3.0/how_fake_accounts.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       18 2023-06-27 11:10:01.000000 how_fake_accounts-0.3.0/how_fake_accounts.egg-info/top_level.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-06-27 11:10:01.202575 how_fake_accounts-0.3.0/setup.cfg
--rw-r--r--   0 joaonogueira   (501) staff       (20)      450 2023-06-27 11:09:52.000000 how_fake_accounts-0.3.0/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 11:17:17.026020 how_fake_accounts-0.3.1/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      889 2023-06-27 11:17:17.025645 how_fake_accounts-0.3.1/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      741 2023-06-27 11:16:18.000000 how_fake_accounts-0.3.1/README.md
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 11:17:17.023106 how_fake_accounts-0.3.1/how_fake_accounts/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       50 2023-06-27 10:33:16.000000 how_fake_accounts-0.3.1/how_fake_accounts/__init__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      881 2023-06-27 11:07:55.000000 how_fake_accounts-0.3.1/how_fake_accounts/__main__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      837 2023-06-27 10:41:12.000000 how_fake_accounts-0.3.1/how_fake_accounts/core.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-06-27 11:17:17.025145 how_fake_accounts-0.3.1/how_fake_accounts.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      889 2023-06-27 11:17:16.000000 how_fake_accounts-0.3.1/how_fake_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      352 2023-06-27 11:17:16.000000 how_fake_accounts-0.3.1/how_fake_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-06-27 11:17:16.000000 how_fake_accounts-0.3.1/how_fake_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       70 2023-06-27 11:17:16.000000 how_fake_accounts-0.3.1/how_fake_accounts.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        6 2023-06-27 11:17:16.000000 how_fake_accounts-0.3.1/how_fake_accounts.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       18 2023-06-27 11:17:16.000000 how_fake_accounts-0.3.1/how_fake_accounts.egg-info/top_level.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-06-27 11:17:17.026312 how_fake_accounts-0.3.1/setup.cfg
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      450 2023-06-27 11:17:09.000000 how_fake_accounts-0.3.1/setup.py
```

### Comparing `how_fake_accounts-0.3.0/how_fake_accounts/__main__.py` & `how_fake_accounts-0.3.1/how_fake_accounts/__main__.py`

 * *Files identical despite different names*

### Comparing `how_fake_accounts-0.3.0/how_fake_accounts/core.py` & `how_fake_accounts-0.3.1/how_fake_accounts/core.py`

 * *Files identical despite different names*

