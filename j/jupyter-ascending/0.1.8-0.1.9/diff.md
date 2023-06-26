# Comparing `tmp/jupyter_ascending-0.1.8.tar.gz` & `tmp/jupyter_ascending-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_ascending-0.1.8.tar", last modified: Thu Nov 12 00:37:03 2020, max compression
+gzip compressed data, was "jupyter_ascending-0.1.9.tar", last modified: Thu Nov 12 19:25:13 2020, max compression
```

## Comparing `jupyter_ascending-0.1.8.tar` & `jupyter_ascending-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1067 2020-07-13 15:02:59.394630 jupyter_ascending-0.1.8/LICENSE
--rw-r--r--   0        0        0      793 2020-10-28 21:41:31.381399 jupyter_ascending-0.1.8/jupyter_ascending/__init__.py
--rw-r--r--   0        0        0      418 2020-10-28 21:57:42.347254 jupyter_ascending-0.1.8/jupyter_ascending/_environment.py
--rw-r--r--   0        0        0      250 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/_frontend.py
--rw-r--r--   0        0        0      253 2020-11-12 00:26:01.819124 jupyter_ascending-0.1.8/jupyter_ascending/_version.py
--rw-r--r--   0        0        0       57 2020-11-11 23:04:07.732187 jupyter_ascending-0.1.8/jupyter_ascending/errors.py
--rw-r--r--   0        0        0     1714 2020-10-28 23:05:03.309157 jupyter_ascending-0.1.8/jupyter_ascending/extension.py
--rw-r--r--   0        0        0      498 2020-11-12 00:02:27.898206 jupyter_ascending-0.1.8/jupyter_ascending/functional.py
--rw-r--r--   0        0        0     1938 2020-11-12 00:22:18.563191 jupyter_ascending-0.1.8/jupyter_ascending/handlers/__init__.py
--rw-r--r--   0        0        0    11381 2020-07-13 16:31:41.658357 jupyter_ascending-0.1.8/jupyter_ascending/handlers/jupyter_notebook.py
--rw-r--r--   0        0        0     6121 2020-11-12 00:33:33.667307 jupyter_ascending-0.1.8/jupyter_ascending/handlers/jupyter_server.py
--rw-r--r--   0        0        0      415 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/json_requests.py
--rw-r--r--   0        0        0     7573 2020-07-13 15:25:36.568884 jupyter_ascending-0.1.8/jupyter_ascending/labextension/jupyter_ascending-0.1.0.tgz
--rw-r--r--   0        0        0      633 2020-11-12 00:36:05.791425 jupyter_ascending-0.1.8/jupyter_ascending/logger.py
--rw-r--r--   0        0        0      370 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/nbextension/__init__.py
--rw-r--r--   0        0        0     5614 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/nbextension/static/extension.js
--rw-r--r--   0        0        0     9951 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/nbextension/static/index.js
--rw-r--r--   0        0        0    28944 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/nbextension/static/index.js.map
--rw-r--r--   0        0        0        0 2020-07-13 15:25:36.564884 jupyter_ascending-0.1.8/jupyter_ascending/notebook/__init__.py
--rw-r--r--   0        0        0     1839 2020-07-13 15:25:36.564884 jupyter_ascending-0.1.8/jupyter_ascending/notebook/data_types.py
--rw-r--r--   0        0        0      830 2020-07-13 15:25:36.564884 jupyter_ascending-0.1.8/jupyter_ascending/notebook/evolve.py
--rw-r--r--   0        0        0     8132 2020-07-13 16:29:48.582823 jupyter_ascending-0.1.8/jupyter_ascending/notebook/merge.py
--rw-r--r--   0        0        0      423 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/requests/__init__.py
--rw-r--r--   0        0        0     1401 2020-11-12 00:27:57.543139 jupyter_ascending-0.1.8/jupyter_ascending/requests/execute.py
--rw-r--r--   0        0        0      545 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/requests/get_status.py
--rw-r--r--   0        0        0     1277 2020-07-13 16:11:23.831201 jupyter_ascending-0.1.8/jupyter_ascending/requests/sync.py
--rw-r--r--   0        0        0        0 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/tests/__init__.py
--rw-r--r--   0        0        0     5951 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/tests/test_cell_matching.py
--rw-r--r--   0        0        0      466 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/tests/test_nbextension_path.py
--rw-r--r--   0        0        0     3184 2020-11-12 00:31:48.423239 jupyter_ascending-0.1.8/jupyter_ascending/tests/test_notebook_matching.py
--rw-r--r--   0        0        0     1534 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/utils.py
--rw-r--r--   0        0        0     1376 2020-07-13 15:25:36.564884 jupyter_ascending-0.1.8/jupyter_ascending/watchers/file_watcher.py
--rw-r--r--   0        0        0     1202 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.8/jupyter_ascending/widget.py
--rw-r--r--   0        0        0      638 2020-11-12 00:26:08.759124 jupyter_ascending-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1087 2020-11-12 00:37:03.080345 jupyter_ascending-0.1.8/setup.py
--rw-r--r--   0        0        0      697 2020-11-12 00:37:03.080562 jupyter_ascending-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2020-07-13 15:02:59.394630 jupyter_ascending-0.1.9/LICENSE
+-rw-r--r--   0        0        0      793 2020-10-28 21:41:31.381399 jupyter_ascending-0.1.9/jupyter_ascending/__init__.py
+-rw-r--r--   0        0        0      418 2020-10-28 21:57:42.347254 jupyter_ascending-0.1.9/jupyter_ascending/_environment.py
+-rw-r--r--   0        0        0      250 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.9/jupyter_ascending/_frontend.py
+-rw-r--r--   0        0        0      253 2020-11-12 19:24:59.489903 jupyter_ascending-0.1.9/jupyter_ascending/_version.py
+-rw-r--r--   0        0        0       57 2020-11-11 23:04:07.732187 jupyter_ascending-0.1.9/jupyter_ascending/errors.py
+-rw-r--r--   0        0        0     1714 2020-10-28 23:05:03.309157 jupyter_ascending-0.1.9/jupyter_ascending/extension.py
+-rw-r--r--   0        0        0      498 2020-11-12 00:02:27.898206 jupyter_ascending-0.1.9/jupyter_ascending/functional.py
+-rw-r--r--   0        0        0     1938 2020-11-12 00:22:18.563191 jupyter_ascending-0.1.9/jupyter_ascending/handlers/__init__.py
+-rw-r--r--   0        0        0    12815 2020-11-12 19:02:05.345868 jupyter_ascending-0.1.9/jupyter_ascending/handlers/jupyter_notebook.py
+-rw-r--r--   0        0        0     5173 2020-11-12 17:55:25.091023 jupyter_ascending-0.1.9/jupyter_ascending/handlers/jupyter_server.py
+-rw-r--r--   0        0        0      479 2020-11-12 17:45:30.090828 jupyter_ascending-0.1.9/jupyter_ascending/json_requests.py
+-rw-r--r--   0        0        0     7573 2020-07-13 15:25:36.568884 jupyter_ascending-0.1.9/jupyter_ascending/labextension/jupyter_ascending-0.1.0.tgz
+-rw-r--r--   0        0        0      633 2020-11-12 00:36:05.791425 jupyter_ascending-0.1.9/jupyter_ascending/logger.py
+-rw-r--r--   0        0        0      370 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.9/jupyter_ascending/nbextension/__init__.py
+-rw-r--r--   0        0        0     7411 2020-11-12 19:10:41.109108 jupyter_ascending-0.1.9/jupyter_ascending/nbextension/static/extension.js
+-rw-r--r--   0        0        0     9951 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.9/jupyter_ascending/nbextension/static/index.js
+-rw-r--r--   0        0        0    28944 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.9/jupyter_ascending/nbextension/static/index.js.map
+-rw-r--r--   0        0        0        0 2020-07-13 15:25:36.564884 jupyter_ascending-0.1.9/jupyter_ascending/notebook/__init__.py
+-rw-r--r--   0        0        0     1964 2020-11-12 19:20:35.514579 jupyter_ascending-0.1.9/jupyter_ascending/notebook/data_types.py
+-rw-r--r--   0        0        0     1205 2020-11-12 19:14:20.347938 jupyter_ascending-0.1.9/jupyter_ascending/notebook/evolve.py
+-rw-r--r--   0        0        0     8130 2020-11-12 19:20:37.058574 jupyter_ascending-0.1.9/jupyter_ascending/notebook/merge.py
+-rw-r--r--   0        0        0      423 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.9/jupyter_ascending/requests/__init__.py
+-rw-r--r--   0        0        0     1401 2020-11-12 00:27:57.543139 jupyter_ascending-0.1.9/jupyter_ascending/requests/execute.py
+-rw-r--r--   0        0        0      695 2020-11-12 16:49:01.807774 jupyter_ascending-0.1.9/jupyter_ascending/requests/execute_all.py
+-rw-r--r--   0        0        0      545 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.9/jupyter_ascending/requests/get_status.py
+-rw-r--r--   0        0        0     1277 2020-07-13 16:11:23.831201 jupyter_ascending-0.1.9/jupyter_ascending/requests/sync.py
+-rw-r--r--   0        0        0        0 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.9/jupyter_ascending/tests/__init__.py
+-rw-r--r--   0        0        0     6323 2020-11-12 19:21:27.482432 jupyter_ascending-0.1.9/jupyter_ascending/tests/test_cell_matching.py
+-rw-r--r--   0        0        0      466 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.9/jupyter_ascending/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0     3184 2020-11-12 00:31:48.423239 jupyter_ascending-0.1.9/jupyter_ascending/tests/test_notebook_matching.py
+-rw-r--r--   0        0        0     1534 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.9/jupyter_ascending/utils.py
+-rw-r--r--   0        0        0     1376 2020-07-13 15:25:36.564884 jupyter_ascending-0.1.9/jupyter_ascending/watchers/file_watcher.py
+-rw-r--r--   0        0        0     1202 2020-07-13 15:25:36.560884 jupyter_ascending-0.1.9/jupyter_ascending/widget.py
+-rw-r--r--   0        0        0      638 2020-11-12 19:25:04.369892 jupyter_ascending-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1087 2020-11-12 19:25:14.023751 jupyter_ascending-0.1.9/setup.py
+-rw-r--r--   0        0        0      697 2020-11-12 19:25:14.023954 jupyter_ascending-0.1.9/PKG-INFO
```

### Comparing `jupyter_ascending-0.1.8/LICENSE` & `jupyter_ascending-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/__init__.py` & `jupyter_ascending-0.1.9/jupyter_ascending/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/extension.py` & `jupyter_ascending-0.1.9/jupyter_ascending/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/handlers/__init__.py` & `jupyter_ascending-0.1.9/jupyter_ascending/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/handlers/jupyter_notebook.py` & `jupyter_ascending-0.1.9/jupyter_ascending/handlers/jupyter_notebook.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import threading
 from http.server import HTTPServer
