# Comparing `tmp/pywa-0.0.1rc10-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 23263 bytes, number of entries: 15
+Zip file size: 23369 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:52 pywa/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jun-27 07:54 pywa/__version__.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jun-27 08:15 pywa/__version__.py
 -rw-rw-r--  2.0 unx    15077 b- defN 23-Jun-26 17:13 pywa/api.py
--rw-rw-r--  2.0 unx    26535 b- defN 23-Jun-26 17:13 pywa/client.py
+-rw-rw-r--  2.0 unx    26563 b- defN 23-Jun-27 08:15 pywa/client.py
 -rw-rw-r--  2.0 unx      989 b- defN 23-Jun-19 21:14 pywa/errors.py
 -rw-rw-r--  2.0 unx    11047 b- defN 23-Jun-26 16:59 pywa/filters.py
 -rw-rw-r--  2.0 unx     1464 b- defN 23-Jun-22 18:21 pywa/handlers.py
 -rw-rw-r--  2.0 unx    32457 b- defN 23-Jun-26 17:29 pywa/types.py
 -rw-rw-r--  2.0 unx      991 b- defN 23-Jun-20 16:58 pywa/utils.py
--rw-rw-r--  2.0 unx     4502 b- defN 23-Jun-26 17:11 pywa/webhook.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jun-27 07:54 pywa-0.0.1rc10.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4490 b- defN 23-Jun-27 07:54 pywa-0.0.1rc10.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 07:54 pywa-0.0.1rc10.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-27 07:54 pywa-0.0.1rc10.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1105 b- defN 23-Jun-27 07:54 pywa-0.0.1rc10.dist-info/RECORD
-15 files, 99963 bytes uncompressed, 21481 bytes compressed:  78.5%
+-rw-rw-r--  2.0 unx     4391 b- defN 23-Jun-27 08:09 pywa/webhook.py
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jun-27 08:17 pywa-0.0.1rc11.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4493 b- defN 23-Jun-27 08:17 pywa-0.0.1rc11.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 08:17 pywa-0.0.1rc11.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-27 08:17 pywa-0.0.1rc11.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1105 b- defN 23-Jun-27 08:17 pywa-0.0.1rc11.dist-info/RECORD
+15 files, 99883 bytes uncompressed, 21587 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pywa/utils.py
 Comment: 
 
 Filename: pywa/webhook.py
 Comment: 
 
-Filename: pywa-0.0.1rc10.dist-info/LICENSE
+Filename: pywa-0.0.1rc11.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc10.dist-info/METADATA
+Filename: pywa-0.0.1rc11.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc10.dist-info/WHEEL
+Filename: pywa-0.0.1rc11.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc10.dist-info/top_level.txt
+Filename: pywa-0.0.1rc11.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc10.dist-info/RECORD
+Filename: pywa-0.0.1rc11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc10"
+__version__ = "0.0.1rc11"
```

## pywa/client.py

```diff
@@ -1,18 +1,20 @@
+"""The WhatsApp client."""
+
 import hashlib
 import mimetypes
 import os
 import requests
 from typing import Callable, Any, Iterable
 from pywa.api import WhatsAppCloudApi
 from pywa.handlers import Handler, MessageHandler, ButtonCallbackHandler, SelectionCallbackHandler, RawUpdateHandler, \
     MessageStatusHandler
 from pywa.types import InlineButton, SectionList, Message, CallbackButton, CallbackSelection, MessageStatus, Contact, \
     MediaUrlResponse
-from pywa import webhook
+from pywa.webhook import Webhook
 
 
 class WhatsApp:
     def __init__(
             self,
             phone_id: str | int,
             token: str,
@@ -48,15 +50,15 @@
             session=session or requests.Session(),
             base_url=base_url,
             api_version=float(api_version),
         )
         if server is not None:
             if verify_token is None:
                 raise ValueError("When listening for incoming messages, a verify token must be provided.")
