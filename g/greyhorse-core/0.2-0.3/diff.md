# Comparing `tmp/greyhorse_core-0.2.tar.gz` & `tmp/greyhorse_core-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse_core-0.2.tar", max compression
+gzip compressed data, was "greyhorse_core-0.3.tar", max compression
```

## Comparing `greyhorse_core-0.2.tar` & `greyhorse_core-0.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0        0 2023-04-24 18:05:03.042538 greyhorse_core-0.2/greyhorse_core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 18:45:18.959739 greyhorse_core-0.2/greyhorse_core/app/__init__.py
--rw-r--r--   0        0        0     6377 2023-04-24 20:21:29.479688 greyhorse_core-0.2/greyhorse_core/app/application.py
--rw-r--r--   0        0        0     2576 2023-04-26 18:21:39.345299 greyhorse_core-0.2/greyhorse_core/app/base.py
--rw-r--r--   0        0        0     7745 2023-04-24 20:21:29.311692 greyhorse_core-0.2/greyhorse_core/app/module.py
--rw-r--r--   0        0        0     4195 2023-04-24 20:21:28.631707 greyhorse_core-0.2/greyhorse_core/app/service.py
--rw-r--r--   0        0        0       57 2023-04-24 20:21:28.679706 greyhorse_core-0.2/greyhorse_core/context/__init__.py
--rw-r--r--   0        0        0     1683 2023-04-24 20:39:33.731147 greyhorse_core-0.2/greyhorse_core/context/data.py
--rw-r--r--   0        0        0        0 2023-04-24 19:30:35.532333 greyhorse_core-0.2/greyhorse_core/data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 19:32:47.064406 greyhorse_core-0.2/greyhorse_core/data/cache/__init__.py
--rw-r--r--   0        0        0     1909 2023-04-24 20:21:29.083697 greyhorse_core-0.2/greyhorse_core/data/cache/base.py
--rw-r--r--   0        0        0     2467 2023-04-24 20:21:28.907701 greyhorse_core-0.2/greyhorse_core/data/cache/method.py
--rw-r--r--   0        0        0        0 2023-04-26 18:11:49.403523 greyhorse_core-0.2/greyhorse_core/data/models/__init__.py
--rw-r--r--   0        0        0     1878 2023-05-06 20:27:15.000505 greyhorse_core-0.2/greyhorse_core/data/models/base.py
--rw-r--r--   0        0        0     3621 2023-04-26 18:45:50.368589 greyhorse_core-0.2/greyhorse_core/data/models/fields.py
--rw-r--r--   0        0        0     2088 2023-06-05 00:54:27.830750 greyhorse_core-0.2/greyhorse_core/data/models/filterable.py
--rw-r--r--   0        0        0     4491 2023-06-07 18:56:58.759508 greyhorse_core-0.2/greyhorse_core/data/models/model.py
--rw-r--r--   0        0        0     1620 2023-04-26 18:40:56.383656 greyhorse_core-0.2/greyhorse_core/data/models/serializable.py
--rw-r--r--   0        0        0        0 2023-04-24 19:45:59.112951 greyhorse_core-0.2/greyhorse_core/data/repositories/__init__.py
--rw-r--r--   0        0        0     2752 2023-06-07 18:56:58.847505 greyhorse_core-0.2/greyhorse_core/data/repositories/base.py
--rw-r--r--   0        0        0     2387 2023-06-07 18:56:58.927503 greyhorse_core-0.2/greyhorse_core/data/repositories/filterable.py
--rw-r--r--   0        0        0      117 2023-04-24 20:21:28.447712 greyhorse_core-0.2/greyhorse_core/data/serializers/__init__.py
--rw-r--r--   0        0        0      580 2023-04-24 20:21:28.335714 greyhorse_core-0.2/greyhorse_core/data/serializers/base.py
--rw-r--r--   0        0        0      523 2023-04-26 18:21:39.277304 greyhorse_core-0.2/greyhorse_core/data/serializers/pickle.py
--rw-r--r--   0        0        0        0 2023-04-25 12:15:10.040554 greyhorse_core-0.2/greyhorse_core/engines/__init__.py
--rw-r--r--   0        0        0     1451 2023-04-26 17:59:27.740179 greyhorse_core-0.2/greyhorse_core/engines/base.py
--rw-r--r--   0        0        0     1102 2023-04-25 12:36:12.576326 greyhorse_core-0.2/greyhorse_core/engines/factory.py
--rw-r--r--   0        0        0       67 2023-04-24 20:21:28.403712 greyhorse_core-0.2/greyhorse_core/i18n/__init__.py
--rw-r--r--   0        0        0     2798 2023-05-06 23:36:14.668431 greyhorse_core-0.2/greyhorse_core/i18n/translator.py
--rw-r--r--   0        0        0     1584 2023-04-24 20:21:28.723705 greyhorse_core-0.2/greyhorse_core/logging.py
--rw-r--r--   0        0        0     2340 2023-04-26 19:36:39.848852 greyhorse_core-0.2/greyhorse_core/result.py
--rw-r--r--   0        0        0        0 2023-04-24 18:46:51.552811 greyhorse_core-0.2/greyhorse_core/utils/__init__.py
--rw-r--r--   0        0        0      397 2023-04-24 20:21:29.039698 greyhorse_core-0.2/greyhorse_core/utils/confs.py
--rw-r--r--   0        0        0     2154 2023-04-24 20:21:29.255693 greyhorse_core-0.2/greyhorse_core/utils/dicts.py
--rw-r--r--   0        0        0      573 2023-04-24 20:21:28.247716 greyhorse_core-0.2/greyhorse_core/utils/hashes.py
--rw-r--r--   0        0        0      922 2023-04-26 18:21:39.397295 greyhorse_core-0.2/greyhorse_core/utils/imports.py
--rw-r--r--   0        0        0      865 2023-04-24 20:21:28.567709 greyhorse_core-0.2/greyhorse_core/utils/invoke.py
--rw-r--r--   0        0        0      452 2023-04-24 20:27:59.930714 greyhorse_core-0.2/greyhorse_core/utils/json.py
--rw-r--r--   0        0        0      823 2023-05-07 00:18:41.443382 greyhorse_core-0.2/greyhorse_core/utils/strings.py
--rw-r--r--   0        0        0     1101 2023-04-24 20:34:00.643458 greyhorse_core-0.2/greyhorse_core/utils/time.py
--rw-r--r--   0        0        0     1060 2023-06-07 18:55:02.811162 greyhorse_core-0.2/pyproject.toml
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 greyhorse_core-0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 18:05:03.042538 greyhorse_core-0.3/greyhorse_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 18:45:18.959739 greyhorse_core-0.3/greyhorse_core/app/__init__.py
+-rw-r--r--   0        0        0     6952 2023-06-26 23:41:57.914036 greyhorse_core-0.3/greyhorse_core/app/application.py
+-rw-r--r--   0        0        0     3735 2023-06-26 23:41:57.914036 greyhorse_core-0.3/greyhorse_core/app/base.py
+-rw-r--r--   0        0        0     1568 2023-06-26 23:41:57.914036 greyhorse_core-0.3/greyhorse_core/app/context.py
+-rw-r--r--   0        0        0     2283 2023-06-26 23:41:57.914036 greyhorse_core-0.3/greyhorse_core/app/module.py
+-rw-r--r--   0        0        0      538 2023-06-26 23:41:57.914036 greyhorse_core-0.3/greyhorse_core/app/service.py
+-rw-r--r--   0        0        0     7684 2023-06-26 23:41:57.914036 greyhorse_core-0.3/greyhorse_core/app/visitors.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:30:35.532333 greyhorse_core-0.3/greyhorse_core/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:32:47.064406 greyhorse_core-0.3/greyhorse_core/data/cache/__init__.py
+-rw-r--r--   0        0        0     1909 2023-04-24 20:21:29.083697 greyhorse_core-0.3/greyhorse_core/data/cache/base.py
+-rw-r--r--   0        0        0     2467 2023-04-24 20:21:28.907701 greyhorse_core-0.3/greyhorse_core/data/cache/method.py
+-rw-r--r--   0        0        0        0 2023-04-26 18:11:49.403523 greyhorse_core-0.3/greyhorse_core/data/models/__init__.py
+-rw-r--r--   0        0        0     1878 2023-05-06 20:27:15.000505 greyhorse_core-0.3/greyhorse_core/data/models/base.py
+-rw-r--r--   0        0        0     3621 2023-04-26 18:45:50.368589 greyhorse_core-0.3/greyhorse_core/data/models/fields.py
+-rw-r--r--   0        0        0     2088 2023-06-05 00:54:27.830750 greyhorse_core-0.3/greyhorse_core/data/models/filterable.py
+-rw-r--r--   0        0        0     4491 2023-06-07 18:56:58.759508 greyhorse_core-0.3/greyhorse_core/data/models/model.py
+-rw-r--r--   0        0        0     1620 2023-04-26 18:40:56.383656 greyhorse_core-0.3/greyhorse_core/data/models/serializable.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:45:59.112951 greyhorse_core-0.3/greyhorse_core/data/repositories/__init__.py
+-rw-r--r--   0        0        0     2752 2023-06-07 18:56:58.847505 greyhorse_core-0.3/greyhorse_core/data/repositories/base.py
+-rw-r--r--   0        0        0     2387 2023-06-07 18:56:58.927503 greyhorse_core-0.3/greyhorse_core/data/repositories/filterable.py
+-rw-r--r--   0        0        0      117 2023-04-24 20:21:28.447712 greyhorse_core-0.3/greyhorse_core/data/serializers/__init__.py
+-rw-r--r--   0        0        0      580 2023-04-24 20:21:28.335714 greyhorse_core-0.3/greyhorse_core/data/serializers/base.py
+-rw-r--r--   0        0        0      523 2023-04-26 18:21:39.277304 greyhorse_core-0.3/greyhorse_core/data/serializers/pickle.py
+-rw-r--r--   0        0        0        0 2023-04-25 12:15:10.040554 greyhorse_core-0.3/greyhorse_core/engines/__init__.py
+-rw-r--r--   0        0        0     1451 2023-04-26 17:59:27.740179 greyhorse_core-0.3/greyhorse_core/engines/base.py
+-rw-r--r--   0        0        0     1102 2023-04-25 12:36:12.576326 greyhorse_core-0.3/greyhorse_core/engines/factory.py
+-rw-r--r--   0        0        0       67 2023-04-24 20:21:28.403712 greyhorse_core-0.3/greyhorse_core/i18n/__init__.py
+-rw-r--r--   0        0        0     2774 2023-06-26 23:41:57.914036 greyhorse_core-0.3/greyhorse_core/i18n/translator.py
+-rw-r--r--   0        0        0     1584 2023-04-24 20:21:28.723705 greyhorse_core-0.3/greyhorse_core/logging.py
+-rw-r--r--   0        0        0     2575 2023-06-26 23:41:57.914036 greyhorse_core-0.3/greyhorse_core/messagebus.py
+-rw-r--r--   0        0        0     2340 2023-04-26 19:36:39.848852 greyhorse_core-0.3/greyhorse_core/result.py
+-rw-r--r--   0        0        0        0 2023-04-24 18:46:51.552811 greyhorse_core-0.3/greyhorse_core/utils/__init__.py
+-rw-r--r--   0        0        0      397 2023-04-24 20:21:29.039698 greyhorse_core-0.3/greyhorse_core/utils/confs.py
+-rw-r--r--   0        0        0     2154 2023-04-24 20:21:29.255693 greyhorse_core-0.3/greyhorse_core/utils/dicts.py
+-rw-r--r--   0        0        0      573 2023-04-24 20:21:28.247716 greyhorse_core-0.3/greyhorse_core/utils/hashes.py
+-rw-r--r--   0        0        0      922 2023-04-26 18:21:39.397295 greyhorse_core-0.3/greyhorse_core/utils/imports.py
+-rw-r--r--   0        0        0     1096 2023-06-26 23:41:57.914036 greyhorse_core-0.3/greyhorse_core/utils/invoke.py
+-rw-r--r--   0        0        0      452 2023-04-24 20:27:59.930714 greyhorse_core-0.3/greyhorse_core/utils/json.py
+-rw-r--r--   0        0        0      823 2023-05-07 00:18:41.443382 greyhorse_core-0.3/greyhorse_core/utils/strings.py
+-rw-r--r--   0        0        0     1101 2023-04-24 20:34:00.643458 greyhorse_core-0.3/greyhorse_core/utils/time.py
+-rw-r--r--   0        0        0     1099 2023-06-26 23:41:57.934035 greyhorse_core-0.3/pyproject.toml
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 greyhorse_core-0.3/PKG-INFO
```

### Comparing `greyhorse_core-0.2/greyhorse_core/app/base.py` & `greyhorse_core-0.3/greyhorse_core/app/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,140 @@
 from abc import ABC, abstractmethod
