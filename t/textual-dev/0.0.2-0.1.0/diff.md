# Comparing `tmp/textual_dev-0.0.2.tar.gz` & `tmp/textual_dev-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "textual_dev-0.1.0.tar", max compression
```

## Comparing `textual_dev-0.0.2.tar` & `textual_dev-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,30 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/__about__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/__main__.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/cli.py
--rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/client.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/redirect_output.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/renderables.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/server.py
--rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/previews/__init__.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/previews/borders.py
--rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/previews/colors.css
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/previews/colors.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/previews/easing.css
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 textual_dev-0.0.2/src/textual_dev/previews/easing.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 textual_dev-0.0.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 textual_dev-0.0.2/LICENSE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 textual_dev-0.0.2/README.md
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 textual_dev-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 textual_dev-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-10-25 13:47:18.602610 textual_dev-0.1.0/LICENSE
+-rw-r--r--   0        0        0       44 2022-10-25 13:47:18.602735 textual_dev-0.1.0/README.md
+-rw-r--r--   0        0        0     1673 2023-06-27 12:11:30.096166 textual_dev-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-27 12:09:27.878115 textual_dev-0.1.0/src/textual_dev/__init__.py
+-rw-r--r--   0        0        0       59 2023-06-27 12:09:27.878216 textual_dev-0.1.0/src/textual_dev/__main__.py
+-rw-r--r--   0        0        0     6124 2023-06-27 12:09:27.878759 textual_dev-0.1.0/src/textual_dev/cli.py
+-rw-r--r--   0        0        0     9776 2023-06-27 12:09:27.878909 textual_dev-0.1.0/src/textual_dev/client.py
+-rw-r--r--   0        0        0      246 2023-06-27 12:09:27.879032 textual_dev-0.1.0/src/textual_dev/previews/__init__.py
+-rw-r--r--   0        0        0     1736 2023-06-27 12:09:27.879537 textual_dev-0.1.0/src/textual_dev/previews/borders.py
+-rw-r--r--   0        0        0     5903 2023-06-27 12:09:27.879653 textual_dev-0.1.0/src/textual_dev/previews/colors.css
+-rw-r--r--   0        0        0     2118 2023-06-27 12:09:27.879770 textual_dev-0.1.0/src/textual_dev/previews/colors.py
+-rw-r--r--   0        0        0      748 2023-06-27 12:09:27.879871 textual_dev-0.1.0/src/textual_dev/previews/easing.css
+-rw-r--r--   0        0        0     3691 2023-06-27 12:09:27.879984 textual_dev-0.1.0/src/textual_dev/previews/easing.py
+-rw-r--r--   0        0        0     1861 2023-06-27 12:09:27.880054 textual_dev-0.1.0/src/textual_dev/previews/keys.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:09:27.880084 textual_dev-0.1.0/src/textual_dev/py.typed
+-rw-r--r--   0        0        0     4278 2023-06-27 12:09:27.880682 textual_dev-0.1.0/src/textual_dev/redirect_output.py
+-rw-r--r--   0        0        0     4237 2023-06-27 12:09:27.881448 textual_dev-0.1.0/src/textual_dev/renderables.py
+-rw-r--r--   0        0        0     2278 2023-06-27 12:09:27.881594 textual_dev-0.1.0/src/textual_dev/server.py
+-rw-r--r--   0        0        0    11060 2023-06-27 12:09:27.881773 textual_dev-0.1.0/src/textual_dev/service.py
+-rw-r--r--   0        0        0     4514 2023-06-27 12:09:27.881905 textual_dev-0.1.0/src/textual_dev/tools/diagnose.py
+-rw-r--r--   0        0        0     3901 2023-06-27 12:09:27.881987 textual_dev-0.1.0/src/textual_dev/tools/run.py
+-rw-r--r--   0        0        0      627 2023-06-27 12:09:27.882134 textual_dev-0.1.0/tests/devtools/__init__.py
+-rw-r--r--   0        0        0      791 2023-06-27 12:09:27.882199 textual_dev-0.1.0/tests/devtools/conftest.py
+-rw-r--r--   0        0        0     2889 2023-06-27 12:09:27.882271 textual_dev-0.1.0/tests/devtools/test_devtools.py
+-rw-r--r--   0        0        0     3774 2023-06-27 12:09:27.882343 textual_dev-0.1.0/tests/devtools/test_devtools_client.py
+-rw-r--r--   0        0        0     3726 2023-06-27 12:09:27.882415 textual_dev-0.1.0/tests/devtools/test_redirect_output.py
+-rw-r--r--   0        0        0      253 2023-06-27 12:09:27.882473 textual_dev-0.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0       46 2023-06-27 12:09:27.882573 textual_dev-0.1.0/tests/utilities/__init__.py
+-rw-r--r--   0        0        0     1121 2023-06-27 12:09:27.882648 textual_dev-0.1.0/tests/utilities/wait_for_predicate.py
+-rw-r--r--   0        0        0     1483 1970-01-01 00:00:00.000000 textual_dev-0.1.0/PKG-INFO
```

### Comparing `textual_dev-0.0.2/src/textual_dev/client.py` & `textual_dev-0.1.0/src/textual_dev/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,60 +5,52 @@
 import json
 import pickle
 from asyncio import Queue, QueueFull, Task
 from io import StringIO
 from time import time
 from typing import Any, NamedTuple, Type
 
