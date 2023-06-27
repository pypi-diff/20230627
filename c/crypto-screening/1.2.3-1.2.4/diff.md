# Comparing `tmp/crypto-screening-1.2.3.tar.gz` & `tmp/crypto-screening-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.2.3.tar", last modified: Tue Jun 27 10:24:24 2023, max compression
+gzip compressed data, was "crypto-screening-1.2.4.tar", last modified: Tue Jun 27 10:27:06 2023, max compression
```

## Comparing `crypto-screening-1.2.3.tar` & `crypto-screening-1.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 10:24:24.704482 crypto-screening-1.2.3/
--rw-rw-rw-   0        0        0       98 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-27 10:24:24.704482 crypto-screening-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.2.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.2.3/build.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:24:24.688481 crypto-screening-1.2.3/crypto_screening/
--rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.2.3/crypto_screening/base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:24:24.703506 crypto-screening-1.2.3/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17353 2023-06-27 10:23:45.000000 crypto-screening-1.2.3/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0      496 2023-06-27 10:17:11.000000 crypto-screening-1.2.3/crypto_screening/collect/document.py
--rw-rw-rw-   0        0        0     4032 2023-06-27 10:16:15.000000 crypto-screening-1.2.3/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0     7755 2023-06-27 09:28:30.000000 crypto-screening-1.2.3/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    17220 2023-06-27 10:23:45.000000 crypto-screening-1.2.3/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12447 2023-06-25 20:15:20.000000 crypto-screening-1.2.3/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      869 2023-06-27 10:20:56.000000 crypto-screening-1.2.3/crypto_screening/document.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.2.3/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.2.3/crypto_screening/hints.py
--rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.2.3/crypto_screening/interval.py
--rw-rw-rw-   0        0        0    32476 2023-06-25 20:34:03.000000 crypto-screening-1.2.3/crypto_screening/ohlcv.py
--rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.2.3/crypto_screening/orderbook.py
--rw-rw-rw-   0        0        0     2378 2023-06-27 10:23:45.000000 crypto-screening-1.2.3/crypto_screening/process.py
--rw-rw-rw-   0        0        0    31848 2023-06-27 09:29:28.000000 crypto-screening-1.2.3/crypto_screening/screener.py
--rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.2.3/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.2.3/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:24:24.698482 crypto-screening-1.2.3/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      812 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-27 10:24:24.000000 crypto-screening-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-06-27 07:30:41.000000 crypto-screening-1.2.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 10:24:24.704482 crypto-screening-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-27 10:24:20.000000 crypto-screening-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:27:06.453599 crypto-screening-1.2.4/
+-rw-rw-rw-   0        0        0       98 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-27 10:27:06.453599 crypto-screening-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.2.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.2.4/build.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:27:06.436601 crypto-screening-1.2.4/crypto_screening/
+-rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.2.4/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:27:06.452601 crypto-screening-1.2.4/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17353 2023-06-27 10:23:45.000000 crypto-screening-1.2.4/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0      496 2023-06-27 10:17:11.000000 crypto-screening-1.2.4/crypto_screening/collect/document.py
+-rw-rw-rw-   0        0        0     4032 2023-06-27 10:16:15.000000 crypto-screening-1.2.4/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0     8370 2023-06-27 10:25:51.000000 crypto-screening-1.2.4/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    17220 2023-06-27 10:23:45.000000 crypto-screening-1.2.4/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12447 2023-06-25 20:15:20.000000 crypto-screening-1.2.4/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      869 2023-06-27 10:20:56.000000 crypto-screening-1.2.4/crypto_screening/document.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.2.4/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.2.4/crypto_screening/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.2.4/crypto_screening/interval.py
+-rw-rw-rw-   0        0        0    32476 2023-06-25 20:34:03.000000 crypto-screening-1.2.4/crypto_screening/ohlcv.py
+-rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.2.4/crypto_screening/orderbook.py
+-rw-rw-rw-   0        0        0     2378 2023-06-27 10:23:45.000000 crypto-screening-1.2.4/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    31848 2023-06-27 09:29:28.000000 crypto-screening-1.2.4/crypto_screening/screener.py
+-rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.2.4/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.2.4/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:27:06.448631 crypto-screening-1.2.4/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-27 10:27:06.000000 crypto-screening-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-06-27 07:30:41.000000 crypto-screening-1.2.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.2.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 10:27:06.454647 crypto-screening-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-27 10:26:59.000000 crypto-screening-1.2.4/setup.py
```

### Comparing `crypto-screening-1.2.3/PKG-INFO` & `crypto-screening-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.2.3
+Version: 1.2.4
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.2.3/README.md` & `crypto-screening-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/build.py` & `crypto-screening-1.2.4/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/base.py` & `crypto-screening-1.2.4/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/collect/assets.py` & `crypto-screening-1.2.4/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/collect/exchanges.py` & `crypto-screening-1.2.4/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/collect/screeners.py` & `crypto-screening-1.2.4/crypto_screening/collect/screeners.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     "matching_screener_signatures",
     "matching_screener_pair",
     "matching_screener_pairs",
     "MarketScreenerSignature",
     "find_screeners",
     "structure_screeners",
     "live_screeners",
-    "remove_empty_screeners"
+    "remove_empty_screeners",
+    "screeners_exchanges_symbols"
 ]
 
 AssetMatches = Iterable[Iterable[str]]
 
 def matching_screener_pair(
         screener1: BaseScreener,
         screener2: BaseScreener, /, *,
@@ -261,8 +262,29 @@
     :param screeners: The screeners of the assets and exchanges.
     """
 
     return [
         screener for screener in screeners
         if len(screener.market) > 0
     ]
-# end remove_empty_screeners
+# end remove_empty_screeners
+
+def screeners_exchanges_symbols(screeners: Iterable[BaseScreener]) -> Dict[str, List[str]]:
+    """
+    Collects the structure of the screeners exchanges and symbols.
+
+    :param screeners: The screeners to process.
+
+    :return: The collected structure of exchanges and symbols.
+    """
+
+    data = {}
+
+    for screener in screeners:
+        data.setdefault(screener.exchange, []).append(screener.symbol)
+    # end for
+
+    return {
+        exchange: list(set(symbols))
+        for exchange, symbols in data.items()
+    }
+# end screeners_exchanges_symbols
```

### Comparing `crypto-screening-1.2.3/crypto_screening/collect/symbols.py` & `crypto-screening-1.2.4/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/dataset.py` & `crypto-screening-1.2.4/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/document.py` & `crypto-screening-1.2.4/crypto_screening/document.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/interval.py` & `crypto-screening-1.2.4/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/ohlcv.py` & `crypto-screening-1.2.4/crypto_screening/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/orderbook.py` & `crypto-screening-1.2.4/crypto_screening/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/process.py` & `crypto-screening-1.2.4/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/screener.py` & `crypto-screening-1.2.4/crypto_screening/screener.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/symbols.py` & `crypto-screening-1.2.4/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening/validate.py` & `crypto-screening-1.2.4/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.2.4/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.2.3
+Version: 1.2.4
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.2.3/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.2.4/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.2.3/pyproject.toml` & `crypto-screening-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.2.3'
+version = '1.2.4'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.2.3/setup.py` & `crypto-screening-1.2.4/setup.py`

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
-        version='1.2.3',
+        version='1.2.4',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

