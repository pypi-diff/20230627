# Comparing `tmp/emmett_sentry-0.5.1.tar.gz` & `tmp/emmett_sentry-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett_sentry-0.5.1.tar", max compression
+gzip compressed data, was "emmett_sentry-0.5.2.tar", max compression
```

## Comparing `emmett_sentry-0.5.1.tar` & `emmett_sentry-0.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1486 2023-06-20 12:53:19.919255 emmett_sentry-0.5.1/LICENSE
--rw-r--r--   0        0        0     1845 2023-06-20 12:53:19.919255 emmett_sentry-0.5.1/README.md
--rw-r--r--   0        0        0       31 2023-06-20 12:53:19.919255 emmett_sentry-0.5.1/emmett_sentry/__init__.py
--rw-r--r--   0        0        0       22 2023-06-20 12:53:19.919255 emmett_sentry-0.5.1/emmett_sentry/__version__.py
--rw-r--r--   0        0        0     3415 2023-06-20 12:53:19.919255 emmett_sentry-0.5.1/emmett_sentry/ext.py
--rw-r--r--   0        0        0     7322 2023-06-20 12:53:19.919255 emmett_sentry-0.5.1/emmett_sentry/helpers.py
--rw-r--r--   0        0        0     5197 2023-06-20 12:53:19.919255 emmett_sentry-0.5.1/emmett_sentry/instrument.py
--rw-r--r--   0        0        0     1298 2023-06-20 12:53:19.919255 emmett_sentry-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 emmett_sentry-0.5.1/setup.py
--rw-r--r--   0        0        0     3316 1970-01-01 00:00:00.000000 emmett_sentry-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-06-27 10:39:38.212771 emmett_sentry-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1845 2023-06-27 10:39:38.212771 emmett_sentry-0.5.2/README.md
+-rw-r--r--   0        0        0       31 2023-06-27 10:39:38.212771 emmett_sentry-0.5.2/emmett_sentry/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-27 10:39:38.212771 emmett_sentry-0.5.2/emmett_sentry/__version__.py
+-rw-r--r--   0        0        0     3659 2023-06-27 10:39:38.212771 emmett_sentry-0.5.2/emmett_sentry/ext.py
+-rw-r--r--   0        0        0     7730 2023-06-27 10:39:38.212771 emmett_sentry-0.5.2/emmett_sentry/helpers.py
+-rw-r--r--   0        0        0     5197 2023-06-27 10:39:38.212771 emmett_sentry-0.5.2/emmett_sentry/instrument.py
+-rw-r--r--   0        0        0     1298 2023-06-27 10:39:38.212771 emmett_sentry-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 emmett_sentry-0.5.2/setup.py
+-rw-r--r--   0        0        0     3316 1970-01-01 00:00:00.000000 emmett_sentry-0.5.2/PKG-INFO
```

### Comparing `emmett_sentry-0.5.1/LICENSE` & `emmett_sentry-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett_sentry-0.5.1/README.md` & `emmett_sentry-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `emmett_sentry-0.5.1/emmett_sentry/ext.py` & `emmett_sentry-0.5.2/emmett_sentry/ext.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from typing import Any, Awaitable, Callable, Optional, TypeVar
+from typing import Any, Awaitable, Callable, Dict, Optional, TypeVar
 
 import sentry_sdk
 
 from emmett.extensions import Extension, Signals, listen_signal
 from sentry_sdk.hub import Hub
 
 from .helpers import _capture_exception, _capture_message, patch_routers
@@ -77,31 +77,35 @@
     def _before_send(self, event, hint):
         for callback in self._before_send_callbacks:
             event = callback(event, hint)
             if not event:
                 break
         return event
 
-    def exception(self, exc_info: Any = None, **kwargs: Any):
+    def exception(self, exc_info: Any = None, **kwargs: Dict[str, Any]):
         assert self._initialized, self._errmsg
-        capture_exception(exc_info or sys.exc_info())
+        capture_exception(exc_info or sys.exc_info(), **kwargs)
 
-    def message(self, msg: str, level: Optional[str] = None, **kwargs: Any):
+    def message(self, msg: str, level: Optional[str] = None, **kwargs: Dict[str, Any]):
         assert self._initialized, self._errmsg
-        capture_message(msg, level)
+        capture_message(msg, level, **kwargs)
 
     def extra_scope(self, name: str, builder: Callable[[], Awaitable[Any]]):
         self._scopes[name] = builder
 
     def before_send(self, f: T) -> T:
         self._before_send_callbacks.append(f)
         return f
 
 
-def capture_exception(exception):
+def capture_exception(exception, **contexts):
     with Hub(Hub.current) as hub:
+        for key, val in contexts.items():
+            hub.scope.set_context(key, val)
         _capture_exception(hub, exception)
 
 
-def capture_message(message, level):
+def capture_message(message, level, **contexts):
     with Hub(Hub.current) as hub:
+        for key, val in contexts.items():
+            hub.scope.set_context(key, val)
         _capture_message(hub, message, level=level)
```