+import aiohttp
+import msgpack
+from aiohttp import ClientConnectorError, ClientResponseError, ClientWebSocketResponse
 from rich.console import Console
 from rich.segment import Segment
-
 from textual._log import LogGroup, LogVerbosity
+from textual.constants import DEVTOOLS_PORT
 
-
-import aiohttp
-import msgpack
-from aiohttp import (
-    ClientConnectorError,
-    ClientResponseError,
-    ClientWebSocketResponse,
-)
-
-
-DEVTOOLS_PORT = 8081
 WEBSOCKET_CONNECT_TIMEOUT = 3
 LOG_QUEUE_MAXSIZE = 512
 
 
 class DevtoolsLog(NamedTuple):
     """A devtools log message.
 
     Attributes:
-        objects_or_string (tuple[Any, ...]): Corresponds to the data that will
+        objects_or_string: Corresponds to the data that will
             ultimately be passed to Console.print in order to generate the log
             Segments.
-        caller (inspect.FrameInfo): Information about where this log message was
+        caller: Information about where this log message was
             created. In other words, where did the user call `print` or `App.log`
             from. Used to display line number and file name in the devtools window.
     """
 
     objects_or_string: tuple[Any, ...] | str
-    caller: inspect.FrameInfo
+    caller: inspect.Traceback
 
 
 class DevtoolsConsole(Console):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.record = True
 
     def export_segments(self) -> list[Segment]:
         """Return the list of Segments that have be printed using this console
 
         Returns:
-            list[Segment]: The list of Segments that have been printed using this console
+            The list of Segments that have been printed using this console
         """
         with self._record_buffer_lock:
             segments = self._record_buffer[:]
             self._record_buffer.clear()
         return segments
 
 
@@ -90,19 +82,21 @@
 
     A `"client_spillover"` message has a `"payload"` format as follows:
     ```
     {"spillover": <int, the number of messages discarded by rate-limiting>}
     ```
 
     Args:
-        host (str): The host the devtools server is running on, defaults to "127.0.0.1"
-        port (int): The port the devtools server is accessed via, defaults to 8081
+        host: The host the devtools server is running on, defaults to "127.0.0.1"
+        port: The port the devtools server is accessed via, `DEVTOOLS_PORT` by default.
     """
 
-    def __init__(self, host: str = "127.0.0.1", port: int = DEVTOOLS_PORT) -> None:
+    def __init__(self, host: str = "127.0.0.1", port: int | None = None) -> None:
+        if port is None:
+            port = DEVTOOLS_PORT
         self.url: str = f"ws://{host}:{port}"
         self.session: aiohttp.ClientSession | None = None
         self.log_queue_task: Task | None = None
         self.update_console_task: Task | None = None
         self.console: DevtoolsConsole = DevtoolsConsole(file=StringIO())
         self.websocket: ClientWebSocketResponse | None = None
         self.log_queue: Queue[str | bytes | Type[ClientShutdown]] | None = None
@@ -132,14 +126,15 @@
         async def update_console() -> None:
             """Coroutine function scheduled as a Task, which listens on
             the websocket for updates from the server regarding any changes
             in the server Console dimensions. When the client learns of this
             change, it will update its own Console to ensure it renders at
             the correct width for server-side display.
             """
+            assert self.websocket is not None
             async for message in self.websocket:
                 if message.type == aiohttp.WSMsgType.TEXT:
                     message_json = json.loads(message.data)
                     if message_json["type"] == "server_info":
                         payload = message_json["payload"]
                         self.console.width = payload["width"]
                         self.console.height = payload["height"]
@@ -193,35 +188,35 @@
         await self._stop_incoming_message_processing()
 
     @property
     def is_connected(self) -> bool:
         """Checks connection to devtools server.
 
         Returns:
