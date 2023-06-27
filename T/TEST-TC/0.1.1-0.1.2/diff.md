# Comparing `tmp/TEST_TC-0.1.1.tar.gz` & `tmp/TEST_TC-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-0.1.1.tar", last modified: Sat Jun 24 15:48:31 2023, max compression
+gzip compressed data, was "TEST_TC-0.1.2.tar", last modified: Tue Jun 27 09:56:12 2023, max compression
```

## Comparing `TEST_TC-0.1.1.tar` & `TEST_TC-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,48 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.445142 TEST_TC-0.1.1/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      197 2023-06-24 15:48:31.445142 TEST_TC-0.1.1/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.1/README.md
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.408406 TEST_TC-0.1.1/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      197 2023-06-24 15:48:31.000000 TEST_TC-0.1.1/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      797 2023-06-24 15:48:31.000000 TEST_TC-0.1.1/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-24 15:48:31.000000 TEST_TC-0.1.1/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      169 2023-06-24 15:48:31.000000 TEST_TC-0.1.1/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-24 15:48:31.000000 TEST_TC-0.1.1/TEST_TC.egg-info/top_level.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      844 2023-06-24 15:37:51.000000 TEST_TC-0.1.1/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-24 15:48:31.445142 TEST_TC-0.1.1/setup.cfg
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       78 2023-06-24 15:22:08.000000 TEST_TC-0.1.1/setup.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.408406 TEST_TC-0.1.1/tc_uc4/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       22 2023-06-24 15:48:16.000000 TEST_TC-0.1.1/tc_uc4/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.408406 TEST_TC-0.1.1/tc_uc4/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.1/tc_uc4/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     8060 2023-06-22 17:55:31.000000 TEST_TC-0.1.1/tc_uc4/algorithms/algorithm.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.418959 TEST_TC-0.1.1/tc_uc4/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.1/tc_uc4/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2626 2023-06-24 11:28:22.000000 TEST_TC-0.1.1/tc_uc4/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.418959 TEST_TC-0.1.1/tc_uc4/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.1/tc_uc4/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7536 2023-06-24 10:26:50.000000 TEST_TC-0.1.1/tc_uc4/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.429487 TEST_TC-0.1.1/tc_uc4/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.1/tc_uc4/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    18679 2023-06-22 17:55:31.000000 TEST_TC-0.1.1/tc_uc4/datapreparation/preprocessing.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.429487 TEST_TC-0.1.1/tc_uc4/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.1/tc_uc4/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.429487 TEST_TC-0.1.1/tc_uc4/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.1/tc_uc4/datavisualization/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.429487 TEST_TC-0.1.1/tc_uc4/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.1/tc_uc4/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.1/tc_uc4/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2235 2023-06-23 19:40:15.000000 TEST_TC-0.1.1/tc_uc4/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6174 2023-06-13 16:27:38.000000 TEST_TC-0.1.1/tc_uc4/utility/tele_logger.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-24 15:48:31.445142 TEST_TC-0.1.1/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      200 2023-06-23 19:40:15.000000 TEST_TC-0.1.1/tests/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2748 2023-06-24 11:28:22.000000 TEST_TC-0.1.1/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1641 2023-06-24 11:28:22.000000 TEST_TC-0.1.1/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1237 2023-06-24 11:28:22.000000 TEST_TC-0.1.1/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2096 2023-06-23 19:40:15.000000 TEST_TC-0.1.1/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2898 2023-06-23 19:40:15.000000 TEST_TC-0.1.1/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.703727 TEST_TC-0.1.2/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 09:56:12.702725 TEST_TC-0.1.2/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/README.md
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.635802 TEST_TC-0.1.2/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 09:56:12.000000 TEST_TC-0.1.2/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      978 2023-06-27 09:56:12.000000 TEST_TC-0.1.2/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 09:56:12.000000 TEST_TC-0.1.2/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 09:56:12.000000 TEST_TC-0.1.2/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 09:56:12.000000 TEST_TC-0.1.2/TEST_TC.egg-info/top_level.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1125 2023-06-27 09:48:36.000000 TEST_TC-0.1.2/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 09:56:12.704725 TEST_TC-0.1.2/setup.cfg
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       84 2023-06-24 15:58:09.000000 TEST_TC-0.1.2/setup.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.638873 TEST_TC-0.1.2/tc_uc4/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 09:56:03.000000 TEST_TC-0.1.2/tc_uc4/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.644615 TEST_TC-0.1.2/tc_uc4/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5799 2023-06-26 14:08:09.000000 TEST_TC-0.1.2/tc_uc4/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15585 2023-06-27 09:06:09.000000 TEST_TC-0.1.2/tc_uc4/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.649121 TEST_TC-0.1.2/tc_uc4/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2826 2023-06-26 09:19:22.000000 TEST_TC-0.1.2/tc_uc4/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.653554 TEST_TC-0.1.2/tc_uc4/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7529 2023-06-26 12:58:12.000000 TEST_TC-0.1.2/tc_uc4/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.660557 TEST_TC-0.1.2/tc_uc4/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17971 2023-06-26 17:37:41.000000 TEST_TC-0.1.2/tc_uc4/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3120 2023-06-26 17:37:02.000000 TEST_TC-0.1.2/tc_uc4/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.663088 TEST_TC-0.1.2/tc_uc4/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.665010 TEST_TC-0.1.2/tc_uc4/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/datavisualization/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.675214 TEST_TC-0.1.2/tc_uc4/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.2/tc_uc4/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2222 2023-06-26 14:08:09.000000 TEST_TC-0.1.2/tc_uc4/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6174 2023-06-13 16:27:38.000000 TEST_TC-0.1.2/tc_uc4/utility/tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.699725 TEST_TC-0.1.2/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      200 2023-06-26 17:37:24.000000 TEST_TC-0.1.2/tests/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2469 2023-06-26 13:54:38.000000 TEST_TC-0.1.2/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2748 2023-06-26 18:05:01.000000 TEST_TC-0.1.2/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15247 2023-06-27 09:06:09.000000 TEST_TC-0.1.2/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1850 2023-06-26 09:19:22.000000 TEST_TC-0.1.2/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1237 2023-06-24 11:28:22.000000 TEST_TC-0.1.2/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2866 2023-06-26 17:45:00.000000 TEST_TC-0.1.2/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16902 2023-06-27 09:06:09.000000 TEST_TC-0.1.2/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2096 2023-06-23 19:40:15.000000 TEST_TC-0.1.2/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2898 2023-06-23 19:40:15.000000 TEST_TC-0.1.2/tests/test_tele_logger.py
```

### Comparing `TEST_TC-0.1.1/README.md` & `TEST_TC-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.1/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-0.1.2/TEST_TC.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,25 +5,31 @@
 TEST_TC.egg-info/SOURCES.txt
 TEST_TC.egg-info/dependency_links.txt
 TEST_TC.egg-info/requires.txt
 TEST_TC.egg-info/top_level.txt
 tc_uc4/__init__.py
 tc_uc4/algorithms/__init__.py
 tc_uc4/algorithms/algorithm.py
