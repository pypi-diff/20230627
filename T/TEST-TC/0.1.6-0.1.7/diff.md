# Comparing `tmp/TEST_TC-0.1.6.tar.gz` & `tmp/TEST_TC-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-0.1.6.tar", last modified: Tue Jun 27 14:30:38 2023, max compression
+gzip compressed data, was "TEST_TC-0.1.7.tar", last modified: Tue Jun 27 15:32:44 2023, max compression
```

## Comparing `TEST_TC-0.1.6.tar` & `TEST_TC-0.1.7.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.994900 TEST_TC-0.1.6/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 14:30:38.994400 TEST_TC-0.1.6/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/README.md
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.911037 TEST_TC-0.1.6/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 14:30:38.000000 TEST_TC-0.1.6/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1006 2023-06-27 14:30:38.000000 TEST_TC-0.1.6/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 14:30:38.000000 TEST_TC-0.1.6/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 14:30:38.000000 TEST_TC-0.1.6/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 14:30:38.000000 TEST_TC-0.1.6/TEST_TC.egg-info/top_level.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1125 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 14:30:38.995561 TEST_TC-0.1.6/setup.cfg
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       84 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/setup.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.913161 TEST_TC-0.1.6/tc_uc4/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 14:30:31.000000 TEST_TC-0.1.6/tc_uc4/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.921297 TEST_TC-0.1.6/tc_uc4/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5803 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/algorithms/algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/algorithms/prophet_utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.927220 TEST_TC-0.1.6/tc_uc4/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2830 2023-06-27 10:14:15.000000 TEST_TC-0.1.6/tc_uc4/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.930894 TEST_TC-0.1.6/tc_uc4/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7535 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.941216 TEST_TC-0.1.6/tc_uc4/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17975 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/datapreparation/datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3126 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/datapreparation/prep.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.944913 TEST_TC-0.1.6/tc_uc4/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.948083 TEST_TC-0.1.6/tc_uc4/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/datavisualization/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.962398 TEST_TC-0.1.6/tc_uc4/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      949 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/utility/constants.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.6/tc_uc4/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2222 2023-06-26 14:08:09.000000 TEST_TC-0.1.6/tc_uc4/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6351 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/utility/tele_logger.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.990129 TEST_TC-0.1.6/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      200 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2469 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2748 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15247 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1850 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1237 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2866 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_prep.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16902 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_prophet_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2096 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2898 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.153612 TEST_TC-0.1.7/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 15:32:44.152607 TEST_TC-0.1.7/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/README.md
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.085813 TEST_TC-0.1.7/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 15:32:44.000000 TEST_TC-0.1.7/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      997 2023-06-27 15:32:44.000000 TEST_TC-0.1.7/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 15:32:44.000000 TEST_TC-0.1.7/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 15:32:44.000000 TEST_TC-0.1.7/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 15:32:44.000000 TEST_TC-0.1.7/TEST_TC.egg-info/top_level.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1126 2023-06-27 14:56:18.000000 TEST_TC-0.1.7/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 15:32:44.153612 TEST_TC-0.1.7/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.087490 TEST_TC-0.1.7/tc_uc4/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 15:32:32.000000 TEST_TC-0.1.7/tc_uc4/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.094323 TEST_TC-0.1.7/tc_uc4/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5803 2023-06-27 15:13:46.000000 TEST_TC-0.1.7/tc_uc4/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-06-27 15:13:53.000000 TEST_TC-0.1.7/tc_uc4/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.101132 TEST_TC-0.1.7/tc_uc4/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2810 2023-06-27 15:04:47.000000 TEST_TC-0.1.7/tc_uc4/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.104130 TEST_TC-0.1.7/tc_uc4/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7308 2023-06-27 15:01:58.000000 TEST_TC-0.1.7/tc_uc4/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.111374 TEST_TC-0.1.7/tc_uc4/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17975 2023-06-27 15:15:06.000000 TEST_TC-0.1.7/tc_uc4/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3126 2023-06-27 15:15:12.000000 TEST_TC-0.1.7/tc_uc4/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.115376 TEST_TC-0.1.7/tc_uc4/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.117421 TEST_TC-0.1.7/tc_uc4/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/datavisualization/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.128336 TEST_TC-0.1.7/tc_uc4/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.7/tc_uc4/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      949 2023-06-27 14:58:09.000000 TEST_TC-0.1.7/tc_uc4/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.7/tc_uc4/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2119 2023-06-27 14:58:38.000000 TEST_TC-0.1.7/tc_uc4/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6298 2023-06-27 15:19:59.000000 TEST_TC-0.1.7/tc_uc4/utility/tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 15:32:44.150608 TEST_TC-0.1.7/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2762 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15261 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1864 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2873 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-06-27 14:54:10.000000 TEST_TC-0.1.7/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2070 2023-06-27 15:28:35.000000 TEST_TC-0.1.7/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2905 2023-06-27 15:12:14.000000 TEST_TC-0.1.7/tests/test_tele_logger.py
```

### Comparing `TEST_TC-0.1.6/README.md` & `TEST_TC-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.6/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-0.1.7/TEST_TC.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 README.md
 pyproject.toml
