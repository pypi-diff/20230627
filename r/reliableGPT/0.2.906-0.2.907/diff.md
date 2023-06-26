# Comparing `tmp/reliableGPT-0.2.906.tar.gz` & `tmp/reliableGPT-0.2.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.906.tar", last modified: Mon Jun 26 22:46:56 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.907.tar", last modified: Mon Jun 26 22:51:21 2023, max compression
```

## Comparing `reliableGPT-0.2.906.tar` & `reliableGPT-0.2.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:46:56.630522 reliableGPT-0.2.906/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.906/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 22:46:56.630421 reliableGPT-0.2.906/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.906/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:46:56.629104 reliableGPT-0.2.906/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 22:46:56.000000 reliableGPT-0.2.906/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      354 2023-06-26 22:46:56.000000 reliableGPT-0.2.906/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 22:46:56.000000 reliableGPT-0.2.906/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 22:46:56.000000 reliableGPT-0.2.906/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 22:46:56.000000 reliableGPT-0.2.906/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:46:56.630150 reliableGPT-0.2.906/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.906/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3049 2023-06-26 22:46:08.000000 reliableGPT-0.2.906/reliablegpt/api_handler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 22:46:07.000000 reliableGPT-0.2.906/reliablegpt/custom_queue.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    14392 2023-06-26 22:45:07.000000 reliableGPT-0.2.906/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1427 2023-06-26 22:46:47.000000 reliableGPT-0.2.906/reliablegpt/test_batching.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.906/reliablegpt/tests_main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 22:46:56.630562 reliableGPT-0.2.906/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      351 2023-06-26 22:46:23.000000 reliableGPT-0.2.906/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:51:21.658309 reliableGPT-0.2.907/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.907/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 22:51:21.658208 reliableGPT-0.2.907/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.907/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:51:21.657421 reliableGPT-0.2.907/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 22:51:21.000000 reliableGPT-0.2.907/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      354 2023-06-26 22:51:21.000000 reliableGPT-0.2.907/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 22:51:21.000000 reliableGPT-0.2.907/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 22:51:21.000000 reliableGPT-0.2.907/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 22:51:21.000000 reliableGPT-0.2.907/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 22:51:21.658050 reliableGPT-0.2.907/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      142 2023-06-26 22:50:20.000000 reliableGPT-0.2.907/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3049 2023-06-26 22:46:08.000000 reliableGPT-0.2.907/reliablegpt/api_handler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 22:46:07.000000 reliableGPT-0.2.907/reliablegpt/custom_queue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    14392 2023-06-26 22:45:07.000000 reliableGPT-0.2.907/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1427 2023-06-26 22:46:47.000000 reliableGPT-0.2.907/reliablegpt/test_batching.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.907/reliablegpt/tests_main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 22:51:21.658344 reliableGPT-0.2.907/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      351 2023-06-26 22:50:31.000000 reliableGPT-0.2.907/setup.py
```

### Comparing `reliableGPT-0.2.906/LICENSE` & `reliableGPT-0.2.907/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.906/README.md` & `reliableGPT-0.2.907/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.906/reliablegpt/api_handler.py` & `reliableGPT-0.2.907/reliablegpt/api_handler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.906/reliablegpt/custom_queue.py` & `reliableGPT-0.2.907/reliablegpt/custom_queue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.906/reliablegpt/main.py` & `reliableGPT-0.2.907/reliablegpt/main.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.906/reliablegpt/test_batching.py` & `reliableGPT-0.2.907/reliablegpt/test_batching.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.906/reliablegpt/tests_main.py` & `reliableGPT-0.2.907/reliablegpt/tests_main.py`

 * *Files identical despite different names*

