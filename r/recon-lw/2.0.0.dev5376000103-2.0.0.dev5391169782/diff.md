# Comparing `tmp/recon_lw-2.0.0.dev5376000103.tar.gz` & `tmp/recon_lw-2.0.0.dev5391169782.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5376000103.tar", last modified: Mon Jun 26 08:40:13 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5391169782.tar", last modified: Tue Jun 27 14:38:43 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5376000103.tar` & `recon_lw-2.0.0.dev5391169782.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-26 08:39:47.000000 recon_lw-2.0.0.dev5376000103/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    33427 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-27 14:38:24.000000 recon_lw-2.0.0.dev5391169782/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33433 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:38:43.000000 recon_lw-2.0.0.dev5391169782/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-27 14:38:00.000000 recon_lw-2.0.0.dev5391169782/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5391169782/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5391169782/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5391169782/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5391169782/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5391169782/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5391169782/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5391169782/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5391169782/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,15 +732,15 @@
     keys = ["bid_aggr","bid_aggr"]
     shifts = [0,5]
     for i in range(levels):
         line = []
         for key, shift in zip(keys, shifts):
             if i < len(order_book[key]):
                 for j in range(5):
-                    line.append(order_book[key][i][header[j+shift]])
+                    line.append(order_book[key][i].get([header[j+shift]]))
             else:
                 line.extend([None]*5)
         result.append(line)
     return result
 
 
 def display_l3(order_book):
```

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5391169782/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5391169782/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5391169782/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/setup.py` & `recon_lw-2.0.0.dev5391169782/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5376000103/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5391169782/test/test_recon_ob.py`

 * *Files identical despite different names*