### Comparing `emmett_sentry-0.5.1/emmett_sentry/helpers.py` & `emmett_sentry-0.5.2/emmett_sentry/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,35 @@
 
 from emmett import current
 from emmett.asgi.wrappers import Request as ASGIRequest, Websocket as ASGIWebsocket
 from emmett.http import HTTPResponse
 from emmett.rsgi.wrappers import Request as RSGIRequest, Websocket as RSGIWebsocket
 from sentry_sdk.hub import Hub, _should_send_default_pii
 from sentry_sdk.integrations._wsgi_common import _filter_headers
-from sentry_sdk.tracing import Transaction
+from sentry_sdk.tracing import Transaction, TRANSACTION_SOURCE_ROUTE
 from sentry_sdk.utils import capture_internal_exceptions, event_from_exception
 
 
 def _capture_exception(hub, exception):
     with capture_internal_exceptions():
         event, hint = event_from_exception(
             exception,
             client_options=hub.client.options,
             mechanism={"type": "emmett", "handled": False},
         )
         hub.capture_event(event, hint=hint)
 
 
 def _capture_message(hub, message, level = None):
-    hub.capture_message(
-        message,
-        level=level
-    )
+    with capture_internal_exceptions():
+        hub.capture_message(message, level=level)
+
+
+def _configure_transaction(scope, wrapper):
+    scope.set_transaction_name(wrapper.name, source=TRANSACTION_SOURCE_ROUTE)
 
 
 def _process_common_asgi(data, wrapper):
     data["query_string"] = urllib.parse.unquote(
         wrapper._scope["query_string"].decode("latin-1")
     )
 
@@ -64,48 +66,45 @@
 
     with capture_internal_exceptions():
         data = event.setdefault("request", {})
         _process_common(data, wrapper)
         data["method"] = wrapper.method
         data["content_length"] = wrapper.content_length
 
-    event["transaction"] = wrapper.name
-
     return event
 
 
 def _process_ws(event, hint):
     if not hasattr(current, "websocket"):
         return event
 
     wrapper = current.websocket
 
     with capture_internal_exceptions():
         data = event.setdefault("request", {})
         _process_common(data, wrapper)
 
-    event["transaction"] = wrapper.name
-
     return event
 
 
 def _build_http_dispatcher_wrapper_err(ext, dispatch_method):
     @wraps(dispatch_method)
     async def wrap(*args, **kwargs):
         hub = Hub.current
         with hub.push_scope() as scope:
+            _configure_transaction(scope, current.request)
             scope.add_event_processor(_process_http)
             for key, builder in ext._scopes.items():
-                scope.set_extra(key, await builder())
+                scope.set_context(key, await builder())
             try:
                 return await dispatch_method(*args, **kwargs)
             except HTTPResponse:
                 raise
             except Exception as exc:
-                scope.set_extra(
+                scope.set_context(
                     "body_params",
                     await current.request.body_params
                 )
                 _capture_exception(hub, exc)
                 raise
     return wrap
 
@@ -113,48 +112,51 @@
 def _build_http_dispatcher_wrapper_txn(ext, dispatch_method):
     @wraps(dispatch_method)
     async def wrap(*args, **kwargs):
         hub = Hub.current
         with hub.push_scope() as scope:
             scope.add_event_processor(_process_http)
             for key, builder in ext._scopes.items():
-                scope.set_extra(key, await builder())
+                scope.set_context(key, await builder())
 
             proto = (
                 "rsgi" if hasattr(current.request._scope, "rsgi_version") else "asgi"
             )
             txn = Transaction.continue_from_headers(
                 current.request.headers,
-                op="http.server"
+                op="http.server",
+                name=current.request.name,
+                source=TRANSACTION_SOURCE_ROUTE
             )
             txn.set_tag(f"{proto}.type", "http")
 
             with hub.start_transaction(txn):
                 try:
                     return await dispatch_method(*args, **kwargs)
                 except HTTPResponse:
                     raise
                 except Exception as exc:
-                    scope.set_extra(
+                    scope.set_context(
                         "body_params",
                         await current.request.body_params
                     )
                     _capture_exception(hub, exc)
                     raise
     return wrap
 
 
 def _build_ws_dispatcher_wrapper_err(ext, dispatch_method):
     @wraps(dispatch_method)
     async def wrap(*args, **kwargs):
         hub = Hub.current
         with hub.push_scope() as scope:
+            _configure_transaction(scope, current.websocket)
             scope.add_event_processor(_process_ws)
             for key, builder in ext._scopes.items():
-                scope.set_extra(key, await builder())
+                scope.set_context(key, await builder())
             try:
                 return await dispatch_method(*args, **kwargs)
             except Exception as exc:
                 _capture_exception(hub, exc)
                 raise
     return wrap
 
@@ -162,22 +164,24 @@
 def _build_ws_dispatcher_wrapper_txn(ext, dispatch_method):
     @wraps(dispatch_method)
     async def wrap(*args, **kwargs):
         hub = Hub.current
         with hub.push_scope() as scope:
             scope.add_event_processor(_process_ws)
             for key, builder in ext._scopes.items():
-                scope.set_extra(key, await builder())
+                scope.set_context(key, await builder())
 
             proto = (
                 "rsgi" if hasattr(current.websocket._scope, "rsgi_version") else "asgi"
             )
             txn = Transaction.continue_from_headers(
                 current.websocket.headers,
-                op="websocket.server"
+                op="websocket.server",
+                name=current.websocket.name,
+                source=TRANSACTION_SOURCE_ROUTE
             )
             txn.set_tag(f"{proto}.type", "websocket")
 
             with hub.start_transaction(txn):
                 try:
                     return await dispatch_method(*args, **kwargs)
                 except Exception as exc:
```

### Comparing `emmett_sentry-0.5.1/emmett_sentry/instrument.py` & `emmett_sentry-0.5.2/emmett_sentry/instrument.py`

 * *Files identical despite different names*

### Comparing `emmett_sentry-0.5.1/pyproject.toml` & `emmett_sentry-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett-sentry"
-version = "0.5.1"
+version = "0.5.2"
 description = "Sentry extension for Emmett framework"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/sentry"
 repository = "https://github.com/emmett-framework/sentry"
```

### Comparing `emmett_sentry-0.5.1/setup.py` & `emmett_sentry-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['emmett>=2.5.0,<3.0.0', 'sentry-sdk>=1.25.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'emmett-sentry',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'Sentry extension for Emmett framework',
     'long_description': '# Emmett-Sentry\n\nEmmett-Sentry is an [Emmett framework](https://emmett.sh) extension integrating [Sentry](https://sentry.io) monitoring platform.\n\n[![pip version](https://img.shields.io/pypi/v/emmett-sentry.svg?style=flat)](https://pypi.python.org/pypi/emmett-sentry) \n\n## Installation\n\nYou can install Emmett-Sentry using pip:\n\n    pip install emmett-sentry\n\nAnd add it to your Emmett application:\n\n```python\nfrom emmett_sentry import Sentry\n\nsentry = app.use_extension(Sentry)\n```\n\n## Configuration\n\nHere is the complete list of parameters of the extension configuration:\n\n| param | default | description |\n| --- | --- | --- |\n| dsn | | Sentry project\'s DSN |\n| environment | development | Application environment |\n| release | | Application release |\n| auto\\_load | `True` | Automatically inject extension on routes |\n| sample\\_rate | 1 | Error sampling rate |\n| integrations | | List of integrations to pass to the SDK |\n| enable\\_tracing | `False` | Enable tracing on routes |\n| tracing\\_sample\\_rate | | Traces sampling rate |\n| tracing\\_exclude\\_routes | | List of specific routes to exclude from tracing | \n| trace\\_websockets | `False` | Enable tracing on websocket routes |\n| trace\\_orm | `True` | Enable tracing on ORM queries |\n| trace\\_templates | `True` | Enable tracing on templates rendering |\n| trace\\_sessions | `True` | Enable tracing on sessions load/store |\n| trace\\_cache | `True` | Enable tracing on cache get/set |\n| trace\\_pipes | `False` | Enable tracing on pipes |\n\n## Usage\n\nThe extension exposes two methods to manually track events:\n\n- exception\n- message\n\nYou call these methods directly within your code:\n\n```python\n# track an error\ntry:\n    1 / 0\nexcept Exception:\n    sentry.exception()\n\n# track a message\nsentry.message("some event", level="info")\n```\n\n## License\n\nEmmett-Sentry is released under BSD license.\n',
     'author': 'Giovanni Barillari',
     'author_email': 'g@baro.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/emmett-framework/sentry',
```

### Comparing `emmett_sentry-0.5.1/PKG-INFO` & `emmett_sentry-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett-sentry
-Version: 0.5.1
+Version: 0.5.2
 Summary: Sentry extension for Emmett framework
 Home-page: https://github.com/emmett-framework/sentry
 License: BSD-3-Clause
 Keywords: sentry,logging,emmett
 Author: Giovanni Barillari
 Author-email: g@baro.dev
 Requires-Python: >=3.8,<4.0
```

