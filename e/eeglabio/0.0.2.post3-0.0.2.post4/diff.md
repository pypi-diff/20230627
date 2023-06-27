# Comparing `tmp/eeglabio-0.0.2.post3.tar.gz` & `tmp/eeglabio-0.0.2.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eeglabio-0.0.2.post3.tar", last modified: Sat Oct 22 01:41:09 2022, max compression
+gzip compressed data, was "eeglabio-0.0.2.post4.tar", last modified: Mon Jun 26 23:59:52 2023, max compression
```

## Comparing `eeglabio-0.0.2.post3.tar` & `eeglabio-0.0.2.post4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 01:41:09.980460 eeglabio-0.0.2.post3/
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-10-22 01:40:27.000000 eeglabio-0.0.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-22 01:40:27.000000 eeglabio-0.0.2.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2669 2022-10-22 01:41:09.980460 eeglabio-0.0.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-10-22 01:40:27.000000 eeglabio-0.0.2.post3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 01:41:09.980460 eeglabio-0.0.2.post3/eeglabio/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-10-22 01:40:27.000000 eeglabio-0.0.2.post3/eeglabio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-10-22 01:40:27.000000 eeglabio-0.0.2.post3/eeglabio/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     8928 2022-10-22 01:40:27.000000 eeglabio-0.0.2.post3/eeglabio/epochs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-10-22 01:40:27.000000 eeglabio-0.0.2.post3/eeglabio/raw.py
--rw-r--r--   0 runner    (1001) docker     (121)     6491 2022-10-22 01:40:27.000000 eeglabio-0.0.2.post3/eeglabio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 01:41:09.980460 eeglabio-0.0.2.post3/eeglabio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2669 2022-10-22 01:41:09.000000 eeglabio-0.0.2.post3/eeglabio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-10-22 01:41:09.000000 eeglabio-0.0.2.post3/eeglabio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-22 01:41:09.000000 eeglabio-0.0.2.post3/eeglabio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-22 01:41:09.000000 eeglabio-0.0.2.post3/eeglabio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-22 01:41:09.000000 eeglabio-0.0.2.post3/eeglabio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-22 01:40:27.000000 eeglabio-0.0.2.post3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-22 01:41:09.980460 eeglabio-0.0.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-10-22 01:40:27.000000 eeglabio-0.0.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:59:52.962158 eeglabio-0.0.2.post4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-26 23:59:14.000000 eeglabio-0.0.2.post4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 23:59:14.000000 eeglabio-0.0.2.post4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-26 23:59:52.962158 eeglabio-0.0.2.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-26 23:59:14.000000 eeglabio-0.0.2.post4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:59:52.962158 eeglabio-0.0.2.post4/eeglabio/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 23:59:14.000000 eeglabio-0.0.2.post4/eeglabio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 23:59:14.000000 eeglabio-0.0.2.post4/eeglabio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-06-26 23:59:14.000000 eeglabio-0.0.2.post4/eeglabio/epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-26 23:59:14.000000 eeglabio-0.0.2.post4/eeglabio/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-06-26 23:59:14.000000 eeglabio-0.0.2.post4/eeglabio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:59:52.962158 eeglabio-0.0.2.post4/eeglabio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-26 23:59:52.000000 eeglabio-0.0.2.post4/eeglabio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-26 23:59:52.000000 eeglabio-0.0.2.post4/eeglabio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 23:59:52.000000 eeglabio-0.0.2.post4/eeglabio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 23:59:52.000000 eeglabio-0.0.2.post4/eeglabio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 23:59:52.000000 eeglabio-0.0.2.post4/eeglabio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 23:59:14.000000 eeglabio-0.0.2.post4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 23:59:52.962158 eeglabio-0.0.2.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-26 23:59:14.000000 eeglabio-0.0.2.post4/setup.py
```

### Comparing `eeglabio-0.0.2.post3/LICENSE` & `eeglabio-0.0.2.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `eeglabio-0.0.2.post3/PKG-INFO` & `eeglabio-0.0.2.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eeglabio
-Version: 0.0.2.post3
+Version: 0.0.2.post4
 Summary: I/O support for EEGLAB files in Python
 Home-page: https://github.com/jackz314/eeglabio
 Download-URL: https://github.com/jackz314/eeglabio
 Author: Jack Zhang
 Author-email: zhangmengyu10@gmail.com
 License: BSD (3-clause)
 Project-URL: Source, https://github.com/jackz314/eeglabio
```

### Comparing `eeglabio-0.0.2.post3/README.md` & `eeglabio-0.0.2.post4/README.md`

 * *Files identical despite different names*

### Comparing `eeglabio-0.0.2.post3/eeglabio/epochs.py` & `eeglabio-0.0.2.post4/eeglabio/epochs.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     ev_dur = np.zeros_like(ev_lat, dtype=np.int64)
 
     # indices of epochs each event belongs to
     ev_epoch = ev_lat // epoch_len + 1
     if len(ev_epoch) > 0 and max(ev_epoch) > trials:
         # probably due to shifted/wrong events latency
         # reset events to start at the beginning of each epoch
-        ev_epoch = np.arange(1, trials + 1)
+        ev_epoch = np.arange(1, trials + 1, dtype=np.int64)
         ev_lat = (ev_epoch - 1) * epoch_len
         logger.warning("Invalid event latencies, ignored for export.")
 
     # merge annotations into events array
     if annotations is not None:
         data_len = epoch_len * trials
         annot_lat = np.array(annotations[1]) * sfreq + 1  # +1 for eeglab
```

### Comparing `eeglabio-0.0.2.post3/eeglabio/raw.py` & `eeglabio-0.0.2.post4/eeglabio/raw.py`

 * *Files identical despite different names*

### Comparing `eeglabio-0.0.2.post3/eeglabio/utils.py` & `eeglabio-0.0.2.post4/eeglabio/utils.py`

 * *Files identical despite different names*

### Comparing `eeglabio-0.0.2.post3/eeglabio.egg-info/PKG-INFO` & `eeglabio-0.0.2.post4/eeglabio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eeglabio
-Version: 0.0.2.post3
+Version: 0.0.2.post4
 Summary: I/O support for EEGLAB files in Python
 Home-page: https://github.com/jackz314/eeglabio
 Download-URL: https://github.com/jackz314/eeglabio
 Author: Jack Zhang
 Author-email: zhangmengyu10@gmail.com
 License: BSD (3-clause)
 Project-URL: Source, https://github.com/jackz314/eeglabio
```

### Comparing `eeglabio-0.0.2.post3/setup.py` & `eeglabio-0.0.2.post4/setup.py`

 * *Files identical despite different names*

