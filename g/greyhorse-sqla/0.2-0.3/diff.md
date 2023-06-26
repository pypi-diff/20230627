# Comparing `tmp/greyhorse_sqla-0.2.tar.gz` & `tmp/greyhorse_sqla-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse_sqla-0.2.tar", max compression
+gzip compressed data, was "greyhorse_sqla-0.3.tar", max compression
```

## Comparing `greyhorse_sqla-0.2.tar` & `greyhorse_sqla-0.3.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0       96 2023-05-06 23:35:23.266980 greyhorse_sqla-0.2/greyhorse_sqla/__init__.py
--rw-r--r--   0        0        0     3254 2023-04-26 11:42:15.504046 greyhorse_sqla-0.2/greyhorse_sqla/config.py
--rw-r--r--   0        0        0     4266 2023-04-26 17:19:18.163605 greyhorse_sqla-0.2/greyhorse_sqla/containers.py
--rw-r--r--   0        0        0     5421 2023-06-07 18:56:59.071498 greyhorse_sqla-0.2/greyhorse_sqla/engine.py
--rw-r--r--   0        0        0     5138 2023-05-06 23:38:34.861859 greyhorse_sqla-0.2/greyhorse_sqla/factory.py
--rw-r--r--   0        0        0     3155 2023-06-07 18:56:58.679510 greyhorse_sqla-0.2/greyhorse_sqla/model.py
--rw-r--r--   0        0        0     1422 2023-05-06 20:57:55.966776 greyhorse_sqla-0.2/greyhorse_sqla/query.py
--rw-r--r--   0        0        0    13372 2023-06-07 18:53:02.342965 greyhorse_sqla-0.2/greyhorse_sqla/repository.py
--rw-r--r--   0        0        0     2874 2023-04-26 15:29:49.359126 greyhorse_sqla-0.2/greyhorse_sqla/resources.py
--rw-r--r--   0        0        0      237 2023-05-06 23:37:41.048322 greyhorse_sqla-0.2/greyhorse_sqla/translations.toml
--rw-r--r--   0        0        0     1444 2023-06-07 18:55:03.467141 greyhorse_sqla-0.2/pyproject.toml
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 greyhorse_sqla-0.2/PKG-INFO
+-rw-r--r--   0        0        0       96 2023-05-06 23:35:23.266980 greyhorse_sqla-0.3/greyhorse_sqla/__init__.py
+-rw-r--r--   0        0        0     3254 2023-04-26 11:42:15.504046 greyhorse_sqla-0.3/greyhorse_sqla/config.py
+-rw-r--r--   0        0        0     4767 2023-06-26 23:41:57.934035 greyhorse_sqla-0.3/greyhorse_sqla/containers.py
+-rw-r--r--   0        0        0     3270 2023-06-26 23:41:57.934035 greyhorse_sqla-0.3/greyhorse_sqla/contexts.py
+-rw-r--r--   0        0        0     5425 2023-06-26 23:41:57.934035 greyhorse_sqla-0.3/greyhorse_sqla/engine.py
+-rw-r--r--   0        0        0     5138 2023-05-06 23:38:34.861859 greyhorse_sqla-0.3/greyhorse_sqla/factory.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:41:57.934035 greyhorse_sqla-0.3/greyhorse_sqla/migration/__init__.py
+-rw-r--r--   0        0        0     2281 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/migration/app.py
+-rw-r--r--   0        0        0     2121 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/migration/cmd.py
+-rw-r--r--   0        0        0      440 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/migration/containers.py
+-rw-r--r--   0        0        0     4973 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/migration/operator.py
+-rw-r--r--   0        0        0     1559 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/migration/utils.py
+-rw-r--r--   0        0        0     3161 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/model.py
+-rw-r--r--   0        0        0     1422 2023-05-06 20:57:55.966776 greyhorse_sqla-0.3/greyhorse_sqla/query.py
+-rw-r--r--   0        0        0    13404 2023-06-26 23:41:57.942035 greyhorse_sqla-0.3/greyhorse_sqla/repository.py
+-rw-r--r--   0        0        0     5876 2023-06-26 23:41:57.942035 greyhorse_sqla-0.3/greyhorse_sqla/resources.py
+-rw-r--r--   0        0        0      237 2023-05-06 23:37:41.048322 greyhorse_sqla-0.3/greyhorse_sqla/translations.toml
+-rw-r--r--   0        0        0     1444 2023-06-26 23:41:57.958034 greyhorse_sqla-0.3/pyproject.toml
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 greyhorse_sqla-0.3/PKG-INFO
```

### Comparing `greyhorse_sqla-0.2/greyhorse_sqla/config.py` & `greyhorse_sqla-0.3/greyhorse_sqla/config.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.2/greyhorse_sqla/containers.py` & `greyhorse_sqla-0.3/greyhorse_sqla/containers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dependency_injector import containers, providers
 
 from greyhorse_core.utils.confs import default_value
 from greyhorse_sqla.config import EngineConfig, SqlEngineType
