# Comparing `tmp/crypto-screening-1.1.0.tar.gz` & `tmp/crypto-screening-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.1.0.tar", last modified: Sun Jun 25 21:03:34 2023, max compression
+gzip compressed data, was "crypto-screening-1.2.0.tar", last modified: Tue Jun 27 09:30:41 2023, max compression
```

## Comparing `crypto-screening-1.1.0.tar` & `crypto-screening-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 21:03:34.778503 crypto-screening-1.1.0/
--rw-rw-rw-   0        0        0       98 2023-06-25 21:03:34.000000 crypto-screening-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-25 21:03:34.778503 crypto-screening-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.1.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.1.0/build.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:03:34.762505 crypto-screening-1.1.0/crypto_screening/
--rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.1.0/crypto_screening/base.py
--rw-rw-rw-   0        0        0    28635 2023-06-25 20:53:52.000000 crypto-screening-1.1.0/crypto_screening/collect.py
--rw-rw-rw-   0        0        0    12447 2023-06-25 20:15:20.000000 crypto-screening-1.1.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      860 2023-06-25 14:10:00.000000 crypto-screening-1.1.0/crypto_screening/document.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.1.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.1.0/crypto_screening/hints.py
--rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.1.0/crypto_screening/interval.py
--rw-rw-rw-   0        0        0    32476 2023-06-25 20:34:03.000000 crypto-screening-1.1.0/crypto_screening/ohlcv.py
--rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.1.0/crypto_screening/orderbook.py
--rw-rw-rw-   0        0        0     2392 2023-06-25 15:15:52.000000 crypto-screening-1.1.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0    36839 2023-06-25 21:01:22.000000 crypto-screening-1.1.0/crypto_screening/screener.py
--rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.1.0/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:03:34.777504 crypto-screening-1.1.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-25 21:03:34.000000 crypto-screening-1.1.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-06-25 21:03:34.000000 crypto-screening-1.1.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 21:03:34.000000 crypto-screening-1.1.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-06-25 21:03:34.000000 crypto-screening-1.1.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-25 21:03:34.000000 crypto-screening-1.1.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-25 21:03:34.000000 crypto-screening-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       73 2023-06-23 16:55:08.000000 crypto-screening-1.1.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 21:03:34.779504 crypto-screening-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-25 21:03:24.000000 crypto-screening-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:30:41.378118 crypto-screening-1.2.0/
+-rw-rw-rw-   0        0        0       98 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-27 09:30:41.378118 crypto-screening-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.2.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.2.0/build.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:30:41.354584 crypto-screening-1.2.0/crypto_screening/
+-rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.2.0/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:30:41.377117 crypto-screening-1.2.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    14550 2023-06-27 09:23:43.000000 crypto-screening-1.2.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     3355 2023-06-27 09:25:09.000000 crypto-screening-1.2.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0     7755 2023-06-27 09:28:30.000000 crypto-screening-1.2.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    15005 2023-06-27 09:25:09.000000 crypto-screening-1.2.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12447 2023-06-25 20:15:20.000000 crypto-screening-1.2.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      860 2023-06-25 14:10:00.000000 crypto-screening-1.2.0/crypto_screening/document.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.2.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.2.0/crypto_screening/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.2.0/crypto_screening/interval.py
+-rw-rw-rw-   0        0        0    32476 2023-06-25 20:34:03.000000 crypto-screening-1.2.0/crypto_screening/ohlcv.py
+-rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.2.0/crypto_screening/orderbook.py
+-rw-rw-rw-   0        0        0     2384 2023-06-27 08:28:20.000000 crypto-screening-1.2.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    31848 2023-06-27 09:29:28.000000 crypto-screening-1.2.0/crypto_screening/screener.py
+-rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.2.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.2.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:30:41.374117 crypto-screening-1.2.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-06-27 07:30:41.000000 crypto-screening-1.2.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:30:41.378118 crypto-screening-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-27 09:30:33.000000 crypto-screening-1.2.0/setup.py
```

### Comparing `crypto-screening-1.1.0/PKG-INFO` & `crypto-screening-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.1.0
+Version: 1.2.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.1.0/README.md` & `crypto-screening-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.1.0/build.py` & `crypto-screening-1.2.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.1.0/crypto_screening/base.py` & `crypto-screening-1.2.0/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.1.0/crypto_screening/dataset.py` & `crypto-screening-1.2.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.1.0/crypto_screening/document.py` & `crypto-screening-1.2.0/crypto_screening/document.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.1.0/crypto_screening/interval.py` & `crypto-screening-1.2.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.1.0/crypto_screening/ohlcv.py` & `crypto-screening-1.2.0/crypto_screening/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.1.0/crypto_screening/orderbook.py` & `crypto-screening-1.2.0/crypto_screening/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.1.0/crypto_screening/process.py` & `crypto-screening-1.2.0/crypto_screening/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,8 +93,8 @@
 
     return {
         key: [
             value for value in data[key]
             if minimum <= values.get(value, 0) <= maximum
         ] for key in data
     }