+tc_uc4/algorithms/prophet_utils.py
 tc_uc4/analytics/__init__.py
 tc_uc4/analytics/evaluationMetrics.py
 tc_uc4/datahandler/__init__.py
 tc_uc4/datahandler/datahandler.py
 tc_uc4/datapreparation/__init__.py
-tc_uc4/datapreparation/preprocessing.py
+tc_uc4/datapreparation/datapreparation_utils.py
+tc_uc4/datapreparation/prep.py
 tc_uc4/dataset/__init__.py
 tc_uc4/datavisualization/__init__.py
 tc_uc4/utility/__init__.py
 tc_uc4/utility/exceptions.py
 tc_uc4/utility/resources.py
 tc_uc4/utility/tele_logger.py
 tests/__init__.py
+tests/test_algorithm.py
 tests/test_datahandler.py
+tests/test_datapreparation_utils.py
 tests/test_evaluations.py
 tests/test_exceptions.py
+tests/test_prep.py
+tests/test_prophet_utils.py
 tests/test_resources.py
 tests/test_tele_logger.py
```

### Comparing `TEST_TC-0.1.1/pyproject.toml` & `TEST_TC-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system] 
-requires = ["setuptools>=42", "wheel"] #cython is optional
+requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta" 
 
 [project] 
 name = "TEST_TC"
 authors = [{name = "Flavio", email= "f.ischiboni@skienda.it"}]
-description = "<small description>"
+description = "Lo scopo di questa libreria è fornire uno strumento completo per il rilascio di modelli predittivi basati su serie temporali nell'ambito della Telemedicina, al fine di supportare la gestione e la pianificazione delle attività sulla Piattaforma Nazionale di Telemedicina (PNT)"
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3"]
-dependencies = ["geopandas==0.13.0","holidays==0.24","numpy==1.25.0","pandas==2.0.2",
-                "prophet==1.1.1","scikit_learn==1.2.2","setuptools==58.1.0","tabulate==0.9.0",
-                "tomli==2.0.1","typing_extensions==4.6.3"]
+dependencies = ["geopandas==0.13.0","holidays==0.24","numpy==1.25.0","pandas==2.0.2","prophet==1.1.1",
+                "scikit_learn==1.2.2","tabulate==0.9.0","tomli==2.0.1","typing_extensions==4.6.3", "pytest==7.3.1",
+                "setuptools==58.1.0", "statsmodels==0.14.0"]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
 where = ["./"]
-include = ["*"]#or define list of packages
+include = ["*"]# or define list of packages
 exclude = []
 namespaces = false
 
 [tool.setuptools.dynamic]
-version = {attr = "tc_uc4.__version__"}#read __version__ from packages __init__.py 
+version = {attr = "tc_uc4.__version__"} # read __version__ from packages __init__.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TEST_TC-0.1.1/tc_uc4/analytics/evaluationMetrics.py` & `TEST_TC-0.1.2/tc_uc4/analytics/evaluationMetrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
     logger.info('START Ealuating results')
 
     df_real= df_real.set_index(date).dropna()
     df_pred= df_pred.set_index(date).dropna()
     inter = df_real.index.intersection(df_pred.index)
 
+    if len(inter) == 0:
+        raise Exception('Length of intersection between Predictions and Ground Truth Datasets is Null. Probably one of the two Datasets has not available data (all NaN).')
+
     df_real = df_real.loc[inter]
     df_pred = df_pred.loc[inter]
 
     # Mean Absolute Error
     logger.info('Evaluating MAE')
     mae = round(mean_absolute_error(df_real[y_true], df_pred[y_pred]),2)
     # Root Mean Square Error
```

### Comparing `TEST_TC-0.1.1/tc_uc4/datahandler/datahandler.py` & `TEST_TC-0.1.2/tc_uc4/datahandler/datahandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,18 +163,17 @@
         datatype = os.path.splitext(filename)[-1].lower()
         supp_datatype = [".parquet", ".csv"]
 
         if datatype not in supp_datatype:
             raise Exception(
                 f'File extension "{datatype}" not supported. Supported extensions are {supp_datatype}'
             )
-
         if not os.path.isdir(os.path.join(self.data_folder, folder)):
             raise Exception(
-                f'Can not write "{filename}" because folder "{folder}" does not exist in {self.data_folder}. Please create it.'
+                f'Can not write "{filename}" because folder "{os.path.join(self.data_folder, folder)}". Please create it.'
             )
 
         path = os.path.join(self.data_folder, folder, filename)
 
         logger.info(msg=f"START writing {os.path.join(self.data_folder, folder, filename)}", important=True)
 
         if datatype == ".csv":
