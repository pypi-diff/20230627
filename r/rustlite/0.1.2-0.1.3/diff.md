# Comparing `tmp/rustlite-0.1.2.tar.gz` & `tmp/rustlite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustlite-0.1.2.tar", last modified: Tue Jun 27 07:57:01 2023, max compression
+gzip compressed data, was "rustlite-0.1.3.tar", last modified: Tue Jun 27 08:09:26 2023, max compression
```

## Comparing `rustlite-0.1.2.tar` & `rustlite-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 07:57:01.388037 rustlite-0.1.2/
--rw-rw-rw-   0        0        0      445 2023-06-27 07:57:01.386667 rustlite-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-06-27 07:40:19.000000 rustlite-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 07:57:01.380752 rustlite-0.1.2/rustlite/
--rw-rw-rw-   0        0        0       58 2023-06-26 20:35:57.000000 rustlite-0.1.2/rustlite/__init__.py
--rw-rw-rw-   0        0        0     3183 2023-06-27 07:37:24.000000 rustlite-0.1.2/rustlite/enumerable.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:57:01.386667 rustlite-0.1.2/rustlite.egg-info/
--rw-rw-rw-   0        0        0      445 2023-06-27 07:57:01.000000 rustlite-0.1.2/rustlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-27 07:57:01.000000 rustlite-0.1.2/rustlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 07:57:01.000000 rustlite-0.1.2/rustlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 07:57:01.000000 rustlite-0.1.2/rustlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 07:57:01.388037 rustlite-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      565 2023-06-27 07:56:45.000000 rustlite-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:09:26.228732 rustlite-0.1.3/
+-rw-rw-rw-   0        0        0      978 2023-06-27 08:09:26.228732 rustlite-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-06-27 08:07:58.000000 rustlite-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 08:09:26.217840 rustlite-0.1.3/rustlite/
+-rw-rw-rw-   0        0        0       58 2023-06-26 20:35:57.000000 rustlite-0.1.3/rustlite/__init__.py
+-rw-rw-rw-   0        0        0     3183 2023-06-27 07:37:24.000000 rustlite-0.1.3/rustlite/enumerable.py
+drwxrwxrwx   0        0        0        0 2023-06-27 08:09:26.227733 rustlite-0.1.3/rustlite.egg-info/
+-rw-rw-rw-   0        0        0      978 2023-06-27 08:09:26.000000 rustlite-0.1.3/rustlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-27 08:09:26.000000 rustlite-0.1.3/rustlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 08:09:26.000000 rustlite-0.1.3/rustlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 08:09:26.000000 rustlite-0.1.3/rustlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 08:09:26.229970 rustlite-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-06-27 08:09:22.000000 rustlite-0.1.3/setup.py
```

### Comparing `rustlite-0.1.2/rustlite/enumerable.py` & `rustlite-0.1.3/rustlite/enumerable.py`

 * *Files identical despite different names*