-            bool: True if this host is connected to the server. False otherwise.
+            True if this host is connected to the server. False otherwise.
         """
         if not self.session or not self.websocket:
             return False
         return not (self.session.closed or self.websocket.closed)
 
     def log(
         self,
         log: DevtoolsLog,
         group: LogGroup = LogGroup.UNDEFINED,
         verbosity: LogVerbosity = LogVerbosity.NORMAL,
     ) -> None:
         """Queue a log to be sent to the devtools server for display.
 
         Args:
-            log (DevtoolsLog): The log to write to devtools
+            log: The log to write to devtools
         """
         if isinstance(log.objects_or_string, str):
-            self.console.print(log.objects_or_string)
+            self.console.print(log.objects_or_string, markup=False)
         else:
-            self.console.print(*log.objects_or_string)
+            self.console.print(*log.objects_or_string, markup=False)
 
         segments = self.console.export_segments()
 
         encoded_segments = self._encode_segments(segments)
         message: bytes | None = msgpack.packb(
             {
                 "type": "client_log",
@@ -256,14 +251,14 @@
             self.spillover += 1
 
     @classmethod
     def _encode_segments(cls, segments: list[Segment]) -> bytes:
         """Pickle a list of Segments
 
         Args:
-            segments (list[Segment]): A list of Segments to encode
+            segments: A list of Segments to encode
 
         Returns:
-            bytes: The Segment list pickled with the latest protocol.
+            The Segment list pickled with the latest protocol.
         """
         pickled = pickle.dumps(segments, protocol=4)
         return pickled
```

### Comparing `textual_dev-0.0.2/src/textual_dev/redirect_output.py` & `textual_dev-0.1.0/src/textual_dev/redirect_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import inspect
-
 from typing import TYPE_CHECKING, cast
-from .client import DevtoolsLog
+
 from textual._log import LogGroup, LogVerbosity
+from .client import DevtoolsLog
 
 if TYPE_CHECKING:
     from .client import DevtoolsClient
 
 
 class StdoutRedirector:
     """
@@ -17,33 +17,36 @@
     data written using `print` (or any other stdout writes) to the devtools and/or to the
     log file.
     """
 
     def __init__(self, devtools: DevtoolsClient) -> None:
         """
         Args:
-            devtools (DevtoolsClient): The running Textual app instance.
-            log_file (TextIOWrapper): The log file for the Textual App.
+            devtools: The running Textual app instance.
+            log_file: The log file for the Textual App.
         """
         self.devtools = devtools
         self._buffer: list[DevtoolsLog] = []
 
     def write(self, string: str) -> None:
         """Write the log string to the internal buffer. If the string contains
         a newline character `\n`, the whole string will be buffered and then the
         buffer will be flushed immediately after.
 
         Args:
-            string (str): The string to write to the buffer.
+            string: The string to write to the buffer.
         """
 
         if not self.devtools.is_connected:
             return
 
-        previous_frame = inspect.currentframe().f_back
+        current_frame = inspect.currentframe()
+        assert current_frame is not None
+        previous_frame = current_frame.f_back
+        assert previous_frame is not None
         caller = inspect.getframeinfo(previous_frame)
 
         self._buffer.append(DevtoolsLog(string, caller=caller))
 
         # By default, `print` adds a "\n" suffix which results in a buffer
         # flush. You can choose a different suffix with the `end` parameter.
         # If you modify the `end` parameter to something other than "\n",
@@ -87,15 +90,15 @@
         e.g. `print("a", "b", "c")` is 3 calls to `write`, so we batch
         up these 3 write calls since they come from the same location, so that
         they appear inside the same log message in the devtools window
         rather than a single `print` statement resulting in 3 separate
         logs being displayed.
 
         Args:
-            log_batch (list[DevtoolsLog]): A batch of logs to send to the
+            log_batch: A batch of logs to send to the
                 devtools server as one. Log content will be joined together.
         """
 
         # This code is only called via stdout.write, and so by this point we know
         # that the log message content is a string. The cast below tells mypy this.
         batched_log = "".join(cast(str, log.objects_or_string) for log in log_batch)
         batched_log = batched_log.rstrip()
```

### Comparing `textual_dev-0.0.2/src/textual_dev/renderables.py` & `textual_dev-0.1.0/src/textual_dev/renderables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 from __future__ import annotations
 
