# Comparing `tmp/fastapi_debug_toolbar-0.3.2.tar.gz` & `tmp/fastapi_debug_toolbar-0.4.0.tar.gz`

## Comparing `fastapi_debug_toolbar-0.3.2.tar` & `fastapi_debug_toolbar-0.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/api.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/py.typed
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/responses.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/settings.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/toolbar.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/types.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/utils.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/__init__.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/headers.py
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/logging.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/profiling.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/pydantic.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/redirects.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/request.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/routes.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/settings.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/sql.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/sqlalchemy.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/timer.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/tortoise.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/versions.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/css/print.css
--rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/css/toolbar.css
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/img/icon-green.svg
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/img/icon-white.svg
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/redirect.js
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/refresh.js
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/timer.js
--rw-r--r--   0        0        0     8772 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/toolbar.js
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/utils.js
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/versions.js
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/base.html
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/redirect.html
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/includes/panel_button.html
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/includes/panel_content.html
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/headers.html
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/logging.html
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/profiling.html
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/pydantic.html
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/request.html
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/routes.html
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/settings.html
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/sql.html
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/timer.html
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/versions.html
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/.gitignore
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/LICENSE
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/README.md
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/api.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/py.typed
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/responses.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/settings.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/toolbar.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/types.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/utils.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/__init__.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/headers.py
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/logging.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/profiling.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/pydantic.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/redirects.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/request.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/routes.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/settings.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/sql.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/sqlalchemy.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/timer.py
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/tortoise.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/versions.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/css/print.css
+-rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/css/toolbar.css
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/img/icon-green.svg
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/img/icon-white.svg
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/redirect.js
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/refresh.js
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/timer.js
+-rw-r--r--   0        0        0     8772 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/toolbar.js
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/utils.js
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/versions.js
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/base.html
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/redirect.html
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/includes/panel_button.html
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/includes/panel_content.html
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/headers.html
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/logging.html
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/profiling.html
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/pydantic.html
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/request.html
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/routes.html
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/settings.html
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/sql.html
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/timer.html
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/versions.html
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/README.md
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.4.0/PKG-INFO
```

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/api.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/api.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/middleware.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,23 @@
         self.settings = DebugToolbarSettings(**settings)
         self.show_toolbar = import_string(self.settings.SHOW_TOOLBAR_CALLBACK)
         self.router: APIRouter = app  # type: ignore[assignment]
 
         while not isinstance(self.router, APIRouter):
             self.router = self.router.app
         try:
-            self.router.url_path_for(name="debug_toolbar.render_panel")
+            self.router.url_path_for("debug_toolbar.render_panel")
         except NoMatchFound:
             self.init_toolbar()
 
     def init_toolbar(self) -> None:
         self.router.get(
             self.settings.API_URL,
             name="debug_toolbar.render_panel",
+            include_in_schema=False,
         )(self.require_show_toolbar(render_panel))
 
         self.router.mount(
             self.settings.STATIC_URL,
             StaticFiles(packages=[__package__]),
             name="debug_toolbar.static",
         )
```

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/settings.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/toolbar.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/toolbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         self.store_id: t.Optional[str] = None
 
     @classmethod
     def get_panel_classes(
         cls: t.Type[DT],
         panels: t.Sequence[str],
     ) -> t.Sequence[t.Type[Panel]]:
-
         if cls._panel_classes is None:
             cls._panel_classes = [import_string(panel_path) for panel_path in panels]
         return cls._panel_classes
 
     @property
     def panels(self) -> t.Sequence[Panel]:
         return list(self._panels.values())
