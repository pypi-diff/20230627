# Comparing `tmp/ewelink-0.0.1-py3-none-any.whl.zip` & `tmp/ewelink-0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 3784 bytes, number of entries: 7
+Zip file size: 15731 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 ewelink/__init__.py
--rw-r--r--  2.0 unx     4962 b- defN 80-Jan-01 00:00 ewelink/ewelink.py
--rw-r--r--  2.0 unx     1011 b- defN 80-Jan-01 00:00 ewelink/types.py
--rw-r--r--  2.0 unx     1490 b- defN 80-Jan-01 00:00 ewelink-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 ewelink-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 80-Jan-01 00:00 ewelink-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      519 b- defN 80-Jan-01 00:00 ewelink-0.0.1.dist-info/RECORD
-7 files, 8141 bytes uncompressed, 2868 bytes compressed:  64.8%
+-rw-r--r--  2.0 unx     4544 b- defN 80-Jan-01 00:00 ewelink/ewelink.py
+-rw-r--r--  2.0 unx      649 b- defN 80-Jan-01 00:00 ewelink/types.py
+-rw-r--r--  2.0 unx    34902 b- defN 80-Jan-01 00:00 ewelink-0.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1513 b- defN 80-Jan-01 00:00 ewelink-0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 ewelink-0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 80-Jan-01 00:00 ewelink-0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      600 b- defN 80-Jan-01 00:00 ewelink-0.1.dist-info/RECORD
+8 files, 42367 bytes uncompressed, 14691 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -3,20 +3,23 @@
 
 Filename: ewelink/ewelink.py
 Comment: 
 
 Filename: ewelink/types.py
 Comment: 
 
-Filename: ewelink-0.0.1.dist-info/METADATA
+Filename: ewelink-0.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: ewelink-0.0.1.dist-info/WHEEL
+Filename: ewelink-0.1.dist-info/METADATA
 Comment: 
 
-Filename: ewelink-0.0.1.dist-info/top_level.txt
+Filename: ewelink-0.1.dist-info/WHEEL
 Comment: 
 
-Filename: ewelink-0.0.1.dist-info/RECORD
+Filename: ewelink-0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: ewelink-0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ewelink/ewelink.py