```

### Comparing `TEST_TC-0.1.1/tc_uc4/datapreparation/preprocessing.py` & `TEST_TC-0.1.2/tc_uc4/datapreparation/datapreparation_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,67 @@
-import numpy as np
 import pandas as pd
-from datetime import datetime
-import holidays
 from utility.tele_logger import logger
-from datahandler.datahandler import DataHandler
-from utility.resources import *
-import os
-# import shutil
-import sys
-
-
-dict_regioni = {
-
-                        30: 'Lombardia',190: 'Sicilia',50: 'Veneto',80: 'Emilia-Romagna',120: 'Lazio',200: 'Sardegna',
-
-                        150: 'Campania',10: 'Piemonte',42: 'Trento',70: 'Liguria',130: 'Abruzzo',100: 'Umbria',
-
-                        180: 'Calabria',160: 'Puglia',110: 'Marche',90: 'Toscana',20: "Valle D'Aosta",170: 'Basilicata',
-
-                         60: 'Friuli-Venezia-Giulia',41: 'Bolzano',140: 'Molise'
-
-                         }
-
-dict_spec = {
-                "Cardiologia": 2,"Chirurgia Vascolare": 5, "Endocrinologia": 9,
-                "Neurologia": 15, "Oculistica": 16, "Ortopedia": 19,
-                "Ginecologia": 20, "Otorinolaringoiatra": 21, "Urologia": 25,
-                "Dermatologia": 27, "Fisiatria": 12,"Gastroenterologia": 10,"Oncologia": 18,"Pneumologia": 22
-            }
-
-dict_spec_reversed = {v:k for k,v in dict_spec.items()}
+from utility.exceptions import InputTypeError
+from statsmodels.tsa.seasonal import seasonal_decompose
+from sklearn.base import BaseEstimator, TransformerMixin
+from typing_extensions import Self
+from typing import Union, Dict, List
 
+class PreprocessingTeleconsulto:
 
+    def prophet(self,
+                df: pd.DataFrame) -> pd.DataFrame:
+        
+        """
+        Sequential execution of transformations to obtain a DataFrame with a time series structure
 
-def get_path_and_make_root(folder_name = str) -> str:
+        Returns:
+            pd.DataFrame: DataFrame identifying the timeseries generated according to specified hierarchies and time span
+        """
+        # Raw dataset from which to generate the time serie
+        self.df = df.copy()
+        # column name identifying the columns to index on
+        self.datetime_index = "data_richiesta"
+        # column name identifying column from which to generate target
+        self.target = "id_teleconsulto"
+
+         # Verify that df is of type pd.DataFrame
+        if not isinstance(df, pd.DataFrame):
+            logger.info("Input 'df' must be of type pd.DataFrame", important=True)
+            raise InputTypeError('datapreparation_utils.prophet')
+        # Verify that datetime_index is a non-empty string and a column in df
+        if  self.datetime_index not in df.columns:
+            logger.info("Invalid value for 'datetime_index'. It must be a column in 'df'", important=True)
+            raise InputTypeError('datapreparation_utils.prophet')
+        # Verify that target is a non-empty string and a column in df
+        if self.target not in df.columns:
+            logger.info("Invalid value for 'target'. It must be a column in 'df'", important=True)
+            raise InputTypeError('datapreparation_utils.prophet')
+
+        logger.info('Starting preparing data', important = True)
+        
+        logger.info('Extracting date from datetime column')
+        self.df["Timestamp"] = from_timestamp_to_date(self.df[self.datetime_index])
 
-    """ Creates the folder where data used to feed the model will be saved
+        logger.info('Generating the timeseries target')
+        self.df_target = generating_target(self.df, ["Timestamp"],self.target)
 
-    Parameters
-    folder_name: str
-        Name of the folder to create
+        logger.info('Creating the entire timeline to complete the target')
+        self.df_calendar = pd.DataFrame(resample_date(self.df_target, "Timestamp",target=self.target))['Timestamp']
+            
+        df_ts = pd.merge(self.df_calendar, self.df_target, how='left', on="Timestamp")
+        logger.info('Generating the complete timeseries', important = True)
+        df_ts.rename(columns={self.target:'Target'}, inplace=True)
 
-    Returns
-    -------
-    str:
-       path of the folder where data will be saved 
-        
-    
-    """
-    
-    path = os.path.dirname(os.path.abspath(__file__))
-    path = os.path.split(os.path.split(path)[0])[0] + "/data/output/"
+        return df_ts
     
-    os.makedirs(path + folder_name, exist_ok=True)
-    return path + folder_name
 
 
-def code_to_name(cod: pd.Series, convers_dict: dict) -> pd.Series:
+def code_to_name(cod: pd.Series, convers_dict: Dict) -> pd.Series:
+    
     """
     The function generates a new column converting the code number into a meaningful string
 
     Parameters
     ----------
     cod: pd.Series
        The code number column
@@ -68,447 +69,475 @@
         The mapping dictionary from code to string
 
     Returns
     -------
         pd.Series
         Returns the modified column based on the mapping dictionary
     """
+    if not isinstance(cod, pd.Series):
+        logger.info("Input 'cod' must be of type pd.Series")
+        raise InputTypeError('datapreparation_utils.cod_to_name')
+    if not isinstance(convers_dict, dict):
+        logger.info("Input 'convers_dict' must be of type dict")
+        raise InputTypeError('datapreparation_utils.cod_to_name')
+                  
     return cod.apply(lambda i: convers_dict[int(i)])
 