+from contextlib import AbstractContextManager, AbstractAsyncContextManager
 from pathlib import Path
-from typing import Callable, List, Optional, Protocol, runtime_checkable, Self
+from typing import Callable, Optional, Self
 
 from dependency_injector.containers import Container
 
 
-@runtime_checkable
-class BaseResource(Protocol):
-    pass
+class Resource(ABC):
+    def __init__(self):
+        self._active: bool = False
 
-
-class Resource(BaseResource):
-    def __init__(self, *args, **kwargs):
-        self._initialized: bool = False
+    def accept(self, visitor: 'Visitor'):
+        return visitor.visit_resource(self)
 
     @property
-    def initialized(self) -> bool:
-        return self._initialized
-
-    def sync_startup(self, application, module, service, *args, **kwargs):
-        pass
-
-    def sync_shutdown(self, application, module, service, *args, **kwargs):
-        pass
-
-    async def startup(self, application, module, service, *args, **kwargs):
-        pass
-
-    async def shutdown(self, application, module, service, *args, **kwargs):
-        pass
+    def active(self) -> bool:
+        return self._active
 
-
-class SessionResource(Resource):
-    def sync_session_begin(self, application, module, service, *args, **kwargs):
+    @abstractmethod
+    def create(
+        self, application: 'Application',
+        module: Optional['Module'] = None,
+        service: Optional['Service'] = None,
+    ):
         pass
 
