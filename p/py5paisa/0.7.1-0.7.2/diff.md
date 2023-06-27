# Comparing `tmp/py5paisa-0.7.1.tar.gz` & `tmp/py5paisa-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py5paisa-0.7.1.tar", last modified: Tue May  9 07:48:06 2023, max compression
+gzip compressed data, was "py5paisa-0.7.2.tar", last modified: Tue Jun 27 07:59:31 2023, max compression
```

## Comparing `py5paisa-0.7.1.tar` & `py5paisa-0.7.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:06.001703 py5paisa-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 07:47:46.000000 py5paisa-0.7.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-09 07:47:46.000000 py5paisa-0.7.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-09 07:47:46.000000 py5paisa-0.7.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-09 07:47:46.000000 py5paisa-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-05-09 07:48:06.001703 py5paisa-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-09 07:47:46.000000 py5paisa-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:05.997703 py5paisa-0.7.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:05.997703 py5paisa-0.7.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    48489 2023-05-09 07:47:46.000000 py5paisa-0.7.1/docs/images/5-paisa-img.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:05.997703 py5paisa-0.7.1/py5paisa/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    34000 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/py5paisa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-09 07:47:46.000000 py5paisa-0.7.1/py5paisa/urlconst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:06.001703 py5paisa-0.7.1/py5paisa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 07:48:05.000000 py5paisa-0.7.1/py5paisa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-09 07:48:06.001703 py5paisa-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-09 07:47:46.000000 py5paisa-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:48:06.001703 py5paisa-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:47:46.000000 py5paisa-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 07:47:46.000000 py5paisa-0.7.1/tests/test_py5paisa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:59:31.395125 py5paisa-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-27 07:59:15.000000 py5paisa-0.7.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-27 07:59:15.000000 py5paisa-0.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 07:59:15.000000 py5paisa-0.7.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-27 07:59:15.000000 py5paisa-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-06-27 07:59:31.395125 py5paisa-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-27 07:59:15.000000 py5paisa-0.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:59:31.387125 py5paisa-0.7.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:59:31.391125 py5paisa-0.7.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    48489 2023-06-27 07:59:15.000000 py5paisa-0.7.2/docs/images/5-paisa-img.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:59:31.391125 py5paisa-0.7.2/py5paisa/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 07:59:15.000000 py5paisa-0.7.2/py5paisa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-27 07:59:15.000000 py5paisa-0.7.2/py5paisa/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-27 07:59:15.000000 py5paisa-0.7.2/py5paisa/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-27 07:59:15.000000 py5paisa-0.7.2/py5paisa/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-27 07:59:15.000000 py5paisa-0.7.2/py5paisa/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33961 2023-06-27 07:59:15.000000 py5paisa-0.7.2/py5paisa/py5paisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-06-27 07:59:15.000000 py5paisa-0.7.2/py5paisa/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-27 07:59:15.000000 py5paisa-0.7.2/py5paisa/urlconst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:59:31.395125 py5paisa-0.7.2/py5paisa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-06-27 07:59:31.000000 py5paisa-0.7.2/py5paisa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-27 07:59:31.000000 py5paisa-0.7.2/py5paisa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:59:31.000000 py5paisa-0.7.2/py5paisa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:59:31.000000 py5paisa-0.7.2/py5paisa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-27 07:59:31.000000 py5paisa-0.7.2/py5paisa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 07:59:31.000000 py5paisa-0.7.2/py5paisa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 07:59:31.395125 py5paisa-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-27 07:59:15.000000 py5paisa-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:59:31.395125 py5paisa-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:59:15.000000 py5paisa-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 07:59:15.000000 py5paisa-0.7.2/tests/test_py5paisa.py
```

### Comparing `py5paisa-0.7.1/CONTRIBUTING.rst` & `py5paisa-0.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.1/PKG-INFO` & `py5paisa-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py5paisa
-Version: 0.7.1
+Version: 0.7.2
 Summary:  Python SDK for 5paisa APIs natively written in VB.NET
 Home-page: https://github.com/5paisa/py5paisa
 Author: 5paisa
 Author-email: coreteam@5paisa.com
 Keywords: py5paisa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -56,29 +56,30 @@
     "APP_NAME":"YOUR APP_NAME",
     "APP_SOURCE":"YOUR APP_SOURCE",
     "USER_ID":"YOUR USER_ID",
     "PASSWORD":"YOUR PASSWORD",
     "USER_KEY":"YOUR USERKEY",
     "ENCRYPTION_KEY":"YOUR ENCRYPTION_KEY"
     }