+
+def from_timestamp_to_date(df: pd.Series) -> pd.Series:
+        """  
+        Extract the date from datetime
+
+        Parameters
+        ----------
+        df: pandas.Series 
+            Pandas.series object identifying datetime to convert
+
+        Returns
+        -------
+        to_date: pandas.Series 
+            pandas.Series datetime64[ns] object identifying date
+
+        """  
+        #Verify that df is of type pd.Series
+        if not isinstance(df, pd.Series):
+            logger.info("Input df must be a pandas.Series")
+            raise(InputTypeError('datapreparation_utils.from_timestamp_to_date'))
+        #verify that df is a pandas.Series of type datetime
+        if not pd.api.types.is_datetime64_any_dtype(df.dtype):
+            logger.info("Input df must be of type datetime")
+            raise TypeError("Input df must be of type datetime")
+       
+        to_date = pd.to_datetime(df.dt.date)
+        return to_date
+
 def generating_target(df: pd.DataFrame,
-                      col_index: list,
+                      col_index: List,
                       target_col: str) -> pd.DataFrame:
         
         """ Creates the timeseries target
 
         Parameters
         ----------
         df: pd.DataFrame
             DataFrame with the fixed ennuple and date column used to generate timeseries 
 
         col_index: list
-            column names identifying the columns to  aggregate on
+            column names identifying the columns to aggregate on
 
         target_col: str
             column name identifying the target (e.g.: id_teleconsulto)
 
         Returns
         -------
         grouped_df: pd.DatFrame 
             Dataframe with the aggregation
 
         """
         
-        grouped_df = df.groupby(col_index).agg(target = (target_col,"count")).reset_index()
+         # Verify that df is of type pd.DataFrame
+        if not isinstance(df, pd.DataFrame):
+            logger.info("Input 'df' must be of type pd.DataFrame")
+            raise(InputTypeError('datapreparation_utils.generating_target'))
+
+        # Verify that col_index is a non-empty list
+        if not isinstance(col_index, list) or len(col_index) == 0:
+            logger.info("Input 'col_index' must be a non-empty list")
+            raise(InputTypeError('datapreparation_utils.generating_target'))
+
+         # Verify that elements in col_index are non-empty strings 
+        if not all(isinstance(col, str) and len(col) > 0 for col in col_index):
+            logger.info("Elements in 'col_index' must be non-empty strings")
+
+        # Verify that target_col is a non-empty string
+        if not isinstance(target_col, str) or len(target_col) == 0:
+            logger.info("Input 'target_col' must be a non-empty string")
+            raise(InputTypeError('datapreparation_utils.generating_target'))
+        
+        # Verify that columns in col_index exist in df
+        missing_columns = [col for col in col_index if col not in df.columns]
+        if missing_columns:
+            logger.info(f"The following columns are missing in 'df': {', '.join(missing_columns)}")
+            raise(InputTypeError('datapreparation_utils.generating_target'))
+
+        # Verify that che target_col is a df column
+        if target_col not in df.columns:
+            logger.info(f"Column '{target_col}' is missing in 'df'")
+            raise(InputTypeError('datapreparation_utils.generating_target'))
+
+        grouped_df = df.groupby(col_index).agg({target_col:"count"}).reset_index()
 
         return grouped_df
 
-def from_timestamp_to_date(df: pd.Series) -> pd.Series:
-        """  
-        Extract the date from datetime
+def resample_date(df: pd.DataFrame,
+                  datetime_col : str = "Timestamp",
+                  grouping_cols : List = [None],
+                  target : str = "Target",
+                  s: str = "D") -> pd.DataFrame:
+
+        """Creates the entire daily time series in a fixed datetime range 
 
         Parameters
         ----------
-        df: pandas.Series 
-            Pandas.series object identifying datetime to convert
+        df: pd.DataFrame
+           pandas DataFrame from which resample time-series data
+        datetime_col: str
+           column on which to insert missing dates
+        grouping_cols: list
+           list of columns specifying a hierarchy. If None, no hierarchy should be considered
+        target: str
+           column identifying target column 
+        s: str
+            Date Offset to consider, tipically "D" (daily), "W" (weekly), "M" (monthly)
 
         Returns
         -------
-        to_date: pandas.Series 
-            pandas.Series datetime64[ns] object identifying date
+        s: pd.DataFrame 
+           Resampled time-series data
 
-        """  
+        """
+        
+        # Verify that "df" is a pd.DataFrame
+        if not isinstance(df, pd.DataFrame):
+            logger.info("Input 'df' must be of type pd.DataFrame")
+            raise(InputTypeError('datapreparation_utils.resample_date'))
+        
+        # Verify that datetime_col is a non-empty string
+        if not isinstance(datetime_col, str) or len(datetime_col) == 0:
+            logger.info("Input 'datetime_col' must be a non-empty string")
+            raise(InputTypeError('datapreparation_utils.resample_date'))
+        
+        # Verify that grouping_cols is either a list or None
+        if grouping_cols !=[None] and not isinstance(grouping_cols, list):
+            logger.info("Input 'grouping_cols' must be a list or None")
+            raise(InputTypeError('datapreparation_utils.resample_date'))
+        
+        # Verify that columns in grouping_cols exist in df
+        if grouping_cols !=[None]:
+            print(grouping_cols)
+            if not all(col in df.columns for col in grouping_cols):
+                logger.info("Columns in 'grouping_cols' must exist in the DataFrame")
+                raise(InputTypeError('datapreparation_utils.resample_date'))
+        
+        # Verify that target is a non-empty string
+        if not isinstance(target, str) or len(target) == 0:
+            logger.info("Input 'target' must be a non-empty string")
+            raise(InputTypeError('datapreparation_utils.resample_date'))
+
+        # Verify that s is a non-empty string
+        if not isinstance(s, str) or len(s) == 0:
+            logger.info("Input 's' must be a non-empty string")
+            raise(InputTypeError('datapreparation_utils.resample_date'))
+        
+        # Verify that datetime_col is a dataframe column of type pd.Datetime 
+        if datetime_col not in df.columns or not pd.api.types.is_datetime64_any_dtype(df[datetime_col].dtype):
+            logger.info("Input 'datetime_col' must be a column of type pd.Datetime")
 
-        # to_date = df.dt.date
-        to_date = pd.to_datetime(df.dt.date)
 