-# end collect_mutual_assets
+# end mutual_assets
```

### Comparing `crypto-screening-1.1.0/crypto_screening/screener.py` & `crypto-screening-1.2.0/crypto_screening/screener.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,54 +2,47 @@
 
 import warnings
 import datetime as dt
 import time
 from abc import ABCMeta
 import threading
 from typing import (
-    Optional, Union, Dict, Iterable, Any, List, Tuple
+    Optional, Union, Dict, Iterable, Any, List
 )
 
 import pandas as pd
 
 from represent import BaseModel, Modifiers
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.dataset import (
     DATE_TIME, save_dataset, load_dataset
 )
 from crypto_screening.hints import Number
 from crypto_screening.symbols import Separator
 from crypto_screening.process import find_string_value
-from crypto_screening.collect import (
-    validate_exchange, validate_symbol, matching_symbol_pair
+from crypto_screening.validate import (
+    validate_exchange, validate_symbol
 )
 
 __all__ = [
     "BaseScreener",
     "wait_for_update",
     "wait_for_initialization",
     "WaitingState",
     "DataCollector",
-    "collect_screeners",
     "wait_for_dynamic_update",
     "wait_for_dynamic_initialization",
     "BaseMultiScreener",
-    "live_screeners",
     "create_market_dataframe",
-    "structure_screeners",
-    "find_screeners",
     "MarketRecorder",
     "structure_screeners_datasets",
     "structure_screener_datasets",
-    "validate_market",
-    "matching_screener_pairs",
-    "matching_screener_pair",
-    "remove_empty_screeners",
+    "validate_market"
 ]
 
 class WaitingState(BaseModel):
     """A class to represent the waiting state of screener objects."""
 
     modifiers = Modifiers(hidden=["screeners"], properties=["time"])
 
@@ -845,40 +838,14 @@
             )
         # end for
 
         multi_threaded_call(callers=callers)
     # end load_datasets
 # end BaseScreener
 
-def collect_screeners(
-        symbol: str,
-        exchange: str,
-        screeners: Iterable[BaseScreener]
-) -> List[BaseScreener]:
-    """
-    Finds the create_screeners with the given source exchange and symbol.
-
-    :param symbol: The symbol of the screener.
-    :param exchange: The exchange name of the screener.
-    :param screeners: The create_screeners to search in.
-
-    :return: A list of the matching create_screeners.
-    """
-
-    found = []
-
-    for screener in screeners:
-        if (screener.exchange == exchange) and (screener.symbol == symbol):
-            found.append(screener)
-        # end if
-    # end for
-
-    return found
-# end collect_screeners
-
 def wait_for_dynamic_initialization(
         screeners: Iterable[Union[BaseScreener, BaseMultiScreener]],
         delay: Optional[Union[Number, dt.timedelta]] = None,
         once: Optional[bool] = False,
         stop: Optional[Union[bool, int]] = False,
         cancel: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
 ) -> WaitingState:
@@ -1122,60 +1089,14 @@
 
     return wait_for_dynamic_update(
         screeners, delay=delay, once=once,
         stop=stop, cancel=cancel
     )
 # end wait_for_update
 
