# Comparing `tmp/TEST_TC-0.1.5.tar.gz` & `tmp/TEST_TC-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-0.1.5.tar", last modified: Tue Jun 27 11:08:14 2023, max compression
+gzip compressed data, was "TEST_TC-0.1.6.tar", last modified: Tue Jun 27 14:30:38 2023, max compression
```

## Comparing `TEST_TC-0.1.5.tar` & `TEST_TC-0.1.6.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.498220 TEST_TC-0.1.5/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 11:08:14.497206 TEST_TC-0.1.5/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/README.md
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.424541 TEST_TC-0.1.5/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 11:08:14.000000 TEST_TC-0.1.5/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      969 2023-06-27 11:08:14.000000 TEST_TC-0.1.5/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 11:08:14.000000 TEST_TC-0.1.5/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 11:08:14.000000 TEST_TC-0.1.5/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 11:08:14.000000 TEST_TC-0.1.5/TEST_TC.egg-info/top_level.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1126 2023-06-27 11:08:07.000000 TEST_TC-0.1.5/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 11:08:14.499207 TEST_TC-0.1.5/setup.cfg
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.426263 TEST_TC-0.1.5/tc_uc4/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 11:06:09.000000 TEST_TC-0.1.5/tc_uc4/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.431845 TEST_TC-0.1.5/tc_uc4/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5830 2023-06-27 10:40:34.000000 TEST_TC-0.1.5/tc_uc4/algorithms/algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15599 2023-06-27 10:41:03.000000 TEST_TC-0.1.5/tc_uc4/algorithms/prophet_utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.436822 TEST_TC-0.1.5/tc_uc4/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2830 2023-06-27 10:14:15.000000 TEST_TC-0.1.5/tc_uc4/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.440820 TEST_TC-0.1.5/tc_uc4/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7550 2023-06-27 10:39:52.000000 TEST_TC-0.1.5/tc_uc4/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.448591 TEST_TC-0.1.5/tc_uc4/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17985 2023-06-27 10:39:31.000000 TEST_TC-0.1.5/tc_uc4/datapreparation/datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3141 2023-06-27 10:39:30.000000 TEST_TC-0.1.5/tc_uc4/datapreparation/prep.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.451357 TEST_TC-0.1.5/tc_uc4/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.454435 TEST_TC-0.1.5/tc_uc4/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/datavisualization/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.466286 TEST_TC-0.1.5/tc_uc4/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.5/tc_uc4/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2222 2023-06-26 14:08:09.000000 TEST_TC-0.1.5/tc_uc4/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6174 2023-06-13 16:27:38.000000 TEST_TC-0.1.5/tc_uc4/utility/tele_logger.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.493208 TEST_TC-0.1.5/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:42:45.000000 TEST_TC-0.1.5/tests/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-06-27 10:41:26.000000 TEST_TC-0.1.5/tests/test_algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2762 2023-06-27 10:41:39.000000 TEST_TC-0.1.5/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15261 2023-06-27 10:41:47.000000 TEST_TC-0.1.5/tests/test_datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1864 2023-06-27 10:42:00.000000 TEST_TC-0.1.5/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-06-27 10:42:03.000000 TEST_TC-0.1.5/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2873 2023-06-27 10:42:07.000000 TEST_TC-0.1.5/tests/test_prep.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-06-27 10:42:13.000000 TEST_TC-0.1.5/tests/test_prophet_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2103 2023-06-27 10:42:17.000000 TEST_TC-0.1.5/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2905 2023-06-27 10:42:20.000000 TEST_TC-0.1.5/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.994900 TEST_TC-0.1.6/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 14:30:38.994400 TEST_TC-0.1.6/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/README.md
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.911037 TEST_TC-0.1.6/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 14:30:38.000000 TEST_TC-0.1.6/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1006 2023-06-27 14:30:38.000000 TEST_TC-0.1.6/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 14:30:38.000000 TEST_TC-0.1.6/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 14:30:38.000000 TEST_TC-0.1.6/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 14:30:38.000000 TEST_TC-0.1.6/TEST_TC.egg-info/top_level.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1125 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 14:30:38.995561 TEST_TC-0.1.6/setup.cfg
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       84 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/setup.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.913161 TEST_TC-0.1.6/tc_uc4/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 14:30:31.000000 TEST_TC-0.1.6/tc_uc4/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.921297 TEST_TC-0.1.6/tc_uc4/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5803 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.927220 TEST_TC-0.1.6/tc_uc4/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2830 2023-06-27 10:14:15.000000 TEST_TC-0.1.6/tc_uc4/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.930894 TEST_TC-0.1.6/tc_uc4/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7535 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.941216 TEST_TC-0.1.6/tc_uc4/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17975 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3126 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.944913 TEST_TC-0.1.6/tc_uc4/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.948083 TEST_TC-0.1.6/tc_uc4/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/datavisualization/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.962398 TEST_TC-0.1.6/tc_uc4/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.6/tc_uc4/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      949 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/utility/constants.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.6/tc_uc4/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2222 2023-06-26 14:08:09.000000 TEST_TC-0.1.6/tc_uc4/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6351 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tc_uc4/utility/tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 14:30:38.990129 TEST_TC-0.1.6/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      200 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2469 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2748 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15247 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1850 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1237 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2866 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16902 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2096 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2898 2023-06-27 14:29:28.000000 TEST_TC-0.1.6/tests/test_tele_logger.py
```

### Comparing `TEST_TC-0.1.5/README.md` & `TEST_TC-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.5/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-0.1.6/TEST_TC.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 README.md
 pyproject.toml
