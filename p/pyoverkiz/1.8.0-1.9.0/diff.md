# Comparing `tmp/pyoverkiz-1.8.0.tar.gz` & `tmp/pyoverkiz-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoverkiz-1.8.0.tar", max compression
+gzip compressed data, was "pyoverkiz-1.9.0.tar", max compression
```

## Comparing `pyoverkiz-1.8.0.tar` & `pyoverkiz-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1073 2023-06-07 19:12:22.663895 pyoverkiz-1.8.0/LICENSE
--rw-r--r--   0        0        0     3319 2023-06-07 19:12:22.663895 pyoverkiz-1.8.0/README.md
--rw-r--r--   0        0        0        0 2023-06-07 19:12:22.675895 pyoverkiz-1.8.0/pyoverkiz/__init__.py
--rw-r--r--   0        0        0    31572 2023-06-07 19:12:22.675895 pyoverkiz-1.8.0/pyoverkiz/client.py
--rw-r--r--   0        0        0     3917 2023-06-07 19:12:22.675895 pyoverkiz-1.8.0/pyoverkiz/const.py
--rw-r--r--   0        0        0      220 2023-06-07 19:12:22.675895 pyoverkiz-1.8.0/pyoverkiz/enums/__init__.py
--rw-r--r--   0        0        0     8866 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/command.py
--rw-r--r--   0        0        0     1888 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/execution.py
--rw-r--r--   0        0        0     2945 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/gateway.py
--rw-r--r--   0        0        0    17241 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/general.py
--rw-r--r--   0        0        0     2141 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/measured_value_type.py
--rw-r--r--   0        0        0     1052 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/protocol.py
--rw-r--r--   0        0        0    14019 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/state.py
--rw-r--r--   0        0        0    18346 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/enums/ui.py
--rw-r--r--   0        0        0     1774 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/exceptions.py
--rw-r--r--   0        0        0    24495 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/models.py
--rw-r--r--   0        0        0     1869 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/obfuscate.py
--rw-r--r--   0        0        0        0 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/py.typed
--rw-r--r--   0        0        0      518 2023-06-07 19:12:22.679895 pyoverkiz-1.8.0/pyoverkiz/types.py
--rw-r--r--   0        0        0      987 2023-06-07 19:12:46.656016 pyoverkiz-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 pyoverkiz-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-27 17:33:31.662286 pyoverkiz-1.9.0/LICENSE
+-rw-r--r--   0        0        0     3319 2023-06-27 17:33:31.662286 pyoverkiz-1.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/__init__.py
+-rw-r--r--   0        0        0    31865 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/client.py
+-rw-r--r--   0        0        0     4183 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/const.py
+-rw-r--r--   0        0        0      242 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/__init__.py
+-rw-r--r--   0        0        0     8866 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/command.py
+-rw-r--r--   0        0        0     1888 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/execution.py
+-rw-r--r--   0        0        0     2945 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/gateway.py
+-rw-r--r--   0        0        0    17241 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/general.py
+-rw-r--r--   0        0        0     2141 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/measured_value_type.py
+-rw-r--r--   0        0        0     1052 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/protocol.py
+-rw-r--r--   0        0        0      645 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/server.py
+-rw-r--r--   0        0        0    14019 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/state.py
+-rw-r--r--   0        0        0    18346 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/ui.py
+-rw-r--r--   0        0        0     1774 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/exceptions.py
+-rw-r--r--   0        0        0    24495 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/models.py
+-rw-r--r--   0        0        0     1869 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/obfuscate.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/py.typed
+-rw-r--r--   0        0        0      518 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/types.py
+-rw-r--r--   0        0        0      824 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/utils.py
+-rw-r--r--   0        0        0      987 2023-06-27 17:33:55.635128 pyoverkiz-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 pyoverkiz-1.9.0/PKG-INFO
```

### Comparing `pyoverkiz-1.8.0/LICENSE` & `pyoverkiz-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/README.md` & `pyoverkiz-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/client.py` & `pyoverkiz-1.9.0/pyoverkiz/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,25 @@
 from aiohttp import ClientResponse, ClientSession, FormData, ServerDisconnectedError
 from botocore.config import Config
 from warrant_lite import WarrantLite
 
 from pyoverkiz.const import (
     COZYTOUCH_ATLANTIC_API,
     COZYTOUCH_CLIENT_ID,
+    LOCAL_API_PATH,
     NEXITY_API,
     NEXITY_COGNITO_CLIENT_ID,
     NEXITY_COGNITO_REGION,
     NEXITY_COGNITO_USER_POOL,
     SOMFY_API,
     SOMFY_CLIENT_ID,
     SOMFY_CLIENT_SECRET,
     SUPPORTED_SERVERS,
 )
