# Comparing `tmp/async_wrapper-0.1.2.tar.gz` & `tmp/async_wrapper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.1.2.tar", max compression
+gzip compressed data, was "async_wrapper-0.1.3.tar", max compression
```

## Comparing `async_wrapper-0.1.2.tar` & `async_wrapper-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-06-26 12:05:22.641344 async_wrapper-0.1.2/LICENSE
--rw-r--r--   0        0        0     1534 2023-06-26 12:05:22.641344 async_wrapper-0.1.2/README.md
--rw-r--r--   0        0        0     3648 2023-06-26 12:05:36.381400 async_wrapper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      279 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-06-26 12:05:36.425400 async_wrapper-0.1.2/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      109 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/__init__.py
--rw-r--r--   0        0        0      919 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/_loky.py
--rw-r--r--   0        0        0      706 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/_thread.py
--rw-r--r--   0        0        0      409 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/base.py
--rw-r--r--   0        0        0      652 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/main.py
--rw-r--r--   0        0        0     1723 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      107 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/synclib/__init__.py
--rw-r--r--   0        0        0     1006 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/synclib/_loky.py
--rw-r--r--   0        0        0     1217 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/synclib/_thread.py
--rw-r--r--   0        0        0     1581 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/synclib/base.py
--rw-r--r--   0        0        0      662 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/synclib/main.py
--rw-r--r--   0        0        0        0 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      113 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     2357 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/task_group/_anyio.py
--rw-r--r--   0        0        0     2208 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/task_group/_asyncio.py
--rw-r--r--   0        0        0     1889 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/task_group/base.py
--rw-r--r--   0        0        0     1244 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/task_group/main.py
--rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 async_wrapper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1610 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/README.md
+-rw-r--r--   0        0        0     3648 2023-06-27 12:37:49.717504 async_wrapper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-27 12:37:49.749504 async_wrapper-0.1.3/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/__init__.py
+-rw-r--r--   0        0        0      896 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/_loky.py
+-rw-r--r--   0        0        0      706 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/_thread.py
+-rw-r--r--   0        0        0      409 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/base.py
+-rw-r--r--   0        0        0      654 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/main.py
+-rw-r--r--   0        0        0     1721 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      107 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/synclib/__init__.py
+-rw-r--r--   0        0        0      983 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/synclib/_loky.py
+-rw-r--r--   0        0        0     1217 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/synclib/_thread.py
+-rw-r--r--   0        0        0     1581 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/synclib/base.py
+-rw-r--r--   0        0        0      656 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/synclib/main.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      165 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     2561 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/task_group/_anyio.py
+-rw-r--r--   0        0        0     2253 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/task_group/_asyncio.py
+-rw-r--r--   0        0        0     2123 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/task_group/base.py
+-rw-r--r--   0        0        0     1966 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/task_group/main.py
+-rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 async_wrapper-0.1.3/PKG-INFO
```

### Comparing `async_wrapper-0.1.2/LICENSE` & `async_wrapper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.2/README.md` & `async_wrapper-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 $ pip install "async_wrapper[anyio]"
 # or
 $ pip install "async_wrapper[loky]"
 ```
 
 ## how to use
 ```python
+from __future__ import annotations
+
 import asyncio
 
-from aiotools import TaskGroup
 # or(>=py311)
 # from asyncio.taskgroups import TaskGroup
-
-from async_wrapper import async_to_sync, get_taskgroup_wrapper
+from async_wrapper import async_to_sync, get_task_group_factory, get_task_group_wrapper
 
 
 @async_to_sync("thread")
 async def sample_func() -> int:
     await asyncio.sleep(1)
     return 1
 
@@ -40,16 +40,17 @@
 
 async def sample_func_2(x: int) -> int:
     await asyncio.sleep(1)
     return x
 
 
 async def main():
-    wrapper = get_taskgroup_wrapper("asyncio")
-    async with TaskGroup() as task_group:
+    wrapper = get_task_group_wrapper("asyncio")
+    factory = get_task_group_factory("asyncio")
+    async with factory() as task_group:
         value_1 = wrapper(sample_func_2, task_group)(1)
         value_2 = wrapper(sample_func_2, task_group)(2)
 
     assert isinstance(value_1.value, int)
     assert isinstance(value_2.value, int)
     assert value_1.value == 1
     assert value_2.value == 2
```

### Comparing `async_wrapper-0.1.2/pyproject.toml` & `async_wrapper-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.1.2"
+version = "0.1.3"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
```

### Comparing `async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/_loky.py` & `async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/_loky.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def sync_to_async(
     func: Callable[ParamT, ValueT],
 ) -> Callable[ParamT, Coroutine[Any, Any, ValueT]]:
     try:
         from loky.process_executor import (  # type: ignore
             ProcessPoolExecutor,  # type: ignore
         )