-        return to_date
-    
-    
-def resample_date(df: pd.DataFrame,
-                  s: str) -> pd.DataFrame:
+        if grouping_cols==[None]:
+            output = df.set_index(datetime_col).resample(s.title()).sum().reset_index()
+        else:
+            output = df.set_index(datetime_col).groupby(grouping_cols)[target].apply(lambda x: x.asfreq(s.title()))
 
-        """Creates the entire daily time series in a fixed datetime range 
+        return output
+
+
+class Normalizer(TransformerMixin, BaseEstimator):
+
+    """Normalization class for time series (between 0 and 1)
+    """
+
+    def __init__(self):
+        pass
+
+    def fit(self, X: pd.DataFrame) -> Self:
+
+        """Compute value min and max useful to normalize data
 
         Parameters
         ----------
-        df: pd.DataFrame
-           pandas DataFrame from which resample time-series data
+        X : pd.DataFrame
+            dataframe containing two columns (timestamp and volumes of time series)         
 
         Returns
         -------
-        s: pd.DataFrame 
-           Resampled time-series data
+        self : object
+            fitted normalizer
+        """
+
+        self.min = X.iloc[:,1].min()
+        self.max = X.iloc[:,1].max()
+
+        return self
 
+    def transform(self, X: pd.DataFrame) -> pd.DataFrame:
+
+        """Perform normalization between 0 and 1
+
+        Parameters
+        ----------
+        X : pd.DataFrame
+            dataframe containing two columns (timestamp and volumes of time series)
+
+        Returns
+        -------
+        X : pd.DataFrame
+            transformed time series
         """
-        
-        return df.set_index('timeline').resample(s).sum().reset_index()
 
-class NotEnoughDataPoints(Exception):
-    """Thrown when the data points inside the dataframe are less than or equal to 1"""
-    pass
-
-class Preprocessing_Prophet:
-
-    @log_exception(logger)
-    def __init__(self,
-                #  df: pd.DataFrame,
-                 raw_filename: str = None,
-                 regione: str = None,
-                 asl: str = None,
-                 branca: str = None,
-                 to_delete = False
-                 ):
+        normalized = (X.iloc[:,1] - self.min) / (self.max - self.min)
+        ris = pd.concat([X.iloc[:,0],normalized],axis=1)
+        ris.columns = X.columns
+        
+        return ris
     
-        """
-        Preprocessing class
+class ReplacerNA(TransformerMixin, BaseEstimator):
+
+    def __init__(self, method: Union[str,int] = 0) -> Self:
+
+        """class for handling of NA
 
         Parameters
         ----------
-        df: pd.DataFrame
-        The original dataframe
-            
-        regione: str
-        name of the first level of hierarchy. It could be None, meaning Italy, or one from Italian regions name
+        method : str | int
+            if str specify the method to replace NA value (mean,median,zero), if int specify the value to replace NA value
+
+        Returns
+        -------
+        self : object
+        """
         
-        asl: str
-        name of the second level of hierarchy, valued only if "regione" is not None, indicating an "asl"
-        of the specified region
+        self.method = method
 
-        branca: str
-        name of the third level of hierarchy, valued only if both "regione" and "asl"  aren't None, indicating
-        a medical branch of the specified region-asl pair
+    def fit(self, X: pd.DataFrame) -> Self:
 
-        to_delete: bool
-        Flag to set files overwriting
+        """Compute value useful for replacing NA
 
+        Parameters
+        ----------
+        X : pd.DataFrame
+            dataframe containing two columns (timestamp and volumes of time series)         
+
+        Returns
+        -------
+        self : object
+            fitted replacer
         """
+        
+        if self.method == "mean":
+            self.value = X.iloc[:,1].mean()
+            self.method_for_df = None
+        elif self.method == "median":
+            self.value = X.iloc[:,1].median()
+            self.method_for_df = None
+        elif self.method == "zero":
+            self.value = 0
+            self.method_for_df = None
+        elif self.method == "bfill":
+            self.value = None
+            self.method_for_df = "bfill"
+        elif self.method == "ffill":
+            self.value = None
+            self.method_for_df = "ffill"
+        else:
+            self.value = self.method
+            self.method_for_df = None
 
-        global dict_regioni
-        global dict_spec_reversed
+        return self
 
-        if raw_filename == None:
-            for f in os.listdir(os.path.join(DataHandler().data_folder, 'input')):
-                if f.endswith('.parquet'):
-                    raw_filename = f
-                    break
+    def transform(self, X: pd.DataFrame) -> pd.DataFrame:
 
-        path = get_path_and_make_root(folder_name =  "prophet/")
-        
-        self.path = path
-        self.regione = [regione.title() if regione !=None else regione][0]
-        self.asl = [asl.upper() if asl!= None else asl][0]
-        self.branca = [branca.title() if branca !=None else branca][0]
-        self.to_delete = to_delete
+        """Perform replacement of missing values
 
-        self.params = {}
-        self.params = GetConfiguration("input_parameters_prophet")
-        # self.df = df
-        self.df = DataHandler().read(filename=raw_filename, folder='input')
-        self.df["regione"] = code_to_name(self.df[self.params["spatial_hierarchy"]],dict_regioni)
-        self.df["specializzazioni"] = code_to_name(self.df[self.params["specialty_index"]],dict_spec_reversed)
+        Parameters
+        ----------
+        X : pd.DataFrame
+            dataframe containing two columns (timestamp and volumes of time series)
 
+        Returns
+        -------
+        X : pd.DataFrame
+            transformed time series
+        """
+         
+        return X.fillna(self.value, method=self.method_for_df)
+    
+class Detrender(TransformerMixin, BaseEstimator):
 
-        return 
+    def __init__(self, period: int) -> Self:
 
-    def generating_files_according_to_hierarchy(self) -> list:
+        """Detrending time series
 
-        """Create folders and data files according to the specified input hierarchy 
+        Parameters
+        ----------
+        period : int
+            specify period considered for compute additive decomposition
 