-# First get a token by logging in to -> https://dev-openapi.5paisa.com/WebVendorLogin/VLogin/Index?VendorKey=<Your Vendor Key>&ResponseURL=<Redirect URL>
-# VendorKey is UesrKey for individuals user
-# for e.g. you can use ResponseURL as https://www.5paisa.com/technology/developer-apis
-# Pass the token received in the response url after successful login to get an access token (this also sets the token for all the APIs you use)-
-
-# Please note that you need to copy the request token from URL and paste in this code and start the code within 30s.
 
 #This function will automatically take care of generating and sending access token for all your API's
 
 client = FivePaisaClient(cred=cred)
 
 # New TOTP based authentication
 client.get_totp_session('Your ClientCode','TOTP from authenticator app','Your Pin')
 
-# If you have the have the token(OAUTH Approach)
+# OAUTH Approach
+# First get a token by logging in to -> https://dev-openapi.5paisa.com/WebVendorLogin/VLogin/Index?VendorKey=<Your Vendor Key>&ResponseURL=<Redirect URL>
+# VendorKey is UesrKey for individuals user
+# for e.g. you can use ResponseURL as https://www.5paisa.com/technology/developer-apis
+# Pass the token received in the response url after successful login to get an access token (this also sets the token for all the APIs you use)-
+
+# Please note that you need to copy the request token from URL and paste in this code and start the code within 30s.
+
 client.get_oauth_session('Your Response Token')
 
 After successful authentication, you should get a `Logged in!!` message in console
 ```
 
 #### Market Feed
 
@@ -334,22 +335,30 @@
 def on_message(ws, message):
     print(message)
 client.receive_data(on_message)
 
 Note:- Instruments in payload above is a list(array) in format as <exchange><exchange type><scrip code>
 ```
 
+#### Level 5 Market Depth 
+```py
+print(client.fetch_market_depth_by_scrip(Exchange="N",ExchangeType="C",ScripCode="1660"))
+print(client.fetch_market_depth_by_scrip(Exchange="N",ExchangeType="C",ScripData="RELIANCE_EQ"))
+```
+
 #### Full Market Snapshot 
 ```py
 a=[{"Exchange":"N","ExchangeType":"C","ScripCode":"2885"},
    {"Exchange":"N","ExchangeType":"C","ScripCode":"1660"},
    ]
 print(client.fetch_market_depth(a))
 ```
 
+
+
 #### Full Market Snapshot(By Symbol)
 ```py
 a=[{"Exchange":"N","ExchangeType":"C","Symbol":"ITC"},
    {"Exchange":"N","ExchangeType":"D","Symbol":"BANKNIFTY 31 Feb 2022 CE 41600.00"},
    ]
 print(client.fetch_market_depth_by_symbol(a))
 ```
