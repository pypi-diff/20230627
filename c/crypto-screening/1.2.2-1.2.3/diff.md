# Comparing `tmp/crypto-screening-1.2.2.tar.gz` & `tmp/crypto-screening-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.2.2.tar", last modified: Tue Jun 27 10:21:02 2023, max compression
+gzip compressed data, was "crypto-screening-1.2.3.tar", last modified: Tue Jun 27 10:24:24 2023, max compression
```

## Comparing `crypto-screening-1.2.2.tar` & `crypto-screening-1.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 10:21:02.038897 crypto-screening-1.2.2/
--rw-rw-rw-   0        0        0       98 2023-06-27 10:21:01.000000 crypto-screening-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-27 10:21:02.038897 crypto-screening-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.2.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.2.2/build.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:21:02.019894 crypto-screening-1.2.2/crypto_screening/
--rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.2.2/crypto_screening/base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:21:02.037897 crypto-screening-1.2.2/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17295 2023-06-27 10:20:06.000000 crypto-screening-1.2.2/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0      496 2023-06-27 10:17:11.000000 crypto-screening-1.2.2/crypto_screening/collect/document.py
--rw-rw-rw-   0        0        0     4032 2023-06-27 10:16:15.000000 crypto-screening-1.2.2/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0     7755 2023-06-27 09:28:30.000000 crypto-screening-1.2.2/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    17206 2023-06-27 10:02:29.000000 crypto-screening-1.2.2/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12447 2023-06-25 20:15:20.000000 crypto-screening-1.2.2/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      869 2023-06-27 10:20:56.000000 crypto-screening-1.2.2/crypto_screening/document.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.2.2/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.2.2/crypto_screening/hints.py
--rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.2.2/crypto_screening/interval.py
--rw-rw-rw-   0        0        0    32476 2023-06-25 20:34:03.000000 crypto-screening-1.2.2/crypto_screening/ohlcv.py
--rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.2.2/crypto_screening/orderbook.py
--rw-rw-rw-   0        0        0     2384 2023-06-27 08:28:20.000000 crypto-screening-1.2.2/crypto_screening/process.py
--rw-rw-rw-   0        0        0    31848 2023-06-27 09:29:28.000000 crypto-screening-1.2.2/crypto_screening/screener.py
--rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.2.2/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.2.2/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:21:02.033896 crypto-screening-1.2.2/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-27 10:21:01.000000 crypto-screening-1.2.2/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      812 2023-06-27 10:21:01.000000 crypto-screening-1.2.2/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 10:21:01.000000 crypto-screening-1.2.2/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-27 10:21:01.000000 crypto-screening-1.2.2/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-27 10:21:01.000000 crypto-screening-1.2.2/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-27 10:16:30.000000 crypto-screening-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-06-27 07:30:41.000000 crypto-screening-1.2.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 10:21:02.038897 crypto-screening-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-27 10:16:25.000000 crypto-screening-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:24:24.704482 crypto-screening-1.2.3/
+-rw-rw-rw-   0        0        0       98 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-27 10:24:24.704482 crypto-screening-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.2.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.2.3/build.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:24:24.688481 crypto-screening-1.2.3/crypto_screening/
+-rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.2.3/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:24:24.703506 crypto-screening-1.2.3/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17353 2023-06-27 10:23:45.000000 crypto-screening-1.2.3/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0      496 2023-06-27 10:17:11.000000 crypto-screening-1.2.3/crypto_screening/collect/document.py
+-rw-rw-rw-   0        0        0     4032 2023-06-27 10:16:15.000000 crypto-screening-1.2.3/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0     7755 2023-06-27 09:28:30.000000 crypto-screening-1.2.3/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    17220 2023-06-27 10:23:45.000000 crypto-screening-1.2.3/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12447 2023-06-25 20:15:20.000000 crypto-screening-1.2.3/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      869 2023-06-27 10:20:56.000000 crypto-screening-1.2.3/crypto_screening/document.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.2.3/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.2.3/crypto_screening/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.2.3/crypto_screening/interval.py
+-rw-rw-rw-   0        0        0    32476 2023-06-25 20:34:03.000000 crypto-screening-1.2.3/crypto_screening/ohlcv.py
+-rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.2.3/crypto_screening/orderbook.py
+-rw-rw-rw-   0        0        0     2378 2023-06-27 10:23:45.000000 crypto-screening-1.2.3/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    31848 2023-06-27 09:29:28.000000 crypto-screening-1.2.3/crypto_screening/screener.py
+-rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.2.3/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.2.3/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:24:24.698482 crypto-screening-1.2.3/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-06-27 07:30:41.000000 crypto-screening-1.2.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 10:24:24.704482 crypto-screening-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-27 10:24:20.000000 crypto-screening-1.2.3/setup.py
```

### Comparing `crypto-screening-1.2.2/PKG-INFO` & `crypto-screening-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.2.2
+Version: 1.2.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.2.2/README.md` & `crypto-screening-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/build.py` & `crypto-screening-1.2.3/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/base.py` & `crypto-screening-1.2.3/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/collect/assets.py` & `crypto-screening-1.2.3/crypto_screening/collect/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # assets.py
 
 from typing import Optional, Dict, Iterable, List, Union
 