```

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/utils.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/__init__.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typing as t
 
 from fastapi import Request, Response
+from starlette.datastructures import URL
 from starlette.middleware.base import RequestResponseEndpoint
 
 from debug_toolbar.types import ServerTiming, Stats
 from debug_toolbar.utils import get_name_from_obj
 
 if t.TYPE_CHECKING:
     from debug_toolbar.toolbar import DebugToolbar
@@ -62,19 +63,19 @@
         if self.has_content:
             return self.render(**self.get_stats())
         return ""
 
     def render(self, **context: t.Any) -> str:
         return self.toolbar.render(self.template, **context)
 
-    def url_for(self, name: str, **path_params: t.Any) -> str:
+    def url_for(self, name: str, **path_params: t.Any) -> URL:
         return self.toolbar.request.url_for(name, **path_params)
 
     @property
-    def scripts(self) -> t.List[str]:
+    def scripts(self) -> t.List[URL]:
         return []
 
     async def process_request(self, request: Request) -> Response:
         return await self.call_next(request)
 
     async def generate_stats(self, request: Request, response: Response) -> Stats:
         return {}
```

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/headers.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/headers.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/logging.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/logging.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/profiling.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/profiling.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/pydantic.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/pydantic.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/redirects.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/redirects.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/request.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/request.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/sql.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/sql.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/sqlalchemy.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/sqlalchemy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,48 @@
 import typing as t
 from time import perf_counter
 
 from fastapi import Request, Response
 from fastapi.concurrency import AsyncExitStack
 from fastapi.dependencies.utils import solve_dependencies
 from sqlalchemy import event
-from sqlalchemy.engine import Connection, Engine
-from sqlalchemy.engine.default import DefaultExecutionContext
+from sqlalchemy.engine import Connection, Engine, ExecutionContext
 from sqlalchemy.orm import Session
 
 from debug_toolbar.panels.sql import SQLPanel
 
 
 class SQLAlchemyPanel(SQLPanel):
     title = "SQLAlchemy"
 
     def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         super().__init__(*args, **kwargs)
         self.engines: t.Set[Engine] = set()
 
     def register(self, engine: Engine) -> None:
-        event.listen(engine, "before_cursor_execute", self.before_execute)
-        event.listen(engine, "after_cursor_execute", self.after_execute)
+        event.listen(engine, "before_cursor_execute", self.before_execute, named=True)
+        event.listen(engine, "after_cursor_execute", self.after_execute, named=True)
 
     def unregister(self, engine: Engine) -> None:
         event.remove(engine, "before_cursor_execute", self.before_execute)
         event.remove(engine, "after_cursor_execute", self.after_execute)
 
-    def before_execute(
-        self,
-        conn: Connection,
-        cursor: t.Any,
-        statement: str,
-        parameters: t.Union[t.Sequence, t.Dict],
-        context: DefaultExecutionContext,
-        executemany: bool,
-    ) -> None:
-        conn.info.setdefault("start_time", []).append(perf_counter())
-
-    def after_execute(
-        self,
-        conn: Connection,
-        cursor: t.Any,
-        statement: str,
-        parameters: t.Union[t.Sequence, t.Dict],
-        context: DefaultExecutionContext,
-        executemany: bool,
-    ) -> None:
+    def before_execute(self, context: ExecutionContext, **kwargs: t.Any) -> None:
+        context._start_time = perf_counter()  # type: ignore[attr-defined]
+
+    def after_execute(self, context: ExecutionContext, **kwargs: t.Any) -> None:
         query = {
-            "duration": (perf_counter() - conn.info["start_time"].pop(-1)) * 1000,
-            "sql": statement,
-            "params": parameters,
-            "is_select": context.invoked_statement.is_select,
+            "duration": (
+                perf_counter() - context._start_time  # type: ignore[attr-defined]
+            )
+            * 1000,
+            "sql": context.statement,
+            "params": context.parameters,
         }
-        self.add_query(str(conn.engine.url), query)
+        self.add_query(str(context.engine.url), query)
 
     async def add_engines(self, request: Request):
         route = request["route"]
 
         if hasattr(route, "dependant"):
             if "fastapi_astack" not in request:
                 async with AsyncExitStack() as stack:
@@ -66,15 +51,20 @@
             solved_result = await solve_dependencies(
                 request=request,
                 dependant=route.dependant,
                 dependency_overrides_provider=route.dependency_overrides_provider,
             )
             for value in solved_result[0].values():
                 if isinstance(value, Session):