```

### Comparing `py5paisa-0.7.1/README.rst` & `py5paisa-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.1/docs/images/5-paisa-img.jpg` & `py5paisa-0.7.2/docs/images/5-paisa-img.jpg`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.1/py5paisa/auth.py` & `py5paisa-0.7.2/py5paisa/auth.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.1/py5paisa/const.py` & `py5paisa-0.7.2/py5paisa/const.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.1/py5paisa/order.py` & `py5paisa-0.7.2/py5paisa/order.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.1/py5paisa/py5paisa.py` & `py5paisa-0.7.2/py5paisa/py5paisa.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,20 @@
 import websocket
 from .urlconst import *
 from enum import Enum
 
 
 class FivePaisaClient:
 
-    def __init__(self, email=None, passwd=None, dob=None, cred=None):
+    def __init__(self, cred=None):
         """
         Main constructor for client.
         Expects user's email, password and date of birth in YYYYMMDD format.
         """
         try:
-            self.email = email
-            self.passwd = passwd
-            self.dob = dob
             self.client_code = ""
             self.Jwt_token = ""
             self.Aspx_auth = None
             self.web_url = None
             self.market_depth_url = None
             self.Res_Data = None
             self.ws = None
@@ -41,39 +38,14 @@
             self.ENCRYPTION_KEY = cred["ENCRYPTION_KEY"]
             self.create_payload()
             self.set_url()
 
         except Exception as e:
             log_response(e)
 
-    def login(self):
-        try:
-            encryption_client = EncryptionClient(self.ENCRYPTION_KEY)
-            secret_email = encryption_client.encrypt(self.email)
-            secret_passwd = encryption_client.encrypt(self.passwd)
-            secret_dob = encryption_client.encrypt(self.dob)
-            self.login_payload["body"]["Email_id"] = secret_email
-            self.login_payload["body"]["Password"] = secret_passwd
-            self.login_payload["body"]["My2PIN"] = secret_dob
-            self.login_payload["head"]["requestCode"] = "5PLoginV4"
-            self.login_payload["head"]["appName"] = self.APP_NAME
-            self.login_payload["head"]["key"] = self.USER_KEY
-            self.login_payload["head"]["userId"] = self.USER_ID
-            self.login_payload["head"]["password"] = self.PASSWORD
-            res = self._login_request(self.LOGIN_ROUTE)
-
-            message = res["body"]["Message"]
-            if message == "":
-                log_response("Logged in!!")
-            else:
-                log_response(message)
-            self._set_client_code(res["body"]["ClientCode"])
-        except Exception as e:
-            log_response(e)
-
     def holdings(self):
         try:
             return self._user_info_request("HOLDINGS")
         except Exception as e:
             log_response(e)
 
     def margin(self):
@@ -175,14 +147,18 @@
                 self.payload["head"]["requestCode"] = "5PTrdInfo"
             elif req_type == "TH":
                 url = self.TRADE_HISTORY_ROUTE
             elif req_type == "MF":
                 url = self.MARKET_FEED_ROUTE
                 self.payload["head"]["requestCode"] = "5PMF"
                 self.payload["body"]["COUNT"] = self.client_code
+            elif req_type == "MF1":
+                url = self.MARKET_FEED_ROUTE_BY_SCRIP
+                self.payload["head"]["requestCode"] = "5PMF"
+                self.payload["body"]["COUNT"] = self.client_code
             elif req_type == "BM":
                 url = self.BRACKET_MOD_ROUTE
                 # self.payload["head"]["requestCode"] = "5PSModMOOrd"
                 # self.payload["body"]["legtype"]=0
                 # self.payload["body"]["TMOPartnerOrderID"]=0
             elif req_type == "CM":
                 url = self.COVER_MOD_ROUTE
@@ -201,14 +177,17 @@
                 url = self.COVER_CANCEL_ROUTE
             elif req_type == "MD":
                 url = self.MARKET_DEPTH_ROUTE
                 # self.payload["head"]["requestCode"] = "5PMD"
             elif req_type == "MDS":
                 url = self.MARKET_DEPTH_BY_SYMBOL_ROUTE
                 # self.payload["head"]["requestCode"] = "5PMD"
+            elif req_type == "MDSC":
+                url = self.MARKET_DEPTH_BY_SCRIP
+                # self.payload["head"]["requestCode"] = "5PMD"
             elif req_type == "TB":
                 url = self.TRADEBOOK_ROUTE
                 # self.payload["head"]["requestCode"] = "5PTrdBkV1"
             elif req_type == "GB":
                 url = self.GET_BASKET_ROUTE
             elif req_type == "CB":
                 url = self.CREATE_BASKET_ROUTE
@@ -276,27 +255,48 @@
             self.payload["body"]["Count"] = "1"
             self.payload["body"]["Data"] = req_list
 
             return self.order_request("MDS")
         except Exception as e:
             log_response(e)
 
+    def fetch_market_depth_by_scrip(self, **param):
+        try:
+            self.payload["body"]["ClientCode"] = self.client_code
+            self.set_payload(param)
+            return self.order_request("MDSC")
+        except Exception as e:
+            log_response(e)
+
     def fetch_market_feed(self, req_list: list):
         """
             market feed api
         """
         try:
             self.payload["body"]["MarketFeedData"] = req_list
             self.payload["body"]["ClientLoginType"] = 0
             self.payload["body"]["LastRequestTime"] = f"/Date({TODAY_TIMESTAMP})/"
             self.payload["body"]["RefreshRate"] = "H"
             return self.order_request("MF")
         except Exception as e:
             log_response(e)
 
+    def fetch_market_feed_scrip(self, req_list: list):
+        """
+            market feed api
+        """
+        try:
+            self.payload["body"]["MarketFeedData"] = req_list
+            self.payload["body"]["ClientLoginType"] = 0
+            self.payload["body"]["LastRequestTime"] = f"/Date({TODAY_TIMESTAMP})/"
+            self.payload["body"]["RefreshRate"] = "H"
+            return self.order_request("MF1")
+        except Exception as e:
+            log_response(e)
+
     def set_payload(self, order) -> None:
         try:
             for key, value in order.items():
                 self.payload["body"][key] = value
         except Exception as e:
             log_response(e)
 
@@ -421,31 +421,31 @@
                 return self.order_request("BC")
         except Exception as e:
             log_response(e)
 
     def cover_order(self, **order):
         try:
             self.set_payload(order)
-           # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
+            # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
             return self.order_request("CO")
         except Exception as e:
             log_response(e)
 
     def modify_cover_order(self, **order):
         try:
             self.set_payload(order)
-           # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
+            # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
             return self.order_request("CM")
         except Exception as e:
             log_response(e)
 
     def cancel_cover_order(self, **order):
         try:
             self.set_payload(order)
-           # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
+            # self.payload["body"]["TriggerPriceForSL"] = order.stoploss_price
             return self.order_request("CC")
         except Exception as e:
             log_response(e)
 
     def Request_Feed(self, Method: str, Operation: str, req_list: list):
         try:
             Method_dict = {"mf": "MarketFeedV3", "md": "MarketDepthService",
@@ -530,15 +530,15 @@
             log_response(e)
 
     def historical_data(self, Exch: str, ExchangeSegment: str, ScripCode: int, time: str, From: str, To: str):
         try:
             self.jwt_headers['x-clientcode'] = self.client_code
             self.jwt_headers['x-auth-token'] = self.Jwt_token
             url = f'{self.HISTORICAL_DATA_ROUTE}{Exch}/{ExchangeSegment}/{ScripCode}/{time}?from={From}&end={To}'
-            timeList = ['1m', '3m','5m', '10m', '15m', '30m', '60m', '1d']
+            timeList = ['1m', '3m', '5m', '10m', '15m', '30m', '60m', '1d']
             if time not in timeList:
                 return 'Invalid Time Frame. it should be within [1m,5m,10m,15m,30m,60m,1d].'
             else:
                 response = self.session.get(
                     url, headers=self.jwt_headers).json()
                 candleList = response['data']['candles']
                 df = pd.DataFrame(candleList)
@@ -601,14 +601,15 @@
             self.BRACKET_MOD_ROUTE = BRACKET_MOD_ROUTE
             self.BRACKET_ORDER_ROUTE = BRACKET_ORDER_ROUTE
             self.BRACKET_CANCEL_ROUTE = BRACKET_CANCEL_ROUTE
             self.COVER_MOD_ROUTE = COVER_MOD_ROUTE
             self.COVER_ORDER_ROUTE = COVER_ORDER_ROUTE
             self.COVER_CANCEL_ROUTE = COVER_CANCEL_ROUTE
             self.MARKET_FEED_ROUTE = MARKET_FEED_ROUTE
+            self.MARKET_FEED_ROUTE_BY_SCRIP = MARKET_FEED_ROUTE_BY_SCRIP
             self.LOGIN_CHECK_ROUTE = LOGIN_CHECK_ROUTE
             self.MARKET_DEPTH_ROUTE = MARKET_DEPTH_ROUTE
             self.JWT_VALIDATION_ROUTE = JWT_VALIDATION_ROUTE
             self.HISTORICAL_DATA_ROUTE = HISTORICAL_DATA_ROUTE
             self.IDEAS_ROUTE = IDEAS_ROUTE
             self.TRADEBOOK_ROUTE = TRADEBOOK_ROUTE
             self.ACCESS_TOKEN_ROUTE = ACCESS_TOKEN_ROUTE
@@ -626,14 +627,15 @@
             self.OPTION_CHAIN_ROUTE = OPTION_CHAIN_ROUTE
             self.GET_OPTION_CHAIN_ROUTE = GET_OPTION_CHAIN_ROUTE
             self.CANCEL_BULK_ORDER_ROUTE = CANCEL_BULK_ORDER_ROUTE
             self.SQUAREOFF_ROUTE = SQUAREOFF_ROUTE
             self.MARKET_DEPTH_ROUTE_20 = MARKET_DEPTH_ROUTE_20
             self.POSITION_CONVERSION_ROUTE = POSITION_CONVERSION_ROUTE
             self.MARKET_DEPTH_BY_SYMBOL_ROUTE = MARKET_DEPTH_BY_SYMBOL_ROUTE
+            self.MARKET_DEPTH_BY_SCRIP = MARKET_DEPTH_BY_SCRIP
         except Exception as e:
             log_response(e)
 
     def create_payload(self):
         try:
             self.payload = GENERIC_PAYLOAD
             self.login_payload = LOGIN_PAYLOAD
@@ -682,15 +684,15 @@
             url = GET_REQUEST_TOKEN_ROUTE
 
             res = self.session.post(url, json=self.payload).json()
             message = res["body"]["Status"]
 
             if message == 0:
                 self.request_token = res["body"]["RequestToken"]
-                log_response("RequestToken: "+self.request_token)
+                log_response("RequestToken: " + self.request_token)
                 return self.request_token
             else:
                 log_response(res["body"])
         except Exception as e:
             log_response(e)
 
     def get_totp_session(self, client_code, totp, pin):
@@ -809,15 +811,15 @@
     def squareoff_all(self):
         try:
             if self.client_code != None:
                 return self.order_request("SO")
         except Exception as e:
             log_response(e)
 
-    def position_convertion(self, Exch: str, ExchType: str, ScripData: str, TradeType: str, ConvertQty: int, ConvertFrom: str, ConvertTo: str):
+    def position_convertion(self, Exch: str, ExchType: str, ScripData: str, TradeType: str, ConvertQty: int,ConvertFrom: str, ConvertTo: str):
         try:
             if self.client_code != None:
                 self.payload["body"]["Exch"] = Exch
                 self.payload["body"]["ExchType"] = ExchType
                 self.payload["body"]["ScripData"] = ScripData
                 self.payload["body"]["TradeType"] = TradeType
                 self.payload["body"]["ConvertQty"] = ConvertQty
```

