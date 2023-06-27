# Comparing `tmp/crypto-screening-1.2.0.tar.gz` & `tmp/crypto-screening-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.2.0.tar", last modified: Tue Jun 27 09:30:41 2023, max compression
+gzip compressed data, was "crypto-screening-1.2.1.tar", last modified: Tue Jun 27 09:38:04 2023, max compression
```

## Comparing `crypto-screening-1.2.0.tar` & `crypto-screening-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:30:41.378118 crypto-screening-1.2.0/
--rw-rw-rw-   0        0        0       98 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-27 09:30:41.378118 crypto-screening-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.2.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.2.0/build.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:30:41.354584 crypto-screening-1.2.0/crypto_screening/
--rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.2.0/crypto_screening/base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:30:41.377117 crypto-screening-1.2.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    14550 2023-06-27 09:23:43.000000 crypto-screening-1.2.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     3355 2023-06-27 09:25:09.000000 crypto-screening-1.2.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0     7755 2023-06-27 09:28:30.000000 crypto-screening-1.2.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    15005 2023-06-27 09:25:09.000000 crypto-screening-1.2.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12447 2023-06-25 20:15:20.000000 crypto-screening-1.2.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      860 2023-06-25 14:10:00.000000 crypto-screening-1.2.0/crypto_screening/document.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.2.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.2.0/crypto_screening/hints.py
--rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.2.0/crypto_screening/interval.py
--rw-rw-rw-   0        0        0    32476 2023-06-25 20:34:03.000000 crypto-screening-1.2.0/crypto_screening/ohlcv.py
--rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.2.0/crypto_screening/orderbook.py
--rw-rw-rw-   0        0        0     2384 2023-06-27 08:28:20.000000 crypto-screening-1.2.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0    31848 2023-06-27 09:29:28.000000 crypto-screening-1.2.0/crypto_screening/screener.py
--rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.2.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.2.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:30:41.374117 crypto-screening-1.2.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-27 09:30:41.000000 crypto-screening-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-06-27 07:30:41.000000 crypto-screening-1.2.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 09:30:41.378118 crypto-screening-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-27 09:30:33.000000 crypto-screening-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:38:04.042430 crypto-screening-1.2.1/
+-rw-rw-rw-   0        0        0       98 2023-06-27 09:38:03.000000 crypto-screening-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-27 09:38:04.042430 crypto-screening-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.2.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.2.1/build.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:38:04.028429 crypto-screening-1.2.1/crypto_screening/
+-rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.2.1/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:38:04.041430 crypto-screening-1.2.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    14549 2023-06-27 09:37:49.000000 crypto-screening-1.2.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     3360 2023-06-27 09:37:44.000000 crypto-screening-1.2.1/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0     7755 2023-06-27 09:28:30.000000 crypto-screening-1.2.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    17057 2023-06-27 09:37:39.000000 crypto-screening-1.2.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12447 2023-06-25 20:15:20.000000 crypto-screening-1.2.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      860 2023-06-25 14:10:00.000000 crypto-screening-1.2.1/crypto_screening/document.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.2.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.2.1/crypto_screening/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.2.1/crypto_screening/interval.py
+-rw-rw-rw-   0        0        0    32476 2023-06-25 20:34:03.000000 crypto-screening-1.2.1/crypto_screening/ohlcv.py
+-rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.2.1/crypto_screening/orderbook.py
+-rw-rw-rw-   0        0        0     2384 2023-06-27 08:28:20.000000 crypto-screening-1.2.1/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    31848 2023-06-27 09:29:28.000000 crypto-screening-1.2.1/crypto_screening/screener.py
+-rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.2.1/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.2.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:38:04.038431 crypto-screening-1.2.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-27 09:38:03.000000 crypto-screening-1.2.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-06-27 09:38:03.000000 crypto-screening-1.2.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:38:03.000000 crypto-screening-1.2.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-27 09:38:03.000000 crypto-screening-1.2.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-27 09:38:03.000000 crypto-screening-1.2.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-27 09:38:03.000000 crypto-screening-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-06-27 07:30:41.000000 crypto-screening-1.2.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:38:04.042430 crypto-screening-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-27 09:37:59.000000 crypto-screening-1.2.1/setup.py
```

### Comparing `crypto-screening-1.2.0/PKG-INFO` & `crypto-screening-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.2.0
+Version: 1.2.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.2.0/README.md` & `crypto-screening-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/build.py` & `crypto-screening-1.2.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/base.py` & `crypto-screening-1.2.1/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/collect/assets.py` & `crypto-screening-1.2.1/crypto_screening/collect/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# collect.py
+# assets.py
 
 from typing import Optional, Dict, Iterable, List, Union
 
 from crypto_screening.process import collect_mutual_string_values
 from crypto_screening.symbols import symbol_to_parts
 from crypto_screening.collect.exchanges import exchanges_data
 from crypto_screening.collect.symbols import (
```

### Comparing `crypto-screening-1.2.0/crypto_screening/collect/exchanges.py` & `crypto-screening-1.2.1/crypto_screening/collect/exchanges.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# data.py
+# exchanges.py
 
 from typing import (
     Optional, Dict, Iterable,
     Callable, Union, Any
 )
 
 from multithreading import Caller, multi_threaded_call
```

### Comparing `crypto-screening-1.2.0/crypto_screening/collect/screeners.py` & `crypto-screening-1.2.1/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/collect/symbols.py` & `crypto-screening-1.2.1/crypto_screening/collect/symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# collect.py
+# symbols.py
 
 from typing import (
     Optional, Dict, Iterable,
     List, Union, Tuple
 )
 
 from represent import BaseModel
@@ -25,15 +25,17 @@
     "include_symbols",
     "exclude_symbols",
     "exchange_symbols",
     "all_exchange_symbols",
     "matching_symbol_pair",
     "matching_symbol_pairs",
     "MarketSymbolSignature",
-    "matching_symbol_signatures"
+    "matching_symbol_signatures",
+    "include_exchanges_symbols",
+    "exclude_exchanges_symbols"
 ]
 
 def include_symbols(
         symbols: Iterable[str],
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         bases: Optional[Iterable[str]] = None,
@@ -148,14 +150,78 @@
 
         saved.append(symbol)
     # end for
 
     return saved
 # end exclude_symbols
 
+def include_exchanges_symbols(
+        data: Dict[str, Iterable[str]],
+        bases: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None,
+        included: Optional[Iterable[str]] = None
+) -> Dict[str, List[str]]:
+    """
+    Removes all symbols with not matching base or quote.
+
+    :param data: The data to filter.
+    :param bases: The bases to include.
+    :param quotes: The quotes to include.
+    :param included: The symbols to include.
+
+    :return: The filtered symbols.
+    """
+
+    if all(value is None for value in (bases, quotes, included)):
+        return {exchange: list(symbols) for exchange, symbols in data.items()}
+    # end if
+
+    return {
+        exchange: saved for exchange, symbols in data.items()
+        if (
+            saved := include_symbols(
+                symbols=symbols, bases=bases,
+                quotes=quotes, included=included
+            )
+        )
+    }
+# end include_exchanges_symbols
+
+def exclude_exchanges_symbols(
+        data: Dict[str, Iterable[str]],
+        bases: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None,
+        excluded: Optional[Iterable[str]] = None
+) -> Dict[str, List[str]]:
+    """
+    Removes all symbols with the matching base or quote.
+
+    :param data: The data to filter.
+    :param bases: The bases to exclude.
+    :param quotes: The quotes to exclude.
+    :param excluded: The symbols to exclude.
+
+    :return: The filtered symbols.
+    """
+
+    if all(value is None for value in (bases, quotes, excluded)):
+        return {exchange: list(symbols) for exchange, symbols in data.items()}
+    # end if
+
+    return {
+        exchange: saved for exchange, symbols in data.items()
+        if (
+            saved := exclude_symbols(
+                symbols=symbols, bases=bases,
+                quotes=quotes, excluded=excluded
+            )
+        )
+    }
+# end exclude_exchanges_symbols
+
 def all_exchange_symbols(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         test: Optional[bool] = False
 ) -> Iterable[str]:
     """
```

### Comparing `crypto-screening-1.2.0/crypto_screening/dataset.py` & `crypto-screening-1.2.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/document.py` & `crypto-screening-1.2.1/crypto_screening/document.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/interval.py` & `crypto-screening-1.2.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/ohlcv.py` & `crypto-screening-1.2.1/crypto_screening/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/orderbook.py` & `crypto-screening-1.2.1/crypto_screening/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/process.py` & `crypto-screening-1.2.1/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/screener.py` & `crypto-screening-1.2.1/crypto_screening/screener.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/symbols.py` & `crypto-screening-1.2.1/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening/validate.py` & `crypto-screening-1.2.1/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.2.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.2.0
+Version: 1.2.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.2.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.2.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.0/pyproject.toml` & `crypto-screening-1.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.2.0'
+version = '1.2.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.2.0/setup.py` & `crypto-screening-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.2.0',
+        version='1.2.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