-def live_screeners(
-        screeners: Iterable[Union[BaseScreener, BaseMultiScreener]]
-) -> List[Union[BaseScreener, BaseMultiScreener]]:
-    """
-    Returns a list of all the live create_screeners.
-
-    :param screeners: The create_screeners to search from.
-
-    :return: A list the live create_screeners.
-    """
-
-    return [
-        screener for screener in screeners
-        if (
-            screener.running and (
-                isinstance(screener, BaseMultiScreener) or
-                len(screener.market) > 0
-            )
-        )
-    ]
-# end live_screeners
-
-def structure_screeners(
-        screeners: Iterable[BaseScreener]
-) -> Dict[str, Dict[str, List[BaseScreener]]]:
-    """
-    Structures the screener objects by exchanges and symbols
-
-    :param screeners: The screeners to structure.
-
-    :return: The structure of the screeners.
-    """
-
-    structure: Dict[str, Dict[str, List[BaseScreener]]] = {}
-
-    for screener in screeners:
-        (
-            structure.
-            setdefault(screener.exchange, {}).
-            setdefault(screener.symbol, [])
-        ).append(screener)
-    # end for
-
-    return structure
-# end structure_screeners
-
 def structure_screeners_datasets(
         screeners: Iterable[BaseScreener]
 ) -> Dict[str, Dict[str, List[pd.DataFrame]]]:
     """
     Structures the screener objects by exchanges and symbols
 
     :param screeners: The screeners to structure.
@@ -1214,106 +1135,8 @@
             structure.
             setdefault(screener.exchange, {}).
             setdefault(screener.symbol, screener.market)
         )
     # end for
 
     return structure
-# end structure_screener_datasets
-
-def find_screeners(
-        screeners: Iterable[BaseScreener], exchange: str, symbol: str
-) -> List[BaseScreener]:
-    """
-    Finds all the screeners with the matching exchange and symbol name.
-
-    :param screeners: The screeners to process.
-    :param exchange: The exchange name for the symbol.
-    :param symbol: The pair symbol to search its screeners.
-
-    :return: The matching screeners.
-    """
-
-    return [
-        screener for screener in screeners
-        if (
-            (screener.symbol.lower() == symbol.lower()) and
-            (exchange.lower() == screener.exchange.lower())
-        )
-    ]
-# end find_screeners
-
-def matching_screener_pair(
-        screener1: BaseScreener,
-        screener2: BaseScreener, /, *,
-        matches: Optional[Iterable[Iterable[str]]] = None,
-        separator: Optional[str] = None
-) -> bool:
-    """
-    Checks if the symbols are valid with the matching currencies.
-
-    :param screener1: The first ticker.
-    :param screener2: The second ticker.
-    :param matches: The currencies.
-    :param separator: The separator of the assets.
-
-    :return: The validation value for the symbols.
-    """
-
-    return (
-        (screener1.exchange != screener2.exchange) and
-        matching_symbol_pair(
-            screener1.symbol, screener2.symbol,
-            matches=matches, separator=separator
-        )
-    )
-# end matching_screener_pair
-
-def matching_screener_pairs(
-        screeners: Iterable[BaseScreener],
-        matches: Optional[Iterable[Iterable[str]]] = None,
-        separator: Optional[str] = None,
-        empty: Optional[bool] = True
-) -> List[Tuple[BaseScreener, BaseScreener]]:
-    """
-    Checks if the screeners are valid with the matching currencies.
-
-    :param screeners: The screeners.
-    :param matches: The currencies.
-    :param separator: The separator of the assets.
-    :param empty: Allows empty screeners.
-
-    :return: The validation value for the symbols.
-    """
-
-    pairs = []
-
-    if not empty:
-        screeners = remove_empty_screeners(screeners=screeners)
-    # end if
-
-    for screener1 in screeners:
-        for screener2 in screeners:
-            if matching_screener_pair(
-                screener1, screener2,
-                matches=matches, separator=separator
-            ):
-                pairs.append((screener1, screener2))
-            # end if
-        # end for
-    # end for
-
-    return pairs
-# end matching_screener_pairs
-
-def remove_empty_screeners(screeners: Iterable[BaseScreener]) -> List[BaseScreener]:
-    """
-    Removes the empty screeners.
-
-    :param screeners: The screeners of the assets and exchanges.
-    """
-
-    return [
-        screener for screener in screeners
-        if len(screener.market) > 0
-    ]
-# end remove_empty_screeners
+# end structure_screener_datasets
```

### Comparing `crypto-screening-1.1.0/crypto_screening/symbols.py` & `crypto-screening-1.2.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.1.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.2.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.1.0
+Version: 1.2.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.1.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.2.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 README.md
 build.py
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.py
 crypto_screening/base.py
-crypto_screening/collect.py
 crypto_screening/dataset.py
 crypto_screening/document.py
 crypto_screening/exchanges.py
 crypto_screening/hints.py
 crypto_screening/interval.py
 crypto_screening/ohlcv.py
 crypto_screening/orderbook.py
 crypto_screening/process.py
 crypto_screening/screener.py
 crypto_screening/symbols.py
+crypto_screening/validate.py
 crypto_screening.egg-info/PKG-INFO
 crypto_screening.egg-info/SOURCES.txt
 crypto_screening.egg-info/dependency_links.txt
 crypto_screening.egg-info/requires.txt
-crypto_screening.egg-info/top_level.txt
+crypto_screening.egg-info/top_level.txt
+crypto_screening/collect/assets.py
+crypto_screening/collect/exchanges.py
+crypto_screening/collect/screeners.py
+crypto_screening/collect/symbols.py
```

### Comparing `crypto-screening-1.1.0/pyproject.toml` & `crypto-screening-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.1.0'
+version = '1.2.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.1.0/setup.py` & `crypto-screening-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.1.0',
+        version='1.2.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