+from pyoverkiz.enums import APIType, Server
 from pyoverkiz.exceptions import (
     AccessDeniedToGatewayException,
     BadCredentialsException,
     CozyTouchBadCredentialsException,
     CozyTouchServiceException,
     InvalidCommandException,
     InvalidEventListenerIdException,
@@ -91,14 +93,15 @@
     password: str
     server: OverkizServer
     setup: Setup | None
     devices: list[Device]
     gateways: list[Gateway]
     event_listener_id: str | None
     session: ClientSession
+    api_type: APIType
 
     _refresh_token: str | None = None
     _expires_in: datetime.datetime | None = None
     _access_token: str | None = None
 
     def __init__(
         self,
@@ -125,14 +128,19 @@
         self.setup: Setup | None = None
         self.devices: list[Device] = []
         self.gateways: list[Gateway] = []
         self.event_listener_id: str | None = None
 
         self.session = session if session else ClientSession()
 
+        if LOCAL_API_PATH in self.server.endpoint:
+            self.api_type = APIType.LOCAL
+        else:
+            self.api_type = APIType.CLOUD
+
     async def __aenter__(self) -> OverkizClient:
         return self
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
@@ -152,39 +160,40 @@
         register_event_listener: bool | None = True,
     ) -> bool:
         """
         Authenticate and create an API session allowing access to the other operations.
         Caller must provide one of [userId+userPassword, userId+ssoToken, accessToken, jwt]
         """
         # Local authentication
-        if "/enduser-mobile-web/1/enduserAPI/" in self.server.endpoint:
+        if self.api_type == APIType.LOCAL:
             if register_event_listener:
                 await self.register_event_listener()
             else:
                 # Call a simple endpoint to verify if our token is correct
+                # Since local API does not have a /login endpoint
                 await self.get_gateways()
 
             return True
 
         # Somfy TaHoma authentication using access_token
-        if self.server == SUPPORTED_SERVERS["somfy_europe"]:
+        if self.server == SUPPORTED_SERVERS[Server.SOMFY_EUROPE]:
             await self.somfy_tahoma_get_access_token()
 
             if register_event_listener:
                 await self.register_event_listener()
 
             return True
 
         # CozyTouch authentication using jwt
-        if self.server == SUPPORTED_SERVERS["atlantic_cozytouch"]:
+        if self.server == SUPPORTED_SERVERS[Server.ATLANTIC_COZYTOUCH]:
             jwt = await self.cozytouch_login()
             payload = {"jwt": jwt}
 
         # Nexity authentication using ssoToken
-        elif self.server == SUPPORTED_SERVERS["nexity"]:
+        elif self.server == SUPPORTED_SERVERS[Server.NEXITY]:
             sso_token = await self.nexity_login()
             user_id = self.username.replace("@", "_-_")  # Replace @ for _-_
             payload = {"ssoToken": sso_token, "userId": user_id}
 
         # Regular authentication using userId+userPassword
         else:
             payload = {"userId": self.username, "userPassword": self.password}
@@ -235,15 +244,15 @@
 
             return self._access_token
 
     async def refresh_token(self) -> None:
         """
         Update the access and the refresh token. The refresh token will be valid 14 days.
         """
-        if self.server != SUPPORTED_SERVERS["somfy_europe"]:
+        if self.server != SUPPORTED_SERVERS[Server.SOMFY_EUROPE]:
             return
 
         if not self._refresh_token:
             raise ValueError("No refresh token provided. Login method must be used.")
 
         # &grant_type=refresh_token&refresh_token=REFRESH_TOKEN
         # Request access token
```

### Comparing `pyoverkiz-1.8.0/pyoverkiz/const.py` & `pyoverkiz-1.9.0/pyoverkiz/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from pyoverkiz.enums import Server
 from pyoverkiz.models import OverkizServer
 
 COZYTOUCH_ATLANTIC_API = "https://apis.groupe-atlantic.com"
 COZYTOUCH_CLIENT_ID = (
     "Q3RfMUpWeVRtSUxYOEllZkE3YVVOQmpGblpVYToyRWNORHpfZHkzNDJVSnFvMlo3cFNKTnZVdjBh"
 )
 
@@ -12,93 +13,101 @@
 NEXITY_COGNITO_USER_POOL = "eu-west-1_wj277ucoI"
 NEXITY_COGNITO_REGION = "eu-west-1"
 
 SOMFY_API = "https://accounts.somfy.com"
 SOMFY_CLIENT_ID = "0d8e920c-1478-11e7-a377-02dd59bd3041_1ewvaqmclfogo4kcsoo0c8k4kso884owg08sg8c40sk4go4ksg"
 SOMFY_CLIENT_SECRET = "12k73w1n540g8o4cokg0cw84cog840k84cwggscwg884004kgk"
 
+LOCAL_API_PATH = "/enduser-mobile-web/1/enduserAPI/"
+
+SERVERS_WITH_LOCAL_API = [
+    Server.SOMFY_EUROPE,
+    Server.SOMFY_OCEANIA,
+    Server.SOMFY_AMERICA,
+]
+
 SUPPORTED_SERVERS: dict[str, OverkizServer] = {
-    "atlantic_cozytouch": OverkizServer(
+    Server.ATLANTIC_COZYTOUCH: OverkizServer(
         name="Atlantic Cozytouch",
         endpoint="https://ha110-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Atlantic",
         configuration_url=None,
     ),
-    "brandt": OverkizServer(
+    Server.BRANDT: OverkizServer(
         name="Brandt Smart Control",
         endpoint="https://ha3-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Brandt",
         configuration_url=None,
     ),
-    "flexom": OverkizServer(
+    Server.FLEXOM: OverkizServer(
         name="Flexom",
         endpoint="https://ha108-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Bouygues",
         configuration_url=None,
     ),
-    "hexaom_hexaconnect": OverkizServer(
+    Server.HEXAOM_HEXACONNECT: OverkizServer(
         name="Hexaom HexaConnect",
         endpoint="https://ha5-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Hexaom",
         configuration_url=None,
     ),
-    "hi_kumo_asia": OverkizServer(
+    Server.HI_KUMO_ASIA: OverkizServer(
         name="Hitachi Hi Kumo (Asia)",
         endpoint="https://ha203-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Hitachi",
         configuration_url=None,
     ),
-    "hi_kumo_europe": OverkizServer(
+    Server.HI_KUMO_EUROPE: OverkizServer(
         name="Hitachi Hi Kumo (Europe)",
         endpoint="https://ha117-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Hitachi",
         configuration_url=None,
     ),
-    "hi_kumo_oceania": OverkizServer(
+    Server.HI_KUMO_OCEANIA: OverkizServer(
         name="Hitachi Hi Kumo (Oceania)",
         endpoint="https://ha203-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Hitachi",
         configuration_url=None,
     ),
-    "nexity": OverkizServer(
+    Server.NEXITY: OverkizServer(
         name="Nexity Eugénie",
         endpoint="https://ha106-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Nexity",
         configuration_url=None,
     ),
-    "rexel": OverkizServer(
+    Server.REXEL: OverkizServer(
         name="Rexel Energeasy Connect",
         endpoint="https://ha112-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Rexel",
         configuration_url="https://utilisateur.energeasyconnect.com/user/#/zone/equipements",
     ),
-    "simu_livein2": OverkizServer(  # alias of https://tahomalink.com
+    Server.SIMU_LIVEIN2: OverkizServer(  # alias of https://tahomalink.com
         name="SIMU (LiveIn2)",
         endpoint="https://ha101-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Somfy",
         configuration_url=None,
     ),
-    "somfy_europe": OverkizServer(  # alias of https://tahomalink.com
+    Server.SOMFY_EUROPE: OverkizServer(  # alias of https://tahomalink.com
         name="Somfy (Europe)",
         endpoint="https://ha101-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Somfy",
         configuration_url="https://www.tahomalink.com",
     ),
-    "somfy_america": OverkizServer(
+    Server.SOMFY_AMERICA: OverkizServer(
         name="Somfy (North America)",
         endpoint="https://ha401-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Somfy",
         configuration_url=None,
     ),
-    "somfy_oceania": OverkizServer(
+    Server.SOMFY_OCEANIA: OverkizServer(
         name="Somfy (Oceania)",
         endpoint="https://ha201-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Somfy",
         configuration_url=None,
     ),
-    "ubiwizz": OverkizServer(
+    Server.UBIWIZZ: OverkizServer(
         name="Ubiwizz",
         endpoint="https://ha129-1.overkiz.com/enduser-mobile-web/enduserAPI/",
         manufacturer="Decelect",
         configuration_url=None,
     ),
 }
```

### Comparing `pyoverkiz-1.8.0/pyoverkiz/enums/command.py` & `pyoverkiz-1.9.0/pyoverkiz/enums/command.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/enums/execution.py` & `pyoverkiz-1.9.0/pyoverkiz/enums/execution.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/enums/gateway.py` & `pyoverkiz-1.9.0/pyoverkiz/enums/gateway.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/enums/general.py` & `pyoverkiz-1.9.0/pyoverkiz/enums/general.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/enums/measured_value_type.py` & `pyoverkiz-1.9.0/pyoverkiz/enums/measured_value_type.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/enums/protocol.py` & `pyoverkiz-1.9.0/pyoverkiz/enums/protocol.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/enums/state.py` & `pyoverkiz-1.9.0/pyoverkiz/enums/state.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/enums/ui.py` & `pyoverkiz-1.9.0/pyoverkiz/enums/ui.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/exceptions.py` & `pyoverkiz-1.9.0/pyoverkiz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/models.py` & `pyoverkiz-1.9.0/pyoverkiz/models.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/obfuscate.py` & `pyoverkiz-1.9.0/pyoverkiz/obfuscate.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyoverkiz/types.py` & `pyoverkiz-1.9.0/pyoverkiz/types.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.8.0/pyproject.toml` & `pyoverkiz-1.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyoverkiz"
-version = "1.8.0"
+version = "1.9.0"
 description = "Async Python client to interact with internal OverKiz API (e.g. used by Somfy TaHoma)."
 authors = ["Mick Vleeshouwer", "Vincent Le Bourlot", "Thibaut Etienne"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/iMicknl/python-overkiz-api"
 repository = "https://github.com/iMicknl/python-overkiz-api"
 packages = [
@@ -19,21 +19,21 @@
 backoff = ">=1.10.0,<3.0"
 attrs = ">=21.2,<24.0"
 boto3 = "^1.18.59"
 warrant-lite = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 tox = "^3.28"
-pytest = "^7.3"
+pytest = "^7.4"
 pytest-cov = "^4.1.0"
 pre-commit = "^2.21"
 black = {version = "^22.12", allow-prereleases = true}
 pylint = "^2.13.9"
 isort = "^5.11.5"
-mypy = "^1.3"
+mypy = "^1.4"
 flake8 = "^5.0.4"
 pyupgrade = "^3.3.2"
 pytest-asyncio = "^0.21.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `pyoverkiz-1.8.0/PKG-INFO` & `pyoverkiz-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoverkiz
-Version: 1.8.0
+Version: 1.9.0
 Summary: Async Python client to interact with internal OverKiz API (e.g. used by Somfy TaHoma).
 Home-page: https://github.com/iMicknl/python-overkiz-api
 License: MIT
 Author: Mick Vleeshouwer
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyoverkiz Version: 1.8.0 Summary: Async Python
+Metadata-Version: 2.1 Name: pyoverkiz Version: 1.9.0 Summary: Async Python
 client to interact with internal OverKiz API (e.g. used by Somfy TaHoma). Home-
 page: https://github.com/iMicknl/python-overkiz-api License: MIT Author: Mick
 Vleeshouwer Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

