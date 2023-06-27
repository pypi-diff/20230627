# Comparing `tmp/pywa-0.0.1rc8-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 22785 bytes, number of entries: 14
--rw-rw-r--  2.0 unx      143 b- defN 23-Jun-26 09:18 pywa/__init__.py
--rw-rw-r--  2.0 unx    14911 b- defN 23-Jun-26 08:51 pywa/api.py
--rw-rw-r--  2.0 unx    26284 b- defN 23-Jun-26 09:16 pywa/client.py
+Zip file size: 23252 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:48 pywa/__init__.py
+-rw-rw-r--  2.0 unx       25 b- defN 23-Jun-27 07:48 pywa/__version__.py
+-rw-rw-r--  2.0 unx    15077 b- defN 23-Jun-26 17:13 pywa/api.py
+-rw-rw-r--  2.0 unx    26535 b- defN 23-Jun-26 17:13 pywa/client.py
 -rw-rw-r--  2.0 unx      989 b- defN 23-Jun-19 21:14 pywa/errors.py
--rw-rw-r--  2.0 unx    11021 b- defN 23-Jun-22 17:14 pywa/filters.py
+-rw-rw-r--  2.0 unx    11047 b- defN 23-Jun-26 16:59 pywa/filters.py
 -rw-rw-r--  2.0 unx     1464 b- defN 23-Jun-22 18:21 pywa/handlers.py
--rw-rw-r--  2.0 unx    32258 b- defN 23-Jun-26 09:16 pywa/types.py
+-rw-rw-r--  2.0 unx    32457 b- defN 23-Jun-26 17:29 pywa/types.py
 -rw-rw-r--  2.0 unx      991 b- defN 23-Jun-20 16:58 pywa/utils.py
--rw-rw-r--  2.0 unx     4161 b- defN 23-Jun-26 07:53 pywa/webhook.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jun-26 09:19 pywa-0.0.1rc8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4489 b- defN 23-Jun-26 09:19 pywa-0.0.1rc8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 09:19 pywa-0.0.1rc8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-26 09:19 pywa-0.0.1rc8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1026 b- defN 23-Jun-26 09:19 pywa-0.0.1rc8.dist-info/RECORD
-14 files, 98900 bytes uncompressed, 21127 bytes compressed:  78.6%
+-rw-rw-r--  2.0 unx     4502 b- defN 23-Jun-26 17:11 pywa/webhook.py
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jun-27 07:48 pywa-0.0.1rc9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4489 b- defN 23-Jun-27 07:48 pywa-0.0.1rc9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-27 07:48 pywa-0.0.1rc9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-27 07:48 pywa-0.0.1rc9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1100 b- defN 23-Jun-27 07:48 pywa-0.0.1rc9.dist-info/RECORD
+15 files, 99956 bytes uncompressed, 21480 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: pywa/__init__.py
 Comment: 
 
+Filename: pywa/__version__.py
+Comment: 
+
 Filename: pywa/api.py
 Comment: 
 
 Filename: pywa/client.py
 Comment: 
 
 Filename: pywa/errors.py
@@ -21,23 +24,23 @@
 
 Filename: pywa/utils.py
 Comment: 
 
 Filename: pywa/webhook.py
 Comment: 
 
-Filename: pywa-0.0.1rc8.dist-info/LICENSE
+Filename: pywa-0.0.1rc9.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc8.dist-info/METADATA
+Filename: pywa-0.0.1rc9.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc8.dist-info/WHEEL
+Filename: pywa-0.0.1rc9.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc8.dist-info/top_level.txt
+Filename: pywa-0.0.1rc9.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc8.dist-info/RECORD
+Filename: pywa-0.0.1rc9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__init__.py

```diff
@@ -1,5 +1,3 @@
 """Python wrapper for the WhatsApp Cloud API. https://github.com/david-lev/pywa"""
 
-__version__ = "0.0.1rc8"
-
 from pywa.client import WhatsApp
```

## pywa/api.py

```diff
@@ -13,14 +13,16 @@
             phone_id: str,
             token: str,
             session: requests.Session,
             base_url: str,
             api_version: float,
     ):
         self.phone_id = phone_id
+        if session.headers.get("Authorization") is not None:
+            raise ValueError("You can't use the same requests.Session for multiple WhatsApp instances!")
         self._session = session
         self._base_url = f"{base_url}/v{api_version}"
         self._session.headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {token}",
         }
         self._common_keys = {
```

## pywa/client.py