-        Returns:
-        list: 
-            list of created-folders paths
+        Returns
+        -------
+        self : object
         """
 
-        if all( x is None for x in [self.regione, self.asl, self.branca]):
-            os.makedirs(self.path, exist_ok=True)
-            path_to_save = self.path
-            path_list = []
-            path_list += self.making_subfolders_writing_files(
-                                                    self.df,
-                                                    path_to_save,
-                                                    to_delete = self.to_delete
-                                                    )
-
-            path_list += self.making_subfolders_writing_files(
-                                                    self.df,
-                                                    path_to_save,
-                                                    "regione",
-                                                    to_delete=self.to_delete)
-
-        elif self.regione != None and self.asl == None:
-            os.makedirs(self.path + self.regione + "/", exist_ok=True)
-            path_list=[]
-            path_to_save = self.path + self.regione + "/"
-            df_ = self.df[self.df["regione"]==self.regione].reset_index(drop=True)
-
-            path_list += self.making_subfolders_writing_files(
-                                        df_,
-                                        path_to_save,
-                                        filename=self.regione + ".parquet",
-                                        to_delete = self.to_delete)
-            
-            path_list += self.making_subfolders_writing_files(
-                                                    df_,
-                                                    path_to_save,
-                                                    self.params["spatial_sub_hierarchy"],
-                                                    to_delete = self.to_delete)
-            
-        elif self.regione != None and self.asl != None:
-            os.makedirs(self.path + self.regione +"/"+ self.asl + "/", exist_ok=True)
-            path_list=[]
-            path_to_save = self.path + self.regione + "/" + self.asl + "/"
-            df_ = self.df[(self.df["regione"]==self.regione) & \
-                        (self.df[self.params["spatial_sub_hierarchy"]]==self.asl)].reset_index(drop=True)
-            if df_.shape[0] <=1:
-                logger.error("No enough data: check your input")
-                raise NotEnoughDataPoints
-
-            path_list += self.making_subfolders_writing_files(
-                                        df_,
-                                        path_to_save,
-                                        filename=self.asl + ".parquet",
-                                        to_delete = self.to_delete)
-            
-            path_list += self.making_subfolders_writing_files(
-                                                    df_,
-                                                    path_to_save,
-                                                    "specializzazioni",
-                                                     to_delete = self.to_delete)
-        return path_list
-
-    def making_subfolders_writing_files(self,
-                                    df_: pd.DataFrame,
-                                    path: str,
-                                    hier_col: str = None,
-                                    to_delete: bool = False,
-                                    filename = "Italia.parquet") -> list:
-        
-        """Writes a pandas DataFrame into the selected folder. Supported extension is parquet
-
-        Parameters
-        ---------- 
-        df_: pd.DataFrame
-        Dataframe from which to generate the timeseries 
+        self.period = period
 
-        path: str
-        path to the root folder where to generate subfolders and save files
-            
-        hier_col: str 
-        Column name indicating the hierarchy level for which to create folders.
 
-        filename: str
-        If hier_col is not specified, filename of the parquet to save
+    def fit(self, X: pd.DataFrame) -> Self:
 
+        """Compute additive decomposition useful to detrend time series
 
-        Returns:
-            list: 
-                list of created-folders paths
+        Parameters
+        ----------
+        X : pd.DataFrame
+            dataframe containing two columns (timestamp and volumes of time series)         
+
+        Returns
+        -------
+        self : object
+            fitted detrender
         """
-        path_list = []
-        DH = DataHandler()
-        if hier_col != None:
-
-            list_dir_to_make = list(df_[hier_col].unique())
-            for folder in list_dir_to_make:
-                os.makedirs(path + folder + "/", exist_ok=True)
-                file_to_save = path + folder + "/" + folder + ".parquet"
-                isExisting = os.path.exists(file_to_save)
-
-                if not isExisting:
-                    temp = df_[df_[hier_col] == folder].reset_index(drop=True)
-                    df_sub = self.execute(temp)
-                    logger.info('non cè niente ->' + file_to_save)
-                    DH.write(df_sub, file_to_save)
-                elif isExisting == True and to_delete == True:
-                    os.remove(file_to_save)
-                    temp = df_[df_[hier_col] == folder].reset_index(drop=True)
-                    df_sub = self.execute(temp)
-                    logger.info('cè qualcosa ->' +file_to_save)
-                    DH.write(df_sub, file_to_save)
-                else:
-                    continue
-                path_list.append(path + folder + "/")
-                
 
-        else:
-            isExisting = os.path.exists(path + filename)
-            if not isExisting:
-                subdf = self.execute(df_)
-                logger.info('non cè niente ->' + path + '------' + filename)
-                DH.write(subdf, path + filename)
-            elif isExisting == True and to_delete == True:
-                os.remove(path + filename)
-                subdf = self.execute(df_)
-                logger.info('cè qualcosa ->' + path + '------' + filename)
-                DH.write(subdf, path + filename)
-            else: 
-                pass     
-            path_list.append(path)
-    
-        return path_list   
+        additive_decomp = seasonal_decompose(X.iloc[:,1], model="additive", period=self.period, extrapolate_trend="freq")
+        self.trend = additive_decomp.trend
 
-    @log_exception(logger)
-    def execute(self, df : pd.DataFrame) -> pd.DataFrame:
-        
-        """
-        Sequential call of class function to generate the timeseries dataframe according to specified hierarchies and time span
+        return self
 
-        Returns:
-            df_ts: pd.DataFrame 
-                DataFrame identifying the timeseries generated according to specified hierarchies and time span
-        """
+    def transform(self, X:pd.DataFrame) -> pd.DataFrame:
 
