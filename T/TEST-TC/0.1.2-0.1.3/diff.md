# Comparing `tmp/TEST_TC-0.1.2.tar.gz` & `tmp/TEST_TC-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEST_TC-0.1.2.tar", last modified: Tue Jun 27 09:56:12 2023, max compression
+gzip compressed data, was "TEST_TC-0.1.3.tar", last modified: Tue Jun 27 10:06:40 2023, max compression
```

## Comparing `TEST_TC-0.1.2.tar` & `TEST_TC-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.703727 TEST_TC-0.1.2/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 09:56:12.702725 TEST_TC-0.1.2/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/README.md
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.635802 TEST_TC-0.1.2/TEST_TC.egg-info/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 09:56:12.000000 TEST_TC-0.1.2/TEST_TC.egg-info/PKG-INFO
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      978 2023-06-27 09:56:12.000000 TEST_TC-0.1.2/TEST_TC.egg-info/SOURCES.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 09:56:12.000000 TEST_TC-0.1.2/TEST_TC.egg-info/dependency_links.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 09:56:12.000000 TEST_TC-0.1.2/TEST_TC.egg-info/requires.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 09:56:12.000000 TEST_TC-0.1.2/TEST_TC.egg-info/top_level.txt
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1125 2023-06-27 09:48:36.000000 TEST_TC-0.1.2/pyproject.toml
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 09:56:12.704725 TEST_TC-0.1.2/setup.cfg
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       84 2023-06-24 15:58:09.000000 TEST_TC-0.1.2/setup.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.638873 TEST_TC-0.1.2/tc_uc4/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 09:56:03.000000 TEST_TC-0.1.2/tc_uc4/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.644615 TEST_TC-0.1.2/tc_uc4/algorithms/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/algorithms/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5799 2023-06-26 14:08:09.000000 TEST_TC-0.1.2/tc_uc4/algorithms/algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15585 2023-06-27 09:06:09.000000 TEST_TC-0.1.2/tc_uc4/algorithms/prophet_utils.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.649121 TEST_TC-0.1.2/tc_uc4/analytics/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/analytics/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2826 2023-06-26 09:19:22.000000 TEST_TC-0.1.2/tc_uc4/analytics/evaluationMetrics.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.653554 TEST_TC-0.1.2/tc_uc4/datahandler/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/datahandler/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7529 2023-06-26 12:58:12.000000 TEST_TC-0.1.2/tc_uc4/datahandler/datahandler.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.660557 TEST_TC-0.1.2/tc_uc4/datapreparation/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/datapreparation/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17971 2023-06-26 17:37:41.000000 TEST_TC-0.1.2/tc_uc4/datapreparation/datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3120 2023-06-26 17:37:02.000000 TEST_TC-0.1.2/tc_uc4/datapreparation/prep.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.663088 TEST_TC-0.1.2/tc_uc4/dataset/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/dataset/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.665010 TEST_TC-0.1.2/tc_uc4/datavisualization/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/datavisualization/__init__.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.675214 TEST_TC-0.1.2/tc_uc4/utility/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.2/tc_uc4/utility/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.2/tc_uc4/utility/exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2222 2023-06-26 14:08:09.000000 TEST_TC-0.1.2/tc_uc4/utility/resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6174 2023-06-13 16:27:38.000000 TEST_TC-0.1.2/tc_uc4/utility/tele_logger.py
-drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 09:56:12.699725 TEST_TC-0.1.2/tests/
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)      200 2023-06-26 17:37:24.000000 TEST_TC-0.1.2/tests/__init__.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2469 2023-06-26 13:54:38.000000 TEST_TC-0.1.2/tests/test_algorithm.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2748 2023-06-26 18:05:01.000000 TEST_TC-0.1.2/tests/test_datahandler.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15247 2023-06-27 09:06:09.000000 TEST_TC-0.1.2/tests/test_datapreparation_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1850 2023-06-26 09:19:22.000000 TEST_TC-0.1.2/tests/test_evaluations.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1237 2023-06-24 11:28:22.000000 TEST_TC-0.1.2/tests/test_exceptions.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2866 2023-06-26 17:45:00.000000 TEST_TC-0.1.2/tests/test_prep.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16902 2023-06-27 09:06:09.000000 TEST_TC-0.1.2/tests/test_prophet_utils.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2096 2023-06-23 19:40:15.000000 TEST_TC-0.1.2/tests/test_resources.py
--rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2898 2023-06-23 19:40:15.000000 TEST_TC-0.1.2/tests/test_tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.174518 TEST_TC-0.1.3/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 10:06:40.172827 TEST_TC-0.1.3/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2974 2023-06-09 08:18:00.000000 TEST_TC-0.1.3/README.md
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.114323 TEST_TC-0.1.3/TEST_TC.egg-info/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      455 2023-06-27 10:06:40.000000 TEST_TC-0.1.3/TEST_TC.egg-info/PKG-INFO
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      978 2023-06-27 10:06:40.000000 TEST_TC-0.1.3/TEST_TC.egg-info/SOURCES.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-27 10:06:40.000000 TEST_TC-0.1.3/TEST_TC.egg-info/dependency_links.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      203 2023-06-27 10:06:40.000000 TEST_TC-0.1.3/TEST_TC.egg-info/requires.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       13 2023-06-27 10:06:40.000000 TEST_TC-0.1.3/TEST_TC.egg-info/top_level.txt
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1125 2023-06-27 10:02:38.000000 TEST_TC-0.1.3/pyproject.toml
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       38 2023-06-27 10:06:40.174833 TEST_TC-0.1.3/setup.cfg
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       84 2023-06-24 15:58:09.000000 TEST_TC-0.1.3/setup.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.115582 TEST_TC-0.1.3/tc_uc4/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)       23 2023-06-27 10:06:30.000000 TEST_TC-0.1.3/tc_uc4/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.120899 TEST_TC-0.1.3/tc_uc4/algorithms/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.3/tc_uc4/algorithms/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     5801 2023-06-27 10:04:56.000000 TEST_TC-0.1.3/tc_uc4/algorithms/algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15587 2023-06-27 10:04:55.000000 TEST_TC-0.1.3/tc_uc4/algorithms/prophet_utils.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.127420 TEST_TC-0.1.3/tc_uc4/analytics/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.3/tc_uc4/analytics/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2828 2023-06-27 10:05:11.000000 TEST_TC-0.1.3/tc_uc4/analytics/evaluationMetrics.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.131422 TEST_TC-0.1.3/tc_uc4/datahandler/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.3/tc_uc4/datahandler/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     7532 2023-06-27 10:03:46.000000 TEST_TC-0.1.3/tc_uc4/datahandler/datahandler.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.136875 TEST_TC-0.1.3/tc_uc4/datapreparation/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.3/tc_uc4/datapreparation/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    17973 2023-06-27 10:05:23.000000 TEST_TC-0.1.3/tc_uc4/datapreparation/datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     3123 2023-06-27 10:05:34.000000 TEST_TC-0.1.3/tc_uc4/datapreparation/prep.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.139877 TEST_TC-0.1.3/tc_uc4/dataset/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.3/tc_uc4/dataset/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.142088 TEST_TC-0.1.3/tc_uc4/datavisualization/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.3/tc_uc4/datavisualization/__init__.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.151061 TEST_TC-0.1.3/tc_uc4/utility/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)        1 2023-06-09 08:18:00.000000 TEST_TC-0.1.3/tc_uc4/utility/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1352 2023-06-24 11:28:22.000000 TEST_TC-0.1.3/tc_uc4/utility/exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2222 2023-06-26 14:08:09.000000 TEST_TC-0.1.3/tc_uc4/utility/resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     6174 2023-06-13 16:27:38.000000 TEST_TC-0.1.3/tc_uc4/utility/tele_logger.py
+drwxrwxrwx   0 flavio    (1000) flavio    (1000)        0 2023-06-27 10:06:40.170827 TEST_TC-0.1.3/tests/
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)      200 2023-06-26 17:37:24.000000 TEST_TC-0.1.3/tests/__init__.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2469 2023-06-26 13:54:38.000000 TEST_TC-0.1.3/tests/test_algorithm.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2748 2023-06-26 18:05:01.000000 TEST_TC-0.1.3/tests/test_datahandler.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    15247 2023-06-27 09:06:09.000000 TEST_TC-0.1.3/tests/test_datapreparation_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1850 2023-06-26 09:19:22.000000 TEST_TC-0.1.3/tests/test_evaluations.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     1237 2023-06-24 11:28:22.000000 TEST_TC-0.1.3/tests/test_exceptions.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2866 2023-06-26 17:45:00.000000 TEST_TC-0.1.3/tests/test_prep.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)    16902 2023-06-27 09:06:09.000000 TEST_TC-0.1.3/tests/test_prophet_utils.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2096 2023-06-23 19:40:15.000000 TEST_TC-0.1.3/tests/test_resources.py
+-rwxrwxrwx   0 flavio    (1000) flavio    (1000)     2898 2023-06-23 19:40:15.000000 TEST_TC-0.1.3/tests/test_tele_logger.py
```

### Comparing `TEST_TC-0.1.2/README.md` & `TEST_TC-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/TEST_TC.egg-info/SOURCES.txt` & `TEST_TC-0.1.3/TEST_TC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/pyproject.toml` & `TEST_TC-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tc_uc4/algorithms/algorithm.py` & `TEST_TC-0.1.3/tc_uc4/algorithms/algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import pickle
 
 from prophet import Prophet
 from typing_extensions import Self
 from .prophet_utils import check_prophet_fit_df, check_prophet_predict_df, check_prophet_save, check_prophet_load
 