```diff
@@ -1,8 +1,7 @@
-import collections
 import hashlib
 import mimetypes
 import os
 import requests
 from typing import Callable, Any, Iterable
 from pywa.api import WhatsAppCloudApi
 from pywa.handlers import Handler, MessageHandler, ButtonCallbackHandler, SelectionCallbackHandler, RawUpdateHandler, \
@@ -13,62 +12,65 @@
 
 
 class WhatsApp:
     def __init__(
             self,
             phone_id: str | int,
             token: str,
-            app: Any | None = None,
-            webhook_endpoint: str = "/pywa",
-            verify_token: str | None = None,
             base_url: str = "https://graph.facebook.com",
-            api_version: float = 17.0,
+            api_version: float | int = 17.0,
             session: requests.Session | None = None,
-    ):
+            server: Any | None = None,
+            webhook_endpoint: str = "/",
+            verify_token: str | None = None,
+            filter_updates: bool = True,
+    ) -> None:
         """
         Initialize the WhatsApp client.
 
         >>> from pywa import WhatsApp
-        >>> wa = WhatsApp(phone_id="100944", token="EAADKQl9oJxx")
+        >>> wa = WhatsApp(phone_id="100944",token="EAADKQl9oJxx")
 
         Args:
-            phone_id: The phone ID of the WhatsApp account.
+            phone_id: The 'Phone number ID'
             token: The token of the WhatsApp account.
-            app: The Flask or FastAPI app.
-            webhook_endpoint: The endpoint to listen for incoming messages (default: `/pywa`).
+            base_url: The base URL of the WhatsApp API. Default: ``https://graph.facebook.com``
+            api_version: The API version of the WhatsApp API. Default: ``17.0``
+            session: The session to use for requests. (Do not use the same session for multiple WhatsApp clients!)
+            server: The Flask or FastAPI app instance.
+            webhook_endpoint: The endpoint to listen for incoming messages (default: ``/``).
             verify_token: The verify token of the registered webhook.
-            base_url: The base URL of the WhatsApp API. Default: `https://graph.facebook.com`
-            api_version: The API version of the WhatsApp API. Default: 17.0
-            session: The session to use for requests. Default: New session.
+            filter_updates: Whether to filter out updates that not sended to this phone number.
         """
         self.phone_id = str(phone_id)
         self.api = WhatsAppCloudApi(
             phone_id=phone_id,
             token=token,
             session=session or requests.Session(),
             base_url=base_url,
-            api_version=api_version,
+            api_version=float(api_version),
         )
-        if app is not None:
+        if server is not None:
             if verify_token is None:
                 raise ValueError("When listening for incoming messages, a verify token must be provided.")
-            webhook.Webhook(
+            self.webhook = webhook.Webhook(
                 wa_client=self,
-                app=app,
+                server=server,
                 verify_token=verify_token,
                 webhook_endpoint=webhook_endpoint,
+                filter_updates=filter_updates,
             )
-            self._handlers = collections.defaultdict(list)
         else:
-            self._handlers = None
+            self.webhook = None
 
     def add_handler(self, handler: Handler):
-        if self._handlers is None:
-            raise ValueError("You must initialize the WhatsApp client with an app (Flask or FastAPI) to add handlers.")
-        self._handlers[handler.__handler_type__].append(handler)
+        if self.webhook is None:
+            raise ValueError("You must initialize the WhatsApp client with an web server"
+                             " (Flask or FastAPI) in order to handle incoming messages.")
+        self.webhook.handlers[handler.__handler_type__].append(handler)
 
     def on_raw_update(self, *filters: Callable[["WhatsApp", dict], bool]):
         """
         Decorator to register a function as a handler for raw updates.
 
         Example:
```

## pywa/filters.py

```diff
@@ -18,14 +18,15 @@
     "DocumentFilter",
     "StickerFilter",
     "ReactionFilter",
     "UnsupportedMsgFilter",
     "LocationFilter",
     "ContactsFilter",
     "CallbackFilter",
+    "MessageStatusFilter"
 )
 
 _ONLY_NUMS_RE = re.compile(r"\D")
 
 
 class TextFilter:
     """Useful filters for text messages."""
```

## pywa/types.py

```diff
@@ -129,14 +129,15 @@
     TEXT = "text"
     IMAGE = "image"
     STICKER = "sticker"
     VIDEO = "video"
     REACTION = "reaction"
     LOCATION = "location"
     CONTACTS = "contacts"
+    INTERACTIVE = "interactive"
     UNSUPPORTED = "unsupported"
 
     # SYSTEM = "system"
     # ORDER = "order"
 
     @classmethod
     def _missing_(cls, value):