### Comparing `py5paisa-0.7.1/py5paisa/strategy.py` & `py5paisa-0.7.2/py5paisa/strategy.py`

 * *Files identical despite different names*

### Comparing `py5paisa-0.7.1/py5paisa/urlconst.py` & `py5paisa-0.7.2/py5paisa/urlconst.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 BaseUrl = 'https://Openapi.5paisa.com/VendorsAPI/Service1.svc/'
 
 
 LOGIN_ROUTE = f'{BaseUrl}V4/LoginRequestMobileNewbyEmail'
 
-MARGIN_ROUTE = f'{BaseUrl}V3/Margin'
-ORDER_BOOK_ROUTE = f'{BaseUrl}V2/OrderBook'
+MARGIN_ROUTE = f'{BaseUrl}V4/Margin'
+ORDER_BOOK_ROUTE = f'{BaseUrl}V3/OrderBook'
 HOLDINGS_ROUTE = f'{BaseUrl}V3/Holding'
-POSITIONS_ROUTE = f'{BaseUrl}V1/NetPositionNetWise'
+POSITIONS_ROUTE = f'{BaseUrl}V2/NetPositionNetWise'
 
 ORDER_PLACEMENT_ROUTE = f'{BaseUrl}V1/PlaceOrderRequest'
 ORDER_MODIFY_ROUTE = f'{BaseUrl}V1/ModifyOrderRequest'
 ORDER_CANCEL_ROUTE = f'{BaseUrl}V1/CancelOrderRequest'
 ORDER_STATUS_ROUTE = f'{BaseUrl}V2/OrderStatus'
 TRADE_INFO_ROUTE = f'{BaseUrl}TradeInformation'
 