```diff
@@ -1,184 +1,164 @@
 import base64
 import hashlib
 import hmac
-import logging
 from aiohttp import ClientResponse, ClientSession, JsonPayload
-from typing import Any, Literal, Optional
+from traceback import TracebackException
+from types import TracebackType
+from typing import Any, Optional
 
-from .types import Device
-
-BASE_URL = "https://eu-apia.coolkit.cc"
-APP_ID = "YzfeftUVcZ6twZw1OoVKPRFYTrGEg01Q"
-APP_SECRET = "4G91qSoboqYO4Y0XJ0LPPKIsq8reHdfa"
+from .types import DOMAINS, AppCredentials, EmailUserCredentials, LoginResponse, Region
 
 
 class EWeLinkError(Exception):
-    def __init__(self, response: ClientResponse, msg: str) -> None:
+    def __init__(
+        self,
+        response: ClientResponse,
+        error: int,
+        msg: str,
+        data: dict[str, Any],
+    ) -> None:
         super().__init__(
-            f"eWeLink API request ({response.method}) to '{response.url}' failed. Error: {msg}."
+            " ".join(
+                [
+                    f"eWeLink API request ({response.method}) to '{response.url}' failed.",
+                    f"Error ({error}): {msg}.",
+                ]
+            )
         )
-
-    ...
+        self.response = response
+        self.error = error
+        self.msg = msg
+        self.data = data
 
 
 class EWeLinkPayload(JsonPayload):
     ...
 
     def __init__(
         self,
         value: Any,
-        app_id: str,
-        app_secret: str,
+        app_cred: AppCredentials,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         super().__init__(value, *args, **kwargs)
 
         # Calculate and set Authentication Sign
         signature = base64.b64encode(
             hmac.new(
-                bytes(app_secret, "utf-8"),
+                bytes(app_cred.secret, "utf-8"),
                 self._value,
                 digestmod=hashlib.sha256,
             ).digest()
         ).decode("utf-8")
 
-        self._headers["X-CK-Appid"] = app_id
+        self._headers["X-CK-Appid"] = app_cred.id
         self._headers["Authorization"] = f"Sign {signature}"
 
 
 class EWeLink:
-    def __init__(self, email: str, password: str) -> None:
-        self._email = email
-        self._password = password
-        self._session = ClientSession()
+    """eWeLink API class."""
 
-        self._at = None
+    def __init__(
+        self,
+        app_cred: AppCredentials,
+        user_cred: EmailUserCredentials,
+        client_session: Optional[ClientSession] = None,
+    ) -> None:
+        """Initiates a new instance.
+
+        Initiation of this class must be done in an async function.
+        """
+        self._app_cred = app_cred
+        self._user_cred = user_cred
+        self._client_session = client_session if client_session else ClientSession()
+        self._login: Optional[LoginResponse] = None
 
     async def __aenter__(self) -> "EWeLink":
         return self
 
-    async def __aexit__(self) -> None:
+    async def __aexit__(
+        self,
+        exc_type: Exception,
+        exc_val: TracebackException,
+        traceback: TracebackType,
+    ) -> None:
         await self.close()
 
     async def close(self) -> None:
         await self.logout()
-        await self._session.close()
+        await self._client_session.close()
 
     async def _request(
         self,
+        region: Region,
         method: str,
         endpoint: str,
         *args: Any,
         **kwargs: Any,
     ) -> dict[str, Any]:
-        async with self._session.request(
+        """Makes a HTTP(S) request."""
+        async with self._client_session.request(
             method,
-            f"{BASE_URL}/{endpoint}",
+            f"{DOMAINS[region]}/{endpoint}",
             *args,
             **kwargs,
         ) as response:
             response.raise_for_status()
             data = await response.json()
 
             if data["error"]:
-                raise EWeLinkError(response, data["msg"])
+                raise EWeLinkError(response, data["error"], data["msg"], data["data"])
 
         return data["data"]
 
     async def _auth_request(
         self,
         method: str,
         endpoint: str,
         headers: Optional[dict[str, str]] = None,
         *args: Any,
         **kwargs: Any,
     ) -> dict[str, Any]:
-        if self._at is None:
-            await self.login()
+        """Makes an authenaticated (user logged in) request."""
+        _login = await self.login()
 
         return await self._request(
+            _login.region,
             method,
             endpoint,
             headers={
                 **(headers if headers else {}),
-                "Authorization": f"Bearer {self._at}",
+                "Authorization": f"Bearer {_login.access_token}",
             },
             *args,
             **kwargs,
         )
 
-    async def login(self) -> None:
-        response = await self._request(
-            "POST",
-            "v2/user/login",
-            data=EWeLinkPayload(
-                {
-                    "email": self._email,
-                    "password": self._password,
-                    "countryCode": "+1",  # Required but irrelevant
-                },
-                APP_ID,
-                APP_SECRET,
-            ),
-        )
-        self._at = response["at"]
-
-    async def logout(self) -> None:
-        await self._auth_request("DELETE", "v2/user/logout", headers={"X-CK-Appid": APP_ID})
-
-    async def get_thing_list(self) -> list[Device]:
-        response = await self._auth_request("GET", "v2/device/thing")
-        things = response["thingList"]
-
-        items = []
-        for thing in things:
-            type = thing["itemType"]
-            data = thing["itemData"]
-
-            if type == 1:
-                items.append(Device.parse_obj(data))
-            else:
-                raise NotImplementedError()
-
-        return items
-
-    async def update_thing_status(
-        self,
-        device: Device,
-        params: dict[str, Any],
-        new_params: bool = False,
-    ) -> None:
-        if new_params is False:
-            new_keys = params.keys() - device.params.keys()
-            if new_keys:
-                logging.warning(
-                    f"Ignoring new params ({new_keys}) not previously set."
-                    " Setting new params may cause undefined behaviors. If this was"
-                    " intentionally, set new_params=True when calling"
-                    " update_thing_status(...)."
+    async def login(self, region: Region = "cn") -> LoginResponse:
+        if self._login is None:
+            try:
+                self._login = LoginResponse.parse_obj(
+                    await self._request(
+                        region,
+                        "POST",
+                        "v2/user/login",
+                        data=EWeLinkPayload(self._user_cred.dict(by_alias=True), self._app_cred),
+                    )
                 )
+            except EWeLinkError as e:
+                if e.error == 10004:
+                    return await self.login(region=e.data["region"])
+                else:
+                    raise
 
-            params = {k: v for k, v in params.items() if k in device.params}
+        return self._login
 
-        await self._auth_request(
-            "POST",
-            "v2/device/thing/status",
-            json={
-                "type": 1,
-                "id": device.id,
-                "params": params,
-            },
-        )
-
-    async def set_device_power_status(
-        self,
-        device: Device,
-        status: Literal["on", "off"],
-    ) -> None:
-        if device.extra.type.channels == 1:
-            params = {"switch": status}
-        else:
-            raise NotImplementedError()
-
-        await self.update_thing_status(device, params)
+    async def logout(self) -> None:
+        if self._login:
+            await self._auth_request(
+                "DELETE",
+                "v2/user/logout",
+                headers={"X-CK-Appid": self._app_cred.id},
+            )
+            self._login = None
```

