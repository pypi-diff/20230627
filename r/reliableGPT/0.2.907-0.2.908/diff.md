# Comparing `tmp/reliableGPT-0.2.907.tar.gz` & `tmp/reliableGPT-0.2.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.907.tar", last modified: Mon Jun 26 22:51:21 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.908.tar", last modified: Mon Jun 26 22:56:22 2023, max compression
```

## Comparing `reliableGPT-0.2.907.tar` & `reliableGPT-0.2.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:51:21.658309 reliableGPT-0.2.907/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.907/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 22:51:21.658208 reliableGPT-0.2.907/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.907/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:51:21.657421 reliableGPT-0.2.907/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 22:51:21.000000 reliableGPT-0.2.907/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      354 2023-06-26 22:51:21.000000 reliableGPT-0.2.907/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 22:51:21.000000 reliableGPT-0.2.907/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 22:51:21.000000 reliableGPT-0.2.907/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 22:51:21.000000 reliableGPT-0.2.907/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:51:21.658050 reliableGPT-0.2.907/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      142 2023-06-26 22:50:20.000000 reliableGPT-0.2.907/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3049 2023-06-26 22:46:08.000000 reliableGPT-0.2.907/reliablegpt/api_handler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 22:46:07.000000 reliableGPT-0.2.907/reliablegpt/custom_queue.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    14392 2023-06-26 22:45:07.000000 reliableGPT-0.2.907/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1427 2023-06-26 22:46:47.000000 reliableGPT-0.2.907/reliablegpt/test_batching.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.907/reliablegpt/tests_main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 22:51:21.658344 reliableGPT-0.2.907/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      351 2023-06-26 22:50:31.000000 reliableGPT-0.2.907/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:56:22.216030 reliableGPT-0.2.908/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.908/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 22:56:22.215931 reliableGPT-0.2.908/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.908/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:56:22.214224 reliableGPT-0.2.908/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 22:56:22.000000 reliableGPT-0.2.908/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      354 2023-06-26 22:56:22.000000 reliableGPT-0.2.908/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 22:56:22.000000 reliableGPT-0.2.908/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       72 2023-06-26 22:56:22.000000 reliableGPT-0.2.908/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 22:56:22.000000 reliableGPT-0.2.908/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:56:22.215677 reliableGPT-0.2.908/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      142 2023-06-26 22:50:20.000000 reliableGPT-0.2.908/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3049 2023-06-26 22:46:08.000000 reliableGPT-0.2.908/reliablegpt/api_handler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 22:46:07.000000 reliableGPT-0.2.908/reliablegpt/custom_queue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    14392 2023-06-26 22:45:07.000000 reliableGPT-0.2.908/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1427 2023-06-26 22:46:47.000000 reliableGPT-0.2.908/reliablegpt/test_batching.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.908/reliablegpt/tests_main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 22:56:22.216067 reliableGPT-0.2.908/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      398 2023-06-26 22:56:14.000000 reliableGPT-0.2.908/setup.py
```

### Comparing `reliableGPT-0.2.907/LICENSE` & `reliableGPT-0.2.908/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.907/README.md` & `reliableGPT-0.2.908/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.907/reliablegpt/api_handler.py` & `reliableGPT-0.2.908/reliablegpt/api_handler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.907/reliablegpt/custom_queue.py` & `reliableGPT-0.2.908/reliablegpt/custom_queue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.907/reliablegpt/main.py` & `reliableGPT-0.2.908/reliablegpt/main.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.907/reliablegpt/test_batching.py` & `reliableGPT-0.2.908/reliablegpt/test_batching.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.907/reliablegpt/tests_main.py` & `reliableGPT-0.2.908/reliablegpt/tests_main.py`

 * *Files identical despite different names*

