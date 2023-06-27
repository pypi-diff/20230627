# Comparing `tmp/wglestaapi-0.2.0.tar.gz` & `tmp/wglestaapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wglestaapi-0.2.0.tar", max compression
+gzip compressed data, was "wglestaapi-0.3.0.tar", max compression
```

## Comparing `wglestaapi-0.2.0.tar` & `wglestaapi-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1100 2022-11-21 11:20:18.922796 wglestaapi-0.2.0/LICENSE
--rw-r--r--   0        0        0      506 2022-11-22 10:21:10.597380 wglestaapi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4826 2022-11-22 10:47:48.866898 wglestaapi-0.2.0/README.md
--rw-r--r--   0        0        0     3076 2022-11-21 11:20:18.927836 wglestaapi-0.2.0/WgLestaAPI/__init__.py
--rw-r--r--   0        0        0     6756 2022-11-22 10:18:17.252250 wglestaapi-0.2.0/WgLestaAPI/Application.py
--rw-r--r--   0        0        0     3534 2022-11-22 10:21:45.679912 wglestaapi-0.2.0/WgLestaAPI/Constants.py
--rw-r--r--   0        0        0      830 2022-11-21 11:20:18.926841 wglestaapi-0.2.0/WgLestaAPI/Exceptions.py
--rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 wglestaapi-0.2.0/setup.py
--rw-r--r--   0        0        0     5578 1970-01-01 00:00:00.000000 wglestaapi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2022-11-19 16:52:14.188783 wglestaapi-0.3.0/LICENSE
+-rw-r--r--   0        0        0      506 2023-06-27 15:28:57.887296 wglestaapi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5382 2023-06-27 15:36:58.473289 wglestaapi-0.3.0/README.md
+-rw-r--r--   0        0        0     3496 2023-06-27 15:28:36.418696 wglestaapi-0.3.0/WgLestaAPI/__init__.py
+-rw-r--r--   0        0        0     6743 2023-06-27 15:34:16.975443 wglestaapi-0.3.0/WgLestaAPI/aio.py
+-rw-r--r--   0        0        0     7538 2023-06-27 14:06:00.860469 wglestaapi-0.3.0/WgLestaAPI/Application.py
+-rw-r--r--   0        0        0     3534 2022-11-22 13:35:17.876100 wglestaapi-0.3.0/WgLestaAPI/Constants.py
+-rw-r--r--   0        0        0      830 2022-11-20 16:54:25.875887 wglestaapi-0.3.0/WgLestaAPI/Exceptions.py
+-rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 wglestaapi-0.3.0/setup.py
+-rw-r--r--   0        0        0     6112 1970-01-01 00:00:00.000000 wglestaapi-0.3.0/PKG-INFO
```

### Comparing `wglestaapi-0.2.0/LICENSE` & `wglestaapi-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `wglestaapi-0.2.0/README.md` & `wglestaapi-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,102 @@
 # WgLestaAPI
 
-Unofficial Python library that facilitates working with **<a href="https://developers.wargaming.net"><img src="https://developers.wargaming.net/static/1.12.2/assets/img/favicon.ico" width=15px> API Wargaming.net</a>** and **<a href="https://developers.lesta.ru"><img src="https://developers.lesta.ru/static/1.13.1_lst/assets/img/favicon.ico" width=15px> API Lesta Games</a>** functionality via **Python**.
+Unofficial Python library that facilitates working with **<a href="https://developers.wargaming.net"><img src="docs/icons/wg.ico" width=15px> API Wargaming.net</a>** and **<a href="https://developers.lesta.ru"><img src="docs/icons/lesta.ico" width=15px> API Lesta Games</a>** functionality via **Python**.
 
 [![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/wglestaapi)
 [![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month)](https://pepy.tech/project/wglestaapi)
 [![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week)](https://pepy.tech/project/wglestaapi)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/wglestaapi)](https://pypi.org/project/wglestaapi)
 [![Version](https://img.shields.io/pypi/v/wglestaapi?color=success)](https://pypi.org/project/wglestaapi)
 [![](https://img.shields.io/pypi/format/wglestaapi)](https://pypi.org/project/wglestaapi)
 [![](https://img.shields.io/pypi/wheel/wglestaapi)](https://pypi.org/project/wglestaapi)
 [![GitHub Repo stars](https://img.shields.io/github/stars/tankalxat34/wglestaapi?style=social)](https://github.com/tankalxat34/wglestaapi)
 
-By downloading this library you fully agree with all official documents **Lesta Games** and **Wargaming.net** about **Lesta Games** and **Wargaming.net** products. *The author of the library (Alexander Podstrechny) is not responsible for your actions performed with the help of this program code.*
+By downloading this library you fully agree with all official documents **Lesta Games** and **Wargaming.net** about **Lesta Games** and **Wargaming.net** products. *The author of the library ([Alexander Podstrechny](https://github.com/tankalxat34)) is not responsible for your actions performed with the help of this program code.*
 
 ## Installing the library
 
 Run the command below at the command line
 
 ```
 pip install WgLestaAPI
 ```
 
 ## Example of use
 
+### Async way
+
+`main.py` contains:
+```py
+from WgLestaAPI import aio
+import asyncio
+
+method = aio.Method("account.info", "wot", account_id=563982544, application_id="your_app_id")
+
+response = asyncio.run(method.execute())
+
+print(response)
+```
+
+`output` is:
+```json
+{"status": "ok", "meta": {"count": 1}, "data": {"563982544": {"client_language": "", "last_battle_time": 1569011404, "account_id": 563982544, "created_at": 1564320823, "updated_at": 1686648157, ... "tanking_factor": 0.0}, "frags": None}, "nickname": "tankalxat34", "logout_at": 1597741881}
+```
+
+### No-async way
+
 ```py
 from WgLestaAPI import Application
 
 # Creating a Query with your application_id
 query = Application.Query(application_id=APP_ID)
 
 # Adding the necessary parameters
 query.extend(search="tank", limit=5)
 
-# Creating the method `account.list` of the game Tanks Blitz on the RU-region with the passed parameters
+# Creating the method `account.list` of the game World of Tanks Blitz on the EU-region with the passed parameters
 m = Application.Method("account.list", game_shortname="wotb", query=query, region="eu")
 
 # Executing the method
 mExecuted = m.execute()
 
