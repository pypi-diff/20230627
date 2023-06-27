# Comparing `tmp/crypto-screening-1.2.4.tar.gz` & `tmp/crypto-screening-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.2.4.tar", last modified: Tue Jun 27 10:27:06 2023, max compression
+gzip compressed data, was "crypto-screening-1.2.5.tar", last modified: Tue Jun 27 12:22:48 2023, max compression
```

## Comparing `crypto-screening-1.2.4.tar` & `crypto-screening-1.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 10:27:06.453599 crypto-screening-1.2.4/
--rw-rw-rw-   0        0        0       98 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-27 10:27:06.453599 crypto-screening-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.2.4/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.2.4/build.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:27:06.436601 crypto-screening-1.2.4/crypto_screening/
--rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.2.4/crypto_screening/base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:27:06.452601 crypto-screening-1.2.4/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17353 2023-06-27 10:23:45.000000 crypto-screening-1.2.4/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0      496 2023-06-27 10:17:11.000000 crypto-screening-1.2.4/crypto_screening/collect/document.py
--rw-rw-rw-   0        0        0     4032 2023-06-27 10:16:15.000000 crypto-screening-1.2.4/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0     8370 2023-06-27 10:25:51.000000 crypto-screening-1.2.4/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    17220 2023-06-27 10:23:45.000000 crypto-screening-1.2.4/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12447 2023-06-25 20:15:20.000000 crypto-screening-1.2.4/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      869 2023-06-27 10:20:56.000000 crypto-screening-1.2.4/crypto_screening/document.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.2.4/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.2.4/crypto_screening/hints.py
--rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.2.4/crypto_screening/interval.py
--rw-rw-rw-   0        0        0    32476 2023-06-25 20:34:03.000000 crypto-screening-1.2.4/crypto_screening/ohlcv.py
--rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.2.4/crypto_screening/orderbook.py
--rw-rw-rw-   0        0        0     2378 2023-06-27 10:23:45.000000 crypto-screening-1.2.4/crypto_screening/process.py
--rw-rw-rw-   0        0        0    31848 2023-06-27 09:29:28.000000 crypto-screening-1.2.4/crypto_screening/screener.py
--rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.2.4/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.2.4/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:27:06.448631 crypto-screening-1.2.4/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      812 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-06-27 07:30:41.000000 crypto-screening-1.2.4/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.2.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 10:27:06.454647 crypto-screening-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-27 10:26:59.000000 crypto-screening-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:22:48.127336 crypto-screening-1.2.5/
+-rw-rw-rw-   0        0        0       98 2023-06-27 12:22:47.000000 crypto-screening-1.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-27 12:22:48.126333 crypto-screening-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.2.5/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.2.5/build.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:22:48.108815 crypto-screening-1.2.5/crypto_screening/
+-rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.2.5/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:22:48.125331 crypto-screening-1.2.5/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17353 2023-06-27 10:23:45.000000 crypto-screening-1.2.5/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0      496 2023-06-27 10:17:11.000000 crypto-screening-1.2.5/crypto_screening/collect/document.py
+-rw-rw-rw-   0        0        0     4032 2023-06-27 10:16:15.000000 crypto-screening-1.2.5/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0     8370 2023-06-27 10:25:51.000000 crypto-screening-1.2.5/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18049 2023-06-27 12:17:52.000000 crypto-screening-1.2.5/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12447 2023-06-25 20:15:20.000000 crypto-screening-1.2.5/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      869 2023-06-27 10:20:56.000000 crypto-screening-1.2.5/crypto_screening/document.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.2.5/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.2.5/crypto_screening/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.2.5/crypto_screening/interval.py
+-rw-rw-rw-   0        0        0    32476 2023-06-25 20:34:03.000000 crypto-screening-1.2.5/crypto_screening/ohlcv.py
+-rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.2.5/crypto_screening/orderbook.py
+-rw-rw-rw-   0        0        0     2378 2023-06-27 10:23:45.000000 crypto-screening-1.2.5/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    31848 2023-06-27 09:29:28.000000 crypto-screening-1.2.5/crypto_screening/screener.py
+-rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.2.5/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.2.5/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:22:48.122327 crypto-screening-1.2.5/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-27 12:22:48.000000 crypto-screening-1.2.5/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2023-06-27 12:22:48.000000 crypto-screening-1.2.5/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:22:48.000000 crypto-screening-1.2.5/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-27 12:22:48.000000 crypto-screening-1.2.5/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-27 12:22:48.000000 crypto-screening-1.2.5/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-27 12:22:45.000000 crypto-screening-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-06-27 07:30:41.000000 crypto-screening-1.2.5/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 12:22:48.127336 crypto-screening-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-27 12:22:41.000000 crypto-screening-1.2.5/setup.py
```

### Comparing `crypto-screening-1.2.4/PKG-INFO` & `crypto-screening-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.2.4
+Version: 1.2.5
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.2.4/README.md` & `crypto-screening-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/build.py` & `crypto-screening-1.2.5/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/base.py` & `crypto-screening-1.2.5/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/collect/assets.py` & `crypto-screening-1.2.5/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/collect/exchanges.py` & `crypto-screening-1.2.5/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/collect/screeners.py` & `crypto-screening-1.2.5/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/collect/symbols.py` & `crypto-screening-1.2.5/crypto_screening/collect/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     "exchange_symbols",
     "all_exchange_symbols",
     "matching_symbol_pair",
     "matching_symbol_pairs",
     "MarketSymbolSignature",
     "matching_symbol_signatures",
     "include_exchanges_symbols",
