# Comparing `tmp/rosetta-ce-1.2.2.tar.gz` & `tmp/rosetta-ce-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.2.2.tar", last modified: Tue Jun 27 13:32:25 2023, max compression
+gzip compressed data, was "rosetta-ce-1.2.3.tar", last modified: Tue Jun 27 14:57:34 2023, max compression
```

## Comparing `rosetta-ce-1.2.2.tar` & `rosetta-ce-1.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-27 13:32:25.595437 rosetta-ce-1.2.2/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.2.2/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11282 2023-06-27 13:32:25.595156 rosetta-ce-1.2.2/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10750 2023-04-26 16:15:22.000000 rosetta-ce-1.2.2/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-27 13:32:25.589413 rosetta-ce-1.2.2/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.2.2/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-27 13:32:25.591172 rosetta-ce-1.2.2/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.2.2/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.2.2/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.2.2/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.2.2/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.2.2/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    32076 2023-06-27 13:30:48.000000 rosetta-ce-1.2.2/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8012 2023-04-26 13:49:21.000000 rosetta-ce-1.2.2/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-27 13:32:25.592952 rosetta-ce-1.2.2/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11282 2023-06-27 13:32:25.000000 rosetta-ce-1.2.2/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-27 13:32:25.000000 rosetta-ce-1.2.2/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-27 13:32:25.000000 rosetta-ce-1.2.2/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-27 13:32:25.000000 rosetta-ce-1.2.2/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-27 13:32:25.000000 rosetta-ce-1.2.2/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-27 13:32:25.595498 rosetta-ce-1.2.2/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-27 13:31:08.000000 rosetta-ce-1.2.2/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-27 13:32:25.594592 rosetta-ce-1.2.2/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.2.2/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.2.2/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.2.2/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-27 14:57:34.947356 rosetta-ce-1.2.3/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.2.3/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11282 2023-06-27 14:57:34.947041 rosetta-ce-1.2.3/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10750 2023-04-26 16:15:22.000000 rosetta-ce-1.2.3/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-27 14:57:34.939009 rosetta-ce-1.2.3/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.2.3/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-27 14:57:34.943557 rosetta-ce-1.2.3/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.2.3/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.2.3/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.2.3/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.2.3/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.2.3/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    32103 2023-06-27 14:56:34.000000 rosetta-ce-1.2.3/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8012 2023-04-26 13:49:21.000000 rosetta-ce-1.2.3/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-27 14:57:34.945404 rosetta-ce-1.2.3/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11282 2023-06-27 14:57:34.000000 rosetta-ce-1.2.3/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-27 14:57:34.000000 rosetta-ce-1.2.3/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-27 14:57:34.000000 rosetta-ce-1.2.3/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-27 14:57:34.000000 rosetta-ce-1.2.3/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-27 14:57:34.000000 rosetta-ce-1.2.3/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-27 14:57:34.947441 rosetta-ce-1.2.3/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-27 14:56:48.000000 rosetta-ce-1.2.3/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-27 14:57:34.946542 rosetta-ce-1.2.3/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.2.3/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.2.3/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.2.3/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.2.2/LICENSE` & `rosetta-ce-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.2/PKG-INFO` & `rosetta-ce-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.2.2
+Version: 1.2.3
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.2.2/README.md` & `rosetta-ce-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.2/rosetta/constants/sensors.py` & `rosetta-ce-1.2.3/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.2/rosetta/constants/sources.py` & `rosetta-ce-1.2.3/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.2/rosetta/constants/systems.py` & `rosetta-ce-1.2.3/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.2/rosetta/rconverter.py` & `rosetta-ce-1.2.3/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.2/rosetta/rfaker.py` & `rosetta-ce-1.2.3/rosetta/rfaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,15 +507,15 @@
         faker = cls._create_faker()
         json_messages = []
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
         for i in range(count):
             timestamp += timedelta(seconds=1)
-            system_time = timestamp
+            system_time = timestamp.strftime('%b %d %H:%M:%S')
             cve_id = random.choice(observables.cve) if observables and observables.cve \
                 else Observables.generator(observable_type=ObservableType.CVE, count=1)
             host = random.choice(observables.src_host) if observables and observables.src_host \
                 else faker.hostname()
             severity = random.choice(observables.severity) if observables and observables.severity \
                 else faker.random_int(min=1, max=5)
             file_hash = random.choice(observables.file_hash) if observables and observables.file_hash \
```

### Comparing `rosetta-ce-1.2.2/rosetta/rsender.py` & `rosetta-ce-1.2.3/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.2/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.2.3/rosetta_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.2.2
+Version: 1.2.3
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.2.2/setup.py` & `rosetta-ce-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.2.2",
+    version="1.2.3",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.2.2/tests/test_rconverter.py` & `rosetta-ce-1.2.3/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.2/tests/test_rfaker.py` & `rosetta-ce-1.2.3/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.2/tests/test_rsender.py` & `rosetta-ce-1.2.3/tests/test_rsender.py`

 * *Files identical despite different names*