+from greyhorse_sqla.contexts import SqlaSyncContext, SqlaAsyncContext
 from greyhorse_sqla.factory import SqlaSyncEngineFactory, SqlaAsyncEngineFactory
 from greyhorse_sqla.resources import SqlaSyncResource, SqlaAsyncResource
 
 
 def _prepare_single_engine_config(config, factory):
     if isinstance(config.engine_config(), EngineConfig):
         engine_config = config.engine_config()
@@ -42,31 +43,41 @@
 
     return None
 
 
 class SqlaSyncContainer(containers.DeclarativeContainer):
     __self__ = providers.Self()
     engine_factory = providers.Singleton(SqlaSyncEngineFactory)
+    context_factory = providers.Dependency(default=SqlaSyncContext)
+    force_rollback = providers.Object(False)
 
     def _create_engine(self, name: str, config: EngineConfig, db_type: SqlEngineType, *args, **kwargs):
         return self.engine_factory()(name, config, db_type, *args, **kwargs)
 
     create_engine = providers.Factory(_create_engine, __self__)
-    instance = providers.Singleton(SqlaSyncResource, engine_factory)
+    instance = providers.Singleton(
+        SqlaSyncResource, engine_factory=engine_factory,
+        context_factory=context_factory, force_rollback=force_rollback,
+    )
 
 
 class SqlaAsyncContainer(containers.DeclarativeContainer):
     __self__ = providers.Self()
     engine_factory = providers.Singleton(SqlaAsyncEngineFactory)
+    context_factory = providers.Dependency(default=SqlaAsyncContext)
+    force_rollback = providers.Object(False)
 
     def _create_engine(self, name: str, config: EngineConfig, db_type: SqlEngineType, *args, **kwargs):
         return self.engine_factory()(name, config, db_type, *args, **kwargs)
 
     create_engine = providers.Factory(_create_engine, __self__)