@@ -20,28 +20,30 @@
 BRACKET_CANCEL_ROUTE = f'{BaseUrl}CancelBracketOrderRequest'
 
 COVER_MOD_ROUTE = f'{BaseUrl}ModifyCoverOrderequest'
 COVER_ORDER_ROUTE = f'{BaseUrl}CoverOrderRequest'
 COVER_CANCEL_ROUTE = f'{BaseUrl}CancelCoverOrderRequest'
 
 MARKET_FEED_ROUTE = f'{BaseUrl}MarketFeed'
+MARKET_FEED_ROUTE_BY_SCRIP = f'{BaseUrl}V1/MarketFeed'
 LOGIN_CHECK_ROUTE = "https://openfeed.5paisa.com/Feeds/api/UserActivity/LoginCheck"
 
 MARKET_DEPTH_ROUTE = f'{BaseUrl}/MarketDepth'
 MARKET_DEPTH_BY_SYMBOL_ROUTE = f'{BaseUrl}V1/MarketDepth'
+MARKET_DEPTH_BY_SCRIP = f'{BaseUrl}V2/MarketDepth'
 JWT_VALIDATION_ROUTE = "https://Openapi.indiainfoline.com/VendorsAPI/Service1.svc/JWTOpenApiValidation"
 HISTORICAL_DATA_ROUTE = "https://openapi.5paisa.com/historical/"
 
 IDEAS_ROUTE = f'{BaseUrl}TraderIDEAs'
 
 TRADEBOOK_ROUTE = f'{BaseUrl}V1/TradeBook'
 GET_REQUEST_TOKEN_ROUTE = f'{BaseUrl}TOTPLogin'
 ACCESS_TOKEN_ROUTE = f'{BaseUrl}GetAccessToken'
 MARKET_STATUS_ROUTE = f'{BaseUrl}MarketStatus'
