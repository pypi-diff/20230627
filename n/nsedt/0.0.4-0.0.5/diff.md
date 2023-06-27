# Comparing `tmp/nsedt-0.0.4.tar.gz` & `tmp/nsedt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsedt-0.0.4.tar", last modified: Sat Jun 10 23:32:01 2023, max compression
+gzip compressed data, was "nsedt-0.0.5.tar", last modified: Tue Jun 27 18:52:42 2023, max compression
```

## Comparing `nsedt-0.0.4.tar` & `nsedt-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:32:01.667057 nsedt-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 23:31:52.000000 nsedt-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-10 23:32:01.667057 nsedt-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-10 23:31:52.000000 nsedt-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:32:01.667057 nsedt-0.0.4/nsedt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/equity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:32:01.667057 nsedt-0.0.4/nsedt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/resources/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:32:01.667057 nsedt-0.0.4/nsedt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-10 23:31:52.000000 nsedt-0.0.4/nsedt/utils/data_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 23:32:01.667057 nsedt-0.0.4/nsedt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-10 23:32:01.000000 nsedt-0.0.4/nsedt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-10 23:32:01.000000 nsedt-0.0.4/nsedt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 23:32:01.000000 nsedt-0.0.4/nsedt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-10 23:32:01.000000 nsedt-0.0.4/nsedt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 23:32:01.000000 nsedt-0.0.4/nsedt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-10 23:32:01.671057 nsedt-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-10 23:31:52.000000 nsedt-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:42.620384 nsedt-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 18:52:28.000000 nsedt-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-27 18:52:42.620384 nsedt-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-27 18:52:28.000000 nsedt-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:42.616384 nsedt-0.0.5/nsedt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/equity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:42.620384 nsedt-0.0.5/nsedt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/resources/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:42.620384 nsedt-0.0.5/nsedt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-27 18:52:28.000000 nsedt-0.0.5/nsedt/utils/data_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:52:42.620384 nsedt-0.0.5/nsedt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-27 18:52:42.000000 nsedt-0.0.5/nsedt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-27 18:52:42.000000 nsedt-0.0.5/nsedt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:52:42.000000 nsedt-0.0.5/nsedt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 18:52:42.000000 nsedt-0.0.5/nsedt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 18:52:42.000000 nsedt-0.0.5/nsedt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-27 18:52:42.620384 nsedt-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-27 18:52:28.000000 nsedt-0.0.5/setup.py
```

### Comparing `nsedt-0.0.4/LICENSE` & `nsedt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.4/PKG-INFO` & `nsedt-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: nsedt
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library to collect NSE data in pandas dataframe
 Home-page: https://github.com/pratik141/nsedt
 Author: Pratik Anand
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nse data
 
 Introduction
 
@@ -63,15 +61,15 @@
 
 #get_companyinfo
                                                info                           metadata securityInfo  ... priceInfo   industryInfo preOpenMarket
 symbol                                           TCS                                TCS          NaN  ...       NaN            NaN           NaN
 atoSellQty                                       NaN                                NaN          NaN  ...       NaN            NaN           491
 
 #get_companyinfo json format
