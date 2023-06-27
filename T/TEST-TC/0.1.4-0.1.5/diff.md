# Comparing `tmp/TEST_TC-0.1.4.tar.gz` & `tmp/TEST_TC-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-0.1.4.tar", last modified: Tue Jun 27 10:10:46 2023, max compression
+gzip compressed data, was "TEST_TC-0.1.5.tar", last modified: Tue Jun 27 11:08:14 2023, max compression
```

## Comparing `TEST_TC-0.1.4.tar` & `TEST_TC-0.1.5.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.967749 TEST_TC-0.1.4/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 10:10:46.966745 TEST_TC-0.1.4/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.4/README.md
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.890746 TEST_TC-0.1.4/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 10:10:46.000000 TEST_TC-0.1.4/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      978 2023-06-27 10:10:46.000000 TEST_TC-0.1.4/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 10:10:46.000000 TEST_TC-0.1.4/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 10:10:46.000000 TEST_TC-0.1.4/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 10:10:46.000000 TEST_TC-0.1.4/TEST_TC.egg-info/top_level.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1125 2023-06-27 10:02:38.000000 TEST_TC-0.1.4/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 10:10:46.967749 TEST_TC-0.1.4/setup.cfg
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       84 2023-06-24 15:58:09.000000 TEST_TC-0.1.4/setup.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.892743 TEST_TC-0.1.4/tc_uc4/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 10:09:55.000000 TEST_TC-0.1.4/tc_uc4/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.901258 TEST_TC-0.1.4/tc_uc4/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.4/tc_uc4/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5803 2023-06-27 10:09:26.000000 TEST_TC-0.1.4/tc_uc4/algorithms/algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15589 2023-06-27 10:09:32.000000 TEST_TC-0.1.4/tc_uc4/algorithms/prophet_utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.906675 TEST_TC-0.1.4/tc_uc4/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.4/tc_uc4/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2830 2023-06-27 10:09:38.000000 TEST_TC-0.1.4/tc_uc4/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.913458 TEST_TC-0.1.4/tc_uc4/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.4/tc_uc4/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7535 2023-06-27 10:09:04.000000 TEST_TC-0.1.4/tc_uc4/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.922282 TEST_TC-0.1.4/tc_uc4/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.4/tc_uc4/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17975 2023-06-27 10:09:13.000000 TEST_TC-0.1.4/tc_uc4/datapreparation/datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3126 2023-06-27 10:09:18.000000 TEST_TC-0.1.4/tc_uc4/datapreparation/prep.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.924195 TEST_TC-0.1.4/tc_uc4/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.4/tc_uc4/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.927044 TEST_TC-0.1.4/tc_uc4/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.4/tc_uc4/datavisualization/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.939112 TEST_TC-0.1.4/tc_uc4/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.4/tc_uc4/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.4/tc_uc4/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2222 2023-06-26 14:08:09.000000 TEST_TC-0.1.4/tc_uc4/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6174 2023-06-13 16:27:38.000000 TEST_TC-0.1.4/tc_uc4/utility/tele_logger.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:10:46.963744 TEST_TC-0.1.4/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      200 2023-06-26 17:37:24.000000 TEST_TC-0.1.4/tests/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2469 2023-06-26 13:54:38.000000 TEST_TC-0.1.4/tests/test_algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2748 2023-06-26 18:05:01.000000 TEST_TC-0.1.4/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15247 2023-06-27 09:06:09.000000 TEST_TC-0.1.4/tests/test_datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1850 2023-06-26 09:19:22.000000 TEST_TC-0.1.4/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1237 2023-06-24 11:28:22.000000 TEST_TC-0.1.4/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2866 2023-06-26 17:45:00.000000 TEST_TC-0.1.4/tests/test_prep.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16902 2023-06-27 09:06:09.000000 TEST_TC-0.1.4/tests/test_prophet_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2096 2023-06-23 19:40:15.000000 TEST_TC-0.1.4/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2898 2023-06-23 19:40:15.000000 TEST_TC-0.1.4/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.498220 TEST_TC-0.1.5/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 11:08:14.497206 TEST_TC-0.1.5/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/README.md
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.424541 TEST_TC-0.1.5/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 11:08:14.000000 TEST_TC-0.1.5/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      969 2023-06-27 11:08:14.000000 TEST_TC-0.1.5/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 11:08:14.000000 TEST_TC-0.1.5/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 11:08:14.000000 TEST_TC-0.1.5/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 11:08:14.000000 TEST_TC-0.1.5/TEST_TC.egg-info/top_level.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1126 2023-06-27 11:08:07.000000 TEST_TC-0.1.5/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 11:08:14.499207 TEST_TC-0.1.5/setup.cfg
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.426263 TEST_TC-0.1.5/tc_uc4/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 11:06:09.000000 TEST_TC-0.1.5/tc_uc4/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.431845 TEST_TC-0.1.5/tc_uc4/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5830 2023-06-27 10:40:34.000000 TEST_TC-0.1.5/tc_uc4/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15599 2023-06-27 10:41:03.000000 TEST_TC-0.1.5/tc_uc4/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.436822 TEST_TC-0.1.5/tc_uc4/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2830 2023-06-27 10:14:15.000000 TEST_TC-0.1.5/tc_uc4/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.440820 TEST_TC-0.1.5/tc_uc4/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7550 2023-06-27 10:39:52.000000 TEST_TC-0.1.5/tc_uc4/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.448591 TEST_TC-0.1.5/tc_uc4/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17985 2023-06-27 10:39:31.000000 TEST_TC-0.1.5/tc_uc4/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3141 2023-06-27 10:39:30.000000 TEST_TC-0.1.5/tc_uc4/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.451357 TEST_TC-0.1.5/tc_uc4/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.454435 TEST_TC-0.1.5/tc_uc4/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/datavisualization/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.466286 TEST_TC-0.1.5/tc_uc4/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.5/tc_uc4/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.5/tc_uc4/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2222 2023-06-26 14:08:09.000000 TEST_TC-0.1.5/tc_uc4/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6174 2023-06-13 16:27:38.000000 TEST_TC-0.1.5/tc_uc4/utility/tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 11:08:14.493208 TEST_TC-0.1.5/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:42:45.000000 TEST_TC-0.1.5/tests/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2476 2023-06-27 10:41:26.000000 TEST_TC-0.1.5/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2762 2023-06-27 10:41:39.000000 TEST_TC-0.1.5/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15261 2023-06-27 10:41:47.000000 TEST_TC-0.1.5/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1864 2023-06-27 10:42:00.000000 TEST_TC-0.1.5/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1244 2023-06-27 10:42:03.000000 TEST_TC-0.1.5/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2873 2023-06-27 10:42:07.000000 TEST_TC-0.1.5/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16909 2023-06-27 10:42:13.000000 TEST_TC-0.1.5/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2103 2023-06-27 10:42:17.000000 TEST_TC-0.1.5/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2905 2023-06-27 10:42:20.000000 TEST_TC-0.1.5/tests/test_tele_logger.py
```

### Comparing `TEST_TC-0.1.4/README.md` & `TEST_TC-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.4/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-0.1.5/TEST_TC.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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