-setup.py
 TEST_TC.egg-info/PKG-INFO
 TEST_TC.egg-info/SOURCES.txt
 TEST_TC.egg-info/dependency_links.txt
 TEST_TC.egg-info/requires.txt
 TEST_TC.egg-info/top_level.txt
 tc_uc4/__init__.py
 tc_uc4/algorithms/__init__.py
```

### Comparing `TEST_TC-0.1.6/pyproject.toml` & `TEST_TC-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 dependencies = ["geopandas==0.13.0","holidays==0.24","numpy==1.25.0","pandas==2.0.2","prophet==1.1.1",
                 "scikit_learn==1.2.2","tabulate==0.9.0","tomli==2.0.1","typing_extensions==4.6.3", "pytest==7.3.1",
                 "setuptools==58.1.0", "statsmodels==0.14.0"]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
 where = ["./"]
-include = ["*"]# or define list of packages
+include = ["*"] # or define list of packages
 exclude = []
 namespaces = false
 
 [tool.setuptools.dynamic]
 version = {attr = "tc_uc4.__version__"} # read __version__ from packages __init__.py
```

### Comparing `TEST_TC-0.1.6/tc_uc4/algorithms/algorithm.py` & `TEST_TC-0.1.7/tc_uc4/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.6/tc_uc4/algorithms/prophet_utils.py` & `TEST_TC-0.1.7/tc_uc4/algorithms/prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.6/tc_uc4/analytics/evaluationMetrics.py` & `TEST_TC-0.1.7/tc_uc4/analytics/evaluationMetrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import warnings;
 warnings.simplefilter('ignore')
 import pandas as pd
-import numpy as np
 from sklearn.metrics import mean_squared_error , r2_score, mean_absolute_error
 from ..utility.exceptions import ColumnNotFound
 from ..utility.tele_logger import logger
 
 
 def evaluations(df_real: pd.DataFrame, df_pred: pd.DataFrame, date: str = 'Timestamp' , y_true: str = 'Target', y_pred: str = 'Pred_mean') -> pd.DataFrame:
     """
```

### Comparing `TEST_TC-0.1.6/tc_uc4/datahandler/datahandler.py` & `TEST_TC-0.1.7/tc_uc4/datahandler/datahandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import os
 from typing import Any
 
 import geopandas as gpd
 import pandas as pd
 from typing_extensions import Self
-from ..utility.exceptions import InputTypeError
-from ..utility.resources import log_exception
-from ..utility.tele_logger import logger
+from tc_uc4.utility.exceptions import InputTypeError
+from tc_uc4.utility.resources import log_exception
+from tc_uc4.utility.tele_logger import logger
 
 class DataHandler:
-    def __init__(self, data_folder : str = None) -> Self:
+    def __init__(self, data_folder : str) -> Self:
         """Class which will handle the read and write of .parquet data
 
         Parameters
         ----------
