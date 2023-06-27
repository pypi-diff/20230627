# Comparing `tmp/TEST_TC-0.1.7.tar.gz` & `tmp/TEST_TC-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-0.1.7.tar", last modified: Tue Jun 27 15:32:44 2023, max compression
+gzip compressed data, was "TEST_TC-0.1.8.tar", last modified: Tue Jun 27 15:44:24 2023, max compression
```

## Comparing `TEST_TC-0.1.7.tar` & `TEST_TC-0.1.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.153612 TEST_TC-0.1.7/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 15:32:44.152607 TEST_TC-0.1.7/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/README.md
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.085813 TEST_TC-0.1.7/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 15:32:44.000000 TEST_TC-0.1.7/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      997 2023-06-27 15:32:44.000000 TEST_TC-0.1.7/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 15:32:44.000000 TEST_TC-0.1.7/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 15:32:44.000000 TEST_TC-0.1.7/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 15:32:44.000000 TEST_TC-0.1.7/TEST_TC.egg-info/top_level.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1126 2023-06-27 14:56:18.000000 TEST_TC-0.1.7/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 15:32:44.153612 TEST_TC-0.1.7/setup.cfg
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.087490 TEST_TC-0.1.7/tc_uc4/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 15:32:32.000000 TEST_TC-0.1.7/tc_uc4/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.094323 TEST_TC-0.1.7/tc_uc4/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5803 2023-06-27 15:13:46.000000 TEST_TC-0.1.7/tc_uc4/algorithms/algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-06-27 15:13:53.000000 TEST_TC-0.1.7/tc_uc4/algorithms/prophet_utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.101132 TEST_TC-0.1.7/tc_uc4/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2810 2023-06-27 15:04:47.000000 TEST_TC-0.1.7/tc_uc4/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.104130 TEST_TC-0.1.7/tc_uc4/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7308 2023-06-27 15:01:58.000000 TEST_TC-0.1.7/tc_uc4/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.111374 TEST_TC-0.1.7/tc_uc4/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17975 2023-06-27 15:15:06.000000 TEST_TC-0.1.7/tc_uc4/datapreparation/datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3126 2023-06-27 15:15:12.000000 TEST_TC-0.1.7/tc_uc4/datapreparation/prep.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.115376 TEST_TC-0.1.7/tc_uc4/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.117421 TEST_TC-0.1.7/tc_uc4/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/datavisualization/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.128336 TEST_TC-0.1.7/tc_uc4/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      949 2023-06-27 14:58:09.000000 TEST_TC-0.1.7/tc_uc4/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.7/tc_uc4/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2119 2023-06-27 14:58:38.000000 TEST_TC-0.1.7/tc_uc4/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6298 2023-06-27 15:19:59.000000 TEST_TC-0.1.7/tc_uc4/utility/tele_logger.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.150608 TEST_TC-0.1.7/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2762 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15261 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1864 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2873 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_prep.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_prophet_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2070 2023-06-27 15:28:35.000000 TEST_TC-0.1.7/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2905 2023-06-27 15:12:14.000000 TEST_TC-0.1.7/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.296789 TEST_TC-0.1.8/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 15:44:24.295788 TEST_TC-0.1.8/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/README.md
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.227731 TEST_TC-0.1.8/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 15:44:24.000000 TEST_TC-0.1.8/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      997 2023-06-27 15:44:24.000000 TEST_TC-0.1.8/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 15:44:24.000000 TEST_TC-0.1.8/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 15:44:24.000000 TEST_TC-0.1.8/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 15:44:24.000000 TEST_TC-0.1.8/TEST_TC.egg-info/top_level.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1126 2023-06-27 14:56:18.000000 TEST_TC-0.1.8/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 15:44:24.296877 TEST_TC-0.1.8/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.229764 TEST_TC-0.1.8/tc_uc4/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 15:37:10.000000 TEST_TC-0.1.8/tc_uc4/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.236762 TEST_TC-0.1.8/tc_uc4/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5803 2023-06-27 15:13:46.000000 TEST_TC-0.1.8/tc_uc4/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-06-27 15:13:53.000000 TEST_TC-0.1.8/tc_uc4/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.241036 TEST_TC-0.1.8/tc_uc4/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2810 2023-06-27 15:04:47.000000 TEST_TC-0.1.8/tc_uc4/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.245181 TEST_TC-0.1.8/tc_uc4/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7308 2023-06-27 15:01:58.000000 TEST_TC-0.1.8/tc_uc4/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.253045 TEST_TC-0.1.8/tc_uc4/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17975 2023-06-27 15:15:06.000000 TEST_TC-0.1.8/tc_uc4/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3126 2023-06-27 15:15:12.000000 TEST_TC-0.1.8/tc_uc4/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.255555 TEST_TC-0.1.8/tc_uc4/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.256558 TEST_TC-0.1.8/tc_uc4/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/datavisualization/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.270014 TEST_TC-0.1.8/tc_uc4/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.8/tc_uc4/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      949 2023-06-27 14:58:09.000000 TEST_TC-0.1.8/tc_uc4/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.8/tc_uc4/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2119 2023-06-27 14:58:38.000000 TEST_TC-0.1.8/tc_uc4/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6328 2023-06-27 15:43:46.000000 TEST_TC-0.1.8/tc_uc4/utility/tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:44:24.292790 TEST_TC-0.1.8/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2762 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15261 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1864 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2873 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-06-27 14:54:10.000000 TEST_TC-0.1.8/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2169 2023-06-27 15:42:28.000000 TEST_TC-0.1.8/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2947 2023-06-27 15:44:13.000000 TEST_TC-0.1.8/tests/test_tele_logger.py
```

### Comparing `TEST_TC-0.1.7/README.md` & `TEST_TC-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-0.1.8/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/pyproject.toml` & `TEST_TC-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tc_uc4/algorithms/algorithm.py` & `TEST_TC-0.1.8/tc_uc4/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tc_uc4/algorithms/prophet_utils.py` & `TEST_TC-0.1.8/tc_uc4/algorithms/prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tc_uc4/analytics/evaluationMetrics.py` & `TEST_TC-0.1.8/tc_uc4/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tc_uc4/datahandler/datahandler.py` & `TEST_TC-0.1.8/tc_uc4/datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tc_uc4/datapreparation/datapreparation_utils.py` & `TEST_TC-0.1.8/tc_uc4/datapreparation/datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tc_uc4/datapreparation/prep.py` & `TEST_TC-0.1.8/tc_uc4/datapreparation/prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tc_uc4/utility/constants.py` & `TEST_TC-0.1.8/tc_uc4/utility/constants.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tc_uc4/utility/exceptions.py` & `TEST_TC-0.1.8/tc_uc4/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tc_uc4/utility/resources.py` & `TEST_TC-0.1.8/tc_uc4/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tc_uc4/utility/tele_logger.py` & `TEST_TC-0.1.8/tc_uc4/utility/tele_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         self.logger = logging.getLogger("logger")
         self.important_logger = logging.getLogger("important_logger")
 
         # Initial construct.
         self.format = format
         self.level = level
         self.name = None