-    "exclude_exchanges_symbols"
+    "exclude_exchanges_symbols",
+    "all_exchanges_symbols"
 ]
 
 def include_symbols(
         symbols: Iterable[str],
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         bases: Optional[Iterable[str]] = None,
@@ -79,16 +80,16 @@
 
             else:
                 raise e
             # end if
         # end try
 
         if (
-            (find_string_value(value=base, values=bases) in bases) or
-            (find_string_value(value=quote, values=quotes) in quotes)
+                (find_string_value(value=base, values=bases) in bases) or
+                (find_string_value(value=quote, values=quotes) in quotes)
         ):
             saved.append(symbol)
         # end if
     # end for
 
     return saved
 # end include_symbols
@@ -138,16 +139,16 @@
 
             else:
                 raise e
             # end if
         # end try
 
         if (
-            (find_string_value(value=base, values=bases) in bases) or
-            (find_string_value(value=quote, values=quotes) in quotes)
+                (find_string_value(value=base, values=bases) in bases) or
+                (find_string_value(value=quote, values=quotes) in quotes)
         ):
             continue
         # end if
 
         saved.append(symbol)
     # end for
 
@@ -219,15 +220,15 @@
 # end exclude_exchanges_symbols
 
 def all_exchange_symbols(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         test: Optional[bool] = False
-) -> Iterable[str]:
+) -> List[str]:
     """
     Collects the symbols from the exchanges.
 
     :param exchange: The name of the exchange.
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
     :param test: Include test assets.
@@ -280,14 +281,40 @@
             # end if
         # end try
     # end for
 
     return symbols
 # end all_exchange_symbols
 
+def all_exchanges_symbols(
+        exchanges: Iterable[str],
+        separator: Optional[str] = None,
+        adjust: Optional[bool] = True,
+        test: Optional[bool] = False
+) -> Dict[str, List[str]]:
+    """
+    Collects the symbols from the exchanges.
+
+    :param exchanges: The name of the exchange.
+    :param adjust: The value to adjust the invalid exchanges.
+    :param separator: The separator of the assets.
+    :param test: Include test assets.
+
+    :return: The data of the exchanges.
+    """
+
+    return {
+        exchange: all_exchange_symbols(
+            exchange=exchange, separator=separator,
+            adjust=adjust, test=test
+        )
+        for exchange in exchanges
+    }
+# end all_exchanges_symbols
+
 def exchange_symbols(
         exchange: Optional[str] = None,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         included: Optional[Iterable[str]] = None,
@@ -423,16 +450,16 @@
 
     for matches in matches:
         if (currency1 in matches) and (currency2 in matches):
             return True
         # end if
 
         if (
-            ((currency1 in matches) and (currency2 not in matches)) or
-            ((currency1 not in matches) and (currency2 in matches))
+                ((currency1 in matches) and (currency2 not in matches)) or
+                ((currency1 not in matches) and (currency2 in matches))
         ):
             return False
         # end if
     # end for
 
     return False
 # end matching_symbol_pair
@@ -472,20 +499,20 @@
                 [
                     *matches.get(exchange1, []),
                     *matches.get(exchange2, [])
                 ]
             )
 
             if (
-                (exchange1 != exchange2) and
-                matching_symbol_pair(
-                    symbol1, symbol2,
-                    matches=exchanges_matches or None,
-                    separator=separator
-                )
+                    (exchange1 != exchange2) and
+                    matching_symbol_pair(
+                        symbol1, symbol2,
+                        matches=exchanges_matches or None,
+                        separator=separator
+                    )
             ):
                 pairs.append(
                     ((exchange1, symbol1), (exchange2, symbol2))
                 )
             # end if
         # end for
     # end for
```

### Comparing `crypto-screening-1.2.4/crypto_screening/dataset.py` & `crypto-screening-1.2.5/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/document.py` & `crypto-screening-1.2.5/crypto_screening/document.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/interval.py` & `crypto-screening-1.2.5/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/ohlcv.py` & `crypto-screening-1.2.5/crypto_screening/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/orderbook.py` & `crypto-screening-1.2.5/crypto_screening/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/process.py` & `crypto-screening-1.2.5/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/screener.py` & `crypto-screening-1.2.5/crypto_screening/screener.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/symbols.py` & `crypto-screening-1.2.5/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening/validate.py` & `crypto-screening-1.2.5/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.2.5/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.2.4
+Version: 1.2.5
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.2.4/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.2.5/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.4/pyproject.toml` & `crypto-screening-1.2.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.2.4'
+version = '1.2.5'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.2.4/setup.py` & `crypto-screening-1.2.5/setup.py`

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
-        version='1.2.4',
+        version='1.2.5',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

