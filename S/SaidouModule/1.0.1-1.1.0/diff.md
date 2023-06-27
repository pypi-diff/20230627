# Comparing `tmp/SaidouModule-1.0.1.tar.gz` & `tmp/SaidouModule-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SaidouModule-1.0.1.tar", last modified: Tue Jun 27 14:03:41 2023, max compression
+gzip compressed data, was "SaidouModule-1.1.0.tar", last modified: Tue Jun 27 17:47:01 2023, max compression
```

## Comparing `SaidouModule-1.0.1.tar` & `SaidouModule-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 14:03:41.269208 SaidouModule-1.0.1/
--rw-rw-rw-   0        0        0      268 2023-06-27 14:03:41.269208 SaidouModule-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      647 2023-06-27 13:09:18.000000 SaidouModule-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 14:03:41.206825 SaidouModule-1.0.1/SaidouModule.egg-info/
--rw-rw-rw-   0        0        0      268 2023-06-27 14:03:41.000000 SaidouModule-1.0.1/SaidouModule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-06-27 14:03:41.000000 SaidouModule-1.0.1/SaidouModule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 14:03:41.000000 SaidouModule-1.0.1/SaidouModule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-27 14:03:41.000000 SaidouModule-1.0.1/SaidouModule.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-06-27 14:03:41.000000 SaidouModule-1.0.1/SaidouModule.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 14:03:41.269208 SaidouModule-1.0.1/SaidouNeurones/
--rw-rw-rw-   0        0        0     6550 2023-06-27 11:56:01.000000 SaidouModule-1.0.1/SaidouNeurones/ReseauNeuronesSaid.py
--rw-rw-rw-   0        0        0       66 2023-06-27 11:57:01.000000 SaidouModule-1.0.1/SaidouNeurones/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:03:41.269208 SaidouModule-1.0.1/SaidouPixels/
--rw-rw-rw-   0        0        0     3322 2023-06-16 19:31:08.000000 SaidouModule-1.0.1/SaidouPixels/Pixels.py
--rw-rw-rw-   0        0        0       63 2023-06-27 11:57:36.000000 SaidouModule-1.0.1/SaidouPixels/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-27 14:03:41.269208 SaidouModule-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-06-27 14:01:43.000000 SaidouModule-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:47:01.001941 SaidouModule-1.1.0/
+-rw-rw-rw-   0        0        0      268 2023-06-27 17:47:00.977490 SaidouModule-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2023-06-27 13:09:18.000000 SaidouModule-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:47:00.957528 SaidouModule-1.1.0/SaidouModule.egg-info/
+-rw-rw-rw-   0        0        0      268 2023-06-27 17:46:58.000000 SaidouModule-1.1.0/SaidouModule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-27 17:46:58.000000 SaidouModule-1.1.0/SaidouModule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:46:58.000000 SaidouModule-1.1.0/SaidouModule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-27 17:46:58.000000 SaidouModule-1.1.0/SaidouModule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-06-27 17:46:58.000000 SaidouModule-1.1.0/SaidouModule.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 17:47:00.971533 SaidouModule-1.1.0/SaidouNeurones/
+-rw-rw-rw-   0        0        0     6550 2023-06-27 11:56:01.000000 SaidouModule-1.1.0/SaidouNeurones/ReseauNeuronesSaid.py
+-rw-rw-rw-   0        0        0     7172 2023-06-27 17:45:02.000000 SaidouModule-1.1.0/SaidouNeurones/SaidouNeuroneV2.py
+-rw-rw-rw-   0        0        0       66 2023-06-27 11:57:01.000000 SaidouModule-1.1.0/SaidouNeurones/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:47:00.975495 SaidouModule-1.1.0/SaidouPixels/
+-rw-rw-rw-   0        0        0     3322 2023-06-16 19:31:08.000000 SaidouModule-1.1.0/SaidouPixels/Pixels.py
+-rw-rw-rw-   0        0        0       63 2023-06-27 11:57:36.000000 SaidouModule-1.1.0/SaidouPixels/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:47:01.001941 SaidouModule-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-06-27 17:45:38.000000 SaidouModule-1.1.0/setup.py
```

### Comparing `SaidouModule-1.0.1/README.md` & `SaidouModule-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `SaidouModule-1.0.1/SaidouNeurones/ReseauNeuronesSaid.py` & `SaidouModule-1.1.0/SaidouNeurones/ReseauNeuronesSaid.py`

 * *Files identical despite different names*

### Comparing `SaidouModule-1.0.1/SaidouPixels/Pixels.py` & `SaidouModule-1.1.0/SaidouPixels/Pixels.py`

 * *Files identical despite different names*

