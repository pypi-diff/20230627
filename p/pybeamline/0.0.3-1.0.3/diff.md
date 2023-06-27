# Comparing `tmp/pybeamline-0.0.3.tar.gz` & `tmp/pybeamline-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybeamline-0.0.3.tar", last modified: Wed Jun 21 11:22:24 2023, max compression
+gzip compressed data, was "pybeamline-1.0.3.tar", last modified: Tue Jun 27 07:50:56 2023, max compression
```

## Comparing `pybeamline-0.0.3.tar` & `pybeamline-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 11:22:24.199225 pybeamline-0.0.3/
--rw-rw-rw-   0        0        0    11548 2023-06-21 08:34:26.000000 pybeamline-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     5018 2023-06-21 11:22:24.198725 pybeamline-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4785 2023-06-21 08:27:01.000000 pybeamline-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 11:22:23.994209 pybeamline-0.0.3/pybeamline/
--rw-rw-rw-   0        0        0        0 2023-06-20 12:16:17.000000 pybeamline-0.0.3/pybeamline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:22:24.027887 pybeamline-0.0.3/pybeamline/algorithms/
--rw-rw-rw-   0        0        0        0 2023-06-20 12:20:46.000000 pybeamline-0.0.3/pybeamline/algorithms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:22:24.050201 pybeamline-0.0.3/pybeamline/algorithms/conformance/
--rw-rw-rw-   0        0        0      195 2023-06-20 15:00:52.000000 pybeamline-0.0.3/pybeamline/algorithms/conformance/__init__.py
--rw-rw-rw-   0        0        0     9830 2023-06-20 15:43:46.000000 pybeamline-0.0.3/pybeamline/algorithms/conformance/behavioral_conformance.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:22:24.094271 pybeamline-0.0.3/pybeamline/algorithms/discovery/
--rw-rw-rw-   0        0        0      230 2023-06-20 12:14:51.000000 pybeamline-0.0.3/pybeamline/algorithms/discovery/__init__.py
--rw-rw-rw-   0        0        0     4690 2023-06-20 12:14:51.000000 pybeamline-0.0.3/pybeamline/algorithms/discovery/heuristics_miner_lossy_counting.py
--rw-rw-rw-   0        0        0     5298 2023-06-19 12:16:01.000000 pybeamline-0.0.3/pybeamline/algorithms/discovery/heuristics_miner_lossy_counting_budget.py
--rw-rw-rw-   0        0        0     1754 2023-06-20 12:16:17.000000 pybeamline-0.0.3/pybeamline/bevent.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:22:24.113274 pybeamline-0.0.3/pybeamline/filters/
--rw-rw-rw-   0        0        0      277 2023-06-20 12:16:17.000000 pybeamline-0.0.3/pybeamline/filters/__init__.py
--rw-rw-rw-   0        0        0     1888 2023-06-20 12:16:17.000000 pybeamline-0.0.3/pybeamline/filters/filters.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:22:24.152598 pybeamline-0.0.3/pybeamline/mappers/
--rw-rw-rw-   0        0        0      184 2023-06-20 12:16:17.000000 pybeamline-0.0.3/pybeamline/mappers/__init__.py
--rw-rw-rw-   0        0        0      753 2023-06-20 12:16:17.000000 pybeamline-0.0.3/pybeamline/mappers/infinite_size_directly_follows_mapper.py
--rw-rw-rw-   0        0        0      992 2023-06-20 12:16:17.000000 pybeamline-0.0.3/pybeamline/mappers/sliding_window_to_log.py
--rw-rw-rw-   0        0        0        0 2023-06-20 12:16:17.000000 pybeamline-0.0.3/pybeamline/pybeamline.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:22:24.189219 pybeamline-0.0.3/pybeamline/sources/
--rw-rw-rw-   0        0        0      666 2023-06-20 12:16:17.000000 pybeamline-0.0.3/pybeamline/sources/__init__.py
--rw-rw-rw-   0        0        0      767 2023-06-20 12:16:17.000000 pybeamline-0.0.3/pybeamline/sources/string_test_source.py
--rw-rw-rw-   0        0        0     1910 2023-06-21 07:29:23.000000 pybeamline-0.0.3/pybeamline/sources/xes_log_source.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:22:24.025959 pybeamline-0.0.3/pybeamline.egg-info/
--rw-rw-rw-   0        0        0     5018 2023-06-21 11:22:23.000000 pybeamline-0.0.3/pybeamline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      919 2023-06-21 11:22:23.000000 pybeamline-0.0.3/pybeamline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 11:22:23.000000 pybeamline-0.0.3/pybeamline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-21 11:22:23.000000 pybeamline-0.0.3/pybeamline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 11:22:23.000000 pybeamline-0.0.3/pybeamline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 11:22:24.199752 pybeamline-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-06-21 11:20:58.000000 pybeamline-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:22:24.197145 pybeamline-0.0.3/tests/
--rw-rw-rw-   0        0        0      850 2023-06-20 12:16:17.000000 pybeamline-0.0.3/tests/test_bevent.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:50:56.517282 pybeamline-1.0.3/
+-rw-rw-rw-   0        0        0    11548 2023-06-21 08:34:26.000000 pybeamline-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1289 2023-06-27 07:50:56.516738 pybeamline-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2023-06-22 06:47:54.000000 pybeamline-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 07:50:56.343802 pybeamline-1.0.3/pybeamline/
+-rw-rw-rw-   0        0        0        0 2023-06-20 12:16:17.000000 pybeamline-1.0.3/pybeamline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:50:56.375978 pybeamline-1.0.3/pybeamline/algorithms/
+-rw-rw-rw-   0        0        0        0 2023-06-20 12:20:46.000000 pybeamline-1.0.3/pybeamline/algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:50:56.399412 pybeamline-1.0.3/pybeamline/algorithms/conformance/
+-rw-rw-rw-   0        0        0      195 2023-06-20 15:00:52.000000 pybeamline-1.0.3/pybeamline/algorithms/conformance/__init__.py
+-rw-rw-rw-   0        0        0     9830 2023-06-20 15:43:46.000000 pybeamline-1.0.3/pybeamline/algorithms/conformance/behavioral_conformance.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:50:56.429655 pybeamline-1.0.3/pybeamline/algorithms/discovery/
+-rw-rw-rw-   0        0        0      230 2023-06-20 12:14:51.000000 pybeamline-1.0.3/pybeamline/algorithms/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4690 2023-06-20 12:14:51.000000 pybeamline-1.0.3/pybeamline/algorithms/discovery/heuristics_miner_lossy_counting.py
+-rw-rw-rw-   0        0        0     5298 2023-06-19 12:16:01.000000 pybeamline-1.0.3/pybeamline/algorithms/discovery/heuristics_miner_lossy_counting_budget.py
+-rw-rw-rw-   0        0        0     1754 2023-06-20 12:16:17.000000 pybeamline-1.0.3/pybeamline/bevent.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:50:56.448309 pybeamline-1.0.3/pybeamline/filters/
+-rw-rw-rw-   0        0        0      277 2023-06-20 12:16:17.000000 pybeamline-1.0.3/pybeamline/filters/__init__.py
+-rw-rw-rw-   0        0        0     1888 2023-06-20 12:16:17.000000 pybeamline-1.0.3/pybeamline/filters/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:50:56.476476 pybeamline-1.0.3/pybeamline/mappers/
+-rw-rw-rw-   0        0        0      184 2023-06-20 12:16:17.000000 pybeamline-1.0.3/pybeamline/mappers/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-06-20 12:16:17.000000 pybeamline-1.0.3/pybeamline/mappers/infinite_size_directly_follows_mapper.py
+-rw-rw-rw-   0        0        0      992 2023-06-20 12:16:17.000000 pybeamline-1.0.3/pybeamline/mappers/sliding_window_to_log.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 12:16:17.000000 pybeamline-1.0.3/pybeamline/pybeamline.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:50:56.506013 pybeamline-1.0.3/pybeamline/sources/
+-rw-rw-rw-   0        0        0      666 2023-06-20 12:16:17.000000 pybeamline-1.0.3/pybeamline/sources/__init__.py
+-rw-rw-rw-   0        0        0      767 2023-06-20 12:16:17.000000 pybeamline-1.0.3/pybeamline/sources/string_test_source.py
+-rw-rw-rw-   0        0        0     1910 2023-06-21 07:29:23.000000 pybeamline-1.0.3/pybeamline/sources/xes_log_source.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:50:56.374580 pybeamline-1.0.3/pybeamline.egg-info/
+-rw-rw-rw-   0        0        0     1289 2023-06-27 07:50:56.000000 pybeamline-1.0.3/pybeamline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      919 2023-06-27 07:50:56.000000 pybeamline-1.0.3/pybeamline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 07:50:56.000000 pybeamline-1.0.3/pybeamline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-27 07:50:56.000000 pybeamline-1.0.3/pybeamline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-27 07:50:56.000000 pybeamline-1.0.3/pybeamline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 07:50:56.517282 pybeamline-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-06-27 07:50:35.000000 pybeamline-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:50:56.515739 pybeamline-1.0.3/tests/
+-rw-rw-rw-   0        0        0      850 2023-06-20 12:16:17.000000 pybeamline-1.0.3/tests/test_bevent.py
```

### Comparing `pybeamline-0.0.3/LICENSE.txt` & `pybeamline-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline/algorithms/conformance/behavioral_conformance.py` & `pybeamline-1.0.3/pybeamline/algorithms/conformance/behavioral_conformance.py`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline/algorithms/discovery/heuristics_miner_lossy_counting.py` & `pybeamline-1.0.3/pybeamline/algorithms/discovery/heuristics_miner_lossy_counting.py`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline/algorithms/discovery/heuristics_miner_lossy_counting_budget.py` & `pybeamline-1.0.3/pybeamline/algorithms/discovery/heuristics_miner_lossy_counting_budget.py`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline/bevent.py` & `pybeamline-1.0.3/pybeamline/bevent.py`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline/filters/filters.py` & `pybeamline-1.0.3/pybeamline/filters/filters.py`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline/mappers/infinite_size_directly_follows_mapper.py` & `pybeamline-1.0.3/pybeamline/mappers/infinite_size_directly_follows_mapper.py`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline/mappers/sliding_window_to_log.py` & `pybeamline-1.0.3/pybeamline/mappers/sliding_window_to_log.py`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline/sources/__init__.py` & `pybeamline-1.0.3/pybeamline/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline/sources/string_test_source.py` & `pybeamline-1.0.3/pybeamline/sources/string_test_source.py`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline/sources/xes_log_source.py` & `pybeamline-1.0.3/pybeamline/sources/xes_log_source.py`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/pybeamline.egg-info/SOURCES.txt` & `pybeamline-1.0.3/pybeamline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybeamline-0.0.3/setup.py` & `pybeamline-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "pybeamline.filters",
         "pybeamline.sources",
         "pybeamline.mappers",
         "pybeamline.algorithms",
         "pybeamline.algorithms.conformance",
         "pybeamline.algorithms.discovery",
     ],
-    version="0.0.3",
+    version="1.0.3",
     description="Python version of Beamline (based on ReactiveX)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Andrea Burattin",
     license="Apache-2.0",
     install_requires=required_packages
 )
```

### Comparing `pybeamline-0.0.3/tests/test_bevent.py` & `pybeamline-1.0.3/tests/test_bevent.py`

 * *Files identical despite different names*

