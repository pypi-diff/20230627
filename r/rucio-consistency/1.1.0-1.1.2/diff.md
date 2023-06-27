# Comparing `tmp/rucio-consistency-1.1.0.tar.gz` & `tmp/rucio-consistency-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.1.0.tar", last modified: Tue May 23 17:50:56 2023, max compression
+gzip compressed data, was "rucio-consistency-1.1.2.tar", last modified: Tue Jun 27 14:49:51 2023, max compression
```

## Comparing `rucio-consistency-1.1.0.tar` & `rucio-consistency-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-23 17:50:56.120522 rucio-consistency-1.1.0/
--rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.1.0/LICENSE
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-05-23 17:50:56.120147 rucio-consistency-1.1.0/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)    12399 2023-05-19 14:17:54.000000 rucio-consistency-1.1.0/README.rst
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-23 17:50:56.113993 rucio-consistency-1.1.0/rucio_consistency/
--rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.1.0/rucio_consistency/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     4635 2023-04-21 14:37:25.000000 rucio-consistency-1.1.0/rucio_consistency/cmplib.py
--rw-r--r--   0 ivm        (501) staff       (20)    11469 2023-04-13 15:28:19.000000 rucio-consistency-1.1.0/rucio_consistency/config.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     5417 2023-04-21 14:37:27.000000 rucio-consistency-1.1.0/rucio_consistency/part.py
--rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.1.0/rucio_consistency/py3.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-23 17:50:56.118488 rucio-consistency-1.1.0/rucio_consistency/scripts/
--rwxr-xr-x   0 ivm        (501) staff       (20)     3532 2023-04-13 22:36:38.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3596 2023-04-13 22:34:51.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     4317 2023-04-13 22:36:42.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    10323 2023-05-23 15:56:13.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/db_dump.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/partition.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/update_stats.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.1.0/rucio_consistency/stats.py
--rw-r--r--   0 ivm        (501) staff       (20)      124 2023-05-23 17:49:31.000000 rucio-consistency-1.1.0/rucio_consistency/version.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-23 17:50:56.119561 rucio-consistency-1.1.0/rucio_consistency/xrootd/
--rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.1.0/rucio_consistency/xrootd/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.1.0/rucio_consistency/xrootd/xrootd_client.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    27445 2023-04-13 19:31:22.000000 rucio-consistency-1.1.0/rucio_consistency/xrootd/xrootd_scanner.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-23 17:50:56.116348 rucio-consistency-1.1.0/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)      850 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (501) staff       (20)      388 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (501) staff       (20)       22 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (501) staff       (20)       18 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (501) staff       (20)       38 2023-05-23 17:50:56.120624 rucio-consistency-1.1.0/setup.cfg
--rw-r--r--   0 ivm        (501) staff       (20)     1391 2023-04-13 14:18:20.000000 rucio-consistency-1.1.0/setup.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-06-27 14:49:51.485765 rucio-consistency-1.1.2/
+-rw-r--r--   0 ivm        (503) staff       (20)    11357 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/LICENSE
+-rw-r--r--   0 ivm        (503) staff       (20)      369 2023-06-27 14:49:51.485478 rucio-consistency-1.1.2/PKG-INFO
+-rw-r--r--   0 ivm        (503) staff       (20)    12399 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/README.rst
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-06-27 14:49:51.479040 rucio-consistency-1.1.2/rucio_consistency/
+-rw-r--r--   0 ivm        (503) staff       (20)      378 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     4635 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (503) staff       (20)    11469 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     5417 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      372 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-06-27 14:49:51.483772 rucio-consistency-1.1.2/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (503) staff       (20)     3532 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     3596 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     4317 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    10323 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/db_dump.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     2737 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1069 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/scripts/update_stats.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     2523 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (503) staff       (20)      124 2023-06-27 14:49:47.000000 rucio-consistency-1.1.2/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-06-27 14:49:51.484959 rucio-consistency-1.1.2/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (503) staff       (20)       39 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     9449 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    27550 2023-06-27 14:40:37.000000 rucio-consistency-1.1.2/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-06-27 14:49:51.481296 rucio-consistency-1.1.2/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (503) staff       (20)      369 2023-06-27 14:49:50.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (503) staff       (20)      850 2023-06-27 14:49:51.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (503) staff       (20)        1 2023-06-27 14:49:50.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (503) staff       (20)      388 2023-06-27 14:49:51.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (503) staff       (20)        1 2023-06-27 14:49:50.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (503) staff       (20)       22 2023-06-27 14:49:51.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (503) staff       (20)       18 2023-06-27 14:49:51.000000 rucio-consistency-1.1.2/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (503) staff       (20)       38 2023-06-27 14:49:51.485885 rucio-consistency-1.1.2/setup.cfg
+-rw-r--r--   0 ivm        (503) staff       (20)     1391 2023-06-27 13:17:59.000000 rucio-consistency-1.1.2/setup.py
```

### Comparing `rucio-consistency-1.1.0/LICENSE` & `rucio-consistency-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/README.rst` & `rucio-consistency-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/cmplib.py` & `rucio-consistency-1.1.2/rucio_consistency/cmplib.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/config.py` & `rucio-consistency-1.1.2/rucio_consistency/config.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/part.py` & `rucio-consistency-1.1.2/rucio_consistency/part.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/scripts/cmp2.py` & `rucio-consistency-1.1.2/rucio_consistency/scripts/cmp2.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/scripts/cmp3.py` & `rucio-consistency-1.1.2/rucio_consistency/scripts/cmp3.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/scripts/cmp5.py` & `rucio-consistency-1.1.2/rucio_consistency/scripts/cmp5.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/scripts/db_dump.py` & `rucio-consistency-1.1.2/rucio_consistency/scripts/db_dump.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/scripts/partition.py` & `rucio-consistency-1.1.2/rucio_consistency/scripts/partition.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/scripts/update_stats.py` & `rucio-consistency-1.1.2/rucio_consistency/scripts/update_stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/stats.py` & `rucio-consistency-1.1.2/rucio_consistency/stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/xrootd/xrootd_client.py` & `rucio-consistency-1.1.2/rucio_consistency/xrootd/xrootd_client.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/rucio_consistency/xrootd/xrootd_scanner.py` & `rucio-consistency-1.1.2/rucio_consistency/xrootd/xrootd_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,17 @@
             self.Timeout = timeout
             self.Failed = False
             self.Error = None
 
         def run(self):
             self.Client = XRootDClient(self.Server, self.IsRedirector, self.ServerRoot, 
                     timeout=self.Timeout, name=f"XRootDClient({self.Root})")