-        data_folder : str, optional
-            Main folder where to find the data, if given as a parameter, by default None
+        data_folder : str
+            Main folder where to find the data, if given as a parameter
         """
-        if data_folder != None and type(data_folder) != str:
+        if type(data_folder) != str:
             raise InputTypeError('DataHandler')
-        
-        if data_folder:
-            self.data_folder = data_folder
-        else:
-            self.data_folder = os.path.join(os.path.split(os.path.split(os.path.dirname(os.path.abspath(__file__)))[0])[0],"data")
+
+        self.data_folder = data_folder
 
     @log_exception(logger)
     def read(self, filename: str, folder: str = "input", in_attr: bool = False, **kwargs: Any) -> pd.DataFrame:
         """
         Read datafile given a folder from <data_folder>/<folder> and the filename. Supported extensions are
         csv and parquet. See: https://pandas.pydata.org/docs/reference/api/pandas.read_parquet.html
         and https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html for more info
```

### Comparing `TEST_TC-0.1.6/tc_uc4/datapreparation/datapreparation_utils.py` & `TEST_TC-0.1.7/tc_uc4/datapreparation/datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.6/tc_uc4/datapreparation/prep.py` & `TEST_TC-0.1.7/tc_uc4/datapreparation/prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.6/tc_uc4/utility/constants.py` & `TEST_TC-0.1.7/tc_uc4/utility/constants.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.6/tc_uc4/utility/exceptions.py` & `TEST_TC-0.1.7/tc_uc4/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.6/tc_uc4/utility/resources.py` & `TEST_TC-0.1.7/tc_uc4/utility/resources.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 import os
 import sys
 from typing import Any, Dict
 
 import tomli
 
-
-def get_configuration(name: str, config_file: str = "web_app.toml", TEST : bool = False) -> Dict[str, Any]:
+def get_configuration(name: str, config_path = str, config_file: str = "web_app.toml") -> Dict[str, Any]:
     """Read the configurations set in the properties.toml file in the config folder and returns them
     as a dictionary
 
     Parameters
     ----------
     name : str
-        Section to be read
+        Section to be 
+    config_path : str
+        Specifies the config path where the .toml configurations resides
     config_file : str, optional
         Specifies the config file to read, by default 'properties.toml'
     TEST : bool, optional
         To set to True only if a unitary test is ran
 
     Returns
     -------
@@ -26,26 +27,21 @@
         Dictionary containing the properties read
 
     Raises
     ------
     Exception
         Raise error if .conf file is not found
     """
-    path = os.path.dirname(os.path.abspath(__file__))
-    path = os.path.split(os.path.split(path)[0])[0] + "/config/"
-
-    if TEST:
-        path, config_file = os.path.split(os.path.join(path, config_file))
 
-    if config_file not in os.listdir(path):
+    if config_file not in os.listdir(config_path):
         raise Exception(
-            f"File {config_file} not found in {path} please double check that the filename is correct."
+            f"File {config_file} not found in {config_path} please double check that the filename is correct."
         )
 
-    config = tomli.load(open(os.path.join(path, config_file), "rb"))
+    config = tomli.load(open(os.path.join(config_path, config_file), "rb"))
     # Read from the specified file, the specified section
     if name in config:
         return config[name]
     else:
         raise Exception("System " + name + " not found in .conf file")
 
 def log_exception(logger=None):
```

### Comparing `TEST_TC-0.1.6/tc_uc4/utility/tele_logger.py` & `TEST_TC-0.1.7/tc_uc4/utility/tele_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import sys
 import os
 import logging
 from logging import INFO
 from time import localtime, strftime
-#from .resources import GetConfiguration
-
 
 class Logger(logging.getLoggerClass()):
     """Logger class used to manage the log routing and writes logs on different files."""
 
     def __init__(self,
                  format: str = "%(asctime)s | %(levelname)s | %(message)s",
                  level: int = INFO):