-                    self.engines.add(value.get_bind())
+                    bind = value.get_bind()
+
+                    if isinstance(bind, Connection):
+                        self.engines.add(bind.engine)
+                    else:
+                        self.engines.add(bind)
 
     async def process_request(self, request: Request) -> Response:
         await self.add_engines(request)
 
         for engine in self.engines:
             self.register(engine)
         try:
```

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/timer.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/timer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing as t
 from time import perf_counter
 
 from fastapi import Request, Response
+from starlette.datastructures import URL
 
 from debug_toolbar.panels import Panel
 from debug_toolbar.types import ServerTiming, Stats
 
 try:
     import resource
 except ImportError:
@@ -41,15 +42,15 @@
                 "Context switches",
                 f"{stats['vcsw']} voluntary, {stats['ivcsw']} involuntary",
             ),
         )
         return self.render(rows=rows)
 
     @property
-    def scripts(self) -> t.List[str]:
+    def scripts(self) -> t.List[URL]:
         scripts = super().scripts
         scripts.append(self.url_for("debug_toolbar.static", path="js/timer.js"))
         return scripts
 
     async def process_request(self, request: Request) -> Response:
         self._start_time = perf_counter()
         if self.has_content:
```

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/tortoise.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/tortoise.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/panels/versions.py` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/panels/versions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import typing as t
 
 from fastapi import Request, Response, __version__
+from starlette.datastructures import URL
 
 from debug_toolbar.panels import Panel
 from debug_toolbar.types import Stats
 
 
 class VersionsPanel(Panel):
     title = "Versions"
     template = "panels/versions.html"
 
     @property
     def nav_subtitle(self) -> str:
         return f"FastAPI {__version__}"
 
     @property
-    def scripts(self) -> t.List[str]:
+    def scripts(self) -> t.List[URL]:
         scripts = super().scripts
         scripts.append(self.url_for("debug_toolbar.static", path="js/versions.js"))
         return scripts
 
     async def generate_stats(self, request: Request, response: Response) -> Stats:
         try:
             import pkg_resources
```

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/css/toolbar.css` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/css/toolbar.css`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/img/icon-green.svg` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/img/icon-green.svg`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/img/icon-white.svg` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/img/icon-white.svg`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/refresh.js` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/refresh.js`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/timer.js` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/timer.js`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/toolbar.js` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/toolbar.js`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/utils.js` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/utils.js`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/statics/js/versions.js` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/statics/js/versions.js`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/base.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/base.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/redirect.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/redirect.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/includes/panel_button.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/includes/panel_button.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/headers.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/headers.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/logging.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/logging.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/pydantic.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/pydantic.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/request.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/request.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/routes.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/routes.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/settings.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/settings.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/sql.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/sql.html`

 * *Files 8% similar despite different names*

```diff
@@ -59,25 +59,14 @@
             <svg class="fastDebugLineChart{% if query.is_slow %} fastDebugLineChartWarning{% endif %}" xmlns="http://www.w3.org/2000/svg" viewbox="0 0 100 5" preserveAspectRatio="none" aria-label="{{ query.width_ratio }}%">
               <rect x="{{ query.start_offset }}" y="0" height="5" width="{{ query.width_ratio }}" fill="{{ query.trace_color }}" />
             </svg>
           </td>
           <td class="fastdt-time">
             {{ '%0.2f'|format(query.duration|float) }}
           </td>