-        logger.info('STEP 1 - Starting preparing data', important = True)
-        
-        logger.info('STEP 1 - Extracting date from datetime column')
-        df[self.params['col_index'] + '_date'] = from_timestamp_to_date(df[self.params['col_index'] ])
+        """Perform detrending of time series
 
-        logger.info('STEP 1 - Generating the timeseries target')
-        df_target = generating_target(df, [self.params['col_index']+"_date"], self.params['target_col'])
-        df_target.columns = ['timeline','target']
+        Parameters
+        ----------
+        X : pd.DataFrame
+            dataframe containing two columns (timestamp and volumes of time series)
 
-        logger.info('STEP 1 - Creating the entire timeline to complete the target')
-        df_calendar = pd.DataFrame(resample_date(df_target, "D")['timeline'])
+        Returns
+        -------
+        X : pd.DataFrame
+            transformed time series
+        """
 
-        df_ts = pd.merge(df_calendar, df_target, how='left', on="timeline")
-        
-        logger.info('STEP 1 - Generating the complete timeseries', important = True)
+        detrend_time_series = X.iloc[:,1] - self.trend
+        ris = pd.concat([X.iloc[:,0],detrend_time_series],axis=1)
+        ris.columns = X.columns
 
-        if self.params['timeline_level'][0].upper() != "D":
-            df_ts = self.resample_date(df_ts, self.params['timeline_level'][0].upper() )
-        else:
-            pass 
+        return  ris
+    
+class Deseasoner(TransformerMixin, BaseEstimator):
 
-        #logger.info('STEP 1 - Filling Missing Values', important = True)
-        #df_ts['filled_target'] = list(self.handling_missing_values(df_ts.timeline,df_ts.target))
-        # df_ts.name = self.filename
+    def __init__(self, period: int) -> Self:
 
-        # Rename timeline to timestamp
-        df_ts.rename(columns={'timeline':'Timestamp', 'target':'Target'}, inplace=True)
+        """Deseasonalises time series
 
-        return df_ts
+        Parameters
+        ----------
+        period : int
+            specify period considered for compute additive decomposition
 
-    def find_time_range(self,timeline:pd.Series) -> tuple:
+        Returns
+        -------
+        self : object
         """
-        The function finds the range of the timeline provided in input
+
+        self.period = period
+
+
+    def fit(self, X: pd.DataFrame) -> Self:
+
+        """Compute additive decomposition useful to deseasonalises time series
 
         Parameters
         ----------
-        timeline: pd.Series (dtype: datetime64[ns])
-            The timeline series.
+        X : pd.DataFrame
+            dataframe containing two columns (timestamp and volumes of time series)         
+
         Returns
         -------
-            Tuple
-            The range of the timeline (minimum date, maximum date)
+        self : object
+            fitted deseasoner
         """
-        start_date, end_date = timeline.min(), timeline.max()
-        return start_date, end_date
+        
+        additive_decomp = seasonal_decompose(X.iloc[:,1], model="additive", period=self.period, extrapolate_trend="freq")
+        self.seasonal = additive_decomp.seasonal
 
-    def generate_holidays(self,start_date: datetime, end_date: datetime, aggregation_frequency: str = 'D') -> pd.Series:
-        """
-        The function generates a series containing 1s for holidays and 0s vice-versa 
-        (Saturdays and Sundays are considered holidays)
+        return self
+
+    def transform(self, X: pd.DataFrame) -> pd.DataFrame:
+
+        """Perform deseasonalises of time series
 
         Parameters
         ----------
-        start_date: datetime
-            Starting date of interest
-        end_date: datetime
-            End date of interest
-        aggregation_frequency: str, optional
-            Time aggregation frequency (default: 'D' -> Days) 
-            
+        X : pd.DataFrame
+            dataframe containing two columns (timestamp and volumes of time series)
+
         Returns
         -------
-            pd.Series 
-            Series containing 1s for holidays and 0s vice-versa
+        X : pd.DataFrame
+            transformed time series
         """
-        italy_holidays = holidays.Italy()
-        holidays_list = []
-        current_date = start_date
-
-        while current_date <= end_date:
-            if current_date in italy_holidays or current_date.weekday() == 5 or current_date.weekday() == 6:
-                holidays_list.append(1)
-            else:
-                holidays_list.append(0)
 
-            current_date += np.timedelta64(1, aggregation_frequency)
+        deseason_time_series = X.iloc[:,1] - self.seasonal
+        ris = pd.concat([X.iloc[:,0],deseason_time_series],axis=1)
+        ris.columns = X.columns
 
-        return pd.Series(holidays_list)
-    
+        return ris
 
-    def imputation_missing_target_holidays(self, holidays: pd.Series, target: pd.Series) -> pd.Series:
-        """
-        The function substitutes the missing values in target with 0s for the holidays.
+class Differencer(TransformerMixin, BaseEstimator):
+
+    def __init__(self, lag: int) -> Self:
 
+        """Differencing time series
+        
         Parameters
         ----------
-        holidays : pd.Series
-            represents holidays with 1s and 0s vice-versa. 
-        target : pd.Series
-            represents the target
+        lag : int
+            differencing time series lag
 
         Returns
         -------
-        pd.Series
-            series with 0s where there are missing values corresponding to holidays.
-
+        self : object
         """
-        modified_target = target.copy()
-        missing_indices = modified_target[modified_target.isna()].index
 
-        for index in missing_indices:
-            if holidays.iloc[index] == 1:
-                modified_target.iloc[index] = 0
+        self.lag = lag
 
-        return pd.Series(modified_target)
+    def fit(self, X: pd.DataFrame) -> Self:
 
-    def fill_missing_values(self, timeline: pd.Series, target: pd.Series,) -> pd.Series:
-        """
-        Estimates the target missing values
+        """Compute value useful to compute differencing time series
 
-        Parameters:
-            target: pd.Series 
-            The target variable series
-            timeline: pd.Series
-            The timeline series
+        Parameters
+        ----------
+        X : pd.DataFrame
+            dataframe containing two columns (timestamp and volumes of time series)         
 