-    except (ImportError, ModuleNotFoundError) as exc:
+    except ImportError as exc:
         raise ImportError("install extas loky first") from exc
 
     @wraps(func)
     async def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
         with ProcessPoolExecutor(1) as pool:
             future = pool.submit(func, *args, **kwargs)  # type: ignore
             coro = asyncio.wrap_future(future)
```

### Comparing `async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/_thread.py` & `async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/main.py` & `async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 if TYPE_CHECKING:
     from async_wrapper.convert.asynclib.base import SyncToAsync
 
 __all__ = ["get_async_convertor"]
 
 DEFAULT_BACKEND = "thread"
-AsyncBackendType = Literal["thread"]
+AsyncBackendType = Literal["thread", "loky"]
 
 
 def get_async_convertor(
-    backend: AsyncBackendType | str | None = None,
+    backend: AsyncBackendType | None = None,
 ) -> SyncToAsync:
     """get async convertor
 
     Args:
         backend: thread. Defaults to None.
 
     Returns:
```

### Comparing `async_wrapper-0.1.2/src/async_wrapper/convert/main.py` & `async_wrapper-0.1.3/src/async_wrapper/convert/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,45 +25,45 @@
 __all__ = ["toggle_func", "async_to_sync", "sync_to_async"]
 
 
 @overload
 def toggle_func(
     func: Callable[ParamT, Coroutine[Any, Any, ValueT]],
     *,
-    backend: SyncBackendType | str | None = None,
+    backend: SyncBackendType | None = None,
 ) -> Callable[ParamT, ValueT]:
     ...
 
 
 @overload
 def toggle_func(
     func: Callable[ParamT, ValueT],
     *,
-    backend: AsyncBackendType | str | None = None,
+    backend: AsyncBackendType | None = None,
 ) -> Callable[ParamT, Coroutine[Any, Any, ValueT]]:
     ...
 
 
 def toggle_func(
     func: Callable[ParamT, ValueT] | Callable[ParamT, Coroutine[Any, Any, ValueT]],
     *,
-    backend: SyncBackendType | AsyncBackendType | str | None = None,
+    backend: SyncBackendType | AsyncBackendType | None = None,
 ) -> Callable[ParamT, ValueT] | Callable[ParamT, Coroutine[Any, Any, ValueT]]:
     """sync to async, async to sync
 
     Args:
         func: sync or async func
         backend: sync or async backend. Defaults to None.
 
     Returns:
         async or sync func
     """
     if iscoroutinefunction(func):
         convertor = get_sync_convertor(backend)
         return convertor(func)  # type: ignore
 
-    convertor = get_async_convertor(backend)
+    convertor = get_async_convertor(backend)  # type: ignore
     return convertor(func)  # type: ignore
 
 
 async_to_sync = get_sync_convertor
 sync_to_async = get_async_convertor
```

### Comparing `async_wrapper-0.1.2/src/async_wrapper/convert/synclib/_loky.py` & `async_wrapper-0.1.3/src/async_wrapper/convert/synclib/_loky.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def async_to_sync(
     func: Callable[ParamT, Awaitable[ValueT]],
 ) -> Callable[ParamT, ValueT]:
     try:
         from loky.process_executor import (  # type: ignore
             ProcessPoolExecutor,  # type: ignore
         )
-    except (ImportError, ModuleNotFoundError) as exc:
+    except ImportError as exc:
         raise ImportError("install extas loky first") from exc
 
     sync_func = as_sync_func(func)
 
     @wraps(func)
     def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
         with ProcessPoolExecutor(1) as pool:
```

### Comparing `async_wrapper-0.1.2/src/async_wrapper/convert/synclib/_thread.py` & `async_wrapper-0.1.3/src/async_wrapper/convert/synclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.2/src/async_wrapper/convert/synclib/base.py` & `async_wrapper-0.1.3/src/async_wrapper/convert/synclib/base.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.2/src/async_wrapper/convert/synclib/main.py` & `async_wrapper-0.1.3/src/async_wrapper/convert/synclib/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __all__ = ["get_sync_convertor"]
 
 DEFAULT_BACKEND = "thread"
 SyncBackendType = Literal["thread", "loky"]
 
 
 def get_sync_convertor(
-    backend: SyncBackendType | str | None = None,
+    backend: SyncBackendType | None = None,
 ) -> AsyncToSync:
     """get sync convertor
 
     Args:
         backend: thread or loky. Defaults to None.
 
     Returns:
```

### Comparing `async_wrapper-0.1.2/src/async_wrapper/task_group/_anyio.py` & `async_wrapper-0.1.3/src/async_wrapper/task_group/_anyio.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 
 from typing_extensions import ParamSpec, override
 
 from async_wrapper.task_group.base import BaseSoonWrapper, SoonValue
 
 try:
     from anyio.abc import TaskGroup  # type: ignore
-except (ImportError, ModuleNotFoundError):
+except ImportError:
     from typing import Any as TaskGroup
 
 
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
-__all__ = ["SoonWrapper", "wrap_soon"]
+__all__ = ["SoonWrapper", "wrap_soon", "get_task_group"]
 
 
 @final
 class SoonWrapper(
     BaseSoonWrapper[TaskGroup, ParamT, ValueT_co],
     Generic[ParamT, ValueT_co],
 ):