-TRADE_HISTORY_ROUTE = f'{BaseUrl}TradeHistory'
+TRADE_HISTORY_ROUTE = f'{BaseUrl}V1/TradeHistory'
 
 GET_BASKET_ROUTE = f'{BaseUrl}GetBaskets'
 CREATE_BASKET_ROUTE = f'{BaseUrl}CreateBasket'
 RENAME_BASKET_ROUTE = f'{BaseUrl}EditBasketName'
 DELETE_BASKET_ROUTE = f'{BaseUrl}DeleteBasket'
 CLONE_BASKET_ROUTE = f'{BaseUrl}CloneBasket'
 EXECUTE_BASKET_ROUTE = f'{BaseUrl}ExecuteBasket'
```

### Comparing `py5paisa-0.7.1/py5paisa.egg-info/PKG-INFO` & `py5paisa-0.7.2/py5paisa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py5paisa
-Version: 0.7.1
+Version: 0.7.2
 Summary:  Python SDK for 5paisa APIs natively written in VB.NET
 Home-page: https://github.com/5paisa/py5paisa
 Author: 5paisa
 Author-email: coreteam@5paisa.com
 Keywords: py5paisa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -56,29 +56,30 @@
     "APP_NAME":"YOUR APP_NAME",
     "APP_SOURCE":"YOUR APP_SOURCE",
     "USER_ID":"YOUR USER_ID",
     "PASSWORD":"YOUR PASSWORD",
     "USER_KEY":"YOUR USERKEY",
     "ENCRYPTION_KEY":"YOUR ENCRYPTION_KEY"
     }