-import sys
 from datetime import datetime
 from pathlib import Path
 from typing import Iterable
 
 from importlib_metadata import version
-
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
 from rich.align import Align
 from rich.console import Console, ConsoleOptions, RenderResult
 from rich.markup import escape
 from rich.rule import Rule
 from rich.segment import Segment, Segments
 from rich.style import Style
 from rich.styled import Styled
 from rich.table import Table
 from rich.text import Text
 from textual._log import LogGroup
+from typing_extensions import Literal
 
 DevConsoleMessageLevel = Literal["info", "warning", "error"]
 
 
 class DevConsoleHeader:
     def __init__(self, verbose: bool = False) -> None:
         self.verbose = verbose
@@ -52,18 +46,18 @@
             yield new_line
 
 
 class DevConsoleLog:
     """Renderable representing a single log message
 
     Args:
-        segments (Iterable[Segment]): The segments to display
-        path (str): The path of the file on the client that the log call was made from
-        line_number (int): The line number of the file on the client the log call was made from
-        unix_timestamp (int): Seconds since January 1st 1970
+        segments: The segments to display
+        path: The path of the file on the client that the log call was made from
+        line_number: The line number of the file on the client the log call was made from
+        unix_timestamp: Seconds since January 1st 1970
     """
 
     def __init__(
         self,
         segments: Iterable[Segment],
         path: str,
         line_number: int,
@@ -115,16 +109,16 @@
             yield from self.segments
 
 
 class DevConsoleNotice:
     """Renderable for messages written by the devtools console itself
 
     Args:
-        message (str): The message to display
-        level (DevtoolsMessageLevel): The message level ("info", "warning", or "error").
+        message: The message to display
+        level: The message level ("info", "warning", or "error").
             Determines colors used to render the message and the perceived importance.
     """
 
     def __init__(self, message: str, *, level: DevConsoleMessageLevel = "info") -> None:
         self.message = message
         self.level = level
```

### Comparing `textual_dev-0.0.2/src/textual_dev/server.py` & `textual_dev-0.1.0/src/textual_dev/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from __future__ import annotations
 
 import asyncio
+
 from aiohttp.web import run_app
 from aiohttp.web_app import Application
 from aiohttp.web_request import Request
 from aiohttp.web_routedef import get
 from aiohttp.web_ws import WebSocketResponse
+from textual.constants import DEVTOOLS_PORT
 
-from textual.devtools.client import DEVTOOLS_PORT
-from textual.devtools.service import DevtoolsService
+from .service import DevtoolsService
 
 DEFAULT_SIZE_CHANGE_POLL_DELAY_SECONDS = 2
 
 
 async def websocket_handler(request: Request) -> WebSocketResponse:
     """aiohttp websocket handler for sending data between devtools client and server
 
     Args:
-        request (Request): The request to the websocket endpoint
+        request: The request to the websocket endpoint
 
     Returns:
-        WebSocketResponse: The websocket response
+        The websocket response
     """
     service: DevtoolsService = request.app["service"]
     return await service.handle(request)
 
 
 async def _on_shutdown(app: Application) -> None:
     """aiohttp shutdown handler, called when the aiohttp server is stopped"""
@@ -33,23 +34,28 @@
 
 
 async def _on_startup(app: Application) -> None:
     service: DevtoolsService = app["service"]
     await service.start()
 
 
-def _run_devtools(verbose: bool, exclude: list[str] | None = None) -> None:
+def _run_devtools(
+    verbose: bool, exclude: list[str] | None = None, port: int | None = None
+) -> None:
     app = _make_devtools_aiohttp_app(verbose=verbose, exclude=exclude)
 
-    def noop_print(_: str):
-        return None
+    def noop_print(_: str) -> None:
+        pass
 
     try:
         run_app(
-            app, port=DEVTOOLS_PORT, print=noop_print, loop=asyncio.get_event_loop()
+            app,
+            port=DEVTOOLS_PORT if port is None else port,
+            print=noop_print,
+            loop=asyncio.get_event_loop(),
         )
     except OSError:
         from rich import print
 
         print()
         print("[bold red]Couldn't start server")
         print("Is there another instance of [reverse]textual console[/] running?")
```

### Comparing `textual_dev-0.0.2/src/textual_dev/service.py` & `textual_dev-0.1.0/src/textual_dev/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """Manages a running devtools instance"""
 from __future__ import annotations
 
 import asyncio
 import json
 import pickle
 from json import JSONDecodeError
-from typing import cast
+from typing import Any
 
-from aiohttp import WSMessage, WSMsgType
+import msgpack
+from aiohttp import WSMsgType
 from aiohttp.abc import Request
 from aiohttp.web_ws import WebSocketResponse
 from rich.console import Console
 from rich.markup import escape
-import msgpack
-
 from textual._log import LogGroup
 from textual._time import time
-from textual.devtools.renderables import (
-    DevConsoleLog,
-    DevConsoleNotice,
-    DevConsoleHeader,
-)
+
+from textual_dev.renderables import DevConsoleHeader, DevConsoleLog, DevConsoleNotice
 
 QUEUEABLE_TYPES = {"client_log", "client_spillover"}
 
 
 class DevtoolsService:
     """A running instance of devtools has a single DevtoolsService which is
     responsible for tracking connected client applications.
@@ -34,27 +30,27 @@
         self,
         update_frequency: float,
         verbose: bool = False,
         exclude: list[str] | None = None,
     ) -> None:
         """
         Args:
-            update_frequency (float): The number of seconds to wait between
+            update_frequency: The number of seconds to wait between
                 sending updates of the console size to connected clients.
-            verbose (bool): Enable verbose logging on client.
-            exclude (list[str]): List of log groups to exclude from output.
+            verbose: Enable verbose logging on client.
+            exclude: List of log groups to exclude from output.
         """
         self.update_frequency = update_frequency
         self.verbose = verbose
-        self.exclude = set(name.upper() for name in exclude) if exclude else set()
+        self.exclude = {name.upper() for name in exclude} if exclude else set()
         self.console = Console()
         self.shutdown_event = asyncio.Event()
         self.clients: list[ClientHandler] = []
 
-    async def start(self):
+    async def start(self) -> None:
         """Starts devtools tasks"""
         self.size_poll_task = asyncio.create_task(self._console_size_poller())
         self.console.print(DevConsoleHeader(verbose=self.verbose))
 
     @property
     def clients_connected(self) -> bool:
         """Returns True if there are connected clients, False otherwise."""
@@ -89,15 +85,15 @@
             await self.send_server_info(client_handler)
 
     async def send_server_info(self, client_handler: ClientHandler) -> None:
         """Send information about the server e.g. width and height of Console to
         a connected client.
 
         Args:
-            client_handler (ClientHandler): The client to send information to
+            client_handler: The client to send information to
         """
         await client_handler.send_message(
             {
                 "type": "server_info",
                 "payload": {
                     "width": self.console.width,
                     "height": self.console.height,
@@ -133,27 +129,27 @@
     corresponds to a single running Textual application instance, and is responsible
     for communication with that Textual app.
     """
 
     def __init__(self, request: Request, service: DevtoolsService) -> None:
         """
         Args:
-            request (Request): The aiohttp.Request associated with this client
-            service (DevtoolsService): The parent DevtoolsService which is responsible
+            request: The aiohttp.Request associated with this client
+            service: The parent DevtoolsService which is responsible
                 for the handling of this client.
         """
         self.request = request
         self.service = service
         self.websocket = WebSocketResponse()
 
     async def send_message(self, message: dict[str, object]) -> None:
         """Send a message to a client
 
         Args:
-            message (dict[str, object]): The dict which will be sent
+            message: The dict which will be sent
                 to the client.
         """
         await self.outgoing_queue.put(message)
 
     async def _consume_outgoing(self) -> None:
         """Consume messages from the outgoing (server -> client) Queue."""
         while True:
@@ -212,52 +208,51 @@
             self.incoming_queue.task_done()
 
     async def run(self) -> WebSocketResponse:
         """Prepare the websocket and communication queues, and continuously
         read messages from the queues.
 
         Returns:
-            WebSocketResponse: The WebSocketResponse associated with this client.
+            The WebSocketResponse associated with this client.
         """
 
         await self.websocket.prepare(self.request)
         self.incoming_queue: asyncio.Queue[dict | None] = asyncio.Queue()
         self.outgoing_queue: asyncio.Queue[dict | None] = asyncio.Queue()
         self.outgoing_messages_task = asyncio.create_task(self._consume_outgoing())
         self.incoming_messages_task = asyncio.create_task(self._consume_incoming())
 
         if self.request.remote:
             self.service.console.print(
                 DevConsoleNotice(f"Client '{escape(self.request.remote)}' connected")
             )
         try:
             await self.service.send_server_info(client_handler=self)
-            async for message in self.websocket:
-                message = cast(WSMessage, message)
-
-                if message.type in (WSMsgType.TEXT, WSMsgType.BINARY):
-
+            async for websocket_message in self.websocket:
+                if websocket_message.type in (WSMsgType.TEXT, WSMsgType.BINARY):
+                    message: dict[str, Any]
                     try:
-                        if isinstance(message.data, bytes):
-                            message = msgpack.unpackb(message.data)
+                        if isinstance(websocket_message.data, bytes):
+                            message = msgpack.unpackb(websocket_message.data)
                         else:
-                            message = json.loads(message.data)
+                            message = json.loads(websocket_message.data)
                     except JSONDecodeError:
-                        self.service.console.print(escape(str(message.data)))
+                        self.service.console.print(escape(str(websocket_message.data)))
                         continue
 
                     type = message.get("type")
                     if not type:
                         continue
                     if (
                         type in QUEUEABLE_TYPES
                         and not self.service.shutdown_event.is_set()
                     ):
                         await self.incoming_queue.put(message)
-                elif message.type == WSMsgType.ERROR:
+                elif websocket_message.type == WSMsgType.ERROR:
+                    self.service.console.print(websocket_message.data)
                     self.service.console.print(
                         DevConsoleNotice("Websocket error occurred", level="error")
                     )
                     break
         except Exception as error:
             self.service.console.print(DevConsoleNotice(str(error), level="error"))
         finally:
```

### Comparing `textual_dev-0.0.2/src/textual_dev/previews/borders.py` & `textual_dev-0.1.0/src/textual_dev/previews/borders.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from textual.app import App, ComposeResult
-from textual.constants import BORDERS
-from textual.widgets import Button, Static
 from textual.containers import Vertical
-
+from textual.css.constants import VALID_BORDER
+from textual.widgets import Button, Label
 
 TEXT = """I must not fear.
 Fear is the mind-killer.
 Fear is the little-death that brings total obliteration.
 I will face my fear.
 I will permit it to pass over me and through me.
 And when it has gone past, I will turn the inner eye to see its path.
@@ -23,43 +22,48 @@
 
     BorderButtons > Button {
         width: 100%;
     }
     """
 
     def compose(self) -> ComposeResult:
-        for border in BORDERS:
+        for border in sorted(VALID_BORDER):
             if border:
                 yield Button(border, id=border)
 
 
-class BorderApp(App):
+class BorderApp(App[None]):
     """Demonstrates the border styles."""
 
     CSS = """
+    Screen {
+        align: center middle;
+        overflow: auto;
+    }
     #text {
         margin: 2 4;
         padding: 2 4;
         border: solid $secondary;
         height: auto;
         background: $panel;
         color: $text;
+        border-title-align: center;
     }
     """
 
-    def compose(self):
+    def compose(self) -> ComposeResult:
         yield BorderButtons()
-        self.text = Static(TEXT, id="text")
+        self.text = Label(TEXT, id="text")
+        self.text.shrink = True
+        self.text.border_title = "solid"
         yield self.text
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
+        self.text.border_title = event.button.id
         self.text.styles.border = (
             event.button.id,
             self.stylesheet._variables["secondary"],
         )
-        self.bell()
-
 
-app = BorderApp()
 
 if __name__ == "__main__":
-    app.run()
+    BorderApp().run()
```

### Comparing `textual_dev-0.0.2/src/textual_dev/previews/colors.css` & `textual_dev-0.1.0/src/textual_dev/previews/colors.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+Label {
+    width: 100%;
+}
 
 ColorButtons {
     dock: left;
     overflow-y: auto;
     width: 30;
 }
 
 ColorButtons > Button {
-    width: 30;
+    width: 100%;
 }
 
 ColorsView {
     width: 100%;
     height: 100%;
     align: center middle;
     overflow-x: auto;
@@ -64,15 +67,15 @@
 
 
 .disabled {
     color: $text-disabled;
 }
 
 
-ColorLabel {
+Label {
     padding: 0 0 1 0;
     content-align: center middle;
     color: $text;
     text-style: bold;
 }
 
 .primary-darken-3 {
```

### Comparing `textual_dev-0.0.2/src/textual_dev/previews/colors.py` & `textual_dev-0.1.0/src/textual_dev/previews/colors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from textual.app import App, ComposeResult
-from textual.containers import Horizontal, Vertical
+from textual.containers import Horizontal, Vertical, VerticalScroll
 from textual.design import ColorSystem
-from textual.widget import Widget
-from textual.widgets import Button, Footer, Static
+from textual.widgets import Button, Footer, Label, Static
 
 
-class ColorButtons(Vertical):
+class ColorButtons(VerticalScroll):
     def compose(self) -> ComposeResult:
         for border in ColorSystem.COLOR_NAMES:
             if border:
                 yield Button(border, id=border)
 
 
 class ColorBar(Static):
@@ -24,68 +23,55 @@
     pass
 
 
 class Content(Vertical):
     pass
 
 
-class ColorLabel(Static):
-    pass
-
-
-class ColorsView(Vertical):
+class ColorsView(VerticalScroll):
     def compose(self) -> ComposeResult:
-
         LEVELS = [
             "darken-3",
             "darken-2",
             "darken-1",
             "",
             "lighten-1",
             "lighten-2",
             "lighten-3",
         ]
 
         for color_name in ColorSystem.COLOR_NAMES:
+            with ColorGroup(id=f"group-{color_name}"):
+                yield Label(f'"{color_name}"')
+                for level in LEVELS:
+                    color = f"{color_name}-{level}" if level else color_name
+                    with ColorItem(classes=color):
+                        yield ColorBar(f"${color}", classes="text label")
+                        yield ColorBar("$text-muted", classes="muted")
+                        yield ColorBar("$text-disabled", classes="disabled")
 
-            items: list[Widget] = [ColorLabel(f'"{color_name}"')]
-            for level in LEVELS:
-                color = f"{color_name}-{level}" if level else color_name
-                item = ColorItem(
-                    ColorBar(f"${color}", classes="text label"),
-                    ColorBar(f"$text-muted", classes="muted"),
-                    ColorBar(f"$text-disabled", classes="disabled"),
-                    classes=color,
-                )
-                items.append(item)
 
-            yield ColorGroup(*items, id=f"group-{color_name}")
-
-
-class ColorsApp(App):
+class ColorsApp(App[None]):
     CSS_PATH = "colors.css"
 
     BINDINGS = [("d", "toggle_dark", "Toggle dark mode")]
 
     def compose(self) -> ComposeResult:
         yield Content(ColorButtons())
         yield Footer()
 
     def on_mount(self) -> None:
-        self.call_later(self.update_view)
+        self.call_after_refresh(self.update_view)
 
     def update_view(self) -> None:
         content = self.query_one("Content", Content)
         content.mount(ColorsView())
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
-        self.bell()
         self.query(ColorGroup).remove_class("-active")
         group = self.query_one(f"#group-{event.button.id}", ColorGroup)
         group.add_class("-active")
         group.scroll_visible(top=True, speed=150)
 
 
-app = ColorsApp()
-
 if __name__ == "__main__":
-    app.run()
+    ColorsApp().run()
```

### Comparing `textual_dev-0.0.2/src/textual_dev/previews/easing.css` & `textual_dev-0.1.0/src/textual_dev/previews/easing.css`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+Label {
+    width: 100%;
+}
+
 EasingButtons > Button {
     width: 100%;
 }
 EasingButtons {
     dock: left;
     overflow-y: scroll;
     width: 20;
```

### Comparing `textual_dev-0.0.2/src/textual_dev/previews/easing.py` & `textual_dev-0.1.0/src/textual_dev/previews/easing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,128 +1,126 @@
 from __future__ import annotations
 
 from rich.console import RenderableType
 from textual._easing import EASING
 from textual.app import App, ComposeResult
-from textual.cli.previews.borders import TEXT
-from textual.containers import Container, Horizontal, Vertical
-from textual.reactive import Reactive
+from textual_dev.previews.borders import TEXT
+from textual.containers import Horizontal, Vertical
+from textual.reactive import reactive, var
 from textual.scrollbar import ScrollBarRender
 from textual.widget import Widget
-from textual.widgets import Button, Footer, Static, Input
+from textual.widgets import Button, Footer, Input, Label
 
 VIRTUAL_SIZE = 100
 WINDOW_SIZE = 10
 START_POSITION = 0.0
 END_POSITION = float(VIRTUAL_SIZE - WINDOW_SIZE)
 
 
 class EasingButtons(Widget):
     def compose(self) -> ComposeResult:
         for easing in sorted(EASING, reverse=True):
             yield Button(easing, id=easing)
 
 
 class Bar(Widget):
-    position = Reactive.init(START_POSITION)
-    animation_running = Reactive(False)
+    position = reactive(START_POSITION)
+    animation_running = reactive(False)
 
     DEFAULT_CSS = """
-    
+
     Bar {
         background: $surface;
         color: $error;
     }
 
     Bar.-active {
         background: $surface;
         color: $success;
     }
-    
     """
 
     def watch_animation_running(self, running: bool) -> None:
         self.set_class(running, "-active")
 
     def render(self) -> RenderableType:
         return ScrollBarRender(
             virtual_size=VIRTUAL_SIZE,
             window_size=WINDOW_SIZE,
             position=self.position,
             style=self.rich_style,
         )
 
 
-class EasingApp(App):
-    position = Reactive.init(START_POSITION)
-    duration = Reactive.var(1.0)
+class EasingApp(App[None]):
+    CSS_PATH = "easing.css"
+
+    position = reactive(START_POSITION)
+    duration = var(1.0)
 
-    def on_load(self):
+    def on_load(self) -> None:
         self.bind(
             "ctrl+p", "focus('duration-input')", description="Focus: Duration Input"
         )
         self.bind("ctrl+b", "toggle_dark", description="Toggle Dark")
 
     def compose(self) -> ComposeResult:
         self.animated_bar = Bar()
         self.animated_bar.position = START_POSITION
         duration_input = Input("1.0", placeholder="Duration", id="duration-input")
 
-        self.opacity_widget = Static(
+        self.opacity_widget = Label(
             f"[b]Welcome to Textual![/]\n\n{TEXT}", id="opacity-widget"
         )
 
         yield EasingButtons()
-        yield Vertical(
-            Horizontal(
-                Static("Animation Duration:", id="label"), duration_input, id="inputs"
-            ),
-            Horizontal(
-                self.animated_bar,
-                Container(self.opacity_widget, id="other"),
-            ),
-            Footer(),
-        )
+        with Vertical():
+            with Horizontal(id="inputs"):
+                yield Label("Animation Duration:", id="label")
+                yield duration_input
+            with Horizontal():
+                yield self.animated_bar
+                yield Vertical(self.opacity_widget, id="other")
+            yield Footer()
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
-        self.bell()
         self.animated_bar.animation_running = True
 
-        def _animation_complete():
+        def _animation_complete() -> None:
             self.animated_bar.animation_running = False
 
         target_position = (
             END_POSITION if self.position == START_POSITION else START_POSITION
         )
+        assert event.button.id is not None  # Should be set to an easing function str.
         self.animate(
             "position",
             value=target_position,
             final_value=target_position,
             duration=self.duration,
             easing=event.button.id,
             on_complete=_animation_complete,
         )
 
-    def watch_position(self, value: int):
+    def watch_position(self, value: int) -> None:
         self.animated_bar.position = value
         self.opacity_widget.styles.opacity = 1 - value / END_POSITION
 
-    def on_input_changed(self, event: Input.Changed):
-        if event.sender.id == "duration-input":
+    def on_input_changed(self, event: Input.Changed) -> None:
+        if event.input.id == "duration-input":
             new_duration = _try_float(event.value)
             if new_duration is not None:
                 self.duration = new_duration
 
-    def action_toggle_dark(self):
+    def action_toggle_dark(self) -> None:
         self.dark = not self.dark
 
 
 def _try_float(string: str) -> float | None:
     try:
         return float(string)
     except ValueError:
         return None
 
 
-app = EasingApp(css_path="easing.css")
 if __name__ == "__main__":
-    app.run()
+    EasingApp().run()
```

### Comparing `textual_dev-0.0.2/LICENSE` & `textual_dev-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_dev-0.0.2/PKG-INFO` & `textual_dev-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
 Name: textual-dev
-Version: 0.0.2
-Summary: Textual dev tools
-Project-URL: Documentation, https://github.com/textualize/textual-dev#readme
-Project-URL: Issues, https://github.com/textualize/textual-dev/issues
-Project-URL: Source, https://github.com/textualize/textual-dev
-Author-email: Will McGugan <will@textualize.io>
-License-File: LICENSE
+Version: 0.1.0
+Summary: Development tools for working with Textual
+Home-page: https://github.com/Textualize/textual-dev
+License: MIT
+Author: Will McGugan
+Author-email: will@textualize.io
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Requires-Dist: aiohttp
-Requires-Dist: click
-Requires-Dist: importlib-metadata>=4.11.3
-Requires-Dist: msgpack
-Requires-Dist: msgpack>=1.0.3
-Requires-Dist: rich
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Typing :: Typed
+Requires-Dist: aiohttp (>=3.8.1)
+Requires-Dist: click (>=8.1.2)
+Requires-Dist: msgpack (>=1.0.3)
 Requires-Dist: textual
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # textual-dev
 Development tools for Textual
+
```