-    def sync_session_finish(self, application, module, service, *args, **kwargs):
+    @abstractmethod
+    def destroy(
+        self, application: 'Application',
+        module: Optional['Module'] = None,
+        service: Optional['Service'] = None,
+    ):
         pass
 
-    async def session_begin(self, application, module, service, *args, **kwargs):
+    @abstractmethod
+    def acquire(
+        self, application: 'Application',
+        module: Optional['Module'] = None,
+        service: Optional['Service'] = None,
+    ):
         pass
 
-    async def session_finish(self, application, module, service, *args, **kwargs):
+    @abstractmethod
+    def release(
+        self, application: 'Application',
+        module: Optional['Module'] = None,
+        service: Optional['Service'] = None,
+    ):
         pass
 
 
 ResourceFactory = Callable[[], Resource]
 
 
-class ContainerResource(Resource):
-    def __init__(self, container: Container, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+class HasContainer:
+    def __init__(self, container: Container):
         self._container = container
 
     @property
     def container(self) -> Container:
         return self._container
 
 
-class Service(Resource, ABC):
-    name: str
+class Service(ABC):
     resources: list[Resource]
 
+    def __init__(self):
+        self._active: bool = False
+
+    def accept(self, visitor: 'Visitor'):
+        return visitor.visit_service(self)
+
+    @property
+    def active(self) -> bool:
+        return self._active
+
     @abstractmethod
     def get_resource(self, name) -> Resource | None:
         ...
 
+    @abstractmethod
+    def start(self, application: 'Application', module: Optional['Module'] = None):
+        ...
+
+    @abstractmethod
+    def stop(self, application: 'Application', module: Optional['Module'] = None):
+        ...
+
 
 ServiceFactory = Callable[[], Service]
 
 
-class Module(Resource, ABC):
+class Module(ABC):
     resources: list[Resource]
     services: list[Service]
     modules: list['Module']
 
+    def __init__(self, name: str):
+        self._name = name
+
+    def accept(self, visitor: 'Visitor'):
+        return visitor.visit_module(self)
+
+    @property
+    def name(self) -> str:
+        return self._name
+
     @abstractmethod
     def get_resource(self, name) -> Resource | None:
         ...
 
     @abstractmethod
     def get_service(self, name) -> Service | None:
         ...
 
     @abstractmethod
     def get_module(self, name) -> Self | None:
         ...
 
+    @abstractmethod
+    def initialize(self, application: 'Application', module: Optional['Module'] = None):
+        ...
+
+    @abstractmethod
+    def finalize(self, application: 'Application', module: Optional['Module'] = None):
+        ...
+
 
 ModuleFactory = Callable[[], Module]
 
 
 class Application(Module, ABC):
-    name: str
-
     @property
     @abstractmethod
     def version(self) -> str:
         ...
 
     @property
     @abstractmethod
@@ -105,13 +142,32 @@
         ...
 
     @abstractmethod
     def get_cwd(self) -> Path:
         ...
 
     @abstractmethod
-    def sync_load_packages(self, *args, **kwargs):
+    def initialize(self, *args, **kwargs):
+        ...
+
+    @abstractmethod
+    def finalize(self, *args, **kwargs):
+        ...
+
+    @abstractmethod
+    def session(self) -> AbstractContextManager | AbstractAsyncContextManager:
         ...
 
     @abstractmethod
-    async def load_packages(self, *args, **kwargs):
+    def load_packages(self, *args, **kwargs):
         ...
+
+
+class Visitor:
+    def visit_resource(self, instance: Resource):
+        pass
+
+    def visit_service(self, instance: Service):
+        pass
+
+    def visit_module(self, instance: Module):
+        pass
```

### Comparing `greyhorse_core-0.2/greyhorse_core/context/data.py` & `greyhorse_core-0.3/greyhorse_core/app/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 
     def __setattr__(self, key, value):
         super().__setattr__(key, self._wrap(value))
 
     def __contains__(self, item):
         return item in self.__dict__
 
-    # @property
-    # def data(self):
-    #     # noinspection PyUnresolvedReferences
-    #     return self._data
-
     @property
     def raw_id(self):
         return self._id
 
     @property
     def session_id(self):
         if self._id:
```

### Comparing `greyhorse_core-0.2/greyhorse_core/data/cache/base.py` & `greyhorse_core-0.3/greyhorse_core/data/cache/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/data/cache/method.py` & `greyhorse_core-0.3/greyhorse_core/data/cache/method.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/data/models/base.py` & `greyhorse_core-0.3/greyhorse_core/data/models/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/data/models/fields.py` & `greyhorse_core-0.3/greyhorse_core/data/models/fields.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/data/models/filterable.py` & `greyhorse_core-0.3/greyhorse_core/data/models/filterable.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/data/models/model.py` & `greyhorse_core-0.3/greyhorse_core/data/models/model.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/data/models/serializable.py` & `greyhorse_core-0.3/greyhorse_core/data/models/serializable.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/data/repositories/base.py` & `greyhorse_core-0.3/greyhorse_core/data/repositories/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/data/repositories/filterable.py` & `greyhorse_core-0.3/greyhorse_core/data/repositories/filterable.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/data/serializers/base.py` & `greyhorse_core-0.3/greyhorse_core/data/serializers/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/data/serializers/pickle.py` & `greyhorse_core-0.3/greyhorse_core/data/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/engines/base.py` & `greyhorse_core-0.3/greyhorse_core/engines/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/engines/factory.py` & `greyhorse_core-0.3/greyhorse_core/engines/factory.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/i18n/translator.py` & `greyhorse_core-0.3/greyhorse_core/i18n/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from importlib.resources import Package, read_text as pkg_read_text, files, as_file
+from importlib.resources import Package, files, as_file
 from pathlib import Path
 
 import tomlkit
 
-from greyhorse_core.context import get_context
+from greyhorse_core.app.context import get_context
 from greyhorse_core.utils.dicts import build_dotted_keys_from_dict
 
 
 class StaticTranslator:
     def __init__(self):
         self._data = dict()
         self._defaults = dict()
```

### Comparing `greyhorse_core-0.2/greyhorse_core/logging.py` & `greyhorse_core-0.3/greyhorse_core/logging.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/result.py` & `greyhorse_core-0.3/greyhorse_core/result.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/utils/dicts.py` & `greyhorse_core-0.3/greyhorse_core/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/utils/hashes.py` & `greyhorse_core-0.3/greyhorse_core/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/utils/imports.py` & `greyhorse_core-0.3/greyhorse_core/utils/imports.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/utils/invoke.py` & `greyhorse_core-0.3/greyhorse_core/utils/invoke.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from asyncio import get_running_loop, iscoroutinefunction, run as run_main
+from asyncio import get_running_loop, iscoroutinefunction, run as run_main, iscoroutine, Future
 from functools import partial
 
 
 def is_awaitable(f):
     while isinstance(f, partial):
         f = f.func
     return iscoroutinefunction(f) or inspect.isawaitable(f)
@@ -16,18 +16,26 @@
         loop = None
 
     if is_awaitable(func):
         if loop:
             return loop.create_task(func(*args, **kwargs))
         else:
             return run_main(func(*args, **kwargs))
-    else:
+    elif callable(func):
         return func(*args, **kwargs)
+    else:
+        return func
 
 
 async def invoke_async(func, *args, **kwargs):
     if is_awaitable(func):
+        if iscoroutine(func):
+            return await func
         return await func(*args, **kwargs)
-    else:
+    elif callable(func):
         loop = get_running_loop()
         func = partial(func, *args, **kwargs)
         return await loop.run_in_executor(None, func)
+    else:
+        future = Future()
+        future.set_result(func)
+        return future
```

### Comparing `greyhorse_core-0.2/greyhorse_core/utils/strings.py` & `greyhorse_core-0.3/greyhorse_core/utils/strings.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/greyhorse_core/utils/time.py` & `greyhorse_core-0.3/greyhorse_core/utils/time.py`

 * *Files identical despite different names*

### Comparing `greyhorse_core-0.2/pyproject.toml` & `greyhorse_core-0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "greyhorse-core"
-version = "0.2"
+version = "0.3"
 description = "Greyhorse Core library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -14,14 +14,16 @@
 
 packages = [
     { include = "greyhorse_core" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
+asyncclick = "^8.1.3"
+click = "^8.1.3"
 dependency-injector = {version = "^4.41", extras = ["pydantic"]}
 pydantic = {version = "^1.10", extras = ["dotenv", "email"]}
 pytz = "^2022.7"
 timeparse-plus = "^1.2"
 tomlkit = "^0.11"
 orjson = "^3.8"
```

### Comparing `greyhorse_core-0.2/PKG-INFO` & `greyhorse_core-0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: greyhorse-core
-Version: 0.2
+Version: 0.3
 Summary: Greyhorse Core library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: asyncclick (>=8.1.3,<9.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dependency-injector[pydantic] (>=4.41,<5.0)
 Requires-Dist: orjson (>=3.8,<4.0)
 Requires-Dist: pydantic[dotenv,email] (>=1.10,<2.0)
 Requires-Dist: pytz (>=2022.7,<2023.0)
 Requires-Dist: timeparse-plus (>=1.2,<2.0)
 Requires-Dist: tomlkit (>=0.11,<0.12)
 Project-URL: Repository, https://gitlab.com/max-plutonium/greyhorse
```

