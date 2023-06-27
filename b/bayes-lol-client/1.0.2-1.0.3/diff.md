# Comparing `tmp/bayes_lol_client-1.0.2.tar.gz` & `tmp/bayes_lol_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayes_lol_client-1.0.2.tar", max compression
+gzip compressed data, was "bayes_lol_client-1.0.3.tar", max compression
```

## Comparing `bayes_lol_client-1.0.2.tar` & `bayes_lol_client-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      221 2023-06-05 01:27:21.470972 bayes_lol_client-1.0.2/bayes_lol_client/__init__.py
--rw-r--r--   0        0        0     8917 2023-06-05 01:29:40.964470 bayes_lol_client-1.0.2/bayes_lol_client/api.py
--rw-r--r--   0        0        0     6521 2023-06-05 01:29:44.616481 bayes_lol_client-1.0.2/bayes_lol_client/emh.py
--rw-r--r--   0        0        0      567 2023-06-05 01:27:21.472972 bayes_lol_client-1.0.2/bayes_lol_client/errors.py
--rw-r--r--   0        0        0     5158 2023-06-05 01:27:21.473973 bayes_lol_client-1.0.2/bayes_lol_client/historic.py
--rw-r--r--   0        0        0      990 2023-06-05 01:27:21.473973 bayes_lol_client-1.0.2/bayes_lol_client/sleep.py
--rw-r--r--   0        0        0     1866 2023-06-05 01:27:21.474973 bayes_lol_client-1.0.2/bayes_lol_client/utils.py
--rw-r--r--   0        0        0    35821 2023-06-05 01:27:21.469971 bayes_lol_client-1.0.2/LICENSE
--rw-r--r--   0        0        0      466 2023-06-05 01:27:43.601824 bayes_lol_client-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      649 2023-06-05 01:27:21.469971 bayes_lol_client-1.0.2/README.md
--rw-r--r--   0        0        0     1371 1970-01-01 00:00:00.000000 bayes_lol_client-1.0.2/setup.py
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 bayes_lol_client-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-06-05 04:15:53.821982 bayes_lol_client-1.0.3/bayes_lol_client/__init__.py
+-rw-r--r--   0        0        0     8607 2023-06-27 08:38:36.641538 bayes_lol_client-1.0.3/bayes_lol_client/api.py
+-rw-r--r--   0        0        0     6514 2023-06-05 04:36:35.002904 bayes_lol_client-1.0.3/bayes_lol_client/emh.py
+-rw-r--r--   0        0        0      942 2023-06-27 07:09:49.643960 bayes_lol_client-1.0.3/bayes_lol_client/errors.py
+-rw-r--r--   0        0        0     5158 2023-06-05 01:27:21.473973 bayes_lol_client-1.0.3/bayes_lol_client/historic.py
+-rw-r--r--   0        0        0      990 2023-06-05 01:27:21.473973 bayes_lol_client-1.0.3/bayes_lol_client/sleep.py
+-rw-r--r--   0        0        0     2123 2023-06-27 08:35:45.509815 bayes_lol_client-1.0.3/bayes_lol_client/utils.py
+-rw-r--r--   0        0        0    35821 2023-06-05 01:27:21.469971 bayes_lol_client-1.0.3/LICENSE
+-rw-r--r--   0        0        0      466 2023-06-27 08:45:04.668885 bayes_lol_client-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      745 2023-06-05 04:18:26.099536 bayes_lol_client-1.0.3/README.md
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 bayes_lol_client-1.0.3/setup.py
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 bayes_lol_client-1.0.3/PKG-INFO
```

### Comparing `bayes_lol_client-1.0.2/bayes_lol_client/api.py` & `bayes_lol_client-1.0.3/bayes_lol_client/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ReadTimeout,
     HTTPError,
 )
 import json
 from datetime import datetime, timedelta
 import os
 from bayes_lol_client.sleep import Sleepers, Sleeper