-# First get a token by logging in to -> https://dev-openapi.5paisa.com/WebVendorLogin/VLogin/Index?VendorKey=<Your Vendor Key>&ResponseURL=<Redirect URL>
-# VendorKey is UesrKey for individuals user
-# for e.g. you can use ResponseURL as https://www.5paisa.com/technology/developer-apis
-# Pass the token received in the response url after successful login to get an access token (this also sets the token for all the APIs you use)-
-
-# Please note that you need to copy the request token from URL and paste in this code and start the code within 30s.
 
 #This function will automatically take care of generating and sending access token for all your API's
 
 client = FivePaisaClient(cred=cred)
 
 # New TOTP based authentication
 client.get_totp_session('Your ClientCode','TOTP from authenticator app','Your Pin')
 
-# If you have the have the token(OAUTH Approach)
+# OAUTH Approach
+# First get a token by logging in to -> https://dev-openapi.5paisa.com/WebVendorLogin/VLogin/Index?VendorKey=<Your Vendor Key>&ResponseURL=<Redirect URL>
+# VendorKey is UesrKey for individuals user
+# for e.g. you can use ResponseURL as https://www.5paisa.com/technology/developer-apis
+# Pass the token received in the response url after successful login to get an access token (this also sets the token for all the APIs you use)-
+
+# Please note that you need to copy the request token from URL and paste in this code and start the code within 30s.
+
 client.get_oauth_session('Your Response Token')
 
 After successful authentication, you should get a `Logged in!!` message in console
 ```
 
 #### Market Feed
 
@@ -334,22 +335,30 @@
 def on_message(ws, message):
     print(message)
 client.receive_data(on_message)
 
 Note:- Instruments in payload above is a list(array) in format as <exchange><exchange type><scrip code>
 ```
 
+#### Level 5 Market Depth 
+```py
+print(client.fetch_market_depth_by_scrip(Exchange="N",ExchangeType="C",ScripCode="1660"))
+print(client.fetch_market_depth_by_scrip(Exchange="N",ExchangeType="C",ScripData="RELIANCE_EQ"))
+```
+
 #### Full Market Snapshot 
 ```py
 a=[{"Exchange":"N","ExchangeType":"C","ScripCode":"2885"},
    {"Exchange":"N","ExchangeType":"C","ScripCode":"1660"},
    ]
 print(client.fetch_market_depth(a))
 ```
 
+
+
 #### Full Market Snapshot(By Symbol)
 ```py
 a=[{"Exchange":"N","ExchangeType":"C","Symbol":"ITC"},
    {"Exchange":"N","ExchangeType":"D","Symbol":"BANKNIFTY 31 Feb 2022 CE 41600.00"},
    ]
 print(client.fetch_market_depth_by_symbol(a))
 ```
```

### Comparing `py5paisa-0.7.1/setup.py` & `py5paisa-0.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,10 +45,10 @@
     keywords='py5paisa',
     name='py5paisa',
     packages=find_packages(include=['py5paisa', 'py5paisa.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/5paisa/py5paisa',
-    version='0.7.1',
+    version='0.7.2',
     zip_safe=False,
 )
```