@@ -21,36 +19,35 @@
         level : log Level, optional
             Log level, by default INFO
         """
 
         self.logger = logging.getLogger("logger")
         self.important_logger = logging.getLogger("important_logger")
 
-        path = os.path.dirname(os.path.abspath(__file__))
-        path = os.path.split(os.path.split(path)[0])[0] + "/logs/"
-
-        self.logging_folder = path
-
         # Initial construct.
         self.format = format
         self.level = level
         self.name = None
 
     def initialize_logger(self,
+                          log_path : str,
                           name: str):
         """Initialize the logging session by creating the logging files 
         <name>_<YYYYMMDD>.log and <name>_<YYYYMMDD>_verbose.log . If a new name 
         is passed then a new log session and files are created aswell
 
         Parameters
         ----------
+        log_path : str
+            Path where Logging will save the logs
         name : str
             Logging session name
         """
         self.name = name
+        self.logging_folder = log_path
 
         # Logger configuration.
         self.console_formatter = logging.Formatter(self.format)
         self.console_logger = logging.StreamHandler(sys.stdout)
         self.console_logger.setFormatter(self.console_formatter)
 
         # Complete logging config.
```

### Comparing `TEST_TC-0.1.6/tests/test_algorithm.py` & `TEST_TC-0.1.7/tests/test_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 import pandas as pd
-from algorithms.algorithm import prophet_tuning, Prophet_model
+from tc_uc4.algorithms.algorithm import prophet_tuning, Prophet_model
 
 ### prophet_tuning ###
 
 @pytest.fixture
 def example_train_df():
     return pd.DataFrame({
         'ds': pd.to_datetime(['2023-06-01', '2023-06-02', '2023-06-03']),
```

### Comparing `TEST_TC-0.1.6/tests/test_datahandler.py` & `TEST_TC-0.1.7/tests/test_datahandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 import pandas as pd
 import geopandas as gpd
 from unittest.mock import patch, MagicMock
 
-from datahandler.datahandler import DataHandler
-from utility.exceptions import InputTypeError
+from tc_uc4.datahandler.datahandler import DataHandler
+from tc_uc4.utility.exceptions import InputTypeError
 
 @pytest.fixture
 def data_handler():
     return DataHandler()
 
 def test_data_handler_configured_init_read(tmp_path):
     # Create a Pandas DataFrame
```

### Comparing `TEST_TC-0.1.6/tests/test_datapreparation_utils.py` & `TEST_TC-0.1.7/tests/test_datapreparation_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import numpy as np
 import pytest
-from datapreparation.datapreparation_utils import (code_to_name, from_timestamp_to_date, generating_target,
+from tc_uc4.datapreparation.datapreparation_utils import (code_to_name, from_timestamp_to_date, generating_target,
                                                    resample_date, Normalizer, ReplacerNA, Detrender,
                                                    Deseasoner, Differencer)
-from utility.exceptions import InputTypeError
+from tc_uc4.utility.exceptions import InputTypeError
 from statsmodels.tsa.seasonal import seasonal_decompose
 
 ### code_to_name ###
 
 # Test case for valid input
 def test_code_to_name_valid_input():
     # Create a sample pd.Series and mapping dictionary for testing
```

### Comparing `TEST_TC-0.1.6/tests/test_evaluations.py` & `TEST_TC-0.1.7/tests/test_evaluations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import numpy as np
 import pytest
-from analytics.evaluationMetrics import evaluations
-from utility.exceptions import ColumnNotFound
+from tc_uc4.analytics.evaluationMetrics import evaluations
+from tc_uc4.utility.exceptions import ColumnNotFound
 
 def test_evaluations():
      # Sample data 
      real_df = pd.DataFrame({'Timestamp': [1, 2, 3], 'Target': [10, 20, 30]})
      prophet_df = pd.DataFrame({'Timestamp': [1, 2, 3], 'Pred_mean': [12, 18, 32]})
 
      # Calculate evaluation metrics
```

### Comparing `TEST_TC-0.1.6/tests/test_exceptions.py` & `TEST_TC-0.1.7/tests/test_exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 import pandas as pd
 from tabulate import tabulate
-from utility.exceptions import InputTypeError, ColumnNotFound
+from tc_uc4.utility.exceptions import InputTypeError, ColumnNotFound
 
 ### InputTypeError ###
 def test_input_type_error_message():
     func_name = "my_function"
     error_message = "Wrong input types have been given to the function."
     error = InputTypeError(func_name)
     assert str(error) == f"{func_name} encountered an error: {error_message}"
```

### Comparing `TEST_TC-0.1.6/tests/test_prep.py` & `TEST_TC-0.1.7/tests/test_prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import pytest
 from sklearn.utils.estimator_checks import check_estimator
 
-from datapreparation.prep import PreprocessingClass
+from tc_uc4.datapreparation.prep import PreprocessingClass
 
 
 
 test_with_data = [
     ('teleconsulto','prophet','data_richiesta','id_teleconsulto')
 ]
 test_no_data = [
```

### Comparing `TEST_TC-0.1.6/tests/test_prophet_utils.py` & `TEST_TC-0.1.7/tests/test_prophet_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import pytest
 import os
-from algorithms.prophet_utils import (check_prophet_fit_df, check_prophet_predict_df,
+from tc_uc4.algorithms.prophet_utils import (check_prophet_fit_df, check_prophet_predict_df,
                                       check_prophet_predict_df, check_prophet_save,
                                       check_prophet_load, check_split_input, train_val_test_split,
                                       save_model_results, preprocess_prophet_output,
                                       check_preprocess_prophet_input, preprocess_prophet_input,
                                       is_not_convertible_to_int_float, literal_evaluation, generate_values,
                                       grid_values_hyperparameters)
```

### Comparing `TEST_TC-0.1.6/tests/test_resources.py` & `TEST_TC-0.1.7/tests/test_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import os
 import sys
 from typing import Any, Dict
 import pytest
 import logging
 from unittest.mock import patch
 
-from utility.resources import get_configuration, log_exception
+from tc_uc4.utility.resources import get_configuration, log_exception
 
 ### get_configuration ###
 @pytest.fixture
 def mock_config_file(tmpdir):
     config_file = tmpdir.join("proprerties.toml")
     config_file.write("[section]\nkey = 'value'")
     return str(config_file)
 
 def test_get_configuration_valid(mock_config_file):
-    result = get_configuration("section", config_file=mock_config_file, TEST=True)
+    result = get_configuration("section", config_file=mock_config_file)
     assert isinstance(result, dict)
     assert result["key"] == "value"
 
 def test_get_configuration_invalid_file():
     with pytest.raises(Exception):
-        get_configuration("section", config_file="non_existent.toml", TEST=True)
+        get_configuration("section", config_file="non_existent.toml")
 
 def test_get_configuration_invalid_section(mock_config_file):
     with pytest.raises(Exception):
-        get_configuration("non_existent_section", config_file=mock_config_file, TEST=True)
+        get_configuration("non_existent_section", config_file=mock_config_file)
 
 ### log_exception ###
 def test_log_exception_with_logger(caplog):
     logger = logging.getLogger("test_logger")
 
     @log_exception(logger)
     def my_function():
```

### Comparing `TEST_TC-0.1.6/tests/test_tele_logger.py` & `TEST_TC-0.1.7/tests/test_tele_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging
 from logging import DEBUG
 from time import localtime, strftime
-from utility.tele_logger import Logger
+from tc_uc4.utility.tele_logger import Logger
 
 def test_logger_initialization():
     logger = Logger()
     assert isinstance(logger.logger, logging.Logger)
     assert isinstance(logger.important_logger, logging.Logger)
     assert logger.name is None
```