-from typing import NoReturn, Any
+from typing import NoReturn, Any, Callable
 from bayes_lol_client.errors import (
     ClientError,
     ServerError,
     NotFoundError,
     TooManyRequests,
     UnauthorizedError,
 )
@@ -136,86 +136,71 @@
 
     @staticmethod
     def make_http_exception_from_status_code(response: requests.Response):
         return HTTPError(
             f"{response.status_code} for url {response.url}", response=response
         )
 
+    @staticmethod
     def sleep_and_retry(
-        self,
-        sleeper: Sleeper,
-        method: str,
-        service: str,
-        endpoint: str,
-        data: dict = None,
-        exception: Exception = None,
-        sleep_time: int = None,
+            sleeper: Sleeper,
+            callback: Callable,
+            exception: Exception = None,
+            sleep_time: int = None,
+            **kwargs
     ):
         sleeper.sleep(exception, sleep_time)
-        return self.do_api_call(
-            method,
-            service,
-            data,
-            ensure_login=False,
+        return callback(
+            **kwargs,
             sleeper=sleeper,
-            endpoint=endpoint,
         )
 
     def handle_response(
-        self,
-        sleeper: Sleeper,
-        response: requests.Response,
-        method: str,
-        service: str,
-        allow_retry: bool,
-        endpoint: str,
-        data: dict = None,
+            self,
+            sleeper: Sleeper,
+            response: requests.Response,
+            allow_retry: bool,
+            callback: Callable,
+            return_json: bool = True,
+            **kwargs,
     ):
         if response.status_code == 401:
             raise UnauthorizedError(response.status_code)
         elif response.status_code == 429:
             if not allow_retry or not self.wait_on_ratelimit:
                 raise TooManyRequests(response.status_code)
-            if "x-rate-limit-retry-after-seconds" in response.headers:
-                sleep_time = int(response.headers["x-rate-limit-retry-after-seconds"])
-            else:
-                sleep_time = None
             return self.sleep_and_retry(
-                method=method,
                 sleeper=sleeper,
-                service=service,
-                data=data,
                 exception=self.make_http_exception_from_status_code(response),
-                sleep_time=sleep_time,
-                endpoint=endpoint,
+                callback=callback,
+                **kwargs
             )
         elif response.status_code == 404:
             raise NotFoundError(response.status_code)
         elif response.status_code >= 500:
             if not allow_retry:
                 raise ServerError(response.status_code)
             return self.sleep_and_retry(
-                method=method,
                 sleeper=sleeper,
-                service=service,
-                data=data,
                 exception=self.make_http_exception_from_status_code(response),
-                endpoint=endpoint,
+                callback=callback,
+                **kwargs
             )
         elif 499 >= response.status_code >= 400:
             raise ClientError(response.status_code)
         response.raise_for_status()
-        return response.json()
+        if return_json:
+            return response.json()
+        return response
 
     def do_api_call(
         self,
         method: str,
         service: str,
         data: dict = None,
-        *,
         allow_retry: bool = True,
         ensure_login: bool = True,
         sleeper: Sleeper = None,
         endpoint: str = None,
     ) -> Any:
         if not sleeper:
             sleeper = self.sleepers.make()
@@ -236,24 +221,28 @@
             ConnectTimeout,
             Timeout,
             ReadTimeout,
         ) as e:
             if not allow_retry:
                 raise e
             return self.sleep_and_retry(
-                method=method,
                 sleeper=sleeper,
+                exception=e,
+                callback=self.do_api_call,
+                method=method,
                 service=service,
                 data=data,
-                exception=e,
                 endpoint=endpoint,
+                ensure_login=False
             )
 
         return self.handle_response(
             method=method,
             service=service,
             data=data,
             sleeper=sleeper,
             response=response,
             allow_retry=allow_retry,
             endpoint=endpoint,
+            callback=self.do_api_call,
+            ensure_login=False
         )