@@ -39,15 +39,15 @@
     def __new__(
         cls,
         func: Callable[OtherParamT, Awaitable[OtherValueT_co]],
         task_group: TaskGroup,
     ) -> SoonWrapper[OtherParamT, OtherValueT_co]:
         try:
             import anyio  # type: ignore # noqa: F401
-        except (ImportError, ModuleNotFoundError) as exc:
+        except ImportError as exc:
             raise ImportError("install extas anyio first") from exc
 
         return super().__new__(cls, func, task_group)  # type: ignore
 
     @override
     def __init__(
         self,
@@ -76,14 +76,22 @@
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
         result: SoonValue[ValueT_co] = SoonValue()
         self._func(result)(*args, **kwargs)
         return result
 
 
+def get_task_group() -> TaskGroup:
+    try:
+        from anyio import create_task_group  # type: ignore
+    except ImportError as exc:
+        raise ImportError("install extas anyio first") from exc
+    return create_task_group()
+
+
 async def _set_value(
     func: Callable[[], Coroutine[Any, Any, ValueT]],
     value: SoonValue[ValueT],
 ) -> None:
     result = await func()
     value.value = result
```

### Comparing `async_wrapper-0.1.2/src/async_wrapper/task_group/_asyncio.py` & `async_wrapper-0.1.3/src/async_wrapper/task_group/_asyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
-__all__ = ["SoonWrapper", "wrap_soon"]
+__all__ = ["SoonWrapper", "wrap_soon", "get_task_group"]
 
 
 @final
 class SoonWrapper(
     BaseSoonWrapper[TaskGroup, ParamT, ValueT_co],
     Generic[ParamT, ValueT_co],
 ):
@@ -84,7 +84,8 @@
     value: SoonValue[ValueT],
 ) -> None:
     result = await func()
     value.value = result
 
 
 wrap_soon = SoonWrapper
+get_task_group = TaskGroup
```

### Comparing `async_wrapper-0.1.2/src/async_wrapper/task_group/base.py` & `async_wrapper-0.1.3/src/async_wrapper/task_group/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from threading import local
-from typing import Any, Awaitable, Callable, Generic, TypeVar
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Generic,
+    Protocol,
+    TypeVar,
+)
 
 from typing_extensions import ParamSpec, override
 
 from async_wrapper.convert.synclib.base import as_coro_func
 
 TaskGroupT = TypeVar("TaskGroupT")
+TaskGroupT_co = TypeVar("TaskGroupT_co", covariant=True)
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 Pending = local()
 
-__all__ = ["PendingError", "BaseSoonWrapper", "SoonValue"]
+__all__ = ["PendingError", "BaseSoonWrapper", "SoonValue", "TaskGroupFactory"]
 
 
 class PendingError(Exception):
     ...
 
 
 class BaseSoonWrapper(ABC, Generic[TaskGroupT, ParamT, ValueT_co]):
@@ -66,7 +74,12 @@
     @value.deleter
     def value(self) -> None:
         raise NotImplementedError
 
     @property
     def is_ready(self) -> bool:  # noqa: D102
         return self._value is not Pending
+
+
+class TaskGroupFactory(Protocol[TaskGroupT_co]):
+    def __call__(self) -> TaskGroupT_co:  # noqa: D102
+        ...
```

### Comparing `async_wrapper-0.1.2/PKG-INFO` & `async_wrapper-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.1.2
+Version: 0.1.3
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -41,21 +41,21 @@
 $ pip install "async_wrapper[anyio]"
 # or
 $ pip install "async_wrapper[loky]"
 ```
 
 ## how to use
 ```python
+from __future__ import annotations
+
 import asyncio
 
-from aiotools import TaskGroup
 # or(>=py311)
 # from asyncio.taskgroups import TaskGroup
-
-from async_wrapper import async_to_sync, get_taskgroup_wrapper
+from async_wrapper import async_to_sync, get_task_group_factory, get_task_group_wrapper
 
 
 @async_to_sync("thread")
 async def sample_func() -> int:
     await asyncio.sleep(1)
     return 1
 
@@ -67,16 +67,17 @@
 
 async def sample_func_2(x: int) -> int:
     await asyncio.sleep(1)
     return x
 
 
 async def main():
-    wrapper = get_taskgroup_wrapper("asyncio")
-    async with TaskGroup() as task_group:
+    wrapper = get_task_group_wrapper("asyncio")
+    factory = get_task_group_factory("asyncio")
+    async with factory() as task_group:
         value_1 = wrapper(sample_func_2, task_group)(1)
         value_2 = wrapper(sample_func_2, task_group)(2)
 
     assert isinstance(value_1.value, int)
     assert isinstance(value_2.value, int)
     assert value_1.value == 1
     assert value_2.value == 2
```