@@ -524,15 +525,15 @@
     from_user_id: str
 
     @classmethod
     def from_dict(cls, data: dict | None):
         return cls(
             message_id=data['id'],
             from_user_id=data['from']
-        ) if data else None
+        ) if (data and 'id' in data) else None
 
 
 @dataclass(frozen=True, slots=True)
 class Metadata:
     """
     Represents the metadata of a message.
 
@@ -842,26 +843,28 @@
     Attributes:
         id: The message ID.
         metadata: The metadata of the message (to which phone number it was sent).
         type: The message type (text, image, video, etc).
         from_user: The user who sent the message.
         timestamp: The timestamp when the message was sent.
         reply_to_message: The message to which this message is a reply to. (optional)
+        forwarded: Whether the message was forwarded.
         text: The text of the message (if the message type is text). (optional)
         image: The image of the message (if the message type is image). (optional)
         video: The video of the message (if the message type is video). (optional)
         sticker: The sticker of the message (if the message type is sticker). (optional)
         document: The document of the message (if the message type is document). (optional)
         audio: The audio of the message (if the message type is audio). (optional)
         reaction: The reaction of the message (if the message type is reaction). (optional)
         location: The location of the message (if the message type is location). (optional)
         contacts: The contacts of the message (if the message type is contacts). (optional)
     """
     type: MessageType
     reply_to_message: ReplyToMessage | None
+    forwarded: bool
     text: str | None
     image: Image | None
     video: Video | None
     sticker: Sticker | None
     document: Document | None
     audio: Audio | None
     reaction: Reaction | None