```

### Comparing `bayes_lol_client-1.0.2/bayes_lol_client/emh.py` & `bayes_lol_client-1.0.3/bayes_lol_client/emh.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from requests import Response
 from datetime import datetime
 
 
 class BayesEMH(object):
     """
     This class makes requests to the /emh/v1 endpoint in the Bayes API.
-    Useful to get summary/details/replay files for professional games
+    Useful to get summary/details/replay files of professional games
     """
 
     endpoint = "https://lolesports-api.bayesesports.com/emh/v1/"
     DEFAULT_MAX_PAGE_SIZE = 500
 
     def __init__(
         self,
@@ -42,15 +42,15 @@
         return self.get_asset(platform_game_id, "GAMH_SUMMARY").json()
 
     def get_game_details(self, platform_game_id: str) -> dict:
         """
         Returns the game details (timeline) as a json file
 
         :param platform_game_id: A Riot esports game ID
-        :return: The game details as a json file
+        :return: The game details (timeline) as a json file
         """
         return self.get_asset(platform_game_id, "GAMH_DETAILS").json()
 
     def get_game_replay(self, platform_game_id: str) -> bytes:
         """
         Returns a replay file as bytes which can later be saved locally
 
@@ -128,22 +128,20 @@
         to_timestamp: Optional[Union[datetime, int, float]] = None,
         limit: Optional[int] = None,
         team1: Optional[str] = None,
         team2: Optional[str] = None,
         max_page_size: Optional[int] = None,
     ) -> list:
         """
-        Gets a list of games which can be filtered using the different function arguments
+        Gets a list of games which can be filtered using the different function parameters
         If no limit is specified, the function will make multiple requests and return every matched game
 
         :param tags: Only return games containing these tags, as a comma-separated string, or a list
-        :param from_timestamp: Only return games after this moment, can be a unix epoch timestamp as int or float, or a
-        datetime object
-        :param to_timestamp: Only return games before this moment, can be a unix epoch timestamp as int or float, or a
-        datetime object
+        :param from_timestamp: Only return games after this moment, can be a unix epoch timestamp as int or float, or a datetime object
+        :param to_timestamp: Only return games before this moment, can be a unix epoch timestamp as int or float, or a datetime object
         :param limit: Maximum number of games to return
         :param team1: Only return games where this team played, this should be the team tricode
         :param team2: Only return games where this team and team1 played, this should be the team tricode
         :param max_page_size: Maximum size for each request, this is only useful for tweaking performance
         :return: A dict of games with the ID as a key and metadata for each one
         """
         if max_page_size is None:
```

### Comparing `bayes_lol_client-1.0.2/bayes_lol_client/historic.py` & `bayes_lol_client-1.0.3/bayes_lol_client/historic.py`

 * *Files identical despite different names*

### Comparing `bayes_lol_client-1.0.2/bayes_lol_client/sleep.py` & `bayes_lol_client-1.0.3/bayes_lol_client/sleep.py`

 * *Files identical despite different names*

### Comparing `bayes_lol_client-1.0.2/bayes_lol_client/utils.py` & `bayes_lol_client-1.0.3/bayes_lol_client/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,25 @@
         JSONDecodeError,
         ConnectionError,
         ConnectTimeout,
         Timeout,
         ReadTimeout,
         HTTPError,
     ) as e:
-        sleeper.sleep(exception=e)
-        return download_game_asset(api=api, asset_url=asset_url, sleeper=sleeper)
-    return response
+        return api.sleep_and_retry(sleeper=sleeper, callback=download_game_asset, exception=e, api=api,
+                                   asset_url=asset_url)
+    return api.handle_response(
+        sleeper=sleeper,
+        response=response,
+        allow_retry=True,
+        callback=download_game_asset,
+        api=api,
+        asset_url=asset_url,
+        return_json=False
+    )
 
 
 def get_list(
     api: BayesAPIClient, params: dict, service: str, limit: int, key: str
 ) -> list:
     ret = []
     while True:
```

### Comparing `bayes_lol_client-1.0.2/LICENSE` & `bayes_lol_client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bayes_lol_client-1.0.2/README.md` & `bayes_lol_client-1.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Bayes LoL Client
 
 This library is used to make queries to the Bayes EMH API, which provides data for League of Legends esports games.
+The (in progress) documentation can be found [here](https://bayes-lol-client.readthedocs.io).
 
 ## Install
 ```
 pip install bayes_lol_client
 ```
 
 If you wish to install the latest development version:
@@ -13,8 +14,8 @@
 ```
 
 ## Bayes Credentials
 In order to use the Bayes API, you must have login credentials, which will be prompted the first time you use the library.
 These will be stored in a file in your user config path.
 
 ## EMH Docs
-The full documentation to use EMH can be found [here](https://docs.bayesesports.com/api/emh_riot)
+The full documentation to use EMH can be found [here](https://docs.bayesesports.com/api/emh_riot).
```

### Comparing `bayes_lol_client-1.0.2/setup.py` & `bayes_lol_client-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pytz>=2022.7,<2023.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'bayes-lol-client',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'Wrapper for Bayes League of Legends API',
-    'long_description': '# Bayes LoL Client\n\nThis library is used to make queries to the Bayes EMH API, which provides data for League of Legends esports games.\n\n## Install\n```\npip install bayes_lol_client\n```\n\nIf you wish to install the latest development version:\n```\npip install -U git+https://github.com/arbolitoloco1/bayes_lol_client\n```\n\n## Bayes Credentials\nIn order to use the Bayes API, you must have login credentials, which will be prompted the first time you use the library.\nThese will be stored in a file in your user config path.\n\n## EMH Docs\nThe full documentation to use EMH can be found [here](https://docs.bayesesports.com/api/emh_riot)',
+    'long_description': '# Bayes LoL Client\n\nThis library is used to make queries to the Bayes EMH API, which provides data for League of Legends esports games.\nThe (in progress) documentation can be found [here](https://bayes-lol-client.readthedocs.io).\n\n## Install\n```\npip install bayes_lol_client\n```\n\nIf you wish to install the latest development version:\n```\npip install -U git+https://github.com/arbolitoloco1/bayes_lol_client\n```\n\n## Bayes Credentials\nIn order to use the Bayes API, you must have login credentials, which will be prompted the first time you use the library.\nThese will be stored in a file in your user config path.\n\n## EMH Docs\nThe full documentation to use EMH can be found [here](https://docs.bayesesports.com/api/emh_riot).',
     'author': 'Santiago Kozak',
     'author_email': 'kozaksantiago@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/arbolitoloco1/bayes_lol_client',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bayes_lol_client-1.0.2/PKG-INFO` & `bayes_lol_client-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayes-lol-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Wrapper for Bayes League of Legends API
 Home-page: https://github.com/arbolitoloco1/bayes_lol_client
 License: GPL-3.0-or-later
 Author: Santiago Kozak
 Author-email: kozaksantiago@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -15,14 +15,15 @@
 Requires-Dist: pytz (>=2022.7,<2023.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Bayes LoL Client
 
 This library is used to make queries to the Bayes EMH API, which provides data for League of Legends esports games.
+The (in progress) documentation can be found [here](https://bayes-lol-client.readthedocs.io).
 
 ## Install
 ```
 pip install bayes_lol_client
 ```
 
 If you wish to install the latest development version:
@@ -31,8 +32,8 @@
 ```
 
 ## Bayes Credentials
 In order to use the Bayes API, you must have login credentials, which will be prompted the first time you use the library.
 These will be stored in a file in your user config path.
 
 ## EMH Docs
-The full documentation to use EMH can be found [here](https://docs.bayesesports.com/api/emh_riot)
+The full documentation to use EMH can be found [here](https://docs.bayesesports.com/api/emh_riot).
```