-from utility.tele_logger import logger
-from utility.resources import log_exception
+from .utility.tele_logger import logger
+from .utility.resources import log_exception
 import itertools
 from sklearn.metrics import mean_squared_error, mean_absolute_error
 import numpy as np
 
 class Prophet_model:
     def __init__(self, dic_param: dict = {
                   "changepoint_prior_scale": 0.5,
```

### Comparing `TEST_TC-0.1.2/tc_uc4/algorithms/prophet_utils.py` & `TEST_TC-0.1.3/tc_uc4/algorithms/prophet_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import numpy as np
 import os
 import ast
 
-from datahandler.datahandler import DataHandler
-from utility.tele_logger import logger
+from .datahandler.datahandler import DataHandler
+from .utility.tele_logger import logger
 
 def check_prophet_fit_df(input_data):
     """
     Esegue i controlli sull'input fornito per il metodo fit() di Prophet.
 
     Parameters
     ----------
```

### Comparing `TEST_TC-0.1.2/tc_uc4/analytics/evaluationMetrics.py` & `TEST_TC-0.1.3/tc_uc4/analytics/evaluationMetrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import warnings;
 warnings.simplefilter('ignore')
 import pandas as pd
 import numpy as np
 from sklearn.metrics import mean_squared_error , r2_score, mean_absolute_error
-from utility.exceptions import ColumnNotFound
-from utility.tele_logger import logger
+from .utility.exceptions import ColumnNotFound
+from .utility.tele_logger import logger
 
 
 def evaluations(df_real: pd.DataFrame, df_pred: pd.DataFrame, date: str = 'Timestamp' , y_true: str = 'Target', y_pred: str = 'Pred_mean') -> pd.DataFrame:
     """
     Create a DataFrame representing the evaluation metrics
 
     Parameters
```

### Comparing `TEST_TC-0.1.2/tc_uc4/datahandler/datahandler.py` & `TEST_TC-0.1.3/tc_uc4/datahandler/datahandler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from typing import Any
 
 import geopandas as gpd
 import pandas as pd
 from typing_extensions import Self
-from utility.exceptions import InputTypeError
-from utility.resources import log_exception
-from utility.tele_logger import logger
+from .utility.exceptions import InputTypeError
+from .utility.resources import log_exception
+from .utility.tele_logger import logger
 
 class DataHandler:
     def __init__(self, data_folder : str = None) -> Self:
         """Class which will handle the read and write of .parquet data
 
         Parameters
         ----------
```

### Comparing `TEST_TC-0.1.2/tc_uc4/datapreparation/datapreparation_utils.py` & `TEST_TC-0.1.3/tc_uc4/datapreparation/datapreparation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
-from utility.tele_logger import logger
-from utility.exceptions import InputTypeError
+from .utility.tele_logger import logger
+from .utility.exceptions import InputTypeError
 from statsmodels.tsa.seasonal import seasonal_decompose
 from sklearn.base import BaseEstimator, TransformerMixin
 from typing_extensions import Self
 from typing import Union, Dict, List
 
 class PreprocessingTeleconsulto:
```

### Comparing `TEST_TC-0.1.2/tc_uc4/datapreparation/prep.py` & `TEST_TC-0.1.3/tc_uc4/datapreparation/prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sklearn.base import BaseEstimator, TransformerMixin
 from typing_extensions import Self, Any
 import pandas as pd
-from utility.tele_logger import logger
-from utility.resources import *
-from datapreparation.datapreparation_utils import PreprocessingTeleconsulto
+from .utility.tele_logger import logger
+from .utility.resources import *
+from .datapreparation.datapreparation_utils import PreprocessingTeleconsulto
 import pickle
 
 class PreprocessingClass(BaseEstimator, TransformerMixin):
 
     def __init__(self,
                  usecase: str = "teleconsulto",
                  model: str = "prophet",
```

### Comparing `TEST_TC-0.1.2/tc_uc4/utility/exceptions.py` & `TEST_TC-0.1.3/tc_uc4/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tc_uc4/utility/resources.py` & `TEST_TC-0.1.3/tc_uc4/utility/resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tc_uc4/utility/tele_logger.py` & `TEST_TC-0.1.3/tc_uc4/utility/tele_logger.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tests/test_algorithm.py` & `TEST_TC-0.1.3/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tests/test_datahandler.py` & `TEST_TC-0.1.3/tests/test_datahandler.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tests/test_datapreparation_utils.py` & `TEST_TC-0.1.3/tests/test_datapreparation_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tests/test_evaluations.py` & `TEST_TC-0.1.3/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tests/test_exceptions.py` & `TEST_TC-0.1.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tests/test_prep.py` & `TEST_TC-0.1.3/tests/test_prep.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tests/test_prophet_utils.py` & `TEST_TC-0.1.3/tests/test_prophet_utils.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tests/test_resources.py` & `TEST_TC-0.1.3/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `TEST_TC-0.1.2/tests/test_tele_logger.py` & `TEST_TC-0.1.3/tests/test_tele_logger.py`

 * *Files identical despite different names*