+from inspect import signature
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Type
 
 import ipywidgets as widgets
 import jupytext
 from IPython.display import display
 from ipykernel.comm import Comm
 from jsonrpcclient import request
 
 from jupyter_ascending._environment import EXECUTE_HOST_URL
 from jupyter_ascending.handlers import ServerMethods
 from jupyter_ascending.handlers import generate_request_handler
+from jupyter_ascending.json_requests import ExecuteAllRequest
 from jupyter_ascending.json_requests import ExecuteRequest
 from jupyter_ascending.json_requests import FocusCellRequest
+from jupyter_ascending.json_requests import GetStatusRequest
 from jupyter_ascending.json_requests import SyncRequest
 from jupyter_ascending.logger import J_LOGGER
 from jupyter_ascending.notebook.data_types import JupyterCell
 from jupyter_ascending.notebook.data_types import NotebookContents
 from jupyter_ascending.notebook.merge import OpCodeAction
 from jupyter_ascending.notebook.merge import OpCodes
 from jupyter_ascending.notebook.merge import opcode_merge_cell_contents
@@ -90,46 +94,79 @@
 def status_func(comm, open_msg):
     @comm.on_msg
     def _recv(msg):
         print(msg)
         J_LOGGER.warning(msg)
 
 
-@notebook_server_methods.add
-def handle_execute_request(data: dict) -> str:
-    request = ExecuteRequest(**data)
+def dispatch_json_request(f):
+    """
+    Automatically dispatch a json request based on the request_type.
+    This means we don't have to repeat ourselves.
+
+    Adds it to notebook_server_methods
+    """
+
+    # Get the type from the first argument of the function.
+    #   This will define the name that we use to generate the method handling.
+    request_type = signature(f).parameters["request_type"].annotation.__args__[0]
+
+    def wrapped(data: Dict) -> str:
+        return f(request_type, data)
+
+    wrapped.__name__ = request_type.__name__
+
+    return notebook_server_methods.add(wrapped)
+
+
+@dispatch_json_request
+def handle_execute_request(request_type: Type[ExecuteRequest], data: dict) -> str:
+    request = request_type(**data)
 
     comm = get_comm()
     execute_cell_contents(comm, request.cell_index)
 
     return f"Executing cell `{request.cell_index}`"
 
 