-        Returns:
-            pd.Series 
-            The series with the imputation for the missing values
+        Returns
+        -------
+        self : object
+            fitted normalizer
         """
-        if target.isnull().sum() == 0:
-            # No missing values in the series, return the original series
-            return target
-        
-        df_intermediate = pd.DataFrame({'timeline': timeline, 'target': target})
-        df_intermediate.set_index('timeline', inplace=True)
-        target_interp = df_intermediate['target'].interpolate(method='time')
-        return target_interp
 
-    def handling_missing_values(self,timeline: pd.Series, target: pd.Series) -> pd.Series:
-        """
-        The function estimates and corrects the missing values in the target series
+        self.shape = X.shape[0]
+        self.lag_time_series = X.iloc[:self.shape-self.lag,1]
+        self.timestamp = X.iloc[self.lag:,0].reset_index(drop=True)
+
+        return self
+    
+    def transform(self, X: pd.DataFrame) -> pd.DataFrame:
+
+        """Perform differencing time series
 
         Parameters
         ----------
-        timeline: datetime
-            it's the timeline series
-        target: pd.Series
-            The target variable series
+        X : pd.DataFrame
+            dataframe containing two columns (timestamp and volumes of time series)
 
         Returns
         -------
-            the target series with the imputation of the missing values
+        X : pd.DataFrame
+            transformed time series
         """
-        if target.isnull().sum() == 0:
-            return target
-        else:
-            date_range = self.find_time_range(timeline)
-            holidays = self.generate_holidays(date_range[0], date_range[1])
-            target_holidays_imputation = self.imputation_missing_target_holidays(holidays, target)
-            final_target = self.fill_missing_values(timeline,target_holidays_imputation)
-            return final_target
 
+        time_series_lagged = X.iloc[self.lag:,1].reset_index(drop=True) - self.lag_time_series
+        ris = pd.concat([self.timestamp,time_series_lagged], axis=1)
+        ris.columns = X.columns
+        
+        return ris
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `TEST_TC-0.1.1/tc_uc4/utility/exceptions.py` & `TEST_TC-0.1.2/tc_uc4/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.1/tc_uc4/utility/resources.py` & `TEST_TC-0.1.2/tc_uc4/utility/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import os
 import sys
-from typing import Any, Dict, List, Union
+from typing import Any, Dict
 
 import tomli
 
 
-def get_configuration(name: str, config_file: str = "web_app.toml", TEST : bool = False) -> dict[str, Any]:
+def get_configuration(name: str, config_file: str = "web_app.toml", TEST : bool = False) -> Dict[str, Any]:
     """Read the configurations set in the properties.toml file in the config folder and returns them
     as a dictionary
 
     Parameters
     ----------
     name : str
         Section to be read
```

### Comparing `TEST_TC-0.1.1/tc_uc4/utility/tele_logger.py` & `TEST_TC-0.1.2/tc_uc4/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.1/tests/test_datahandler.py` & `TEST_TC-0.1.2/tests/test_datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.1/tests/test_evaluations.py` & `TEST_TC-0.1.2/tests/test_evaluations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import pandas as pd
+import numpy as np
 import pytest
 from analytics.evaluationMetrics import evaluations
 from utility.exceptions import ColumnNotFound
 
 def test_evaluations():
      # Sample data 
-    real_df = pd.DataFrame({'Timestamp': [1, 2, 3], 'Target': [10, 20, 30]})
-    prophet_df = pd.DataFrame({'Timestamp': [1, 2, 3], 'Pred_mean': [12, 18, 32]})
+     real_df = pd.DataFrame({'Timestamp': [1, 2, 3], 'Target': [10, 20, 30]})
+     prophet_df = pd.DataFrame({'Timestamp': [1, 2, 3], 'Pred_mean': [12, 18, 32]})
 
-    # Calculate evaluation metrics
-    result = evaluations(real_df, prophet_df)
+     # Calculate evaluation metrics
+     result = evaluations(real_df, prophet_df)
 
-    # Verify the content of the evaluation dataframe
-    assert isinstance(result, pd.DataFrame)  # The result should be a DataFrame
-    assert len(result) == 4  # The DataFrame should have 4 rows
-    assert set(result.columns) == {'Metrics', 'Value'}  # The DataFrame should have the correct columns
-    assert result['Metrics'].tolist() == ['MAE', 'RMSE', 'MSE', 'R2']  # The values in the 'Metrics' column should be correct
-    assert result['Value'].tolist() == [2.0, 2.0, 4.0, 0.94]  # The values in the 'Value' column should be correct
+     # Verify the content of the evaluation dataframe
+     assert isinstance(result, pd.DataFrame)  # The result should be a DataFrame
+     assert len(result) == 4  # The DataFrame should have 4 rows
+     assert set(result.columns) == {'Metrics', 'Value'}  # The DataFrame should have the correct columns
+     assert result['Metrics'].tolist() == ['MAE', 'RMSE', 'MSE', 'R2']  # The values in the 'Metrics' column should be correct
+     assert result['Value'].tolist() == [2.0, 2.0, 4.0, 0.94]  # The values in the 'Value' column should be correct
+
+     prophet_df = pd.DataFrame({'Timestamp': [1, 2, 3], 'Pred_mean': [np.nan, np.nan, np.nan]})
+     with pytest.raises(Exception):
+         evaluations(real_df, prophet_df)
 
 def test_evaluations_column_not_found():
     # Sample data without the 'Pred_mean' column in the pred dataframe
      df_real = pd.DataFrame({'Timestamp': [1, 2, 3], 'Target': [10, 20, 30]})
      df_pred = pd.DataFrame({'Timestamp': [1, 2, 3], 'Value': [12, 18, 32]})
 
      # Sample data without the 'Timestamp' column in the real dataframe
```

### Comparing `TEST_TC-0.1.1/tests/test_exceptions.py` & `TEST_TC-0.1.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.1/tests/test_resources.py` & `TEST_TC-0.1.2/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.1/tests/test_tele_logger.py` & `TEST_TC-0.1.2/tests/test_tele_logger.py`

 * *Files identical despite different names*