+setup.py
 TEST_TC.egg-info/PKG-INFO
 TEST_TC.egg-info/SOURCES.txt
 TEST_TC.egg-info/dependency_links.txt
 TEST_TC.egg-info/requires.txt
 TEST_TC.egg-info/top_level.txt
 tc_uc4/__init__.py
 tc_uc4/algorithms/__init__.py
@@ -15,14 +16,15 @@
 tc_uc4/datahandler/datahandler.py
 tc_uc4/datapreparation/__init__.py
 tc_uc4/datapreparation/datapreparation_utils.py
 tc_uc4/datapreparation/prep.py
 tc_uc4/dataset/__init__.py
 tc_uc4/datavisualization/__init__.py
 tc_uc4/utility/__init__.py
+tc_uc4/utility/constants.py
 tc_uc4/utility/exceptions.py
 tc_uc4/utility/resources.py
 tc_uc4/utility/tele_logger.py
 tests/__init__.py
 tests/test_algorithm.py
 tests/test_datahandler.py
 tests/test_datapreparation_utils.py
```

### Comparing `TEST_TC-0.1.5/pyproject.toml` & `TEST_TC-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 dependencies = ["geopandas==0.13.0","holidays==0.24","numpy==1.25.0","pandas==2.0.2","prophet==1.1.1",
                 "scikit_learn==1.2.2","tabulate==0.9.0","tomli==2.0.1","typing_extensions==4.6.3", "pytest==7.3.1",
                 "setuptools==58.1.0", "statsmodels==0.14.0"]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
 where = ["./"]
-include = ["*"] # or define list of packages
+include = ["*"]# or define list of packages
 exclude = []
 namespaces = false
 
 [tool.setuptools.dynamic]
 version = {attr = "tc_uc4.__version__"} # read __version__ from packages __init__.py
```

### Comparing `TEST_TC-0.1.5/tc_uc4/algorithms/algorithm.py` & `TEST_TC-0.1.6/tc_uc4/algorithms/algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import pickle
 
 from prophet import Prophet
 from typing_extensions import Self
-from tc_uc4.algorithms.prophet_utils import check_prophet_fit_df, check_prophet_predict_df, check_prophet_save, check_prophet_load
+from .prophet_utils import check_prophet_fit_df, check_prophet_predict_df, check_prophet_save, check_prophet_load
 