-            self.webhook = webhook.Webhook(
+            self.webhook = Webhook(
                 wa_client=self,
                 server=server,
                 verify_token=verify_token,
                 webhook_endpoint=webhook_endpoint,
                 filter_updates=filter_updates,
             )
         else:
```

## pywa/webhook.py

```diff
@@ -1,9 +1,12 @@
 from __future__ import annotations
 
+"""The webhook module contains the Webhook class, which is used to register a webhook to listen for incoming 
+messages."""
+
 import collections
 from typing import Union, TYPE_CHECKING, Callable, Any
 from pywa.types import Message, CallbackButton, CallbackSelection, MessageStatus, BaseUpdate
 from pywa import utils
 
 if TYPE_CHECKING:
     from pywa import WhatsApp
@@ -19,77 +22,77 @@
             wa_client: WhatsApp,
             server: Union["flask.Flask", "fastapi.FastAPI"],
             verify_token: str,
             webhook_endpoint: str,
             filter_updates: bool
     ):
         self.handlers: dict[str, list[Callable[[WhatsApp, BaseUpdate | dict], Any]]] = collections.defaultdict(list)
+        self.wa_client = wa_client
+        self.server = server
+        self.verify_token = verify_token
+        self.webhook_endpoint = webhook_endpoint
+        self.filter_updates = filter_updates
 
-        if utils.is_flask_app(server):
+        if utils.is_flask_app(self.server):
             import flask
 
-            @server.before_request
+            @self.server.before_request
             def before_request():
-                if flask.request.path != webhook_endpoint:
+                if flask.request.path != self.webhook_endpoint:
                     return
                 if flask.request.method == "GET":
-                    if verify_token == flask.request.args.get("hub.verify_token"):
+                    if flask.request.args.get("hub.verify_token") == self.verify_token:
                         return flask.request.args.get("hub.challenge"), 200
                     else:
                         return "Error, invalid verification token", 403
                 elif flask.request.method == "POST":
-                    if not filter_updates or (
-                            flask.request.json["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"]
-                            == wa_client.phone_id):
-                        for raw_update_handler in self.handlers["raw_update"]:
-                            raw_update_handler(wa_client, flask.request.json)
-                        update, key = convert_dict_to_update(client=wa_client, d=flask.request.json)
-                        for handler in self.handlers[key]:  # TODO execute in parallel
-                            handler(wa_client, update)
+                    self.call_handlers(update=flask.request.json)
                     return "ok", 200
 
-        elif utils.is_fastapi_app(server):
+        elif utils.is_fastapi_app(self.server):
             import fastapi
 
-            @server.middleware("http")
+            @self.server.middleware("http")
             async def before_request(request: fastapi.Request, call_next: Callable):
-                if request.url.path != webhook_endpoint:
+                if request.url.path != self.webhook_endpoint:
                     return await call_next(request)
                 if request.method == "GET":
-                    if verify_token == request.query_params.get("hub.verify_token"):
+                    if request.query_params.get("hub.verify_token") == self.verify_token:
                         return fastapi.Response(content=request.query_params.get("hub.challenge"), status_code=200)
                     else:
                         return fastapi.Response(content="Error, invalid verification token", status_code=403)
                 elif request.method == "POST":
                     request_body = await request.json()
-                    if not filter_updates or (
-                            request_body["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"]
-                            == wa_client.phone_id):
-                        for raw_update_handler in self.handlers["raw_update"]:
-                            raw_update_handler(wa_client, request_body)
-                        update, key = convert_dict_to_update(client=wa_client, d=request_body)
-                        handler: Callable[[WhatsApp, BaseUpdate], Any]
-                        for handler in self.handlers[key]:  # TODO execute in parallel
-                            handler(wa_client, update)
+                    self.call_handlers(update=request_body)
                     return fastapi.Response(content="ok", status_code=200)
                 return await call_next(request)
 
         else:
             raise ValueError("The app must be a Flask or FastAPI app.")
 
+    def call_handlers(self, update: dict) -> None:
+        """Call the handlers for the given update."""
+        if not self.filter_updates or (
+                update["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"] == self.wa_client.phone_id):
+            for raw_update_handler in self.handlers["raw_update"]:
+                raw_update_handler(self.wa_client, update)
+            update, key = self.convert_dict_to_update(client=self.wa_client, d=update)
+            for handler in self.handlers[key]:  # TODO execute in parallel
+                handler(self.wa_client, update)
+
+    @staticmethod
+    def convert_dict_to_update(client: WhatsApp, d: dict) -> tuple[BaseUpdate, str]:
+        """Convert a webhook dict to a BaseUpdate object."""
+        value = d["entry"][0]["changes"][0]["value"]
+        if 'messages' in value:
+            if value["messages"][0]["type"] != "interactive":
+                return Message.from_dict(client=client, value=value), "message"
+            else:
+                if value["messages"][0]["interactive"]["type"] == "button_reply":
+                    return CallbackButton.from_dict(client=client, value=value), "button"
+                elif value["messages"][0]["interactive"]["type"] == "list_reply":
+                    return CallbackSelection.from_dict(client=client, value=value), "selection"
 