-@notebook_server_methods.add
-def handle_sync_request(data: dict) -> str:
-    request = SyncRequest(**data)
+@dispatch_json_request
+def handle_execute_all_request(request_type: Type[ExecuteAllRequest], data: dict) -> str:
+    request = request_type(**data)
+
+    # TODO: Remind mysefyl why I don't need to say the filename here...
+    comm = get_comm()
+    execute_all_cells(comm)
+
+    return f"Executing all cells in {request.file_name}"
+
+
+@dispatch_json_request
+def handle_sync_request(request_type: Type[SyncRequest], data: dict) -> str:
+    request = request_type(**data)
 
     comm = get_comm()
 
     result = jupytext.reads(request.contents, fmt="py:percent")
+    # import ipdb
+    # ipdb.set_trace()
     update_cell_contents(comm, result)
 
     return "Syncing all cells"
 
 
-@notebook_server_methods.add
-def handle_focus_cell_request(data: dict) -> str:
-    request = FocusCellRequest(**data)
+@dispatch_json_request
+def handle_focus_cell_request(request_type: Type[FocusCellRequest], data: dict) -> str:
+    request = request_type(**data)
 
     print(request)
     raise NotImplementedError
 
 
-@notebook_server_methods.add
-def handle_get_status_request(data: dict) -> str:
+@dispatch_json_request
+def handle_get_status_request(request_type: Type[GetStatusRequest], data: dict) -> str:
     J_LOGGER.info("Attempting get_status")
 
     comm = get_comm()
     comm.send({"command": "get_status"})
 
     J_LOGGER.info("Sent get_status")
 