-from tc_uc4.utility.tele_logger import logger
-from tc_uc4.utility.resources import log_exception
+from ..utility.tele_logger import logger
+from ..utility.resources import log_exception
 import itertools
 from sklearn.metrics import mean_squared_error, mean_absolute_error
 import numpy as np
 
 class Prophet_model:
     def __init__(self, dic_param: dict = {
                   "changepoint_prior_scale": 0.5,
```

### Comparing `TEST_TC-0.1.5/tc_uc4/algorithms/prophet_utils.py` & `TEST_TC-0.1.6/tc_uc4/algorithms/prophet_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import numpy as np
 import os
 import ast
 
-from tc_uc4.datahandler.datahandler import DataHandler
-from tc_uc4.utility.tele_logger import logger
+from ..datahandler.datahandler import DataHandler
+from ..utility.tele_logger import logger
 
 def check_prophet_fit_df(input_data):
     """
     Esegue i controlli sull'input fornito per il metodo fit() di Prophet.
 
     Parameters
     ----------
```

### Comparing `TEST_TC-0.1.5/tc_uc4/analytics/evaluationMetrics.py` & `TEST_TC-0.1.6/tc_uc4/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.5/tc_uc4/datahandler/datahandler.py` & `TEST_TC-0.1.6/tc_uc4/datahandler/datahandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from typing import Any
 
 import geopandas as gpd
 import pandas as pd
 from typing_extensions import Self
-from tc_uc4.utility.exceptions import InputTypeError
-from tc_uc4.utility.resources import log_exception
-from tc_uc4.utility.tele_logger import logger
+from ..utility.exceptions import InputTypeError
+from ..utility.resources import log_exception
+from ..utility.tele_logger import logger
 
 class DataHandler:
     def __init__(self, data_folder : str = None) -> Self:
         """Class which will handle the read and write of .parquet data
 
         Parameters
         ----------
```

### Comparing `TEST_TC-0.1.5/tc_uc4/datapreparation/datapreparation_utils.py` & `TEST_TC-0.1.6/tc_uc4/datapreparation/datapreparation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
-from tc_uc4.utility.tele_logger import logger
-from tc_uc4.utility.exceptions import InputTypeError
+from ..utility.tele_logger import logger
+from ..utility.exceptions import InputTypeError
 from statsmodels.tsa.seasonal import seasonal_decompose
 from sklearn.base import BaseEstimator, TransformerMixin
 from typing_extensions import Self
 from typing import Union, Dict, List
 
 class PreprocessingTeleconsulto:
```

### Comparing `TEST_TC-0.1.5/tc_uc4/datapreparation/prep.py` & `TEST_TC-0.1.6/tc_uc4/datapreparation/prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sklearn.base import BaseEstimator, TransformerMixin
 from typing_extensions import Self, Any
 import pandas as pd
-from tc_uc4.utility.tele_logger import logger
-from tc_uc4.utility.resources import *
-from tc_uc4.datapreparation.datapreparation_utils import PreprocessingTeleconsulto
+from ..utility.tele_logger import logger
+from ..utility.resources import *
+from ..datapreparation.datapreparation_utils import PreprocessingTeleconsulto
 import pickle
 
 class PreprocessingClass(BaseEstimator, TransformerMixin):
 
     def __init__(self,
                  usecase: str = "teleconsulto",
                  model: str = "prophet",
```

### Comparing `TEST_TC-0.1.5/tc_uc4/utility/exceptions.py` & `TEST_TC-0.1.6/tc_uc4/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.5/tc_uc4/utility/resources.py` & `TEST_TC-0.1.6/tc_uc4/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.5/tc_uc4/utility/tele_logger.py` & `TEST_TC-0.1.6/tc_uc4/utility/tele_logger.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-import sys
-import os
-import logging
-from logging import INFO
-from time import localtime, strftime
-#from .resources import GetConfiguration
-
-
-class Logger(logging.getLoggerClass()):
-    """Logger class used to manage the log routing and writes logs on different files."""
-
-    def __init__(self,
-                 format: str = "%(asctime)s | %(levelname)s | %(message)s",
-                 level: int = INFO):
-        """Logger initialization, sets default logging format and log level 
-
-        Parameters
-        ----------
-        format : str, optional
-            Log message format, by default "%(asctime)s | %(levelname)s | %(message)s"
-        level : log Level, optional
-            Log level, by default INFO
-        """
-
-        self.logger = logging.getLogger("logger")
-        self.important_logger = logging.getLogger("important_logger")
-
-        path = os.path.dirname(os.path.abspath(__file__))
-        path = os.path.split(os.path.split(path)[0])[0] + "/logs/"
-
-        self.logging_folder = path
-
-        # Initial construct.
-        self.format = format
-        self.level = level
-        self.name = None
-
-    def initialize_logger(self,
-                          name: str):
-        """Initialize the logging session by creating the logging files 
-        <name>_<YYYYMMDD>.log and <name>_<YYYYMMDD>_verbose.log . If a new name 
-        is passed then a new log session and files are created aswell
-
-        Parameters
-        ----------
-        name : str
-            Logging session name
-        """
-        self.name = name
-
-        # Logger configuration.
-        self.console_formatter = logging.Formatter(self.format)
-        self.console_logger = logging.StreamHandler(sys.stdout)
-        self.console_logger.setFormatter(self.console_formatter)
-
-        # Complete logging config.
-        self.logger.setLevel(self.level)
-        self.important_logger.setLevel(self.level)
-
-        # Logger configuration.
-        self.file_formatter = logging.Formatter(self.format)
-
-        # check if folder exists
-        if not os.path.exists(self.logging_folder):
-            os.makedirs(self.logging_folder)
-        self.file_logger = logging.FileHandler(os.path.join(
-            self.logging_folder, self.name + "_verbose_" + strftime("%Y%m%d", localtime()) + ".log"))
-        self.file_logger.setFormatter(self.file_formatter)
-        self.important_file_logger = logging.FileHandler(
-            os.path.join(self.logging_folder, self.name + "_" + strftime("%Y%m%d", localtime()) + ".log"))
-        self.important_file_logger.setFormatter(self.file_formatter)
-
-        # Complete logging config.
-        handler_list = []
-        for handler in self.logger.handlers:
-            try:
-                handler_list.append(os.path.split(handler.baseFilename)[1])
-                print(handler_list)
-            except AttributeError:
-                pass
-        
-        if self.name + "_verbose_" + strftime("%Y%m%d", localtime()) + ".log" not in handler_list:
-            self.logger.addHandler(self.console_logger)
-            self.logger.addHandler(self.file_logger)
-        if self.name + "_" + strftime("%Y%m%d", localtime()) + ".log" not in handler_list:
-            self.important_logger.addHandler(self.important_file_logger)
-
-    def info(self,
-             msg: str,
-             extra: dict = None,
-             important: bool = False):
-        """Generates a INFO log level row
-
-        Parameters
-        ----------
-        msg : str
-            Message associated to the log line
-        extra : dict, optional
-            Dictionary containing the missing FORMAT attributes 
-            needed to generate the log message, by default None
-        important : bool, optional
-           Specify wether to write or not on main .log file , by default False
-        """
-        self.logger.info(msg, extra=extra)
-        if important:
-            self.important_logger.info(msg, extra=extra)
-
-    def error(self,
-              msg: str,
-              extra: dict = None):
-        """Generates an ERROR log level row
-
-        Parameters
-        ----------
-        msg : str
-            Message associated to the log line
-        extra : dict, optional
-            Dictionary containing the missing FORMAT attributes 
-            needed to generate the log message, by default None
-        """
-        self.logger.error(msg, extra=extra)
-        self.important_logger.error(msg, extra=extra)
-
-    def exception(self,
-                  msg: str,
-                  extra: dict = None):
-        """Generates an EXCEPTION log level row
-
-        Parameters
-        ----------
-        msg : str
-            Message associated to the log line
-        extra : dict, optional
-            Dictionary containing the missing FORMAT attributes 
-            needed to generate the log message, by default None
-        """
-        self.logger.exception(msg, extra=extra)
-        self.important_logger.exception(msg, extra=extra)
-
-    def warning(self,
-                msg: str,
-                extra: dict = None):
-        """Generates a WARNING log level row
-
-        Parameters
-        ----------
-        msg : str
-            Message associated to the log line
-        extra : dict, optional
-            Dictionary containing the missing FORMAT attributes 
-            needed to generate the log message, by default None
-        """
-        self.logger.warning(msg, extra=extra)
-
-    def debug(self,
-              msg: str,
-              extra: dict = None):
-        """Generates a DEBUG log level row
-
-        Parameters
-        ----------
-        msg : str
-            Message associated to the log line
-        extra : dict, optional
-            Dictionary containing the missing FORMAT attributes 
-            needed to generate the log message, by default None
-        """
-        self.logger.debug(msg, extra=extra)
-
-    # def profile_memory_usage(self):
-    #     memory_usage = dict(psutil.virtual_memory()._asdict())
-    #     memory_usage_log = str(
-    #         {key: round(el / (1024 ** 3), 3) if key != "percent" else el for key, el in memory_usage.items()})
-    #     self.logger.info("Memory usage: " + memory_usage_log)
-
-
-logger = Logger()
+import sys
+import os
+import logging
+from logging import INFO
+from time import localtime, strftime
+#from .resources import GetConfiguration
+
+
+class Logger(logging.getLoggerClass()):
+    """Logger class used to manage the log routing and writes logs on different files."""
+
+    def __init__(self,
+                 format: str = "%(asctime)s | %(levelname)s | %(message)s",
+                 level: int = INFO):
+        """Logger initialization, sets default logging format and log level 
+
+        Parameters
+        ----------
+        format : str, optional
+            Log message format, by default "%(asctime)s | %(levelname)s | %(message)s"
+        level : log Level, optional
+            Log level, by default INFO
+        """
+
+        self.logger = logging.getLogger("logger")
+        self.important_logger = logging.getLogger("important_logger")
+
+        path = os.path.dirname(os.path.abspath(__file__))
+        path = os.path.split(os.path.split(path)[0])[0] + "/logs/"
+
+        self.logging_folder = path
+
+        # Initial construct.
+        self.format = format
+        self.level = level
+        self.name = None
+
+    def initialize_logger(self,
+                          name: str):
+        """Initialize the logging session by creating the logging files 
+        <name>_<YYYYMMDD>.log and <name>_<YYYYMMDD>_verbose.log . If a new name 
+        is passed then a new log session and files are created aswell
+
+        Parameters
+        ----------
+        name : str
+            Logging session name
+        """
+        self.name = name
+
+        # Logger configuration.
+        self.console_formatter = logging.Formatter(self.format)
+        self.console_logger = logging.StreamHandler(sys.stdout)
+        self.console_logger.setFormatter(self.console_formatter)
+
+        # Complete logging config.
+        self.logger.setLevel(self.level)
+        self.important_logger.setLevel(self.level)
+
+        # Logger configuration.
+        self.file_formatter = logging.Formatter(self.format)
+
+        # check if folder exists
+        if not os.path.exists(self.logging_folder):
+            os.makedirs(self.logging_folder)
+        self.file_logger = logging.FileHandler(os.path.join(
+            self.logging_folder, self.name + "_verbose_" + strftime("%Y%m%d", localtime()) + ".log"))
+        self.file_logger.setFormatter(self.file_formatter)
+        self.important_file_logger = logging.FileHandler(
+            os.path.join(self.logging_folder, self.name + "_" + strftime("%Y%m%d", localtime()) + ".log"))
+        self.important_file_logger.setFormatter(self.file_formatter)
+
+        # Complete logging config.
+        handler_list = []
+        for handler in self.logger.handlers:
+            try:
+                handler_list.append(os.path.split(handler.baseFilename)[1])
+                print(handler_list)
+            except AttributeError:
+                pass
+        
+        if self.name + "_verbose_" + strftime("%Y%m%d", localtime()) + ".log" not in handler_list:
+            self.logger.addHandler(self.console_logger)
+            self.logger.addHandler(self.file_logger)
+        if self.name + "_" + strftime("%Y%m%d", localtime()) + ".log" not in handler_list:
+            self.important_logger.addHandler(self.important_file_logger)
+
+    def info(self,
+             msg: str,
+             extra: dict = None,
+             important: bool = False):
+        """Generates a INFO log level row
+
+        Parameters
+        ----------
+        msg : str
+            Message associated to the log line
+        extra : dict, optional
+            Dictionary containing the missing FORMAT attributes 
+            needed to generate the log message, by default None
+        important : bool, optional
+           Specify wether to write or not on main .log file , by default False
+        """
+        self.logger.info(msg, extra=extra)
+        if important:
+            self.important_logger.info(msg, extra=extra)
+
+    def error(self,
+              msg: str,
+              extra: dict = None):
+        """Generates an ERROR log level row
+
+        Parameters
+        ----------
+        msg : str
+            Message associated to the log line
+        extra : dict, optional
+            Dictionary containing the missing FORMAT attributes 
+            needed to generate the log message, by default None
+        """
+        self.logger.error(msg, extra=extra)
+        self.important_logger.error(msg, extra=extra)
+
+    def exception(self,
+                  msg: str,
+                  extra: dict = None):
+        """Generates an EXCEPTION log level row
+
+        Parameters
+        ----------
+        msg : str
+            Message associated to the log line
+        extra : dict, optional
+            Dictionary containing the missing FORMAT attributes 
+            needed to generate the log message, by default None
+        """
+        self.logger.exception(msg, extra=extra)
+        self.important_logger.exception(msg, extra=extra)
+
+    def warning(self,
+                msg: str,
+                extra: dict = None):
+        """Generates a WARNING log level row
+
+        Parameters
+        ----------
+        msg : str
+            Message associated to the log line
+        extra : dict, optional
+            Dictionary containing the missing FORMAT attributes 
+            needed to generate the log message, by default None
+        """
+        self.logger.warning(msg, extra=extra)
+
+    def debug(self,
+              msg: str,
+              extra: dict = None):
+        """Generates a DEBUG log level row
+
+        Parameters
+        ----------
+        msg : str
+            Message associated to the log line
+        extra : dict, optional
+            Dictionary containing the missing FORMAT attributes 
+            needed to generate the log message, by default None
+        """
+        self.logger.debug(msg, extra=extra)
+
+    # def profile_memory_usage(self):
+    #     memory_usage = dict(psutil.virtual_memory()._asdict())
+    #     memory_usage_log = str(
+    #         {key: round(el / (1024 ** 3), 3) if key != "percent" else el for key, el in memory_usage.items()})
+    #     self.logger.info("Memory usage: " + memory_usage_log)
+
+
+logger = Logger()
```

### Comparing `TEST_TC-0.1.5/tests/test_algorithm.py` & `TEST_TC-0.1.6/tests/test_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 import pandas as pd
-from tc_uc4.algorithms.algorithm import prophet_tuning, Prophet_model
+from algorithms.algorithm import prophet_tuning, Prophet_model
 
 ### prophet_tuning ###
 
 @pytest.fixture
 def example_train_df():
     return pd.DataFrame({
         'ds': pd.to_datetime(['2023-06-01', '2023-06-02', '2023-06-03']),
```

### Comparing `TEST_TC-0.1.5/tests/test_datahandler.py` & `TEST_TC-0.1.6/tests/test_datahandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 import pandas as pd
 import geopandas as gpd
 from unittest.mock import patch, MagicMock
 
-from tc_uc4.datahandler.datahandler import DataHandler
-from tc_uc4.utility.exceptions import InputTypeError
+from datahandler.datahandler import DataHandler
+from utility.exceptions import InputTypeError
 
 @pytest.fixture
 def data_handler():
     return DataHandler()
 
 def test_data_handler_configured_init_read(tmp_path):
     # Create a Pandas DataFrame
```

### Comparing `TEST_TC-0.1.5/tests/test_datapreparation_utils.py` & `TEST_TC-0.1.6/tests/test_datapreparation_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import numpy as np
 import pytest
-from tc_uc4.datapreparation.datapreparation_utils import (code_to_name, from_timestamp_to_date, generating_target,
+from datapreparation.datapreparation_utils import (code_to_name, from_timestamp_to_date, generating_target,
                                                    resample_date, Normalizer, ReplacerNA, Detrender,
                                                    Deseasoner, Differencer)
-from tc_uc4.utility.exceptions import InputTypeError
+from utility.exceptions import InputTypeError
 from statsmodels.tsa.seasonal import seasonal_decompose
 
 ### code_to_name ###
 
 # Test case for valid input
 def test_code_to_name_valid_input():
     # Create a sample pd.Series and mapping dictionary for testing
```

### Comparing `TEST_TC-0.1.5/tests/test_evaluations.py` & `TEST_TC-0.1.6/tests/test_evaluations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import numpy as np
 import pytest
-from tc_uc4.analytics.evaluationMetrics import evaluations
-from tc_uc4.utility.exceptions import ColumnNotFound
+from analytics.evaluationMetrics import evaluations
+from utility.exceptions import ColumnNotFound
 
 def test_evaluations():
      # Sample data 
      real_df = pd.DataFrame({'Timestamp': [1, 2, 3], 'Target': [10, 20, 30]})
      prophet_df = pd.DataFrame({'Timestamp': [1, 2, 3], 'Pred_mean': [12, 18, 32]})
 
      # Calculate evaluation metrics
```

### Comparing `TEST_TC-0.1.5/tests/test_exceptions.py` & `TEST_TC-0.1.6/tests/test_exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 import pandas as pd
 from tabulate import tabulate
-from tc_uc4.utility.exceptions import InputTypeError, ColumnNotFound
+from utility.exceptions import InputTypeError, ColumnNotFound
 
 ### InputTypeError ###
 def test_input_type_error_message():
     func_name = "my_function"
     error_message = "Wrong input types have been given to the function."
     error = InputTypeError(func_name)
     assert str(error) == f"{func_name} encountered an error: {error_message}"
```

### Comparing `TEST_TC-0.1.5/tests/test_prep.py` & `TEST_TC-0.1.6/tests/test_prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import pytest
 from sklearn.utils.estimator_checks import check_estimator
 
-from tc_uc4.datapreparation.prep import PreprocessingClass
+from datapreparation.prep import PreprocessingClass
 
 
 
 test_with_data = [
     ('teleconsulto','prophet','data_richiesta','id_teleconsulto')
 ]
 test_no_data = [
```

### Comparing `TEST_TC-0.1.5/tests/test_prophet_utils.py` & `TEST_TC-0.1.6/tests/test_prophet_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import pytest
 import os
-from tc_uc4.algorithms.prophet_utils import (check_prophet_fit_df, check_prophet_predict_df,
+from algorithms.prophet_utils import (check_prophet_fit_df, check_prophet_predict_df,
                                       check_prophet_predict_df, check_prophet_save,
                                       check_prophet_load, check_split_input, train_val_test_split,
                                       save_model_results, preprocess_prophet_output,
                                       check_preprocess_prophet_input, preprocess_prophet_input,
                                       is_not_convertible_to_int_float, literal_evaluation, generate_values,
                                       grid_values_hyperparameters)
```

### Comparing `TEST_TC-0.1.5/tests/test_resources.py` & `TEST_TC-0.1.6/tests/test_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from typing import Any, Dict
 import pytest
 import logging
 from unittest.mock import patch
 
-from tc_uc4.utility.resources import get_configuration, log_exception
+from utility.resources import get_configuration, log_exception
 
 ### get_configuration ###
 @pytest.fixture
 def mock_config_file(tmpdir):
     config_file = tmpdir.join("proprerties.toml")
     config_file.write("[section]\nkey = 'value'")
     return str(config_file)
```

### Comparing `TEST_TC-0.1.5/tests/test_tele_logger.py` & `TEST_TC-0.1.6/tests/test_tele_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging
 from logging import DEBUG
 from time import localtime, strftime
-from tc_uc4.utility.tele_logger import Logger
+from utility.tele_logger import Logger
 
 def test_logger_initialization():
     logger = Logger()
     assert isinstance(logger.logger, logging.Logger)
     assert isinstance(logger.important_logger, logging.Logger)
     assert logger.name is None
```