-# Your server response processing
+# Your handing of server response
 print(mExecuted["data"][0]["account_id"]) # 58114596
 
 # If you wish, you can follow a link to the official website of the API owner with documentation
 print(m.docs) # https://developers.wargaming.net/reference/all/wotb/account/list/
 ```
 
 ## Library functionality
 
-The library implements the basic functions of **API Lesta Games** and **API Wargaming.net**. All requests are made through your application, which you previously created on [Lesta Games](https://developers.lesta.ru/applications/) or on [Wargaming.net](https://developers.wargaming.net/applications/). Some features are listed below:
+The library implements the basic functions of **API Lesta Games** and **API Wargaming.net**. All requests are made through your application, which you previously created on [<img src="docs/icons/lesta.ico" width=14px> Lesta Games](https://developers.lesta.ru/applications/) or on [<img src="docs/icons/wg.ico" width=14px> Wargaming.net](https://developers.wargaming.net/applications/). Some features are listed below:
 - Getting information about the player, his equipment and medals.
 - Obtaining information about the clan.
-- Getting information about equipment, equipment mauls.
+- Getting information about vehicles.
 - *And other methods.*
 
 ## Copyright Notice
 
 <div style="justify-content: center; text-align: center;">
-<a href="https://developers.wargaming.net/"><img src="https://developers.wargaming.net/static/1.12.2/assets/img/header/wg_logo.png" width="150px" style="margin: 20px;"></a>
 <a href="https://developers.lesta.ru/"><img src="https://developers.lesta.ru/static/1.13.1_lst/assets/img/header/lesta_dev_logo.png" width="178px" style="margin: 20px;"></a>
+<a href="https://developers.wargaming.net/"><img src="docs/icons/wg_logo.png" width="150px" style="margin: 20px;"></a>
 </div>
 
-- 2022 © Alexander Podstrechnyy. 
+- 2023 © Alexander Podstrechnyy. 
     - [tankalxat34@gmail.com](mailto:tankalxat34@gmail.com?subject=lestagamesapi)
     - [VKontakte](https://vk.com/tankalxat34)
     - [Telegram](https://tankalxat34.t.me)
     - [GithHub](https://github.com/tankalxat34/wglestaapi)
-- 2022 © Wargaming.net. All rights reserved.
+- 2023 © Wargaming.net. All rights reserved.
     - [User Support Center](http://support.wargaming.net/)
     - [Official website](https://wargaming.net/)
     - [License Agreement](https://eu.wargaming.net/user_agreement/)
     - [Privacy Policy](https://eu.wargaming.net/privacy_policy/)
-- 2022 © Lesta Games. All rights reserved. 
+- 2023 © Lesta Games. All rights reserved. 
     - [User Support Center](https://lesta.ru/support/)
     - [Official website](https://lesta.ru/)
     - [License Agreement](https://developers.lesta.ru/documentation/rules/agreement/)
     - [Privacy Policy](https://legal.lesta.ru/privacy-policy/)
 
 *This program code is not a product of Lesta Games and was developed according to Lesta Games DPP rules.*
 
-*This program code is not a product of Wargaming.net and is developed according to WG DPP rules.*
+*This program code is not a product of Wargaming.net and is developed according to WG DPP rules.*
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
-# WgLestaAPI Unofficial Python library that facilitates working with **[https:/
-/developers.wargaming.net/static/1.12.2/assets/img/favicon.ico]_API
-Wargaming.net** and **[https://developers.lesta.ru/static/1.13.1_lst/assets/
-img/favicon.ico]_API_Lesta_Games** functionality via **Python**. [![Downloads]
-(https://static.pepy.tech/personalized-badge/
+# WgLestaAPI Unofficial Python library that facilitates working with **[docs/
+icons/wg.ico]_API_Wargaming.net** and **[docs/icons/lesta.ico]_API_Lesta
+Games** functionality via **Python**. [![Downloads](https://static.pepy.tech/
+personalized-badge/
 wglestaapi?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)]
 (https://pepy.tech/project/wglestaapi) [![Downloads](https://static.pepy.tech/
 personalized-badge/
 wglestaapi?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/
 month)](https://pepy.tech/project/wglestaapi) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 wglestaapi?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/
@@ -16,45 +15,52 @@
 wglestaapi?color=success)](https://pypi.org/project/wglestaapi) [![](https://
 img.shields.io/pypi/format/wglestaapi)](https://pypi.org/project/wglestaapi) [!
 [](https://img.shields.io/pypi/wheel/wglestaapi)](https://pypi.org/project/
 wglestaapi) [![GitHub Repo stars](https://img.shields.io/github/stars/
 tankalxat34/wglestaapi?style=social)](https://github.com/tankalxat34/
 wglestaapi) By downloading this library you fully agree with all official
 documents **Lesta Games** and **Wargaming.net** about **Lesta Games** and
-**Wargaming.net** products. *The author of the library (Alexander Podstrechny)
-is not responsible for your actions performed with the help of this program
-code.* ## Installing the library Run the command below at the command line ```
-pip install WgLestaAPI ``` ## Example of use ```py from WgLestaAPI import
+**Wargaming.net** products. *The author of the library ([Alexander Podstrechny]
+(https://github.com/tankalxat34)) is not responsible for your actions performed
+with the help of this program code.* ## Installing the library Run the command
+below at the command line ``` pip install WgLestaAPI ``` ## Example of use ###
+Async way `main.py` contains: ```py from WgLestaAPI import aio import asyncio
+method = aio.Method("account.info", "wot", account_id=563982544,
+application_id="your_app_id") response = asyncio.run(method.execute()) print
+(response) ``` `output` is: ```json {"status": "ok", "meta": {"count": 1},
+"data": {"563982544": {"client_language": "", "last_battle_time": 1569011404,
+"account_id": 563982544, "created_at": 1564320823, "updated_at": 1686648157,
+... "tanking_factor": 0.0}, "frags": None}, "nickname": "tankalxat34",
+"logout_at": 1597741881} ``` ### No-async way ```py from WgLestaAPI import
 Application # Creating a Query with your application_id query =
 Application.Query(application_id=APP_ID) # Adding the necessary parameters
 query.extend(search="tank", limit=5) # Creating the method `account.list` of
-the game Tanks Blitz on the RU-region with the passed parameters m =
+the game World of Tanks Blitz on the EU-region with the passed parameters m =
 Application.Method("account.list", game_shortname="wotb", query=query,
-region="eu") # Executing the method mExecuted = m.execute() # Your server
-response processing print(mExecuted["data"][0]["account_id"]) # 58114596 # If
-you wish, you can follow a link to the official website of the API owner with
+region="eu") # Executing the method mExecuted = m.execute() # Your handing of
+server response print(mExecuted["data"][0]["account_id"]) # 58114596 # If you
+wish, you can follow a link to the official website of the API owner with
 documentation print(m.docs) # https://developers.wargaming.net/reference/all/
 wotb/account/list/ ``` ## Library functionality The library implements the
 basic functions of **API Lesta Games** and **API Wargaming.net**. All requests
-are made through your application, which you previously created on [Lesta
-Games](https://developers.lesta.ru/applications/) or on [Wargaming.net](https:/
-/developers.wargaming.net/applications/). Some features are listed below: -
-Getting information about the player, his equipment and medals. - Obtaining
-information about the clan. - Getting information about equipment, equipment
-mauls. - *And other methods.* ## Copyright Notice
-[https://developers.wargaming.net/static/1.12.2/assets/img/header/wg_logo.png]
+are made through your application, which you previously created on [[docs/
+icons/lesta.ico] Lesta Games](https://developers.lesta.ru/applications/) or on
+[[docs/icons/wg.ico] Wargaming.net](https://developers.wargaming.net/
+applications/). Some features are listed below: - Getting information about the
+player, his equipment and medals. - Obtaining information about the clan. -
+Getting information about vehicles. - *And other methods.* ## Copyright Notice
 [https://developers.lesta.ru/static/1.13.1_lst/assets/img/header/
-lesta_dev_logo.png]
-- 2022 Â© Alexander Podstrechnyy. - [tankalxat34@gmail.com](mailto:
+lesta_dev_logo.png] [docs/icons/wg_logo.png]
+- 2023 Â© Alexander Podstrechnyy. - [tankalxat34@gmail.com](mailto:
 tankalxat34@gmail.com?subject=lestagamesapi) - [VKontakte](https://vk.com/
 tankalxat34) - [Telegram](https://tankalxat34.t.me) - [GithHub](https://
-github.com/tankalxat34/wglestaapi) - 2022 Â© Wargaming.net. All rights
+github.com/tankalxat34/wglestaapi) - 2023 Â© Wargaming.net. All rights
 reserved. - [User Support Center](http://support.wargaming.net/) - [Official
 website](https://wargaming.net/) - [License Agreement](https://
 eu.wargaming.net/user_agreement/) - [Privacy Policy](https://eu.wargaming.net/
-privacy_policy/) - 2022 Â© Lesta Games. All rights reserved. - [User Support
+privacy_policy/) - 2023 Â© Lesta Games. All rights reserved. - [User Support
 Center](https://lesta.ru/support/) - [Official website](https://lesta.ru/) -
 [License Agreement](https://developers.lesta.ru/documentation/rules/agreement/
 ) - [Privacy Policy](https://legal.lesta.ru/privacy-policy/) *This program code
 is not a product of Lesta Games and was developed according to Lesta Games DPP
 rules.* *This program code is not a product of Wargaming.net and is developed
 according to WG DPP rules.*
```

### Comparing `wglestaapi-0.2.0/WgLestaAPI/__init__.py` & `wglestaapi-0.3.0/WgLestaAPI/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,47 +19,58 @@
 - Getting information about the player, his equipment and medals.
 - Obtaining information about the clan.
 - Getting information about equipment, equipment mauls.
 - And other methods that do not require user authorization.
 
 ## Copyright Notice
 
-- 2022 © Alexander Podstrechnyy. 
+- 2023 © Alexander Podstrechnyy. 
     - [tankalxat34@gmail.com](mailto:tankalxat34@gmail.com?subject=lestagamesapi)
     - [VKontakte](https://vk.com/tankalxat34)
     - [Telegram](https://tankalxat34.t.me)
     - [GitHub](https://github.com/tankalxat34/wglestaapi)
 
-- 2022 © Wargaming.net. All rights reserved.
+- 2023 © Wargaming.net. All rights reserved.
     - [User Support Center](http://support.wargaming.net/)
     - [Official website](https://wargaming.net/)
     - [License Agreement](https://eu.wargaming.net/user_agreement/)
     - [Privacy Policy](https://eu.wargaming.net/privacy_policy/)
     
-- 2022 © Lesta Games. All rights reserved. 
+- 2023 © Lesta Games. All rights reserved. 
     - [User Support Center](https://lesta.ru/support/)
     - [Official website](https://lesta.ru/)
     - [License Agreement](https://developers.lesta.ru/documentation/rules/agreement/)
     - [Privacy Policy](https://legal.lesta.ru/privacy-policy/)
 
 This program code is not a product of Lesta Games and was developed according to Lesta Games DPP rules.
 
 This program code is not a product of Wargaming.net and is developed according to WG DPP rules.
 
 
 #### Example of use
 
+##### Async way
+
+    >>> from WgLestaAPI import aioApp
+    >>> import asyncio
+    >>> m = aioApp.Method("account.info", "wot", account_id=563982544, application_id="your_app_id")
+    >>> response = asyncio.run(m.execute())
+    >>> print(response)
+    {'status': 'ok', 'meta': {'count': 1}, 'data': {'563982544': {'client_language': '', ... 'frags': None}, 'nickname': 'tankalxat34', 'logout_at': 1597741881}}
+
+
+##### No-async way
+
     >>> from WgLestaAPI import Application
     >>> APP_ID = "YOUR_APP_ID"
     >>> myQuery = Application.Query(application_id=APP_ID)
     >>> myQuery.extend(search="tank", limit=5)
     >>> m = Application.Method(api_method="account.list", game_shortname="wotb", query=myQuery)
     >>> print(m.execute())
     {'status': 'ok', 'meta': {'count': 5}, 'data': [{'nickname': 'tank', 'account_id': 58114596}, {'nickname': 'TANK000', 'account_id': 89075933}, {'nickname': 'tank00000', 'account_id': 901694}, {'nickname': 'tank000000', 'account_id': 1984757}, {'nickname': 'tank00000000', 'account_id': 90784051}]}
 
 """
 
 __author__ = "Alexander Podstrechnyy"
 __email__ = "tankalxat34@gmail.com"
-__version__ = "0.1.0"
 __license__ = "MIT"
 __apiholders__ = ["Wargaming.net <https://wargaming.net>", "Lesta Games <https://lesta.ru>"]
```

### Comparing `wglestaapi-0.2.0/WgLestaAPI/Application.py` & `wglestaapi-0.3.0/WgLestaAPI/Application.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def __init__(self, **kwargs):
         """
         Query fields in the URL as `?key1=value1&key2=3000`
         
         If you want to create a query from parameters - just enter them one by one, or unpack the dictionary with the `**` operator.
 
-        If you have a link containing query parameters and you want to unpack them, pass only one url argument containing the link with query parameters here.
+        If you have a string url containing query parameters and you want to unpack them, pass only one `url` argument containing the link with query parameters here.
         """
         self.query = kwargs
 
     def copy(self):
         """Get an object's copy"""
         return Query(**self.dictionary)
 
@@ -102,60 +102,81 @@
         if self.region not in Constants.REGION.ALL_CIS:
             raise Exceptions.RegionDoesNotExisting(value=self.region)
 
         if self.region not in Constants.INFO[self.game_shortname]["region_list"]:
             raise Exceptions.GameDoesNotAppearThisRegion(value=self.region)
 
     def get(self) -> str:
-        """Возвращает ссылку для доступа к API конкретной игры"""
+        """Returns a link to access the API of a particular game"""
         return self.pattern.format(
             api=Constants.INFO[self.game_shortname]["api"],
             game_longname=Constants.INFO[self.game_shortname]["longname"],
             region=self.region,
             game_shortname=self.game_shortname.replace(Constants.GAMENAMES.SHORTNAMES.TANKI, Constants.GAMENAMES.SHORTNAMES.WOT)
         )
 
 
 class Method:
-    def __init__(self, api_method: str, game_shortname: Constants.GAMENAMES.SHORTNAMES, query: Query, region: Constants.REGION = Constants.REGION.RU, type_request: Constants.TYPEREQUESTS = Constants.TYPEREQUESTS.GET) -> None:
+    def __init__(self, api_method: str, game_shortname: Constants.GAMENAMES.SHORTNAMES, query: Query, region: Constants.REGION = Constants.REGION.EU, type_request: Constants.TYPEREQUESTS = Constants.TYPEREQUESTS.GET) -> None:
         """
         Class for executing API methods in `method_block.method_name` format. Use constants from the `Constants` module of this library to enter parameters.
 
         :param api_method       Executable API method. Syntax: `method_block.method_name`
         :param game_shortname   The short name of the game. For example: `wot`, `tanki`, `wotb`, `wows` etc.
         :param query            The `Query` object of this library, necessarily containing `application_id` of your application. Parameters passed to the URL along with the query.
-        :param region           The region in which the game is located. The default is `ru`.
-        :param type_request     Query type: `GET` or `POST`. The default is `GET`.
+        :param region           Optional argument. The region in which the game is located. The default is `eu` if `game_shortname` is not equal `tanki`. If you want to get information from game that are extisting only on RU-region - you need to set up `region` argument as `ru`. Pay attention that Mir tankov (Мир танков) are existing only on SU region.
+        :param type_request     Optional argument. Query type: `GET` or `POST`. The default is `GET`.
         
         """
         self.api_method = api_method
         self.query = query
         self.game_shortname = game_shortname
         self.region = region
         self.type_request = type_request
 
+        if self.game_shortname == Constants.GAMENAMES.SHORTNAMES.TANKI:
+            self.region = Constants.REGION.SU
+
         try:
             self.method_block, self.method_name = self.api_method.split(".")
         except Exception:
             raise Exceptions.IncorrectMethodDeclaration(self.api_method)
 
         self.http = urllib3.PoolManager()
         self.url_constructor = URLConstructor(game_shortname=self.game_shortname, region=self.region)
         
         self.url = self.url_constructor.get() + f"{self.method_block}/{self.method_name}/{self.query.full}"
 
-    def execute(self) -> dict | urllib3.response.HTTPResponse:
+    def __setitem__(self, key, value):
+        setattr(self, key, value)
+
+    def __getitem__(self, key):
+        return getattr(self, key)
+
+    def __str__(self) -> str:
+        return f"WgLestaAPI.Application.Method({self.execute()})"
+
+    def execute(self) -> dict:
         """Executes specified API method. In case of JSON it returns an object of `dict` type. Otherwise it returns `urllib3.response.HTTPResponse` object"""
         res = self.http.request(self.type_request, self.url.lower())
         try:
             return json.loads(res.data)
         except Exception:
             return res
+
+    @property
+    def data(self) -> dict:
+        """
+        Return data from response by key `data`
+
+        :return `dict`:
+        """
+        return self.execute()["data"]
     
     @property
     def docs(self) -> str:
-        """Link to the official description of the method at Wagraming.net or Lesta Games"""
+        """Link to the official description of the method at Wargaming.net or Lesta Games"""
         api_holder = Constants.APIHOLDERS.WG
         if self.region in Constants.REGION.CIS:
             api_holder = Constants.APIHOLDERS.LESTA
         return Constants.URL_PATTERNS["docs"].format(api_holder=api_holder, game_shortname=self.game_shortname.replace(Constants.GAMENAMES.SHORTNAMES.TANKI, Constants.GAMENAMES.SHORTNAMES.WOT), method_block=self.method_block, method_name=self.method_name)
```

### Comparing `wglestaapi-0.2.0/WgLestaAPI/Constants.py` & `wglestaapi-0.3.0/WgLestaAPI/Constants.py`

 * *Files identical despite different names*

### Comparing `wglestaapi-0.2.0/WgLestaAPI/Exceptions.py` & `wglestaapi-0.3.0/WgLestaAPI/Exceptions.py`

 * *Files identical despite different names*

### Comparing `wglestaapi-0.2.0/setup.py` & `wglestaapi-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['wglestaapi']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'wglestaapi',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Unofficial Python library that implements the Wargaming.net API and Lesta Games API functionality',
-    'long_description': '# WgLestaAPI\n\nUnofficial Python library that facilitates working with **<a href="https://developers.wargaming.net"><img src="https://developers.wargaming.net/static/1.12.2/assets/img/favicon.ico" width=15px> API Wargaming.net</a>** and **<a href="https://developers.lesta.ru"><img src="https://developers.lesta.ru/static/1.13.1_lst/assets/img/favicon.ico" width=15px> API Lesta Games</a>** functionality via **Python**.\n\n[![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/wglestaapi)\n[![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month)](https://pepy.tech/project/wglestaapi)\n[![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week)](https://pepy.tech/project/wglestaapi)\n[![Supported Versions](https://img.shields.io/pypi/pyversions/wglestaapi)](https://pypi.org/project/wglestaapi)\n[![Version](https://img.shields.io/pypi/v/wglestaapi?color=success)](https://pypi.org/project/wglestaapi)\n[![](https://img.shields.io/pypi/format/wglestaapi)](https://pypi.org/project/wglestaapi)\n[![](https://img.shields.io/pypi/wheel/wglestaapi)](https://pypi.org/project/wglestaapi)\n[![GitHub Repo stars](https://img.shields.io/github/stars/tankalxat34/wglestaapi?style=social)](https://github.com/tankalxat34/wglestaapi)\n\nBy downloading this library you fully agree with all official documents **Lesta Games** and **Wargaming.net** about **Lesta Games** and **Wargaming.net** products. *The author of the library (Alexander Podstrechny) is not responsible for your actions performed with the help of this program code.*\n\n## Installing the library\n\nRun the command below at the command line\n\n```\npip install WgLestaAPI\n```\n\n## Example of use\n\n```py\nfrom WgLestaAPI import Application\n\n# Creating a Query with your application_id\nquery = Application.Query(application_id=APP_ID)\n\n# Adding the necessary parameters\nquery.extend(search="tank", limit=5)\n\n# Creating the method `account.list` of the game Tanks Blitz on the RU-region with the passed parameters\nm = Application.Method("account.list", game_shortname="wotb", query=query, region="eu")\n\n# Executing the method\nmExecuted = m.execute()\n\n# Your server response processing\nprint(mExecuted["data"][0]["account_id"]) # 58114596\n\n# If you wish, you can follow a link to the official website of the API owner with documentation\nprint(m.docs) # https://developers.wargaming.net/reference/all/wotb/account/list/\n```\n\n## Library functionality\n\nThe library implements the basic functions of **API Lesta Games** and **API Wargaming.net**. All requests are made through your application, which you previously created on [Lesta Games](https://developers.lesta.ru/applications/) or on [Wargaming.net](https://developers.wargaming.net/applications/). Some features are listed below:\n- Getting information about the player, his equipment and medals.\n- Obtaining information about the clan.\n- Getting information about equipment, equipment mauls.\n- *And other methods.*\n\n## Copyright Notice\n\n<div style="justify-content: center; text-align: center;">\n<a href="https://developers.wargaming.net/"><img src="https://developers.wargaming.net/static/1.12.2/assets/img/header/wg_logo.png" width="150px" style="margin: 20px;"></a>\n<a href="https://developers.lesta.ru/"><img src="https://developers.lesta.ru/static/1.13.1_lst/assets/img/header/lesta_dev_logo.png" width="178px" style="margin: 20px;"></a>\n</div>\n\n- 2022 © Alexander Podstrechnyy. \n    - [tankalxat34@gmail.com](mailto:tankalxat34@gmail.com?subject=lestagamesapi)\n    - [VKontakte](https://vk.com/tankalxat34)\n    - [Telegram](https://tankalxat34.t.me)\n    - [GithHub](https://github.com/tankalxat34/wglestaapi)\n- 2022 © Wargaming.net. All rights reserved.\n    - [User Support Center](http://support.wargaming.net/)\n    - [Official website](https://wargaming.net/)\n    - [License Agreement](https://eu.wargaming.net/user_agreement/)\n    - [Privacy Policy](https://eu.wargaming.net/privacy_policy/)\n- 2022 © Lesta Games. All rights reserved. \n    - [User Support Center](https://lesta.ru/support/)\n    - [Official website](https://lesta.ru/)\n    - [License Agreement](https://developers.lesta.ru/documentation/rules/agreement/)\n    - [Privacy Policy](https://legal.lesta.ru/privacy-policy/)\n\n*This program code is not a product of Lesta Games and was developed according to Lesta Games DPP rules.*\n\n*This program code is not a product of Wargaming.net and is developed according to WG DPP rules.*',
+    'long_description': '# WgLestaAPI\n\nUnofficial Python library that facilitates working with **<a href="https://developers.wargaming.net"><img src="docs/icons/wg.ico" width=15px> API Wargaming.net</a>** and **<a href="https://developers.lesta.ru"><img src="docs/icons/lesta.ico" width=15px> API Lesta Games</a>** functionality via **Python**.\n\n[![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/wglestaapi)\n[![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month)](https://pepy.tech/project/wglestaapi)\n[![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week)](https://pepy.tech/project/wglestaapi)\n[![Supported Versions](https://img.shields.io/pypi/pyversions/wglestaapi)](https://pypi.org/project/wglestaapi)\n[![Version](https://img.shields.io/pypi/v/wglestaapi?color=success)](https://pypi.org/project/wglestaapi)\n[![](https://img.shields.io/pypi/format/wglestaapi)](https://pypi.org/project/wglestaapi)\n[![](https://img.shields.io/pypi/wheel/wglestaapi)](https://pypi.org/project/wglestaapi)\n[![GitHub Repo stars](https://img.shields.io/github/stars/tankalxat34/wglestaapi?style=social)](https://github.com/tankalxat34/wglestaapi)\n\nBy downloading this library you fully agree with all official documents **Lesta Games** and **Wargaming.net** about **Lesta Games** and **Wargaming.net** products. *The author of the library ([Alexander Podstrechny](https://github.com/tankalxat34)) is not responsible for your actions performed with the help of this program code.*\n\n## Installing the library\n\nRun the command below at the command line\n\n```\npip install WgLestaAPI\n```\n\n## Example of use\n\n### Async way\n\n`main.py` contains:\n```py\nfrom WgLestaAPI import aio\nimport asyncio\n\nmethod = aio.Method("account.info", "wot", account_id=563982544, application_id="your_app_id")\n\nresponse = asyncio.run(method.execute())\n\nprint(response)\n```\n\n`output` is:\n```json\n{"status": "ok", "meta": {"count": 1}, "data": {"563982544": {"client_language": "", "last_battle_time": 1569011404, "account_id": 563982544, "created_at": 1564320823, "updated_at": 1686648157, ... "tanking_factor": 0.0}, "frags": None}, "nickname": "tankalxat34", "logout_at": 1597741881}\n```\n\n### No-async way\n\n```py\nfrom WgLestaAPI import Application\n\n# Creating a Query with your application_id\nquery = Application.Query(application_id=APP_ID)\n\n# Adding the necessary parameters\nquery.extend(search="tank", limit=5)\n\n# Creating the method `account.list` of the game World of Tanks Blitz on the EU-region with the passed parameters\nm = Application.Method("account.list", game_shortname="wotb", query=query, region="eu")\n\n# Executing the method\nmExecuted = m.execute()\n\n# Your handing of server response\nprint(mExecuted["data"][0]["account_id"]) # 58114596\n\n# If you wish, you can follow a link to the official website of the API owner with documentation\nprint(m.docs) # https://developers.wargaming.net/reference/all/wotb/account/list/\n```\n\n## Library functionality\n\nThe library implements the basic functions of **API Lesta Games** and **API Wargaming.net**. All requests are made through your application, which you previously created on [<img src="docs/icons/lesta.ico" width=14px> Lesta Games](https://developers.lesta.ru/applications/) or on [<img src="docs/icons/wg.ico" width=14px> Wargaming.net](https://developers.wargaming.net/applications/). Some features are listed below:\n- Getting information about the player, his equipment and medals.\n- Obtaining information about the clan.\n- Getting information about vehicles.\n- *And other methods.*\n\n## Copyright Notice\n\n<div style="justify-content: center; text-align: center;">\n<a href="https://developers.lesta.ru/"><img src="https://developers.lesta.ru/static/1.13.1_lst/assets/img/header/lesta_dev_logo.png" width="178px" style="margin: 20px;"></a>\n<a href="https://developers.wargaming.net/"><img src="docs/icons/wg_logo.png" width="150px" style="margin: 20px;"></a>\n</div>\n\n- 2023 © Alexander Podstrechnyy. \n    - [tankalxat34@gmail.com](mailto:tankalxat34@gmail.com?subject=lestagamesapi)\n    - [VKontakte](https://vk.com/tankalxat34)\n    - [Telegram](https://tankalxat34.t.me)\n    - [GithHub](https://github.com/tankalxat34/wglestaapi)\n- 2023 © Wargaming.net. All rights reserved.\n    - [User Support Center](http://support.wargaming.net/)\n    - [Official website](https://wargaming.net/)\n    - [License Agreement](https://eu.wargaming.net/user_agreement/)\n    - [Privacy Policy](https://eu.wargaming.net/privacy_policy/)\n- 2023 © Lesta Games. All rights reserved. \n    - [User Support Center](https://lesta.ru/support/)\n    - [Official website](https://lesta.ru/)\n    - [License Agreement](https://developers.lesta.ru/documentation/rules/agreement/)\n    - [Privacy Policy](https://legal.lesta.ru/privacy-policy/)\n\n*This program code is not a product of Lesta Games and was developed according to Lesta Games DPP rules.*\n\n*This program code is not a product of Wargaming.net and is developed according to WG DPP rules.*\n',
     'author': 'Alexander Podstrechnyy',
     'author_email': 'tankalxat34@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tankalxat34/WgLestaAPI',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['wglestaapi'] package_data = \ {'': ['*']} setup_kwargs = { 'name':
-'wglestaapi', 'version': '0.2.0', 'description': 'Unofficial Python library
+'wglestaapi', 'version': '0.3.0', 'description': 'Unofficial Python library
 that implements the Wargaming.net API and Lesta Games API functionality',
 'long_description': '# WgLestaAPI\n\nUnofficial Python library that facilitates
-working with **[https://developers.wargaming.net/static/1.12.2/assets/img/
-favicon.ico]_API_Wargaming.net** and **[https://developers.lesta.ru/static/
-1.13.1_lst/assets/img/favicon.ico]_API_Lesta_Games** functionality via
-**Python**.\n\n[![Downloads](https://static.pepy.tech/personalized-badge/
+working with **[docs/icons/wg.ico]_API_Wargaming.net** and **[docs/icons/
+lesta.ico]_API_Lesta_Games** functionality via **Python**.\n\n[![Downloads]
+(https://static.pepy.tech/personalized-badge/
 wglestaapi?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)]
 (https://pepy.tech/project/wglestaapi)\n[![Downloads](https://static.pepy.tech/
 personalized-badge/
 wglestaapi?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/
 month)](https://pepy.tech/project/wglestaapi)\n[![Downloads](https://
 static.pepy.tech/personalized-badge/
 wglestaapi?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/
@@ -20,50 +19,58 @@
 wglestaapi?color=success)](https://pypi.org/project/wglestaapi)\n[![](https://
 img.shields.io/pypi/format/wglestaapi)](https://pypi.org/project/wglestaapi)\n
 [![](https://img.shields.io/pypi/wheel/wglestaapi)](https://pypi.org/project/
 wglestaapi)\n[![GitHub Repo stars](https://img.shields.io/github/stars/
 tankalxat34/wglestaapi?style=social)](https://github.com/tankalxat34/
 wglestaapi)\n\nBy downloading this library you fully agree with all official
 documents **Lesta Games** and **Wargaming.net** about **Lesta Games** and
-**Wargaming.net** products. *The author of the library (Alexander Podstrechny)
-is not responsible for your actions performed with the help of this program
-code.*\n\n## Installing the library\n\nRun the command below at the command
-line\n\n```\npip install WgLestaAPI\n```\n\n## Example of use\n\n```py\nfrom
-WgLestaAPI import Application\n\n# Creating a Query with your
-application_id\nquery = Application.Query(application_id=APP_ID)\n\n# Adding
-the necessary parameters\nquery.extend(search="tank", limit=5)\n\n# Creating
-the method `account.list` of the game Tanks Blitz on the RU-region with the
-passed parameters\nm = Application.Method("account.list",
+**Wargaming.net** products. *The author of the library ([Alexander Podstrechny]
+(https://github.com/tankalxat34)) is not responsible for your actions performed
+with the help of this program code.*\n\n## Installing the library\n\nRun the
+command below at the command line\n\n```\npip install WgLestaAPI\n```\n\n##
+Example of use\n\n### Async way\n\n`main.py` contains:\n```py\nfrom WgLestaAPI
+import aio\nimport asyncio\n\nmethod = aio.Method("account.info", "wot",
+account_id=563982544, application_id="your_app_id")\n\nresponse = asyncio.run
+(method.execute())\n\nprint(response)\n```\n\n`output` is:\n```json\n{"status":
+"ok", "meta": {"count": 1}, "data": {"563982544": {"client_language": "",
+"last_battle_time": 1569011404, "account_id": 563982544, "created_at":
+1564320823, "updated_at": 1686648157, ... "tanking_factor": 0.0}, "frags":
+None}, "nickname": "tankalxat34", "logout_at": 1597741881}\n```\n\n### No-async
+way\n\n```py\nfrom WgLestaAPI import Application\n\n# Creating a Query with
+your application_id\nquery = Application.Query(application_id=APP_ID)\n\n#
+Adding the necessary parameters\nquery.extend(search="tank", limit=5)\n\n#
+Creating the method `account.list` of the game World of Tanks Blitz on the EU-
+region with the passed parameters\nm = Application.Method("account.list",
 game_shortname="wotb", query=query, region="eu")\n\n# Executing the
-method\nmExecuted = m.execute()\n\n# Your server response processing\nprint
+method\nmExecuted = m.execute()\n\n# Your handing of server response\nprint
 (mExecuted["data"][0]["account_id"]) # 58114596\n\n# If you wish, you can
 follow a link to the official website of the API owner with
 documentation\nprint(m.docs) # https://developers.wargaming.net/reference/all/
 wotb/account/list/\n```\n\n## Library functionality\n\nThe library implements
 the basic functions of **API Lesta Games** and **API Wargaming.net**. All
-requests are made through your application, which you previously created on
-[Lesta Games](https://developers.lesta.ru/applications/) or on [Wargaming.net]
-(https://developers.wargaming.net/applications/). Some features are listed
-below:\n- Getting information about the player, his equipment and medals.\n-
-Obtaining information about the clan.\n- Getting information about equipment,
-equipment mauls.\n- *And other methods.*\n\n## Copyright Notice\n\n
-\n[https://developers.wargaming.net/static/1.12.2/assets/img/header/
-wg_logo.png]\n[https://developers.lesta.ru/static/1.13.1_lst/assets/img/header/
-lesta_dev_logo.png]\n
-\n\n- 2022 Â© Alexander Podstrechnyy. \n - [tankalxat34@gmail.com](mailto:
+requests are made through your application, which you previously created on [
+[docs/icons/lesta.ico] Lesta Games](https://developers.lesta.ru/applications/
+) or on [[docs/icons/wg.ico] Wargaming.net](https://developers.wargaming.net/
+applications/). Some features are listed below:\n- Getting information about
+the player, his equipment and medals.\n- Obtaining information about the
+clan.\n- Getting information about vehicles.\n- *And other methods.*\n\n##
+Copyright Notice\n\n
+\n[https://developers.lesta.ru/static/1.13.1_lst/assets/img/header/
+lesta_dev_logo.png]\n[docs/icons/wg_logo.png]\n
+\n\n- 2023 Â© Alexander Podstrechnyy. \n - [tankalxat34@gmail.com](mailto:
 tankalxat34@gmail.com?subject=lestagamesapi)\n - [VKontakte](https://vk.com/
 tankalxat34)\n - [Telegram](https://tankalxat34.t.me)\n - [GithHub](https://
-github.com/tankalxat34/wglestaapi)\n- 2022 Â© Wargaming.net. All rights
+github.com/tankalxat34/wglestaapi)\n- 2023 Â© Wargaming.net. All rights
 reserved.\n - [User Support Center](http://support.wargaming.net/)\n -
 [Official website](https://wargaming.net/)\n - [License Agreement](https://
 eu.wargaming.net/user_agreement/)\n - [Privacy Policy](https://
-eu.wargaming.net/privacy_policy/)\n- 2022 Â© Lesta Games. All rights reserved.
+eu.wargaming.net/privacy_policy/)\n- 2023 Â© Lesta Games. All rights reserved.
 \n - [User Support Center](https://lesta.ru/support/)\n - [Official website]
 (https://lesta.ru/)\n - [License Agreement](https://developers.lesta.ru/
 documentation/rules/agreement/)\n - [Privacy Policy](https://legal.lesta.ru/
 privacy-policy/)\n\n*This program code is not a product of Lesta Games and was
 developed according to Lesta Games DPP rules.*\n\n*This program code is not a
-product of Wargaming.net and is developed according to WG DPP rules.*',
+product of Wargaming.net and is developed according to WG DPP rules.*\n',
 'author': 'Alexander Podstrechnyy', 'author_email': 'tankalxat34@gmail.com',
 'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
 tankalxat34/WgLestaAPI', 'packages': packages, 'package_data': package_data,
 'python_requires': '>=3.6,<4.0', } setup(**setup_kwargs)
```

### Comparing `wglestaapi-0.2.0/PKG-INFO` & `wglestaapi-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wglestaapi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Unofficial Python library that implements the Wargaming.net API and Lesta Games API functionality
 Home-page: https://github.com/tankalxat34/WgLestaAPI
 License: MIT
 Author: Alexander Podstrechnyy
 Author-email: tankalxat34@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,86 +16,108 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/tankalxat34/WgLestaAPI
 Description-Content-Type: text/markdown
 
 # WgLestaAPI
 
-Unofficial Python library that facilitates working with **<a href="https://developers.wargaming.net"><img src="https://developers.wargaming.net/static/1.12.2/assets/img/favicon.ico" width=15px> API Wargaming.net</a>** and **<a href="https://developers.lesta.ru"><img src="https://developers.lesta.ru/static/1.13.1_lst/assets/img/favicon.ico" width=15px> API Lesta Games</a>** functionality via **Python**.
+Unofficial Python library that facilitates working with **<a href="https://developers.wargaming.net"><img src="docs/icons/wg.ico" width=15px> API Wargaming.net</a>** and **<a href="https://developers.lesta.ru"><img src="docs/icons/lesta.ico" width=15px> API Lesta Games</a>** functionality via **Python**.
 
 [![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/wglestaapi)
 [![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month)](https://pepy.tech/project/wglestaapi)
 [![Downloads](https://static.pepy.tech/personalized-badge/wglestaapi?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week)](https://pepy.tech/project/wglestaapi)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/wglestaapi)](https://pypi.org/project/wglestaapi)
 [![Version](https://img.shields.io/pypi/v/wglestaapi?color=success)](https://pypi.org/project/wglestaapi)
 [![](https://img.shields.io/pypi/format/wglestaapi)](https://pypi.org/project/wglestaapi)
 [![](https://img.shields.io/pypi/wheel/wglestaapi)](https://pypi.org/project/wglestaapi)
 [![GitHub Repo stars](https://img.shields.io/github/stars/tankalxat34/wglestaapi?style=social)](https://github.com/tankalxat34/wglestaapi)
 
-By downloading this library you fully agree with all official documents **Lesta Games** and **Wargaming.net** about **Lesta Games** and **Wargaming.net** products. *The author of the library (Alexander Podstrechny) is not responsible for your actions performed with the help of this program code.*
+By downloading this library you fully agree with all official documents **Lesta Games** and **Wargaming.net** about **Lesta Games** and **Wargaming.net** products. *The author of the library ([Alexander Podstrechny](https://github.com/tankalxat34)) is not responsible for your actions performed with the help of this program code.*
 
 ## Installing the library
 
 Run the command below at the command line
 
 ```
 pip install WgLestaAPI
 ```
 
 ## Example of use
 
+### Async way
+
+`main.py` contains:
+```py
+from WgLestaAPI import aio
+import asyncio
+
+method = aio.Method("account.info", "wot", account_id=563982544, application_id="your_app_id")
+
+response = asyncio.run(method.execute())
+
+print(response)
+```
+
+`output` is:
+```json
+{"status": "ok", "meta": {"count": 1}, "data": {"563982544": {"client_language": "", "last_battle_time": 1569011404, "account_id": 563982544, "created_at": 1564320823, "updated_at": 1686648157, ... "tanking_factor": 0.0}, "frags": None}, "nickname": "tankalxat34", "logout_at": 1597741881}
+```
+
+### No-async way
+
 ```py
 from WgLestaAPI import Application
 
 # Creating a Query with your application_id
 query = Application.Query(application_id=APP_ID)
 
 # Adding the necessary parameters
 query.extend(search="tank", limit=5)
 
-# Creating the method `account.list` of the game Tanks Blitz on the RU-region with the passed parameters
+# Creating the method `account.list` of the game World of Tanks Blitz on the EU-region with the passed parameters
 m = Application.Method("account.list", game_shortname="wotb", query=query, region="eu")
 
 # Executing the method
 mExecuted = m.execute()
 
-# Your server response processing
+# Your handing of server response
 print(mExecuted["data"][0]["account_id"]) # 58114596
 
 # If you wish, you can follow a link to the official website of the API owner with documentation
 print(m.docs) # https://developers.wargaming.net/reference/all/wotb/account/list/
 ```
 
 ## Library functionality
 
-The library implements the basic functions of **API Lesta Games** and **API Wargaming.net**. All requests are made through your application, which you previously created on [Lesta Games](https://developers.lesta.ru/applications/) or on [Wargaming.net](https://developers.wargaming.net/applications/). Some features are listed below:
+The library implements the basic functions of **API Lesta Games** and **API Wargaming.net**. All requests are made through your application, which you previously created on [<img src="docs/icons/lesta.ico" width=14px> Lesta Games](https://developers.lesta.ru/applications/) or on [<img src="docs/icons/wg.ico" width=14px> Wargaming.net](https://developers.wargaming.net/applications/). Some features are listed below:
 - Getting information about the player, his equipment and medals.
 - Obtaining information about the clan.
-- Getting information about equipment, equipment mauls.
+- Getting information about vehicles.
 - *And other methods.*
 
 ## Copyright Notice
 
 <div style="justify-content: center; text-align: center;">
-<a href="https://developers.wargaming.net/"><img src="https://developers.wargaming.net/static/1.12.2/assets/img/header/wg_logo.png" width="150px" style="margin: 20px;"></a>
 <a href="https://developers.lesta.ru/"><img src="https://developers.lesta.ru/static/1.13.1_lst/assets/img/header/lesta_dev_logo.png" width="178px" style="margin: 20px;"></a>
+<a href="https://developers.wargaming.net/"><img src="docs/icons/wg_logo.png" width="150px" style="margin: 20px;"></a>
 </div>
 
-- 2022 © Alexander Podstrechnyy. 
+- 2023 © Alexander Podstrechnyy. 
     - [tankalxat34@gmail.com](mailto:tankalxat34@gmail.com?subject=lestagamesapi)
     - [VKontakte](https://vk.com/tankalxat34)
     - [Telegram](https://tankalxat34.t.me)
     - [GithHub](https://github.com/tankalxat34/wglestaapi)
-- 2022 © Wargaming.net. All rights reserved.
+- 2023 © Wargaming.net. All rights reserved.
     - [User Support Center](http://support.wargaming.net/)
     - [Official website](https://wargaming.net/)
     - [License Agreement](https://eu.wargaming.net/user_agreement/)
     - [Privacy Policy](https://eu.wargaming.net/privacy_policy/)
-- 2022 © Lesta Games. All rights reserved. 
+- 2023 © Lesta Games. All rights reserved. 
     - [User Support Center](https://lesta.ru/support/)
     - [Official website](https://lesta.ru/)
     - [License Agreement](https://developers.lesta.ru/documentation/rules/agreement/)
     - [Privacy Policy](https://legal.lesta.ru/privacy-policy/)
 
 *This program code is not a product of Lesta Games and was developed according to Lesta Games DPP rules.*
 
 *This program code is not a product of Wargaming.net and is developed according to WG DPP rules.*
+
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: wglestaapi Version: 0.2.0 Summary: Unofficial
+Metadata-Version: 2.1 Name: wglestaapi Version: 0.3.0 Summary: Unofficial
 Python library that implements the Wargaming.net API and Lesta Games API
 functionality Home-page: https://github.com/tankalxat34/WgLestaAPI License: MIT
 Author: Alexander Podstrechnyy Author-email: tankalxat34@gmail.com Requires-
 Python: >=3.6,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Project-URL: Repository,
 https://github.com/tankalxat34/WgLestaAPI Description-Content-Type: text/
 markdown # WgLestaAPI Unofficial Python library that facilitates working with
-**[https://developers.wargaming.net/static/1.12.2/assets/img/favicon.ico]_API
-Wargaming.net** and **[https://developers.lesta.ru/static/1.13.1_lst/assets/
-img/favicon.ico]_API_Lesta_Games** functionality via **Python**. [![Downloads]
-(https://static.pepy.tech/personalized-badge/
+**[docs/icons/wg.ico]_API_Wargaming.net** and **[docs/icons/lesta.ico]_API
+Lesta_Games** functionality via **Python**. [![Downloads](https://
+static.pepy.tech/personalized-badge/
 wglestaapi?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)]
 (https://pepy.tech/project/wglestaapi) [![Downloads](https://static.pepy.tech/
 personalized-badge/
 wglestaapi?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/
 month)](https://pepy.tech/project/wglestaapi) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 wglestaapi?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/
@@ -27,45 +26,52 @@
 wglestaapi?color=success)](https://pypi.org/project/wglestaapi) [![](https://
 img.shields.io/pypi/format/wglestaapi)](https://pypi.org/project/wglestaapi) [!
 [](https://img.shields.io/pypi/wheel/wglestaapi)](https://pypi.org/project/
 wglestaapi) [![GitHub Repo stars](https://img.shields.io/github/stars/
 tankalxat34/wglestaapi?style=social)](https://github.com/tankalxat34/
 wglestaapi) By downloading this library you fully agree with all official
 documents **Lesta Games** and **Wargaming.net** about **Lesta Games** and
-**Wargaming.net** products. *The author of the library (Alexander Podstrechny)
-is not responsible for your actions performed with the help of this program
-code.* ## Installing the library Run the command below at the command line ```
-pip install WgLestaAPI ``` ## Example of use ```py from WgLestaAPI import
+**Wargaming.net** products. *The author of the library ([Alexander Podstrechny]
+(https://github.com/tankalxat34)) is not responsible for your actions performed
+with the help of this program code.* ## Installing the library Run the command
+below at the command line ``` pip install WgLestaAPI ``` ## Example of use ###
+Async way `main.py` contains: ```py from WgLestaAPI import aio import asyncio
+method = aio.Method("account.info", "wot", account_id=563982544,
+application_id="your_app_id") response = asyncio.run(method.execute()) print
+(response) ``` `output` is: ```json {"status": "ok", "meta": {"count": 1},
+"data": {"563982544": {"client_language": "", "last_battle_time": 1569011404,
+"account_id": 563982544, "created_at": 1564320823, "updated_at": 1686648157,
+... "tanking_factor": 0.0}, "frags": None}, "nickname": "tankalxat34",
+"logout_at": 1597741881} ``` ### No-async way ```py from WgLestaAPI import
 Application # Creating a Query with your application_id query =
 Application.Query(application_id=APP_ID) # Adding the necessary parameters
 query.extend(search="tank", limit=5) # Creating the method `account.list` of
-the game Tanks Blitz on the RU-region with the passed parameters m =
+the game World of Tanks Blitz on the EU-region with the passed parameters m =
 Application.Method("account.list", game_shortname="wotb", query=query,
-region="eu") # Executing the method mExecuted = m.execute() # Your server
-response processing print(mExecuted["data"][0]["account_id"]) # 58114596 # If
-you wish, you can follow a link to the official website of the API owner with
+region="eu") # Executing the method mExecuted = m.execute() # Your handing of
+server response print(mExecuted["data"][0]["account_id"]) # 58114596 # If you
+wish, you can follow a link to the official website of the API owner with
 documentation print(m.docs) # https://developers.wargaming.net/reference/all/
 wotb/account/list/ ``` ## Library functionality The library implements the
 basic functions of **API Lesta Games** and **API Wargaming.net**. All requests
-are made through your application, which you previously created on [Lesta
-Games](https://developers.lesta.ru/applications/) or on [Wargaming.net](https:/
-/developers.wargaming.net/applications/). Some features are listed below: -
-Getting information about the player, his equipment and medals. - Obtaining
-information about the clan. - Getting information about equipment, equipment
-mauls. - *And other methods.* ## Copyright Notice
-[https://developers.wargaming.net/static/1.12.2/assets/img/header/wg_logo.png]
+are made through your application, which you previously created on [[docs/
+icons/lesta.ico] Lesta Games](https://developers.lesta.ru/applications/) or on
+[[docs/icons/wg.ico] Wargaming.net](https://developers.wargaming.net/
+applications/). Some features are listed below: - Getting information about the
+player, his equipment and medals. - Obtaining information about the clan. -
+Getting information about vehicles. - *And other methods.* ## Copyright Notice
 [https://developers.lesta.ru/static/1.13.1_lst/assets/img/header/
-lesta_dev_logo.png]
-- 2022 Â© Alexander Podstrechnyy. - [tankalxat34@gmail.com](mailto:
+lesta_dev_logo.png] [docs/icons/wg_logo.png]
+- 2023 Â© Alexander Podstrechnyy. - [tankalxat34@gmail.com](mailto:
 tankalxat34@gmail.com?subject=lestagamesapi) - [VKontakte](https://vk.com/
 tankalxat34) - [Telegram](https://tankalxat34.t.me) - [GithHub](https://
-github.com/tankalxat34/wglestaapi) - 2022 Â© Wargaming.net. All rights
+github.com/tankalxat34/wglestaapi) - 2023 Â© Wargaming.net. All rights
 reserved. - [User Support Center](http://support.wargaming.net/) - [Official
 website](https://wargaming.net/) - [License Agreement](https://
 eu.wargaming.net/user_agreement/) - [Privacy Policy](https://eu.wargaming.net/
-privacy_policy/) - 2022 Â© Lesta Games. All rights reserved. - [User Support
+privacy_policy/) - 2023 Â© Lesta Games. All rights reserved. - [User Support
 Center](https://lesta.ru/support/) - [Official website](https://lesta.ru/) -
 [License Agreement](https://developers.lesta.ru/documentation/rules/agreement/
 ) - [Privacy Policy](https://legal.lesta.ru/privacy-policy/) *This program code
 is not a product of Lesta Games and was developed according to Lesta Games DPP
 rules.* *This program code is not a product of Wargaming.net and is developed
 according to WG DPP rules.*
```