@@ -875,14 +878,15 @@
         return cls(
             _client=client,
             id=message['id'],
             type=msg_type,
             from_user=User.from_dict(value['contacts'][0]),
             timestamp=datetime.fromtimestamp(int(message['timestamp'])),
             metadata=Metadata(**value['metadata']),
+            forwarded=message.get('context', {}).get('forwarded', False),
             reply_to_message=ReplyToMessage.from_dict(message.get('context')),
             text=message['text']['body'] if 'text' in message else None,
             image=Image.from_dict(client=client, data=message.get('image')),
             video=Video.from_dict(client=client, data=message.get('video')),
             sticker=Sticker.from_dict(client=client, data=message.get('sticker')),
             document=Document.from_dict(client=client, data=message.get('document')),
             audio=Audio.from_dict(client=client, data=message.get('audio')),
```

## pywa/webhook.py

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
-from typing import Union, TYPE_CHECKING, Callable
+
+import collections
+from typing import Union, TYPE_CHECKING, Callable, Any
 from pywa.types import Message, CallbackButton, CallbackSelection, MessageStatus, BaseUpdate
 from pywa import utils
 
 if TYPE_CHECKING:
     from pywa import WhatsApp
 
 __all__ = ["Webhook"]
@@ -11,60 +13,66 @@
 
 class Webhook:
     """Register a webhook to listen for incoming messages."""
 
     def __init__(
             self,
             wa_client: WhatsApp,
-            app: Union["flask.Flask", "fastapi.FastAPI"],
+            server: Union["flask.Flask", "fastapi.FastAPI"],
             verify_token: str,
-            webhook_endpoint: str
+            webhook_endpoint: str,
+            filter_updates: bool
     ):
-        if utils.is_flask_app(app):
+        self.handlers: dict[str, list[Callable[[WhatsApp, BaseUpdate | dict], Any]]] = collections.defaultdict(list)
+
+        if utils.is_flask_app(server):
             import flask
 
-            @app.before_request
+            @server.before_request
             def before_request():
                 if flask.request.path != webhook_endpoint:
                     return
                 if flask.request.method == "GET":
                     if verify_token == flask.request.args.get("hub.verify_token"):
                         return flask.request.args.get("hub.challenge"), 200
                     else:
                         return "Error, invalid verification token", 403
                 elif flask.request.method == "POST":
-                    if flask.request.json["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"] \
-                            == wa_client.phone_id:
-                        for raw_update_handler in wa_client._handlers["raw_update"]:
+                    if not filter_updates or (
+                            flask.request.json["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"]
+                            == wa_client.phone_id):
+                        for raw_update_handler in self.handlers["raw_update"]:
                             raw_update_handler(wa_client, flask.request.json)
                         update, key = convert_dict_to_update(client=wa_client, d=flask.request.json)
-                        for handler in wa_client._handlers[key]:  # TODO execute in parallel
+                        for handler in self.handlers[key]:  # TODO execute in parallel
                             handler(wa_client, update)
                     return "ok", 200
 
-        elif utils.is_fastapi_app(app):
+        elif utils.is_fastapi_app(server):
             import fastapi
 
-            @app.middleware("http")
+            @server.middleware("http")
             async def before_request(request: fastapi.Request, call_next: Callable):
                 if request.url.path != webhook_endpoint:
                     return await call_next(request)
                 if request.method == "GET":
                     if verify_token == request.query_params.get("hub.verify_token"):
                         return fastapi.Response(content=request.query_params.get("hub.challenge"), status_code=200)
                     else:
                         return fastapi.Response(content="Error, invalid verification token", status_code=403)
                 elif request.method == "POST":
                     request_body = await request.json()
-                    if request_body["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"] \
-                            == wa_client.phone_id:
-                        for raw_update_handler in wa_client._handlers["raw_update"]:
+                    if not filter_updates or (
+                            request_body["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"]
+                            == wa_client.phone_id):
+                        for raw_update_handler in self.handlers["raw_update"]:
                             raw_update_handler(wa_client, request_body)
                         update, key = convert_dict_to_update(client=wa_client, d=request_body)
-                        for handler in wa_client._handlers[key]:  # TODO execute in parallel
+                        handler: Callable[[WhatsApp, BaseUpdate], Any]
+                        for handler in self.handlers[key]:  # TODO execute in parallel
                             handler(wa_client, update)
                     return fastapi.Response(content="ok", status_code=200)
                 return await call_next(request)
 
         else:
             raise ValueError("The app must be a Flask or FastAPI app.")
```

## Comparing `pywa-0.0.1rc8.dist-info/LICENSE` & `pywa-0.0.1rc9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc8.dist-info/METADATA` & `pywa-0.0.1rc9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc8
+Version: 0.0.1rc9
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
```

## Comparing `pywa-0.0.1rc8.dist-info/RECORD` & `pywa-0.0.1rc9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-pywa/__init__.py,sha256=Fr6IdoF7QKBhoumRqAUgkI-5iHb5-dIWbjJSBWOm2-w,143
-pywa/api.py,sha256=jnP9iAxnW86f1VTndPsvR8aaFglswnrRhXCFbLOvhxg,14911
-pywa/client.py,sha256=YcqpjdvynYlBQDbFbXcbwStk3NXagemyZjy4U-3HA5k,26284
+pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
+pywa/__version__.py,sha256=JO2C_h1DeNnjXWjQYlq8CvqaTeg_9ptCUc5K_xrTJPA,25
+pywa/api.py,sha256=zW7zrkDcWB7df5B0FW2GM6an5wn1cMXxuMCD19krOLU,15077
+pywa/client.py,sha256=_SakRCC-Z-4v7psrTXq6dQg-7w9SsYR1Muam9gvyJ78,26535
 pywa/errors.py,sha256=Vs5SJehEt5PhUrJBbia710gpusoxmTPQmlgDBBnYpWM,989
-pywa/filters.py,sha256=uDkVr9cyJRmEMF9GSoKhUdQZm4I4h3-Q2r4kdJ0dJyU,11021
+pywa/filters.py,sha256=9t2ckte1_gRaKNF6LlISgNY2up3CN7Gnx7IQ1cSEue8,11047
 pywa/handlers.py,sha256=Z4j2jiEwQ0_mzlcybHFDmRg7OR8agakXXkzU85eQyGk,1464
-pywa/types.py,sha256=rz7rPpk31e0zKAGy_qj8Sp04JAvWyWJNcqhjSH3dj4w,32258
+pywa/types.py,sha256=ooFguLLhqx6Y25zyuqQ9O1knwXkWsx-at0RMJhD1Z6g,32457
 pywa/utils.py,sha256=GRTfSvmsuOBd1_Yw2c90XoALqVPuy6HzyvJuqg3xjtI,991
-pywa/webhook.py,sha256=NCJpIrUssm5XXKeRpgupG2GSx38NoTzObKojN-3yMvQ,4161
-pywa-0.0.1rc8.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc8.dist-info/METADATA,sha256=eu_RgdgeWpfODIZwGj8kJU2lYRywjta-yT_iK90TXoI,4489
-pywa-0.0.1rc8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc8.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc8.dist-info/RECORD,,
+pywa/webhook.py,sha256=qt9-W5MLLtMWC-70jlw1vKaWZ4yU7MYwPVNtEtRh8B8,4502
+pywa-0.0.1rc9.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc9.dist-info/METADATA,sha256=EgRAwLw2oRPWjKIxfDlzTA0b6vM2-e03XxXWxnN9L8Q,4489
+pywa-0.0.1rc9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc9.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc9.dist-info/RECORD,,
```