## ewelink/types.py

```diff
@@ -1,43 +1,28 @@
 from pydantic import BaseModel, Field
-from typing import Any
+from typing import Literal
 
-
-class DeviceType:
-    def __init__(self, name: str, channels: int) -> None:
-        self.name = name
-        self.channels = channels
-
-
-DEVICE_TYPES = {
-    1: DeviceType("SOCKET", 1),
-    2: DeviceType("SOCKET_2", 2),
+Region = Literal["as", "cn", "eu", "us"]
+DOMAINS: dict[Region, str] = {
+    "as": "https://as-apia.coolkit.cc",
+    "cn": "https://cn-apia.coolkit.cn",
+    "eu": "https://eu-apia.coolkit.cc",
+    "us": "https://us-apia.coolkit.cc",
 }
 
 
-class DeviceInfo(BaseModel):
-    # model: str
-    # ui: str
-    uiid: int
-    # description: str
-    # manufacturer: str
-    # mac: str
-    # apmac: str
-    # model_info: str = Field(alias="modelInfo")
-    # brand_id: str = Field(alias="brandId")
-    # chip_id: str = Field(alias="chipid")
-
-    @property
-    def type(self) -> DeviceType:
-        return DEVICE_TYPES[self.uiid]
-
-
-class Device(BaseModel):
-    name: str
-    id: str = Field(alias="deviceid")
-    apikey: str
-    extra: DeviceInfo
-    # brand_name: str = Field(alias="brandName")
-    # brand_logo: str = Field(alias="brandLogo")
-    # show_brand: bool = Field(alias="showBrand")
-    # product_model: str = Field(alias="productModel")
-    params: dict[str, Any]
+class AppCredentials(BaseModel):
+    id: str
+    secret: str
+
+
+class EmailUserCredentials(BaseModel):
+    email: str
+    password: str
+    country_code: str = Field("+1", alias="countryCode")
+
+
+class LoginResponse(BaseModel):
+    user: object
+    access_token: str = Field(alias="at")
+    refresh_token: str = Field(alias="rt")
+    region: Region
```

## Comparing `ewelink-0.0.1.dist-info/METADATA` & `ewelink-0.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: ewelink
-Version: 0.0.1
+Version: 0.1
 Requires-Python: >=3.9
+License-File: LICENSE.md
 Requires-Dist: aiohttp
 Requires-Dist: pydantic
 Provides-Extra: black
 Requires-Dist: black (==22.8.0) ; extra == 'black'
 Provides-Extra: dev
 Requires-Dist: tox ; extra == 'dev'
 Requires-Dist: pytest (>=7) ; extra == 'dev'
```

## Comparing `ewelink-0.0.1.dist-info/RECORD` & `ewelink-0.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 ewelink/__init__.py,sha256=IHGyHt5wkDayBWmKGluvVBHxucl87pFqlEcNpAe-r6c,59
-ewelink/ewelink.py,sha256=RWyKt4BNn5LGCvy3b9e23wmme2xuSvP_sgdnEocPh_U,4962
-ewelink/types.py,sha256=EUu9pWBHhgMDvLWS3SVXj8ZPmkT25ge1aoHYEg28ALE,1011
-ewelink-0.0.1.dist-info/METADATA,sha256=MJcFNN33olWpZIZUrgggDsPYQ7GsJB5rXvGeHooESmI,1490
-ewelink-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ewelink-0.0.1.dist-info/top_level.txt,sha256=wHi-hGkJDmwMPYzTRJsEiMaBxk8ar5eNY5xgH4lg-iM,8
-ewelink-0.0.1.dist-info/RECORD,,
+ewelink/ewelink.py,sha256=KK2pxRX-gwiOchnwKg98Z9NGCbf9ppJ7rGesUcXCUkM,4544
+ewelink/types.py,sha256=yVubpPTudac_sCMxpNfyxHQtLaWKjddAbpNQlR3hstk,649
+ewelink-0.1.dist-info/LICENSE.md,sha256=bqhD2fIhoqfLdX1lyGNoufIHWE7Q8mU-SyFadwKn4cc,34902
+ewelink-0.1.dist-info/METADATA,sha256=MUFDeeTlC0JsR5i3YXaBMjQNkaaT5HM_GHHH7kSdHNM,1513
+ewelink-0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ewelink-0.1.dist-info/top_level.txt,sha256=wHi-hGkJDmwMPYzTRJsEiMaBxk8ar5eNY5xgH4lg-iM,8
+ewelink-0.1.dist-info/RECORD,,
```