-from crypto_screening.process import collect_mutual_string_values
+from crypto_screening.process import mutual_string_values
 from crypto_screening.symbols import symbol_to_parts, symbol_to_pair
 from crypto_screening.collect.exchanges import exchanges_data
 from crypto_screening.collect.symbols import (
     all_exchange_symbols, exchange_symbols
 )
 
 __all__ = [
     "exchanges_assets",
-    "mutual_assets",
+    "mutual_exchanges_assets",
     "exchange_assets",
     "exchange_quote_assets",
     "exchange_base_assets",
     "all_exchange_assets",
     "all_exchange_base_assets",
     "all_exchange_quote_assets",
     "exchanges_base_assets",
     "exchanges_quote_assets",
-    "mutual_base_assets",
-    "mutual_quote_assets",
+    "mutual_exchanges_base_assets",
+    "mutual_exchanges_quote_assets",
     "exchanges_symbols_assets",
     "exchanges_symbols_quote_assets",
     "exchanges_symbols_base_assets"
 ]
 
 def all_exchange_assets(
         exchange: str,
@@ -446,15 +446,15 @@
                 for symbol in set(symbols)
             )
         )
         for exchange, symbols in result.items()
     }
 # end exchanges_symbols_quote_assets
 
-def mutual_assets(
+def mutual_exchanges_assets(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
@@ -471,23 +471,23 @@
     :param separator: The separator of the assets.
     :param data: The data to search in.
     :param included: The symbols to include.
 
     :return: The data of the exchanges.
     """
 
-    return collect_mutual_string_values(
+    return mutual_string_values(
         data=data or exchanges_assets(
             exchanges=exchanges, quotes=quotes, bases=bases, included=included,
             excluded=excluded, adjust=adjust, separator=separator
         )
     )
-# end mutual_assets
+# end mutual_exchanges_assets
 
-def mutual_base_assets(
+def mutual_exchanges_base_assets(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
@@ -504,23 +504,23 @@
     :param separator: The separator of the assets.
     :param data: The data to search in.
     :param included: The symbols to include.
 
     :return: The data of the exchanges.
     """
 
-    return collect_mutual_string_values(
+    return mutual_string_values(
         data=data or exchanges_base_assets(
             exchanges=exchanges, quotes=quotes, bases=bases, included=included,
             excluded=excluded, adjust=adjust, separator=separator
         )
     )
-# end mutual_base_assets
+# end mutual_exchanges_base_assets
 
-def mutual_quote_assets(
+def mutual_exchanges_quote_assets(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
@@ -537,14 +537,14 @@
     :param separator: The separator of the assets.
     :param data: The data to search in.
     :param included: The symbols to include.
 
     :return: The data of the exchanges.
     """
 
-    return collect_mutual_string_values(
+    return mutual_string_values(
         data=data or exchanges_quote_assets(
             exchanges=exchanges, quotes=quotes, bases=bases, included=included,
             excluded=excluded, adjust=adjust, separator=separator
         )
     )
-# end mutual_quote_assets
+# end mutual_exchanges_quote_assets
```

### Comparing `crypto-screening-1.2.2/crypto_screening/collect/exchanges.py` & `crypto-screening-1.2.3/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/collect/screeners.py` & `crypto-screening-1.2.3/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/collect/symbols.py` & `crypto-screening-1.2.3/crypto_screening/collect/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 )
 
 from represent import BaseModel
 
 
 from crypto_screening.process import (
     find_string_value, upper_string_values,
-    collect_mutual_string_values
+    mutual_string_values
 )
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import (
     symbol_to_parts, adjust_symbol, Separator
 )
 from crypto_screening.validate import validate_exchange
 from crypto_screening.collect.exchanges import exchanges_data
 
 __all__ = [
     "exchanges_symbols",
-    "mutual_symbols",
+    "mutual_exchanges_symbols",
     "include_symbols",
     "exclude_symbols",
     "exchange_symbols",
     "all_exchange_symbols",
     "matching_symbol_pair",
     "matching_symbol_pairs",
     "MarketSymbolSignature",
@@ -349,15 +349,15 @@
     return exchanges_data(
         collector=exchange_symbols,
         exchanges=exchanges, quotes=quotes, excluded=excluded,
         adjust=adjust, separator=separator, included=included, bases=bases
     )
 # end exchanges_symbols
 
-def mutual_symbols(
+def mutual_exchanges_symbols(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
@@ -374,21 +374,21 @@
     :param data: The data to search in.
     :param included: The symbols to include.
     :param bases: The bases of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
-    return collect_mutual_string_values(
+    return mutual_string_values(
         data=data or exchanges_symbols(
             exchanges=exchanges, quotes=quotes, excluded=excluded,
             adjust=adjust, separator=separator, included=included, bases=bases
         )
     )
-# end mutual_symbols
+# end mutual_exchanges_symbols
 
 AssetMatches = Iterable[Iterable[str]]
 
 def matching_symbol_pair(
         symbol1: str,
         symbol2: str, /, *,
         matches: Optional[AssetMatches] = None,
```

### Comparing `crypto-screening-1.2.2/crypto_screening/dataset.py` & `crypto-screening-1.2.3/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/document.py` & `crypto-screening-1.2.3/crypto_screening/document.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/interval.py` & `crypto-screening-1.2.3/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/ohlcv.py` & `crypto-screening-1.2.3/crypto_screening/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/orderbook.py` & `crypto-screening-1.2.3/crypto_screening/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/process.py` & `crypto-screening-1.2.3/crypto_screening/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Iterable, List, Optional, Dict
 
 __all__ = [
     "find_string_value",
     "upper_string_values",
     "lower_string_values",
-    "collect_mutual_string_values"
+    "mutual_string_values"
 ]
 
 def find_string_value(value: str, values: Iterable[str]) -> str:
     """
     Finds the exchange in the exchanges.
 
     :param value: The name of the exchange.
@@ -56,15 +56,15 @@
 
     :return: The converted values.
     """
 
     return [value.lower() for value in values]
 # end lower_string_values
 
-def collect_mutual_string_values(
+def mutual_string_values(
         data: Dict[str, Iterable[str]],
         minimum: Optional[int] = None,
         maximum: Optional[int] = None
 ) -> Dict[str, List[str]]:
     """
     Collects the symbols from the exchanges.
 
@@ -93,8 +93,8 @@
 
     return {
         key: [
             value for value in data[key]
             if minimum <= values.get(value, 0) <= maximum
         ] for key in data
     }
-# end mutual_assets
+# end mutual_exchanges_assets
```

### Comparing `crypto-screening-1.2.2/crypto_screening/screener.py` & `crypto-screening-1.2.3/crypto_screening/screener.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/symbols.py` & `crypto-screening-1.2.3/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening/validate.py` & `crypto-screening-1.2.3/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.2.3/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.2.2
+Version: 1.2.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.2.2/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.2.3/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.2/pyproject.toml` & `crypto-screening-1.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.2.2'
+version = '1.2.3'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.2.2/setup.py` & `crypto-screening-1.2.3/setup.py`

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
-        version='1.2.2',
+        version='1.2.3',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