-          {# TODO: SELECT actions
-          <td class="fastdt-actions">
-            {% if query.params and query.is_select %}
-              <form method="post">
-                {{ query.form }}
-                <button formaction="{% url_for('debug_toolbar.sqlalchemy_select') %}" class="remoteCall">Sel</button>
-                <button formaction="{% url_for('debug_toolbar.sqlalchemy_explain') %}" class="remoteCall">Expl</button>
-              </form>
-              {% endif %}
-          </td>
-          #}
         </tr>
         <tr class="fastUnselected {% if query.is_slow %} fastDebugRowWarning{% endif %} fastToggleDetails_{{ loop.index }}" id="sqlDetails_{{ loop.index }}">
           <td colspan="2"></td>
           <td colspan="4">
             <div class="fastSQLDetailsDiv">
               {% if query.params %}<p><strong>Params:</strong> <code>{{ query.params }}</code></p>{% endif %}
               <p><strong>Connection:</strong> {{ alias }}</p>
```

#### html2text {}

```diff
@@ -2,29 +2,23 @@
     * {% for alias, info in databases.items() %}
     * {{ alias }} {{ '%0.2f'|format(info.time_spent|float) }} ms ({% if
       info.num_queries == 1 %}{{ info.num_queries }} query{% else %}{
       { info.num_queries }} queries{% endif %} {% if info.sim_count %}
       including {{ info.sim_count }} similar {%- if info.dup_count %} and {
       { info.dup_count }} duplicates {%- endif %} {%- endif %})
     * {% endfor %}
- Query                      Timeline Time (ms)              Action
-   {
-   {
-   query.sql_formatted|safe
-   }} {
-   { query.sql_simple|safe                                  {% if query.params
-   }}                                {{ '%0.2f'|format      and query.is_select
- + {% if query.sim_count %}          (query.duration|float) %}
-   {{ query.sim_count }}             }}                     {{ query.form }}
-   similar queries. {%                                      Sel Expl
-   endif %} {% if                                           {% endif %}
-   query.dup_count %}
-   Duplicated {
-   { query.dup_count }}
-   times. {% endif %}
+ Query                              Timeline Time (ms)                 Action
+   {{ query.sql_formatted|safe }} {
+   { query.sql_simple|safe }}
+   {% if query.sim_count %}  {
+ + { query.sim_count }} similar              {{ '%0.2f'|format
+   queries. {% endif %} {% if                (query.duration|float) }}
+   query.dup_count %}  Duplicated {
+   { query.dup_count }} times. {%
+   endif %}
    {% if query.params %}
    Params: {{ query.params }}
    {% endif %}
    Connection: {{ alias }}
 {% else %}
 No SQL queries were recorded during this request.
 {% endif %}
```

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/timer.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/timer.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/debug_toolbar/templates/panels/versions.html` & `fastapi_debug_toolbar-0.4.0/debug_toolbar/templates/panels/versions.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/LICENSE` & `fastapi_debug_toolbar-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/README.md` & `fastapi_debug_toolbar-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/pyproject.toml` & `fastapi_debug_toolbar-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.3.2/PKG-INFO` & `fastapi_debug_toolbar-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: fastapi-debug-toolbar
-Version: 0.3.2
+Version: 0.4.0
 Summary: A debug toolbar for FastAPI.
 Project-URL: homepage, https://github.com/mongkok/fastapi-debug-toolbar
 Project-URL: repository, https://github.com/mongkok/fastapi-debug-toolbar
 Project-URL: documentation, https://fastapi-debug-toolbar.domake.io
 Project-URL: changelog, https://fastapi-debug-toolbar.domake.io/changelog/
 Author-email: Dani <dani@domake.io>
+License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: debug,fastapi,profiling
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AnyIO
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1 Name: fastapi-debug-toolbar Version: 0.3.2 Summary: A
+Metadata-Version: 2.1 Name: fastapi-debug-toolbar Version: 0.4.0 Summary: A
 debug toolbar for FastAPI. Project-URL: homepage, https://github.com/mongkok/
 fastapi-debug-toolbar Project-URL: repository, https://github.com/mongkok/
 fastapi-debug-toolbar Project-URL: documentation, https://fastapi-debug-
 toolbar.domake.io Project-URL: changelog, https://fastapi-debug-
 toolbar.domake.io/changelog/ Author-email: Dani
-domake.io> License-File: LICENSE Keywords: debug,fastapi,profiling Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Environment :: Web Environment
-Classifier: Framework :: AnyIO Classifier: Framework :: FastAPI Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: System
-Administrators Classifier: License :: OSI Approved :: BSD License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic ::
-Software Development Classifier: Topic :: Software Development :: Debuggers
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Utilities Classifier: Typing :: Typed Requires-Python: >=3.7 Requires-Dist:
-anyio>=3.0.0 Requires-Dist: fastapi>=0.70.0 Requires-Dist: jinja2>=2.9
-Requires-Dist: pyinstrument>=3.0.0 Requires-Dist: sqlparse>=0.2.0 Provides-
-Extra: doc Requires-Dist: markdown-include; extra == 'doc' Requires-Dist:
-mkdocs; extra == 'doc' Requires-Dist: mkdocs-material; extra == 'doc' Requires-
-Dist: mkdocstrings[python]; extra == 'doc' Provides-Extra: test Requires-Dist:
-black; extra == 'test' Requires-Dist: codecov; extra == 'test' Requires-Dist:
-flake8; extra == 'test' Requires-Dist: httpx; extra == 'test' Requires-Dist:
-isort; extra == 'test' Requires-Dist: itsdangerous; extra == 'test' Requires-
-Dist: mypy; extra == 'test' Requires-Dist: pytest; extra == 'test' Requires-
-Dist: pytest-asyncio; extra == 'test' Requires-Dist: pytest-cov; extra ==
-'test' Requires-Dist: python-multipart; extra == 'test' Requires-Dist:
-sqlalchemy; extra == 'test' Requires-Dist: tortoise-orm>=0.19.0; extra ==
-'test' Requires-Dist: types-setuptools; extra == 'test' Description-Content-
-Type: text/markdown # ![FastAPI](https://raw.githubusercontent.com/mongkok/
-fastapi-debug-toolbar/main/debug_toolbar/statics/img/icon-green.svg) Debug
-Toolbar
+domake.io> License-Expression: BSD-3-Clause License-File: LICENSE Keywords:
+debug,fastapi,profiling Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: Web Environment Classifier: Framework :: AnyIO
+Classifier: Framework :: FastAPI Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators Classifier: License ::
+OSI Approved :: BSD License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
+HTTP :: HTTP Servers Classifier: Topic :: Software Development Classifier:
+Topic :: Software Development :: Debuggers Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Topic :: Utilities Classifier: Typing :: Typed
+Requires-Python: >=3.7 Requires-Dist: anyio>=3.0.0 Requires-Dist:
+fastapi>=0.70.0 Requires-Dist: jinja2>=2.9 Requires-Dist: pyinstrument>=3.0.0
+Requires-Dist: sqlparse>=0.2.0 Provides-Extra: doc Requires-Dist: markdown-
+include; extra == 'doc' Requires-Dist: mkdocs; extra == 'doc' Requires-Dist:
+mkdocs-material; extra == 'doc' Requires-Dist: mkdocstrings[python]; extra ==
+'doc' Provides-Extra: test Requires-Dist: black; extra == 'test' Requires-Dist:
+codecov; extra == 'test' Requires-Dist: flake8; extra == 'test' Requires-Dist:
+httpx; extra == 'test' Requires-Dist: isort; extra == 'test' Requires-Dist:
+itsdangerous; extra == 'test' Requires-Dist: mypy; extra == 'test' Requires-
+Dist: pytest; extra == 'test' Requires-Dist: pytest-asyncio; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test' Requires-Dist: python-multipart;
+extra == 'test' Requires-Dist: sqlalchemy; extra == 'test' Requires-Dist:
+tortoise-orm>=0.19.0; extra == 'test' Requires-Dist: types-setuptools; extra ==
+'test' Description-Content-Type: text/markdown # ![FastAPI](https://
+raw.githubusercontent.com/mongkok/fastapi-debug-toolbar/main/debug_toolbar/
+statics/img/icon-green.svg) Debug Toolbar
                             [FastAPI_Debug_Toolbar]
 ðA debug toolbar for FastAPI based on the original django-debug-toolbar.ð
 
                       Swagger UI & GraphQL are supported.
                  [Test] [Coverage] [Codacy] [Package_version]
 --- **Documentation**: [https://fastapi-debug-toolbar.domake.io](https://
 fastapi-debug-toolbar.domake.io) --- ## Installation ```sh pip install fastapi-
```