-def convert_dict_to_update(client: WhatsApp, d: dict) -> tuple[BaseUpdate, str]:
-    """Convert a webhook dict to a BaseUpdate object."""
-    value = d["entry"][0]["changes"][0]["value"]
-    if 'messages' in value:
-        if value["messages"][0]["type"] != "interactive":
-            return Message.from_dict(client=client, value=value), "message"
+        elif 'statuses' in value:
+            return MessageStatus.from_dict(client=client, value=value), "status"
         else:
-            if value["messages"][0]["interactive"]["type"] == "button_reply":
-                return CallbackButton.from_dict(client=client, value=value), "button"
-            elif value["messages"][0]["interactive"]["type"] == "list_reply":
-                return CallbackSelection.from_dict(client=client, value=value), "selection"
-
-    elif 'statuses' in value:
-        return MessageStatus.from_dict(client=client, value=value), "status"
-    else:
-        raise ValueError("Invalid webhook data: " + str(d))
+            raise ValueError("Invalid webhook data: " + str(d))
```

## Comparing `pywa-0.0.1rc10.dist-info/LICENSE` & `pywa-0.0.1rc11.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc10.dist-info/METADATA` & `pywa-0.0.1rc11.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc10
+Version: 0.0.1rc11
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
@@ -119,15 +119,15 @@
     from pywa.types import Message, CallbackButton, InlineButton
     from pywa.filters import TextFilter, CallbackFilter
 
     flask_app = Flask(__name__)
     wa = WhatsApp(
         phone_id='1234567890',
         token='xxxxxxxxxxxxxxx',
-        app=flask_app,
+        server=flask_app,
         verify_token='XYZXYZ',
     )
 
     @wa.on_message(TextFilter.equals('Hello', 'Hi'))
     def hello(client: WhatsApp, message: Message):
         message.react('👋')
         message.reply_text(
```

## Comparing `pywa-0.0.1rc10.dist-info/RECORD` & `pywa-0.0.1rc11.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
-pywa/__version__.py,sha256=hprtffs36hjzdxRBcLhcZRc9xL0CK7CmJwfjRGY6oU4,26
+pywa/__version__.py,sha256=GVsyXElC308caK4I6LjYEqfIc3Uw7LhtajV62yNE0xM,26
 pywa/api.py,sha256=zW7zrkDcWB7df5B0FW2GM6an5wn1cMXxuMCD19krOLU,15077
-pywa/client.py,sha256=_SakRCC-Z-4v7psrTXq6dQg-7w9SsYR1Muam9gvyJ78,26535
+pywa/client.py,sha256=7s-7J9Pb-WLGwD6eizYnZj_pzCwODVH4ssHBwldkR9E,26563
 pywa/errors.py,sha256=Vs5SJehEt5PhUrJBbia710gpusoxmTPQmlgDBBnYpWM,989
 pywa/filters.py,sha256=9t2ckte1_gRaKNF6LlISgNY2up3CN7Gnx7IQ1cSEue8,11047
 pywa/handlers.py,sha256=Z4j2jiEwQ0_mzlcybHFDmRg7OR8agakXXkzU85eQyGk,1464
 pywa/types.py,sha256=ooFguLLhqx6Y25zyuqQ9O1knwXkWsx-at0RMJhD1Z6g,32457
 pywa/utils.py,sha256=GRTfSvmsuOBd1_Yw2c90XoALqVPuy6HzyvJuqg3xjtI,991
-pywa/webhook.py,sha256=qt9-W5MLLtMWC-70jlw1vKaWZ4yU7MYwPVNtEtRh8B8,4502
-pywa-0.0.1rc10.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc10.dist-info/METADATA,sha256=wIMD9ok4Fpma7EsPsWOqh0VA-Eop7bIEziCynnN5Xkg,4490
-pywa-0.0.1rc10.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc10.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc10.dist-info/RECORD,,
+pywa/webhook.py,sha256=ZRqfm8b0-_U-Bx7dw_ATfuyU1EcyWCbz3UFdo4LHdSU,4391
+pywa-0.0.1rc11.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc11.dist-info/METADATA,sha256=kRs8Za6MRJctDTJbvX6xc2fiN9RMoLEV9GWfonRcLKQ,4493
+pywa-0.0.1rc11.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc11.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc11.dist-info/RECORD,,
```