-{"info":{"symbol":"TCS","companyName":"Tata Consultancy Services Limited","industry":"COMPUTERS - SOFTWARE","activeSeries":["EQ"],"debtSeries":[],"tempSuspendedSeries":[],"isFNOSec":true,"isCASec":false,"isSLBSec":true,"isDebtSec":false,"isSuspended":false,"isETFSec":false,"isDelisted":false," ......}
+{"info":{"symbol":"TCS","companyName":"Tata Consultancy Services Limited","industry":"COMPUTERS - SOFTWARE","activeSeries":["EQ"],"debtSeries":[],"tempSuspendedSeries":[],"isFNOSec":true,"isCASec":false,"isSLBSec":true,"isDebtSec":false,"isSuspended":false,"isETFSec":false,"isDelisted":false, ......}
 
 #get_marketstatus
 
            market marketStatus     tradeDate     index     last  ... percentChange marketStatusMessage   expiryDate underlying tradeDateFormatted
 0  Capital Market        Close   09-Jun-2023  NIFTY 50  18563.4  ...         -0.38    Market is Closed          NaN        NaN                NaN
 4  currencyfuture        Close  Invalid date            82.4975  ...                  Market is Closed  16-Jun-2023     USDINR        09-Jun-2023
 
@@ -79,7 +77,37 @@
 #get_chartdata
                  0        1
 0    1686301201000  3300.00
 404  1686301620000  3250.00
 
 
 ```
+---
+
+# API Documentation
+
+## Functions
+
+### get_companyinfo
+
+Function description goes here.
+
+### get_marketstatus
+
+Function description goes here.
+
+### get_price
+
+Function description goes here.
+
+### get_corpinfo
+
+Function description goes here.
+
+### get_event
+
+Function description goes here.
+
+### get_chartdata
+
+Function description goes here.
+
```

### Comparing `nsedt-0.0.4/README.md` & `nsedt-0.0.5/nsedt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: nsedt
+Version: 0.0.5
+Summary: Library to collect NSE data in pandas dataframe
+Home-page: https://github.com/pratik141/nsedt
+Author: Pratik Anand
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nse data
 
 Introduction
 
 Thank you for using Nsedt. Please feel free to send pull requests, comments, and suggestions, as well as get in touch with me if you require any additional help. I sincerely hope you will find this library useful.
 
 ---
@@ -46,15 +61,15 @@
 
 #get_companyinfo
                                                info                           metadata securityInfo  ... priceInfo   industryInfo preOpenMarket
 symbol                                           TCS                                TCS          NaN  ...       NaN            NaN           NaN
 atoSellQty                                       NaN                                NaN          NaN  ...       NaN            NaN           491
 
 #get_companyinfo json format
-{"info":{"symbol":"TCS","companyName":"Tata Consultancy Services Limited","industry":"COMPUTERS - SOFTWARE","activeSeries":["EQ"],"debtSeries":[],"tempSuspendedSeries":[],"isFNOSec":true,"isCASec":false,"isSLBSec":true,"isDebtSec":false,"isSuspended":false,"isETFSec":false,"isDelisted":false," ......}
+{"info":{"symbol":"TCS","companyName":"Tata Consultancy Services Limited","industry":"COMPUTERS - SOFTWARE","activeSeries":["EQ"],"debtSeries":[],"tempSuspendedSeries":[],"isFNOSec":true,"isCASec":false,"isSLBSec":true,"isDebtSec":false,"isSuspended":false,"isETFSec":false,"isDelisted":false, ......}
 
 #get_marketstatus
 
            market marketStatus     tradeDate     index     last  ... percentChange marketStatusMessage   expiryDate underlying tradeDateFormatted
 0  Capital Market        Close   09-Jun-2023  NIFTY 50  18563.4  ...         -0.38    Market is Closed          NaN        NaN                NaN
 4  currencyfuture        Close  Invalid date            82.4975  ...                  Market is Closed  16-Jun-2023     USDINR        09-Jun-2023
 
@@ -62,7 +77,37 @@
 #get_chartdata
                  0        1
 0    1686301201000  3300.00
 404  1686301620000  3250.00
 
 
 ```
+---
+
+# API Documentation
+
+## Functions
+
+### get_companyinfo
+
+Function description goes here.
+
+### get_marketstatus
+
+Function description goes here.
+
+### get_price
+
+Function description goes here.
+
+### get_corpinfo
+
+Function description goes here.
+
+### get_event
+
+Function description goes here.
+
+### get_chartdata
+
+Function description goes here.
+
```

### Comparing `nsedt-0.0.4/nsedt/equity.py` & `nsedt-0.0.5/nsedt/equity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-import datetime
+""" 
+get data for Equity
+"""
 import concurrent
+import datetime
+import logging
+import urllib
 from concurrent.futures import ALL_COMPLETED
+
 import pandas as pd
+
 from nsedt import utils
-from nsedt.utils import data_format
-import urllib
 from nsedt.resources import constants as cns
-import logging
+from nsedt.utils import data_format
 
 logging.basicConfig(
     level=logging.INFO,
-    format=cns.log_format,
+    format=cns.LOG_FORMAT,
     datefmt="%m/%d/%Y %I:%M:%S %p",
 )
 
 
 def get_companyinfo(
     symbol,
     response_type="panda_df",
@@ -28,52 +33,52 @@
         Pandas DataFrame: df containing company info
       or
         Json: json containing company info
 
     """
     params = {}
     cookies = utils.get_cookies()
-    base_url = cns.base_url
-    event_api = cns.equity_info
+    base_url = cns.BASE_URL
+    event_api = cns.EQUITY_INFO
 
     params["symbol"] = symbol
 
     url = base_url + event_api + urllib.parse.urlencode(params)
-    data = utils.fetch_url(url, cookies, key="info")
+    data = utils.fetch_url(url, cookies)
 
-    if response_type == "json":
-        return data.to_json()
-    else:
+    if response_type == "panda_df":
         return data
 
+    return data.to_json()
+
 
 def get_marketstatus(
     response_type="panda_df",
 ):
     """
     Args:
         response_type (str, Optional): define the response type panda_df | json. Default panda_df
     Returns:
         Pandas DataFrame: df containing market status
         Json : Json containing market status
 
     """
 
     cookies = utils.get_cookies()
-    base_url = cns.base_url
-    event_api = cns.marketStatus
+    base_url = cns.BASE_URL
+    event_api = cns.MARKETSTATUS
 
     url = base_url + event_api
     data = utils.fetch_url(url, cookies, key="marketState")
 
-    if response_type == "json":
-        return data.to_json()
-    else:
+    if response_type == "panda_df":
         return data
 
+    return data.to_json()
+
 
 def get_price(
     start_date,
     end_date,
     symbol=None,
     input_type="stock",
     series="EQ",
@@ -85,59 +90,56 @@
         end_date (datetime.datetime): end date
         input_type (str): Either 'stock' or 'index'
         symbol (str, optional): stock symbol. Defaults to None. TODO: implement for index`
     Returns:
         Pandas DataFrame: df containing data for symbol of provided date range
     """
     cookies = utils.get_cookies()
-    base_url = cns.base_url
-    price_api = cns.equity_price_histroy
+    base_url = cns.BASE_URL
+    price_api = cns.EQUITY_PRICE_HISTROY
     url_list = []
 
     # set the window size to one year
-    window_size = datetime.timedelta(days=cns.window_size)
+    window_size = datetime.timedelta(days=cns.WINDOW_SIZE)
 
     current_window_start = start_date
     while current_window_start < end_date:
         current_window_end = current_window_start + window_size
 
         # check if the current window extends beyond the end_date
-        if current_window_end > end_date:
-            current_window_end = end_date
-
-        st = current_window_start.strftime("%d-%m-%Y")
-        et = current_window_end.strftime("%d-%m-%Y")
+        current_window_end = min(current_window_end, end_date)
 
         if input_type == "stock":
             params = {
                 "symbol": symbol,
-                "from": st,
-                "to": et,
+                "from": current_window_start.strftime("%d-%m-%Y"),
+                "to": current_window_end.strftime("%d-%m-%Y"),
                 "dataType": "priceVolumeDeliverable",
                 "series": series,
             }
             url = base_url + price_api + urllib.parse.urlencode(params)
             url_list.append(url)
 
         # move the window start to the next day after the current window end
         current_window_start = current_window_end + datetime.timedelta(days=1)
 
     result = pd.DataFrame()
-    with concurrent.futures.ThreadPoolExecutor(max_workers=cns.max_workers) as executor:
+    with concurrent.futures.ThreadPoolExecutor(max_workers=cns.MAX_WORKERS) as executor:
         future_to_url = {
-            executor.submit(utils.fetch_url, url, cookies): url for url in url_list
+            executor.submit(utils.fetch_url, url, cookies, "data"): url
+            for url in url_list
         }
         concurrent.futures.wait(future_to_url, return_when=ALL_COMPLETED)
         for future in concurrent.futures.as_completed(future_to_url):
             url = future_to_url[future]
             try:
-                df = future.result()
-                result = pd.concat([result, df])
+                dataframe = future.result()
+                result = pd.concat([result, dataframe])
             except Exception as exc:
-                logging.error(f"{url} got exception: {exc}. Please try again later.")
+                logging.error("%s got exception: %s. Please try again later.", url, exc)
                 raise exc
     return data_format.price(result)
 
 
 def get_corpinfo(
     start_date,
     end_date,
@@ -148,33 +150,34 @@
     Create threads for different requests, parses data, combines them and returns dataframe
     Args:
         start_date (datetime.datetime): start date
         end_date (datetime.datetime): end date
         symbol (str, optional): stock symbol. Defaults to None.
     Returns:
         Pandas DataFrame: df containing data for symbol of provided date range
+      or
+        Json: json containing data for symbol of provided date range
     """
     cookies = utils.get_cookies()
     params = {
         "symbol": symbol,
         "from_date": start_date,
         "to_date": end_date,
         "index": "equities",
     }
-    base_url = cns.base_url
-    price_api = cns.equity_corpinfo
+    base_url = cns.BASE_URL
+    price_api = cns.EQUITY_CORPINFO
     url = base_url + price_api + urllib.parse.urlencode(params)
 
     data = utils.fetch_url(url, cookies)
 
-    if response_type == "json":
-        return data.to_json()
-    else:
+    if response_type == "panda_df":
         return data
-    return
+
+    return data.to_json()
 
 
 def get_event(
     start_date=None,
     end_date=None,
     index="equities",
 ):
@@ -184,16 +187,16 @@
         end_date (datetime.datetime,optional): end date
     Returns:
         Pandas DataFrame: df containing event of provided date range
 
     """
     params = {}
     cookies = utils.get_cookies()
-    base_url = cns.base_url
-    event_api = cns.equity_event
+    base_url = cns.BASE_URL
+    event_api = cns.EQUITY_EVENT
 
     params["index"] = index
     if start_date is not None:
         params["from_date"] = start_date
     if end_date is not None:
         params["to_date"] = end_date
 
@@ -210,16 +213,16 @@
         symbol (str): stock symbol.
     Returns:
         Pandas DataFrame: df containing chart data of provided date
 
     """
     params = {}
     cookies = utils.get_cookies()
-    base_url = cns.base_url
-    event_api = cns.equity_chart
+    base_url = cns.BASE_URL
+    event_api = cns.EQUITY_CHART
     try:
         identifier = get_companyinfo(symbol)["info"]["identifier"]
     except KeyError:
         return f"Invalid symbol name: {symbol}"
 
     params["index"] = identifier
     params["preopen"] = preopen
```

### Comparing `nsedt-0.0.4/nsedt/resources/constants.py` & `nsedt-0.0.5/nsedt/resources/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-window_size = 50
-max_workers = 10
-log_format = """{
+"""
+Constants
+"""
+
+WINDOW_SIZE = 50
+MAX_WORKERS = 10
+LOG_FORMAT = """{
     "time": "%(asctime)s",
     "lineno": "%(lineno)d",
     "name": "[%(name)s]",
     "levelname": "%(levelname)s",
     "process": "%(process)s",
     "filename": "%(filename)s",
     "funcName": "%(funcName)s",
     "logmessage": "%(message)s",
 }"""
 
-base_url = "https://www.nseindia.com/"
-equity_price_histroy = "api/historical/securityArchives?"
-equity_corpinfo = "api/corporates-corporateActions?"
-marketStatus = "api/marketStatus"
-equity_event = "api/event-calendar?"
-equity_chart = "api/chart-databyindex?"
-equity_info = "api/quote-equity?"
+BASE_URL = "https://www.nseindia.com/"
+EQUITY_PRICE_HISTROY = "api/historical/securityArchives?"
+EQUITY_CORPINFO = "api/corporates-corporateActions?"
+MARKETSTATUS = "api/marketStatus"
+EQUITY_EVENT = "api/event-calendar?"
+EQUITY_CHART = "api/chart-databyindex?"
+EQUITY_INFO = "api/quote-equity?"
```

### Comparing `nsedt-0.0.4/setup.py` & `nsedt-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
-
+"""
+Install script
+"""
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding="utf-8") as file:
+    long_description = file.read()
 setup(
     name="nsedt",
-    version="0.0.4",
+    version="0.0.5",
     author="Pratik Anand",
-    long_description=open("README.md", "r", encoding="utf-8").read(),
+    long_description=long_description,
     long_description_content_type="text/markdown",
     description="Library to collect NSE data in pandas dataframe",
     packages=find_packages(),
     url="https://github.com/pratik141/nsedt",
     install_requires=[
         "requests",
         "numpy",
         "pandas",
         "six",
-        "click",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
 )
```