-    instance = providers.Singleton(SqlaAsyncResource, engine_factory)
+    instance = providers.Singleton(
+        SqlaAsyncResource, engine_factory=engine_factory,
+        context_factory=context_factory, force_rollback=force_rollback,
+    )
 
 
 class SingleSqlaSyncContainer(SqlaSyncContainer):
     __self__ = providers.Self()
     config = providers.Configuration()
 
     create_engine = providers.Factory(
```

### Comparing `greyhorse_sqla-0.2/greyhorse_sqla/engine.py` & `greyhorse_sqla-0.3/greyhorse_sqla/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from abc import ABC, abstractmethod
 from contextlib import contextmanager, AbstractContextManager, asynccontextmanager, AbstractAsyncContextManager
 from datetime import timedelta
 
 from sqlalchemy.ext.asyncio import AsyncSession as SqlaAsyncSession, async_scoped_session, async_sessionmaker
 from sqlalchemy.orm import Session as SqlaSyncSession, scoped_session, sessionmaker
 
-from greyhorse_core.context import get_context
+from greyhorse_core.app.context import get_context
 from greyhorse_core.engines.base import SyncEngine, AsyncEngine
 from greyhorse_core.i18n import tr
 from greyhorse_core.logging import logger
 from greyhorse_sqla.config import SqlEngineType
 
 
 class SqlaEngine(ABC):
```

### Comparing `greyhorse_sqla-0.2/greyhorse_sqla/factory.py` & `greyhorse_sqla-0.3/greyhorse_sqla/factory.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.2/greyhorse_sqla/model.py` & `greyhorse_sqla-0.3/greyhorse_sqla/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Mapping, Any, Tuple, Self, TYPE_CHECKING
+from typing import Any, Mapping, Self, TYPE_CHECKING, Tuple
 
-from sqlalchemy import ColumnCollection, Column
+from sqlalchemy import Column, ColumnCollection
 from sqlalchemy.orm import DeclarativeBase, joinedload, selectinload
 from sqlalchemy.orm.decl_api import DeclarativeAttributeIntercept
 from sqlalchemy.sql.base import ReadOnlyColumnCollection
 
 from greyhorse_core.data.models.base import IdType
 from greyhorse_core.data.models.filterable import FilterableModel
 from greyhorse_sqla.query import SqlaFiltersQuery, SqlaSortingQuery
@@ -50,15 +50,15 @@
 
     @classmethod
     def bind(cls, repository: 'SqlaModelRepository[IdType, Self, SqlaFiltersQuery, SqlaSortingQuery]'):
         cls._repo = repository
 
     def get_id_value(self) -> IdType:
         # noinspection PyProtectedMember
-        return self._get_column_values(self._repo._get_id_columns())
+        return self._get_column_values(self.__table__.primary_key.columns)
 
     @classmethod
     def get_columns(cls) -> ReadOnlyColumnCollection:
         return cls.__table__.columns()
 
     @classmethod
     def get_relationships(cls) -> Mapping[str, Any]:
```

### Comparing `greyhorse_sqla-0.2/greyhorse_sqla/query.py` & `greyhorse_sqla-0.3/greyhorse_sqla/query.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.2/greyhorse_sqla/repository.py` & `greyhorse_sqla-0.3/greyhorse_sqla/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from contextlib import AbstractContextManager, AbstractAsyncContextManager
 from functools import partial
 from typing import Callable, Type, Mapping, Any, Sequence, TypeVar, cast, Generic
 
 from sqlalchemy import update, CursorResult, select, delete, ColumnCollection, Column, inspect, tuple_, func, \
     literal_column, exists
 from sqlalchemy.exc import NoInspectionAvailable
 from sqlalchemy.ext.asyncio import AsyncSession as SqlaAsyncSession
 from sqlalchemy.orm import Session as SqlaSyncSession, attributes
 from sqlalchemy.orm.base import instance_state
 
 from greyhorse_core.data.repositories.base import IdType, ModelType, ModelFactory, EntityType, EntityFactory
 from greyhorse_core.data.repositories.filterable import FilterableRepository
+from greyhorse_core.engines.base import SyncSessionFactory as BaseSyncSessionFactory, \
+    AsyncSessionFactory as BaseAsyncSessionFactory
 from greyhorse_core.utils.invoke import is_awaitable
 from greyhorse_sqla.model import SqlaModel
 from greyhorse_sqla.query import SqlaFiltersQuery, SqlaSortingQuery
 
-SyncSessionFactory = Callable[[], AbstractContextManager[SqlaSyncSession]]
-AsyncSessionFactory = Callable[[], AbstractAsyncContextManager[SqlaAsyncSession]]
+SyncSessionFactory = BaseSyncSessionFactory[SqlaSyncSession]
+AsyncSessionFactory = BaseAsyncSessionFactory[SqlaAsyncSession]
 
 SqlaModelType = TypeVar('SqlaModelType', bound=SqlaModel, covariant=True)
 SqlaModelTypeFactory = Callable[..., SqlaModelType]
 
 
 class SqlaRepository(
     FilterableRepository[IdType, EntityType, SqlaFiltersQuery, SqlaSortingQuery],
```

### Comparing `greyhorse_sqla-0.2/pyproject.toml` & `greyhorse_sqla-0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "greyhorse-sqla"
-version = "0.2"
+version = "0.3"
 description = "Greyhorse SqlAlchemy library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `greyhorse_sqla-0.2/PKG-INFO` & `greyhorse_sqla-0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greyhorse-sqla
-Version: 0.2
+Version: 0.3
 Summary: Greyhorse SqlAlchemy library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
@@ -17,13 +17,13 @@
 Provides-Extra: mysql
 Provides-Extra: pg
 Provides-Extra: sqlite
 Requires-Dist: aiomysql (>=0.1,<0.2) ; extra == "mysql"
 Requires-Dist: aiosqlite (>=0.18,<0.19) ; extra == "sqlite"
 Requires-Dist: alembic (>=1.10,<2.0)
 Requires-Dist: asyncpg (>=0.27,<0.28) ; extra == "pg"
-Requires-Dist: greyhorse-core (==0.2)
+Requires-Dist: greyhorse-core (==0.3)
 Requires-Dist: psycopg2 (>=2.9,<3.0) ; extra == "pg"
 Requires-Dist: pymysql[rsa] (>=1.0,<2.0) ; extra == "mysql"
 Requires-Dist: sqlalchemy-utils (>=0.41,<0.42)
 Requires-Dist: sqlalchemy[asyncio,mypy] (>=2.0,<3.0)
 Project-URL: Repository, https://gitlab.com/max-plutonium/greyhorse
```

