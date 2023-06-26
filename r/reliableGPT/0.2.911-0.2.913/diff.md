# Comparing `tmp/reliableGPT-0.2.911.tar.gz` & `tmp/reliableGPT-0.2.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.911.tar", last modified: Mon Jun 26 23:14:25 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.913.tar", last modified: Mon Jun 26 23:25:21 2023, max compression
```

## Comparing `reliableGPT-0.2.911.tar` & `reliableGPT-0.2.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:14:25.443653 reliableGPT-0.2.911/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.911/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 23:14:25.443553 reliableGPT-0.2.911/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.911/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:14:25.442395 reliableGPT-0.2.911/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 23:14:25.000000 reliableGPT-0.2.911/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      354 2023-06-26 23:14:25.000000 reliableGPT-0.2.911/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 23:14:25.000000 reliableGPT-0.2.911/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 23:14:25.000000 reliableGPT-0.2.911/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 23:14:25.000000 reliableGPT-0.2.911/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:14:25.443302 reliableGPT-0.2.911/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      142 2023-06-26 23:14:06.000000 reliableGPT-0.2.911/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3049 2023-06-26 23:10:13.000000 reliableGPT-0.2.911/reliablegpt/api_handler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 23:14:04.000000 reliableGPT-0.2.911/reliablegpt/custom_queue.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    14392 2023-06-26 22:45:07.000000 reliableGPT-0.2.911/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1427 2023-06-26 23:10:37.000000 reliableGPT-0.2.911/reliablegpt/test_batching.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.911/reliablegpt/tests_main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 23:14:25.443689 reliableGPT-0.2.911/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      366 2023-06-26 23:14:10.000000 reliableGPT-0.2.911/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:25:21.801084 reliableGPT-0.2.913/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.913/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 23:25:21.800988 reliableGPT-0.2.913/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.913/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:25:21.799725 reliableGPT-0.2.913/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 23:25:21.000000 reliableGPT-0.2.913/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      354 2023-06-26 23:25:21.000000 reliableGPT-0.2.913/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 23:25:21.000000 reliableGPT-0.2.913/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 23:25:21.000000 reliableGPT-0.2.913/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 23:25:21.000000 reliableGPT-0.2.913/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 23:25:21.800753 reliableGPT-0.2.913/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      140 2023-06-26 23:24:12.000000 reliableGPT-0.2.913/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3049 2023-06-26 23:10:13.000000 reliableGPT-0.2.913/reliablegpt/api_handler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 23:14:04.000000 reliableGPT-0.2.913/reliablegpt/custom_queue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    14392 2023-06-26 23:25:10.000000 reliableGPT-0.2.913/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1427 2023-06-26 23:10:37.000000 reliableGPT-0.2.913/reliablegpt/test_batching.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.913/reliablegpt/tests_main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 23:25:21.801123 reliableGPT-0.2.913/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      380 2023-06-26 23:25:14.000000 reliableGPT-0.2.913/setup.py
```

### Comparing `reliableGPT-0.2.911/LICENSE` & `reliableGPT-0.2.913/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.911/README.md` & `reliableGPT-0.2.913/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.911/reliablegpt/api_handler.py` & `reliableGPT-0.2.913/reliablegpt/api_handler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.911/reliablegpt/custom_queue.py` & `reliableGPT-0.2.913/reliablegpt/custom_queue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.911/reliablegpt/main.py` & `reliableGPT-0.2.913/reliablegpt/main.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.911/reliablegpt/test_batching.py` & `reliableGPT-0.2.913/reliablegpt/test_batching.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.911/reliablegpt/tests_main.py` & `reliableGPT-0.2.913/reliablegpt/tests_main.py`

 * *Files identical despite different names*

