# Comparing `tmp/dcentrapi-0.2.85.tar.gz` & `tmp/dcentrapi-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.85.tar", last modified: Tue Jun 27 07:18:38 2023, max compression
+gzip compressed data, was "dcentrapi-0.2.9.tar", last modified: Tue Jun 27 07:19:50 2023, max compression
```

## Comparing `dcentrapi-0.2.85.tar` & `dcentrapi-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 07:18:38.417021 dcentrapi-0.2.85/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.85/LICENSE.rst
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-27 07:18:38.416875 dcentrapi-0.2.85/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.85/README.md
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 07:18:38.415852 dcentrapi-0.2.85/dcentrapi/
--rw-r--r--   0 nivshitrit   (501) staff       (20)      829 2023-05-24 09:45:16.000000 dcentrapi-0.2.85/dcentrapi/Base.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      334 2023-06-27 07:18:35.000000 dcentrapi-0.2.85/dcentrapi/__init__.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      196 2023-06-27 07:15:07.000000 dcentrapi-0.2.85/dcentrapi/common.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     8714 2023-06-05 07:36:17.000000 dcentrapi-0.2.85/dcentrapi/eventPolling.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-03-02 14:02:13.000000 dcentrapi-0.2.85/dcentrapi/gasMonitor.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      556 2023-06-27 07:14:40.000000 dcentrapi-0.2.85/dcentrapi/hackMitigation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.85/dcentrapi/merkleTree.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3059 2023-06-05 07:36:17.000000 dcentrapi-0.2.85/dcentrapi/rpcAggregation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      804 2023-05-31 13:35:59.000000 dcentrapi-0.2.85/dcentrapi/web3Index.py
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 07:18:38.416669 dcentrapi-0.2.85/dcentrapi.egg-info/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-27 07:18:38.000000 dcentrapi-0.2.85/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)      407 2023-06-27 07:18:38.000000 dcentrapi-0.2.85/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-06-27 07:18:38.000000 dcentrapi-0.2.85/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-06-27 07:18:38.000000 dcentrapi-0.2.85/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-06-27 07:18:38.000000 dcentrapi-0.2.85/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-06-27 07:18:38.417071 dcentrapi-0.2.85/setup.cfg
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.85/setup.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 07:19:50.546691 dcentrapi-0.2.9/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.9/LICENSE.rst
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-06-27 07:19:50.546568 dcentrapi-0.2.9/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.9/README.md
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 07:19:50.545811 dcentrapi-0.2.9/dcentrapi/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      829 2023-05-24 09:45:16.000000 dcentrapi-0.2.9/dcentrapi/Base.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      332 2023-06-27 07:19:17.000000 dcentrapi-0.2.9/dcentrapi/__init__.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      195 2023-06-27 07:19:25.000000 dcentrapi-0.2.9/dcentrapi/common.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     8714 2023-06-05 07:36:17.000000 dcentrapi-0.2.9/dcentrapi/eventPolling.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-03-02 14:02:13.000000 dcentrapi-0.2.9/dcentrapi/gasMonitor.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      525 2023-06-27 07:19:29.000000 dcentrapi-0.2.9/dcentrapi/hackMitigation.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.9/dcentrapi/merkleTree.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3059 2023-06-05 07:36:17.000000 dcentrapi-0.2.9/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      804 2023-05-31 13:35:59.000000 dcentrapi-0.2.9/dcentrapi/web3Index.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-27 07:19:50.546403 dcentrapi-0.2.9/dcentrapi.egg-info/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-06-27 07:19:50.000000 dcentrapi-0.2.9/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      407 2023-06-27 07:19:50.000000 dcentrapi-0.2.9/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-06-27 07:19:50.000000 dcentrapi-0.2.9/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-06-27 07:19:50.000000 dcentrapi-0.2.9/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-06-27 07:19:50.000000 dcentrapi-0.2.9/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-06-27 07:19:50.546731 dcentrapi-0.2.9/setup.cfg
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.9/setup.py
```

### Comparing `dcentrapi-0.2.85/LICENSE.rst` & `dcentrapi-0.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.85/PKG-INFO` & `dcentrapi-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.85
+Version: 0.2.9
 Summary: Dcentralab Pypi packages
 Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `dcentrapi-0.2.85/README.md` & `dcentrapi-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.85/dcentrapi/Base.py` & `dcentrapi-0.2.9/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.85/dcentrapi/eventPolling.py` & `dcentrapi-0.2.9/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.85/dcentrapi/merkleTree.py` & `dcentrapi-0.2.9/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.85/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.9/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.85/dcentrapi/web3Index.py` & `dcentrapi-0.2.9/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.85/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.9/dcentrapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.85
+Version: 0.2.9
 Summary: Dcentralab Pypi packages
 Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `dcentrapi-0.2.85/setup.py` & `dcentrapi-0.2.9/setup.py`

 * *Files identical despite different names*