+        self.log_path = None
 
     def initialize_logger(self,
                           log_path : str,
                           name: str):
         """Initialize the logging session by creating the logging files 
         <name>_<YYYYMMDD>.log and <name>_<YYYYMMDD>_verbose.log . If a new name 
         is passed then a new log session and files are created aswell
```

### Comparing `TEST_TC-0.1.7/tests/test_algorithm.py` & `TEST_TC-0.1.8/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tests/test_datahandler.py` & `TEST_TC-0.1.8/tests/test_datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tests/test_datapreparation_utils.py` & `TEST_TC-0.1.8/tests/test_datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tests/test_evaluations.py` & `TEST_TC-0.1.8/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tests/test_exceptions.py` & `TEST_TC-0.1.8/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tests/test_prep.py` & `TEST_TC-0.1.8/tests/test_prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tests/test_prophet_utils.py` & `TEST_TC-0.1.8/tests/test_prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.7/tests/test_resources.py` & `TEST_TC-0.1.8/tests/test_resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 from tc_uc4.utility.resources import get_configuration, log_exception
 
 ### get_configuration ###
 @pytest.fixture
 def mock_config_file(tmpdir):
     config_file = tmpdir.join("proprerties.toml")
     config_file.write("[section]\nkey = 'value'")
-    return str(config_file)
+    return 'proprerties.toml'
 
-def test_get_configuration_valid(mock_config_file):
-    result = get_configuration("section", config_file=mock_config_file)
+def test_get_configuration_valid(tmpdir, mock_config_file):
+    result = get_configuration("section", config_path=str(tmpdir), config_file=mock_config_file)
     assert isinstance(result, dict)
     assert result["key"] == "value"
 
-def test_get_configuration_invalid_file():
+def test_get_configuration_invalid_file(tmpdir):
     with pytest.raises(Exception):
-        get_configuration("section", config_file="non_existent.toml")
+        get_configuration("section", config_path=str(tmpdir), config_file="non_existent.toml")
 
-def test_get_configuration_invalid_section(mock_config_file):
+def test_get_configuration_invalid_section(tmpdir, mock_config_file):
     with pytest.raises(Exception):
-        get_configuration("non_existent_section", config_file=mock_config_file)
+        get_configuration("non_existent_section", config_path=str(tmpdir), config_file=mock_config_file)
 
 ### log_exception ###
 def test_log_exception_with_logger(caplog):
     logger = logging.getLogger("test_logger")
 
     @log_exception(logger)
     def my_function():
```

### Comparing `TEST_TC-0.1.7/tests/test_tele_logger.py` & `TEST_TC-0.1.8/tests/test_tele_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from tc_uc4.utility.tele_logger import Logger
 
 def test_logger_initialization():
     logger = Logger()
     assert isinstance(logger.logger, logging.Logger)
     assert isinstance(logger.important_logger, logging.Logger)
     assert logger.name is None
+    assert logger.log_path is None
 
 def test_logger_initialize_logger(tmpdir):
     logger = Logger()
-    logger.initialize_logger("test_session")
+    logger.initialize_logger(,name="test_session")
 
     # Check if log files are created
     log_folder = os.path.join(os.path.split(os.path.dirname(os.path.abspath(__file__)))[0], "logs")
     assert os.path.exists(log_folder)
 
     log_files = os.listdir(log_folder)
     assert f"test_session_{strftime('%Y%m%d', localtime())}.log" in log_files
```