### Comparing `TEST_TC-0.1.4/pyproject.toml` & `TEST_TC-0.1.5/pyproject.toml`

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

### Comparing `TEST_TC-0.1.4/tc_uc4/algorithms/algorithm.py` & `TEST_TC-0.1.5/tc_uc4/algorithms/algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import pickle
 
 from prophet import Prophet
 from typing_extensions import Self
-from .prophet_utils import check_prophet_fit_df, check_prophet_predict_df, check_prophet_save, check_prophet_load
+from tc_uc4.algorithms.prophet_utils import check_prophet_fit_df, check_prophet_predict_df, check_prophet_save, check_prophet_load
 
-from ..utility.tele_logger import logger
-from ..utility.resources import log_exception
+from tc_uc4.utility.tele_logger import logger
+from tc_uc4.utility.resources import log_exception
 import itertools
 from sklearn.metrics import mean_squared_error, mean_absolute_error
 import numpy as np
 
 class Prophet_model:
     def __init__(self, dic_param: dict = {
                   "changepoint_prior_scale": 0.5,
```

### Comparing `TEST_TC-0.1.4/tc_uc4/algorithms/prophet_utils.py` & `TEST_TC-0.1.5/tc_uc4/algorithms/prophet_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import numpy as np
 import os
 import ast
 
-from ..datahandler.datahandler import DataHandler
-from ..utility.tele_logger import logger
+from tc_uc4.datahandler.datahandler import DataHandler
+from tc_uc4.utility.tele_logger import logger
 
 def check_prophet_fit_df(input_data):
     """
     Esegue i controlli sull'input fornito per il metodo fit() di Prophet.
 
     Parameters
     ----------
```

### Comparing `TEST_TC-0.1.4/tc_uc4/analytics/evaluationMetrics.py` & `TEST_TC-0.1.5/tc_uc4/analytics/evaluationMetrics.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.4/tc_uc4/datahandler/datahandler.py` & `TEST_TC-0.1.5/tc_uc4/datahandler/datahandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
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
     def __init__(self, data_folder : str = None) -> Self:
         """Class which will handle the read and write of .parquet data
 
         Parameters
         ----------
```

### Comparing `TEST_TC-0.1.4/tc_uc4/datapreparation/datapreparation_utils.py` & `TEST_TC-0.1.5/tc_uc4/datapreparation/datapreparation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
-from ..utility.tele_logger import logger
-from ..utility.exceptions import InputTypeError
+from tc_uc4.utility.tele_logger import logger
+from tc_uc4.utility.exceptions import InputTypeError
 from statsmodels.tsa.seasonal import seasonal_decompose
 from sklearn.base import BaseEstimator, TransformerMixin
 from typing_extensions import Self
 from typing import Union, Dict, List
 
 class PreprocessingTeleconsulto:
```

### Comparing `TEST_TC-0.1.4/tc_uc4/datapreparation/prep.py` & `TEST_TC-0.1.5/tc_uc4/datapreparation/prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sklearn.base import BaseEstimator, TransformerMixin
 from typing_extensions import Self, Any
 import pandas as pd
-from ..utility.tele_logger import logger
-from ..utility.resources import *
-from ..datapreparation.datapreparation_utils import PreprocessingTeleconsulto
+from tc_uc4.utility.tele_logger import logger
+from tc_uc4.utility.resources import *
+from tc_uc4.datapreparation.datapreparation_utils import PreprocessingTeleconsulto
 import pickle
 
 class PreprocessingClass(BaseEstimator, TransformerMixin):
 
     def __init__(self,
                  usecase: str = "teleconsulto",
                  model: str = "prophet",
```

### Comparing `TEST_TC-0.1.4/tc_uc4/utility/exceptions.py` & `TEST_TC-0.1.5/tc_uc4/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.4/tc_uc4/utility/resources.py` & `TEST_TC-0.1.5/tc_uc4/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.4/tc_uc4/utility/tele_logger.py` & `TEST_TC-0.1.5/tc_uc4/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.4/tests/test_algorithm.py` & `TEST_TC-0.1.5/tests/test_algorithm.py`

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

### Comparing `TEST_TC-0.1.4/tests/test_datahandler.py` & `TEST_TC-0.1.5/tests/test_datahandler.py`

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

### Comparing `TEST_TC-0.1.4/tests/test_datapreparation_utils.py` & `TEST_TC-0.1.5/tests/test_datapreparation_utils.py`

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

### Comparing `TEST_TC-0.1.4/tests/test_evaluations.py` & `TEST_TC-0.1.5/tests/test_evaluations.py`

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

### Comparing `TEST_TC-0.1.4/tests/test_exceptions.py` & `TEST_TC-0.1.5/tests/test_exceptions.py`

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

### Comparing `TEST_TC-0.1.4/tests/test_prep.py` & `TEST_TC-0.1.5/tests/test_prep.py`

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

### Comparing `TEST_TC-0.1.4/tests/test_prophet_utils.py` & `TEST_TC-0.1.5/tests/test_prophet_utils.py`

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

### Comparing `TEST_TC-0.1.4/tests/test_resources.py` & `TEST_TC-0.1.5/tests/test_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
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
```

### Comparing `TEST_TC-0.1.4/tests/test_tele_logger.py` & `TEST_TC-0.1.5/tests/test_tele_logger.py`

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