+            print(f"prescanning {self.Server} {self.Root} ...")
             self.Client.prescan(self.Root)
+            print("    will use servers:", self.Client.Servers)
             status, self.Error, _, _ = self.Client.ls(self.Root, False, False)
             self.Failed = status != "OK"
             return not self.Failed
 
     def __init__(self, server, server_root, is_redirector, roots, timeout, max_scanners):
         Primitive.__init__(self)
         self.Good = []              # [client, ...]
@@ -130,15 +132,14 @@
         self.Client = client
         self.Master = master
         self.Location = canonic_path(location)
         self.ForcedFlat = not recursive
         self.WasRecursive = recursive
         self.Subprocess = None
         self.Killed = False
-        self.Started = None
         self.Elapsed = None
         self.RecAttempts = self.MAX_ATTEMPTS_REC if recursive else 0
         self.FlatAttempts = self.MAX_ATTEMPTS_FLAT
         self.ZeroAttempts = self.MAX_REC_ZERO_RETRY
         self.IncludeSizes = include_sizes
         self.ReportEmptyTop = report_empty_top
         self.Timeout = timeout
@@ -161,32 +162,32 @@
         words = path.rsplit('/', 1)
         if len(words) == 1:
             return ""               # relative path ??
         return words[0] or "/"
                 
     def run(self):
         #print("Scanner.run():", self.Master)
-        self.Started = t0 = time.time()
+        t0 = time.time()
         location = self.Location
         if self.RecAttempts > 0:
             recursive = True
             self.RecAttempts -= 1
         else:
             recursive = False
             self.FlatAttempts -= 1
         self.WasRecursive = recursive
         #self.message("start", stats)
-        stats = "r" if recursive else " "
 
         # Location is relative to the server root, it does start with '/'. E.g. /store/mc/run2
         status, reason, dirs, files = self.Client.ls(self.Location, recursive, self.IncludeSizes, timeout=self.Timeout)
         # paths are relative to the Server Root, they do start with '/', e.g. /store/mc/run2/data.file
         files = list(files)
         dirs = list(dirs)
         self.Elapsed = time.time() - self.Started
+        stats = ("r" if recursive else " ") + " t=%6.1fs" % (self.Elapsed,)
         if status != "OK":
             stats += " " + reason
             self.message(status, stats)
             if self.Master is not None:
                 self.Master.scanner_failed(self, f"{status}: {reason}")
             return
 
@@ -667,15 +668,15 @@
     my_stats["roots"] = my_stats_roots = []
     for root, error in failed_roots.items():
         expected = root_file_counts.get(root, 0) > 0
         my_stats_roots.append({
                 "root": root,
                 "expected": expected,
                 "start_time":t0,
-                "timeout":config.ScannerTimeout,
+                "timeout":timeout,
                 "root_failed": True,
                 "error": error,
                 "end_time":t1,
                 "files": 0,
                 "directories": 0,
                 "elapsed_time": t1-t0
             })
```

### Comparing `rucio-consistency-1.1.0/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.1.2/rucio_consistency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.1.0/setup.py` & `rucio-consistency-1.1.2/setup.py`

 * *Files identical despite different names*