@@ -291,14 +328,15 @@
             if current_cells:
                 current_cells.pop(0)
 
                 comm.send(
                     {
                         "command": "op_code__replace_cell",
                         "cell_number": cell_number,
+                        "cell_type": updated_notebook.cells[cell_number].cell_type,
                         "cell_contents": updated_notebook.cells[cell_number].joined_source,
                     }
                 )
             # Otherwise, we have new cells to insert so we don't overwrite existing cells
             else:
                 net_shift = perform_op_code(
                     comm,
@@ -337,7 +375,11 @@
         raise NotImplementedError
 
     return net_shift
 
 
 def execute_cell_contents(comm: Comm, cell_number: int) -> None:
     comm.send({"command": "execute", "cell_number": cell_number})
+
+
+def execute_all_cells(comm: Comm) -> None:
+    comm.send({"command": "execute_all"})
```

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/handlers/jupyter_server.py` & `jupyter_ascending-0.1.9/jupyter_ascending/handlers/jupyter_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,21 +13,15 @@
 
 from jupyter_ascending._environment import EXECUTE_HOST_LOCATION
 from jupyter_ascending._environment import EXECUTE_HOST_URL
 from jupyter_ascending.errors import UnableToFindNotebookException
 from jupyter_ascending.functional import get_matching_tail_tokens
 from jupyter_ascending.handlers import ServerMethods
 from jupyter_ascending.handlers import generate_request_handler
-from jupyter_ascending.handlers.jupyter_notebook import handle_execute_request
-from jupyter_ascending.handlers.jupyter_notebook import handle_get_status_request
-from jupyter_ascending.handlers.jupyter_notebook import handle_sync_request
-from jupyter_ascending.json_requests import ExecuteRequest
-from jupyter_ascending.json_requests import GetStatusRequest
 from jupyter_ascending.json_requests import JsonBaseRequest
-from jupyter_ascending.json_requests import SyncRequest
 from jupyter_ascending.logger import J_LOGGER
 
 GenericJsonRequest = TypeVar("GenericJsonRequest", bound=JsonBaseRequest)
 T = TypeVar("T")
 
 _REGISTERED_SERVERS: Dict[str, int] = {}
 
@@ -118,15 +112,15 @@
 
 
 def request_notebook_command(json_request: GenericJsonRequest):
     try:
         result = request(
             EXECUTE_HOST_URL,
             perform_notebook_request.__name__,
-            command_name=_map_json_request_to_function_name(json_request),
+            command_name=type(json_request).__name__,
             notebook_path=json_request.file_name,
             data=attr.asdict(json_request),
         )
 
         if not result.data.result:
             return
 
@@ -135,27 +129,14 @@
 
     except ConnectionError as e:
         J_LOGGER.error(f"Unable to connect to server. Perhaps notebook is not running? {e}")
     except ReceivedNon2xxResponseError as e:
         J_LOGGER.error(f"Unable to process request. Perhaps something else is running on this port? {e}")
 
 
-def _map_json_request_to_function_name(json_request: GenericJsonRequest) -> str:
-    # TODO: Move this to a dictionary, and check all non-abstract children of BaseJsonRequest
-
-    if isinstance(json_request, ExecuteRequest):
-        return handle_execute_request.__name__
-    elif isinstance(json_request, SyncRequest):
-        return handle_sync_request.__name__
-    elif isinstance(json_request, GetStatusRequest):
-        return handle_get_status_request.__name__
-    else:
-        assert False, json_request
-
-
 def start_server_in_thread():
     try:
         server_executor = HTTPServer(EXECUTE_HOST_LOCATION, JupyterServerRequestHandler)
     except OSError:
         print(f"It appears you already are using {EXECUTE_HOST_LOCATION}")
         print("Use the environment variable: 'JUPYTER_ASCENDING_EXECUTE_PORT' to set a new port")
```

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/labextension/jupyter_ascending-0.1.0.tgz` & `jupyter_ascending-0.1.9/jupyter_ascending/labextension/jupyter_ascending-0.1.0.tgz`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/logger.py` & `jupyter_ascending-0.1.9/jupyter_ascending/logger.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/nbextension/static/extension.js` & `jupyter_ascending-0.1.9/jupyter_ascending/nbextension/static/extension.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 // Entry point for the notebook bundle containing custom model definitions.
 
 // debugger;
-define(['base/js/namespace'], function(Jupyter) {
-    'use strict';
+define(["base/js/namespace"], function(Jupyter) {
+    "use strict";
 
-    window['requirejs'].config({
+    window["requirejs"].config({
         map: {
-            '*': {
-                jupyter_ascending: 'nbextensions/jupyter_ascending/index',
+            "*": {
+                jupyter_ascending: "nbextensions/jupyter_ascending/index",
             },
         },
     });
 
     const IS_DEBUG = false;
-    const TARGET_NAME = 'AUTO_SYNC::notebook';
+    const TARGET_NAME = "AUTO_SYNC::notebook";
 
     function get_notebook_name() {
         // return window.document.getElementById("notebook_name").innerHTML;
         return Jupyter.notebook.notebook_path;
     }
 
     function is_synced_notebook() {
-        return get_notebook_name().includes('.synced.ipynb');
+        return get_notebook_name().includes(".synced.ipynb");
     }
 
     function get_cell_from_notebook(cell_number) {
         let cell = Jupyter.notebook.get_cell(cell_number);
 
         while (cell === null) {
             // Kind of meh hack to just keep spamming cells at bottom until we get to the cell we want.
@@ -37,162 +37,182 @@
         return cell;
     }
 
     function update_cell_contents(data) {
         let cell = get_cell_from_notebook(data.cell_number);
 
         cell.set_text(data.cell_contents);
+
+        // Changed cell types.
+        if (cell.cell_type !== data.cell_type) {
+            if (data.cell_type === "markdown") {
+                Jupyter.notebook.cells_to_markdown([data.cell_number]);
+            } else if (data.cell_type === "code") {
+                Jupyter.notebook.cells_to_code([data.cell_number]);
+            }
+        }
+
+        // Markdown cells need a re-render when we update them.
+        if (cell.cell_type === "markdown") {
+            cell.render();
+        }
     }
 
     function execute_cell_contents(data) {
         let cell = get_cell_from_notebook(data.cell_number);
 
         cell.focus_cell();
         cell.execute();
 
         // TODO: ??
         cell.focus_cell();
     }
 
+    function execute_all_cells() {
+        Jupyter.notebook.execute_all_cells();
+    }
+
     function op_code__delete_cells(data) {
-        console.log('Deleting cell...', data);
+        console.log("Deleting cell...", data);
 
         Jupyter.notebook.delete_cells(data.cell_indices);
     }
 
     function op_code__insert_cell(data) {
-        console.log('Inserting cell...', data);
+        console.log("Inserting cell...", data);
 
         let new_cell = Jupyter.notebook.insert_cell_at_index(
             data.cell_type,
             data.cell_number
         );
         new_cell.set_text(data.cell_contents);
+
+        // Markdown cells need a re-render when we update them.
+        if (new_cell.cell_type === "markdown") {
+            new_cell.render();
+        }
     }
 
     function op_code__replace_cell(data) {
-        console.log('Replacing cell...', data);
+        console.log("Replacing cell...", data);
 
         update_cell_contents(data);
     }
 
     // function focus_cell(data) {
     //   let cell = get_cell_from_notebook(data.cell_number);
 
     //   cell.focus_cell();
     //   // TODO: Focus the output so you can see all of it if it's long
     // }
 
     function get_status(comm_obj) {
         comm_obj.send({
-            command: 'update_status',
+            command: "update_status",
             status: Jupyter.notebook.get_cells(),
         });
     }
 
     function start_sync_notebook(comm_obj, msg) {
         comm_obj.send({
-            command: 'merge_notebooks',
+            command: "merge_notebooks",
             javascript_cells: Jupyter.notebook.get_cells(),
             new_notebook: msg.content.data.cells,
         });
     }
 
     function create_and_register_comm() {
         // Make sure that the extension is loaded.
         //  TODO: Perhaps it's possible to not do  this if it's already loaded,
         //  but it's fine to be run multiple times.
         //
         //  As a note, I think some people would probably disapprove of this?
         //  It just runs code... but that's what plugins do?
-        Jupyter.notebook.kernel.execute('%load_ext jupyter_ascending');
+        Jupyter.notebook.kernel.execute("%load_ext jupyter_ascending");
 
         Jupyter.notebook.kernel.comm_manager.register_target(
             TARGET_NAME,
             // comm is the frontend comm instance
             // msg is the comm_open message, which can carry data
             function(comm, _msg) {
                 // Register handlers for later messages:
                 comm.on_msg(function(msg) {
                     if (IS_DEBUG) {
-                        console.log('Processing a message');
+                        console.log("Processing a message");
                         console.log(msg);
                     }
 
                     const data = msg.content.data;
                     const command = data.command;
 
-                    if (command === 'start_sync_notebook') {
-                        console.log('Starting Sync');
-                        return start_sync_notebook(comm, msg);
-                    }
-
-                    if (command === 'op_code__delete_cells') {
-                        return op_code__delete_cells(data);
-                    }
-
-                    if (command === 'op_code__insert_cell') {
-                        return op_code__insert_cell(data);
-                    }
-
-                    if (command === 'op_code__replace_cell') {
-                        return op_code__replace_cell(data);
-                    }
-
-                    if (command === 'get_status') {
-                        console.log('Sending get_status');
-                        return get_status(comm);
-                    }
-
-                    if (msg.content.data.command === 'update') {
-                        update_cell_contents(msg.content.data);
-                    } else if (msg.content.data.command === 'execute') {
-                        execute_cell_contents(msg.content.data);
-                    } else if (msg.content.data.command === 'status') {
-                        console.log('give em the status');
-                    } else {
-                        // debugger;
-                        console.log('Got an unexpected message: ', msg);
+                    switch (command) {
+                        case "start_sync_notebook":
+                            console.log("Starting Sync");
+                            return start_sync_notebook(comm, msg);
+                        case "op_code__delete_cells":
+                            return op_code__delete_cells(data);
+                        case "op_code__insert_cell":
+                            return op_code__insert_cell(data);
+                        case "op_code__replace_cell":
+                            return op_code__replace_cell(data);
+                        case "get_status":
+                            console.log("Sending get_status");
+                            return get_status(comm);
+                        case "update":
+                            return update_cell_contents(data);
+                        case "execute":
+                            return execute_cell_contents(data);
+                        case "execute_all":
+                            return execute_all_cells();
+                        case "status":
+                            console.log("give em the status");
+                            return;
+                        default:
+                            console.log("Got an unexpected message: ", msg);
+                            return;
                     }
                 });
 
                 comm.on_close(function(msg) {
-                    console.log('close', msg);
+                    console.log("close", msg);
                 });
             }
         );
     }
 
     // Export the required load_ipython_extension function
     return {
         load_ipython_extension: function() {
             Jupyter.notebook.config.loaded
                 .then(
                     function on_config_loaded() {
-                        console.log('Loaded config...');
+                        console.log("Loaded config...");
                     },
                     function on_config_error() {
-                        console.log('ERROR OF LOADING...???');
+                        console.log("ERROR OF LOADING...???");
                     }
                 )
                 .then(function actually_load() {
-                    console.log('===================================');
+                    console.log("===================================");
                     // console.log(ascend);
-                    console.log('Loading Jupyter Ascending extension...');
-                    console.log('Opening... ', get_notebook_name());
-                    console.log('Is synced: ', is_synced_notebook());
+                    console.log("Loading Jupyter Ascending extension...");
+                    console.log("Opening... ", get_notebook_name());
+                    console.log("Is synced: ", is_synced_notebook());
 
-                    console.log('Attemping create comm...');
+                    console.log("Attemping create comm...");
                     if (Jupyter.notebook.kernel) {
                         create_and_register_comm();
                     } else {
-                        Jupyter.notebook.events.one('kernel_ready.Kernel', () => {
-                            create_and_register_comm();
-                        });
+                        Jupyter.notebook.events.one(
+                            "kernel_ready.Kernel",
+                            () => {
+                                create_and_register_comm();
+                            }
+                        );
                     }
-                    console.log('... success!');
+                    console.log("... success!");
 
-                    console.log('===================================');
+                    console.log("===================================");
                 });
         },
     };
 });
```

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/nbextension/static/index.js` & `jupyter_ascending-0.1.9/jupyter_ascending/nbextension/static/index.js`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/nbextension/static/index.js.map` & `jupyter_ascending-0.1.9/jupyter_ascending/nbextension/static/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/notebook/data_types.py` & `jupyter_ascending-0.1.9/jupyter_ascending/notebook/data_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     execution_count: Optional[int] = attr.ib(default=None)
     # metadata: Optional[Dict[str, Any]] = attr.ib(default=None, converter=frozen_dict)
 
     @property
     def joined_source(self) -> str:
         return "".join(self.source)
 
+    @property
+    def complete_source(self) -> str:
+        return f"{self.cell_type}::::{self.joined_source}"
+
     # def __eq__(self, o):
     #     if not isinstance(o, JupyterCell):
     #         return False
 
     #     return self.source == o.source and self.index == o.index and self.cell_type == o.cell_type
 
     # def __hash__(self):
@@ -55,15 +59,15 @@
 @attr.dataclass
 class NotebookContents:
     cells: List[JupyterCell]
 
     # TODO: Make sure cells are in the right order
 
     def _cell_insides(self):
-        return [(x.index, x.source) for x in self.cells]
+        return [(x.index, x.cell_type, x.source) for x in self.cells]
 
     def content_equals(self, other: "NotebookContents") -> bool:
         return self._cell_insides() == other._cell_insides()
 
 
 @attr.dataclass
 class Movement:
```

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/notebook/evolve.py` & `jupyter_ascending-0.1.9/jupyter_ascending/notebook/evolve.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,7 +17,18 @@
     for cell in contents.cells:
         if cell.index == index:
             new_cells.append(attr.evolve(cell, source=source))
         else:
             new_cells.append(cell)
 
     return evolve_notebook_cells(contents, new_cells)
+
+
+def evolve_cell_type(contents: NotebookContents, index: int, cell_type: str) -> NotebookContents:
+    new_cells: List[JupyterCell] = []
+    for cell in contents.cells:
+        if cell.index == index:
+            new_cells.append(attr.evolve(cell, cell_type=cell_type))
+        else:
+            new_cells.append(cell)
+
+    return evolve_notebook_cells(contents, new_cells)
```

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/notebook/merge.py` & `jupyter_ascending-0.1.9/jupyter_ascending/notebook/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from jupyter_ascending.notebook.data_types import NotebookContents
 from jupyter_ascending.notebook.evolve import evolve_notebook_cells
 
 Number = Union[int, float]
 
 
 def _get_raw_contents(notebook: NotebookContents) -> Tuple[str, ...]:
-    return tuple("\n".join(x.source) for x in notebook.cells)
+    return tuple(x.complete_source for x in notebook.cells)
 
 
 class OpCodes(Enum):
     EQUAL = "equal"
     INSERT = "insert"
     DELETE = "delete"
     REPLACE = "replace"
```

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/requests/execute.py` & `jupyter_ascending-0.1.9/jupyter_ascending/requests/execute.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/requests/get_status.py` & `jupyter_ascending-0.1.9/jupyter_ascending/requests/get_status.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/requests/sync.py` & `jupyter_ascending-0.1.9/jupyter_ascending/requests/sync.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/tests/test_cell_matching.py` & `jupyter_ascending-0.1.9/jupyter_ascending/tests/test_cell_matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import attr
 
 from jupyter_ascending.notebook.data_types import JupyterCell
 from jupyter_ascending.notebook.data_types import NotebookContents
 from jupyter_ascending.notebook.evolve import evolve_cell_source
+from jupyter_ascending.notebook.evolve import evolve_cell_type
 from jupyter_ascending.notebook.evolve import evolve_notebook_cells
 from jupyter_ascending.notebook.merge import OpCodes
 from jupyter_ascending.notebook.merge import opcode_merge_cell_contents
 
 SIMPLE_CONTENTS = NotebookContents(cells=[JupyterCell(cell_type="code", index=0, source=["x = 1; x"], output=["1"])])
 
 THREE_CELL_CONTENTS = NotebookContents(
@@ -158,7 +159,16 @@
         OpCodes.EQUAL,
         OpCodes.REPLACE,
         OpCodes.EQUAL,
     ]
 
     assert opcodes[1].current == (1, 2)
     assert opcodes[1].updated == (1, 3)
+
+
+def test_changing_cell_type_sends_replace():
+    new_contents = evolve_cell_type(SIMPLE_CONTENTS, 0, "markdown")
+    opcodes = opcode_merge_cell_contents(SIMPLE_CONTENTS, new_contents)
+
+    assert new_contents != SIMPLE_CONTENTS
+    assert len(opcodes) == 1
+    assert opcodes[0].op_code == OpCodes.REPLACE
```

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/tests/test_notebook_matching.py` & `jupyter_ascending-0.1.9/jupyter_ascending/tests/test_notebook_matching.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/utils.py` & `jupyter_ascending-0.1.9/jupyter_ascending/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/watchers/file_watcher.py` & `jupyter_ascending-0.1.9/jupyter_ascending/watchers/file_watcher.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/jupyter_ascending/widget.py` & `jupyter_ascending-0.1.9/jupyter_ascending/widget.py`

 * *Files identical despite different names*

### Comparing `jupyter_ascending-0.1.8/pyproject.toml` & `jupyter_ascending-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jupyter_ascending"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 jupytext = "^1.3.4"
 jsonrpcserver = {extras = ["requests"], version = "^4.1.2"}
```

### Comparing `jupyter_ascending-0.1.8/setup.py` & `jupyter_ascending-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'jsonrpcserver[requests]>=4.1.2,<5.0.0',
  'jupytext>=1.3.4,<2.0.0',
  'loguru>=0.4.1,<0.5.0',
  'toml>=0.10.0,<0.11.0']
 
 setup_kwargs = {
     'name': 'jupyter-ascending',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `jupyter_ascending-0.1.8/PKG-INFO` & `jupyter_ascending-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-ascending
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

