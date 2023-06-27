# Comparing `tmp/datasaurus-0.0.1.dev1.tar.gz` & `tmp/datasaurus-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasaurus-0.0.1.dev1.tar", max compression
+gzip compressed data, was "datasaurus-0.0.1.dev2.tar", max compression
```

## Comparing `datasaurus-0.0.1.dev1.tar` & `datasaurus-0.0.1.dev2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     4884 2023-06-04 15:44:51.212108 datasaurus-0.0.1.dev1/README.md
--rw-r--r--   0        0        0        0 2023-05-30 20:08:00.050057 datasaurus-0.0.1.dev1/datasaurus/core/__init__.py
--rw-r--r--   0        0        0      179 2023-06-01 12:40:05.370264 datasaurus-0.0.1.dev1/datasaurus/core/loggers.py
--rw-r--r--   0        0        0      292 2023-06-06 17:48:41.370998 datasaurus-0.0.1.dev1/datasaurus/core/models/__init__.py
--rw-r--r--   0        0        0     9309 2023-06-13 18:17:48.496780 datasaurus-0.0.1.dev1/datasaurus/core/models/base.py
--rw-r--r--   0        0        0      452 2023-06-13 18:17:48.500113 datasaurus-0.0.1.dev1/datasaurus/core/models/exceptions.py
--rw-r--r--   0        0        0      465 2023-06-06 11:39:53.539533 datasaurus-0.0.1.dev1/datasaurus/core/models/format.py
--rw-r--r--   0        0        0      110 2023-05-29 10:15:30.715326 datasaurus-0.0.1.dev1/datasaurus/core/storage/__init__.py
--rw-r--r--   0        0        0     1493 2023-05-29 10:21:20.915953 datasaurus-0.0.1.dev1/datasaurus/core/storage/azure.py
--rw-r--r--   0        0        0     3147 2023-06-13 11:01:11.620860 datasaurus-0.0.1.dev1/datasaurus/core/storage/base.py
--rw-r--r--   0        0        0      505 2023-06-06 11:08:38.354503 datasaurus-0.0.1.dev1/datasaurus/core/storage/fields.py
--rw-r--r--   0        0        0     2632 2023-06-13 10:31:57.894140 datasaurus-0.0.1.dev1/datasaurus/core/storage/mixins.py
--rw-r--r--   0        0        0     2580 2023-06-06 17:48:28.990830 datasaurus-0.0.1.dev1/datasaurus/core/storage/storage.py
--rw-r--r--   0        0        0      972 2023-06-14 10:16:02.605632 datasaurus-0.0.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     5876 1970-01-01 00:00:00.000000 datasaurus-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0     4856 2023-06-24 18:01:39.649906 datasaurus-0.0.1.dev2/README.md
+-rw-r--r--   0        0        0      103 2023-06-27 10:20:17.881029 datasaurus-0.0.1.dev2/datasaurus/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:08:00.050057 datasaurus-0.0.1.dev2/datasaurus/core/__init__.py
+-rw-r--r--   0        0        0      179 2023-06-01 12:40:05.370264 datasaurus-0.0.1.dev2/datasaurus/core/loggers.py
+-rw-r--r--   0        0        0      274 2023-06-24 18:01:38.829898 datasaurus-0.0.1.dev2/datasaurus/core/models/__init__.py
+-rw-r--r--   0        0        0    11447 2023-06-27 10:20:17.891029 datasaurus-0.0.1.dev2/datasaurus/core/models/base.py
+-rw-r--r--   0        0        0     8222 2023-06-27 09:54:28.083326 datasaurus-0.0.1.dev2/datasaurus/core/models/columns.py
+-rw-r--r--   0        0        0      459 2023-06-24 18:01:38.829898 datasaurus-0.0.1.dev2/datasaurus/core/models/exceptions.py
+-rw-r--r--   0        0        0      156 2023-06-15 17:04:55.132713 datasaurus-0.0.1.dev2/datasaurus/core/storage/__init__.py
+-rw-r--r--   0        0        0     1512 2023-06-25 09:29:07.613566 datasaurus-0.0.1.dev2/datasaurus/core/storage/azure.py
+-rw-r--r--   0        0        0     3212 2023-06-27 10:19:32.607665 datasaurus-0.0.1.dev2/datasaurus/core/storage/base.py
+-rw-r--r--   0        0        0      846 2023-06-25 16:01:03.238419 datasaurus-0.0.1.dev2/datasaurus/core/storage/format.py
+-rw-r--r--   0        0        0     3388 2023-06-27 09:52:29.243246 datasaurus-0.0.1.dev2/datasaurus/core/storage/mixins.py
+-rw-r--r--   0        0        0     5100 2023-06-15 17:04:55.326051 datasaurus-0.0.1.dev2/datasaurus/core/storage/storage.py
+-rw-r--r--   0        0        0     1154 2023-06-27 10:23:31.704492 datasaurus-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0     6048 1970-01-01 00:00:00.000000 datasaurus-0.0.1.dev2/PKG-INFO
```

### Comparing `datasaurus-0.0.1.dev1/README.md` & `datasaurus-0.0.1.dev2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Datasaurus is a Data Engineering framework written in Python 3.7+
 
 It is based in Polars and heavily influenced by Django.
 
-The intention is to offer an opinionated, feature-rich and powerful framework to help you write
+Datasaurus offers an opinionated, feature-rich and powerful framework to help you write
 data pipelines, ETLs or data manipulation programs.
 
 [Documentation]() (TODO)
 ## It supports:
 - ✅ Fully support read/write operations.
 - ⭕ Not yet but will be implemented.
 - 💀 Won't be implemented in the near future.
 
 ### Storages:
 - Sqlite ✅
 - PostgresSQL ✅
-- MySQL/MariaDB ⭕
+- MySQL ✅
+- Mariadb ✅
 - Local Storage ✅
 - Azure blob storage ⭕
 - AWS S3 ⭕
 
 
 ### Formats:
 - CSV ✅
@@ -33,33 +34,32 @@
 - Delta Tables ⭕
 - Field validations ⭕
 
 ## Simple example
 ```python
 # settings.py 
 from datasaurus.core.storage import PostgresStorage, StorageGroup, SqliteStorage
-from datasaurus.core.models import StringField, IntegerField
+from datasaurus.core.models import StringColumn, IntegerColumn
 
 # We set the environment that will be used.
 os.environ['DATASAURUS_ENVIRONMENT'] = 'dev'
 
 class ProfilesData(StorageGroup):
     dev = SqliteStorage(path='/data/data.sqlite')
     live = PostgresStorage(username='user', password='user', host='localhost', database='postgres')
 
     
 # models.py
-from datasaurus.core.models import Model
-from datasaurus.core.models import StringField, IntegerField
+from datasaurus.core.models import Model, StringColumn, IntegerColumn
 
 class ProfileModel(Model):
-    id = IntegerField()
-    username = StringField()
-    mail = StringField()
-    sex = StringField()
+    id = IntegerColumn()
+    username = StringColumn()
+    mail = StringColumn()
+    sex = StringColumn()
 
     class Meta:
         storage = ProfilesData
         table_name = 'PROFILE'
 
 ```
```

### Comparing `datasaurus-0.0.1.dev1/datasaurus/core/models/base.py` & `datasaurus-0.0.1.dev2/datasaurus/core/models/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from functools import partial
-from typing import Callable, Optional
+from typing import Callable, Optional, Union
 
 import polars
 from polars import DataFrame
 
-from datasaurus.core.models.exceptions import MissingMeta, FormatNotSupportedByModelError, \
-    FormatNeededError, FieldNotExistsError
-from datasaurus.core.models.format import DataFormat
+from datasaurus import classproperty
+from datasaurus.core.models.exceptions import MissingMetaError, FormatNotSupportedByModelError, \
+    FormatNeededError, ColumnNotExistsError
+from datasaurus.core.storage.format import DataFormat
 from datasaurus.core.storage.base import Storage, StorageGroup
-from datasaurus.core.storage.fields import Field
+from datasaurus.core.models.columns import Column, Columns
 
 
 class lazy_func:
     """
     Wraps around a function and its argument to an object, it will call that function when that
     object is obtained by __get__, making it lazy.
     """
@@ -27,58 +28,60 @@
 class Options:
     supported_opts_from_meta = [
         'storage',
         'table_name',
         'auto_select',
         'recalculate',
         'format',
-        'fields',
+        'columns',
     ]
 
     def __init__(self, meta, model):
         self.meta = meta
         self.model = model
 
         # Options from meta
         self.storage = None
         self.table_name = ''
         self.auto_select = False
         self.recalculate = False
         self.format = None
 
         # Options from model
-        self.fields_dict = {}
-        self.fields = []
+        self.columns = Columns()
 
         self._populate_from_meta()
         self._populate_from_model()
 
     def _populate_from_model(self):
         """
-        Populates Options values from the given model on the __init__, we also inherit fields from the parent classes
+        Populates Options values from the given model on the __init__, we also inherit columns from the parent classes
         if they are models.
         """
-        # Fields defined in the current model.
-        new_fields = {
-            field_name: field for field_name, field in self.model.__dict__.items() if isinstance(field, Field)
-        }
-
-        # Set fields from base classes.
-        for base in self.model.mro()[:1]:  # We ignore the first one because it is itself, otherwise it conflicts.
+        # Columns defined in the current model.
+        new_columns = [
+            column for column in
+            self.model.__dict__.values() if isinstance(column, Column)
+        ]
+
+        new_columns = Columns(new_columns)
+
+        # Set columns from base classes (including parents).
+        for base in self.model.mro()[:1]:
+            # We ignore the first one because it is itself, otherwise it conflicts.
             if hasattr(base, '_meta'):
-                for parent_field in base._meta.fields:
-                    if parent_field in new_fields:
+                for column in base._meta.columns:
+                    if column in new_columns:
                         raise ValueError(
-                            f"Field '{parent_field}' from {self.model} clashes with parent model {base}"
+                            f"Column '{column}' from {self.model} clashes with parent model {base}"
                         )
 
-                new_fields.update(base._meta.fields_dict)
+                new_columns.extend(base._meta.columns)
 
-        self.fields = list(new_fields.keys())
-        self.fields_dict = new_fields
+        self.columns = new_columns
 
     def _populate_from_meta(self):
         """
         Populates Options values from the Meta class given on the __init__, only options from supported_opts_from_meta
         are populated, raises Value error if there is an option in Meta that is not defined in supported_opts..
         """
         opts = self.meta.__dict__.copy()
@@ -95,44 +98,43 @@
         if opts:
             raise ValueError(f'Invalid Meta options exists: {opts}')
 
     def __str__(self):
         return f'{self.__class__.__qualname__}({vars(self)})'
 
 
-class ModelBase(type):
+class ModelMeta(type):
     df: DataFrame
     _meta: Options
-    # This is where the data from cls.from_dict will be stored temporarily
     _data_from_cls: Optional[dict] = None
 
     def __new__(cls, name, bases, attrs, **kwargs):
         super_new = super().__new__
 
         # This beauty here has been 'taken' from django itself, it ensures that only
         # subclasses of ModelBase are initiated.
-        parents = [b for b in bases if isinstance(b, ModelBase)]
+        parents = [b for b in bases if isinstance(b, ModelMeta)]
         if not parents:
             return super_new(cls, name, bases, attrs)
 
         _new_class = super_new(cls, name, bases, attrs, **kwargs)
         _new_class._prepare()
         return _new_class
 
     def _prepare(cls):
         meta = getattr(cls, 'Meta', None)
         if not meta:
-            raise MissingMeta(f'Model {cls} does not have Meta')
+            raise MissingMetaError(f'Model {cls} does not have Meta')
 
         opts = Options(meta, cls)
 
         setattr(cls, '_meta', opts)
         setattr(cls, 'df', lazy_func(cls._get_df))
 
-    def _get_storage_or_default(cls, storage: Optional[Storage | StorageGroup],
+    def _get_storage_or_default(cls, storage: Optional[Union[Storage, StorageGroup]],
                                 environment: Optional[str] = None) -> Storage:
         """
         Resolves the appropriate storage and its environment.
 
         - If no storage is passed, the default storage will be returned (from meta).
         - If no environment is passed and either the passed storage or the default storage is a
         StorageGroup, returns the appropriate as per environment variable.
@@ -145,100 +147,154 @@
                 # or Storage.environment directly when passing the storage,
                 # we'd receive a StorageGroup instead of a Storage, by default
                 # return StorageGroup.from_env
                 storage = storage.from_env
 
         if environment:
             storage = storage.storage_group.with_env(environment)
+
         return storage
 
-    def _get_format_or_default(cls, format: Optional[DataFormat]):
+    def _get_format_or_default(cls, format: Optional[Union[DataFormat, str]] = None) -> Optional[
+        Union[DataFormat, str]]:
         """
-        If not format is given tries to infer it from the Meta.table_name
+        If no format is given tries to get it from the model:
+
+        There are two ways of getting it:
+        1. From meta.format
+        2. Inferring it from the meta.table_name
         """
-        if not format and cls._meta.table_name.__contains__('.'):
+        if format:
+            return format
+
+        if cls._meta.format:
+            return cls._meta.format
+
+        if cls._meta.table_name.__contains__('.'):
             table_name, file_extension = cls._meta.table_name.split('.')
             if file_extension:
-                format = file_extension
-        return format
+                return file_extension
+
+        return None
 
-    def _create_df(cls, using: Optional[Storage]) -> DataFrame:
+    def _create_df(cls, storage: Optional[Storage]) -> DataFrame:
         """
         Does the heavy lifting of creating the Dataframe from the right data source, depending on
-        opts (meta), the order of priority is as follows:
+        Options (Meta class in model), the order of priority is as follows:
 
-        1. Data from constructor - Model.from_dict({'column1': [1,2,3})
+        1. Data from constructor - Model.from_dict({'column1': [1,2,3]})
         2. Data from calculation - Model.calculate_data()
         3. Data from Storage - Storage
         """
         if cls._data_from_cls is not None:
-            df = polars.DataFrame(cls._data_from_cls)
+            df = polars.DataFrame(cls._data_from_cls, schema=cls._schema)
             del cls._data_from_cls
             cls._data_from_cls = None
 
         elif cls._meta.recalculate:
-            df = cls.calculate_data(cls)
+            try:
+                df = cls.calculate_data(cls)
+
+            except NotImplementedError as e:
+                raise ValueError(
+                    'Cannot generate dataframe, do you have recalculate=True in your model while'
+                    ' calculate_data is not defined in the model? If you are trying to create the'
+                    ' dataframe from existing data, set recalculate=False (default)') from e
+
+            if not isinstance(df, DataFrame):
+                raise ValueError(
+                    f'Function calculate_data has to return a polars Dataframe, not a {type(df)}')
 
         else:
-            using = cls._get_storage_or_default(using)
-            format = cls._meta.format
-            if format and not using.supports_format(format):
+            storage = cls._get_storage_or_default(storage)
+            format = cls._get_format_or_default()
+
+            if isinstance(format, str):
+                format = storage.supported_formats[format]
+
+            if format and not storage.supports_format(format):
                 raise ValueError(
-                    f"Storage of type '{type(using)}' does not support format '{format}',"
-                    f" supported formats by this storage are '{using.supported_formats}'"
+                    f"Storage of type '{type(storage)}' does not support format '{format}',"
+                    f" supported formats by this storage are '{storage.supported_formats}'"
                 )
-            df = using.read_file(cls._meta.table_name, cls._meta.fields, format)
+
+            if storage.needs_format and not format:
+                raise FormatNeededError(
+                    f"Cannot create Dataframe because storage of type '{type(storage)}'"
+                    " needs a format and it was not provided in the Meta class or it could"
+                    " not be inferred from the table_name attribute. To fix this add format "
+                    " in the Model's Meta class or an extension to the table_name"
+                )
+
+            df = storage.read_file(cls._meta.table_name,
+                                   cls._meta.columns.get_df_column_names(),
+                                   format=format)
+
         return df
 
-    def _get_df(cls, storage: Optional[Storage | StorageGroup] = None):
+    def _get_df(cls, storage: Optional[Union[Storage, StorageGroup]] = None):
         """
-        Applies schema validation, data validations and options to the newly created dataframe.
+        Applies schema validation (dtypes), data validations and options to the newly created dataframe.
         """
-        df = cls._create_df(using=storage)
+        df = cls._create_df(storage=storage)
 
         if cls._meta.auto_select:
-            df = df.select(cls._meta.fields)
+            df = df.select(cls._meta.columns.get_df_column_names())
 
         columns_from_df = frozenset(df.columns)
-        missing_columns = columns_from_df.difference(cls._meta.fields)
+        missing_columns = columns_from_df.difference(cls._meta.columns.get_df_column_names())
 
         if missing_columns:
             raise ValueError(
-                f"Dataframe columns do not match. df.columns: {df.columns}, models: {cls._meta.fields}"
+                f"Dataframe columns do not match. df.columns: {df.columns},"
+                f" models: {cls._meta.columns.get_df_column_names()}"
             )
+
+        columns_with_dtypes = cls._meta.columns.get_df_columns_polars(df.schema)
+        unique_columns = cls._meta.columns.get_df_column_names_by_attrs(unique=True)
+
+        df = df.with_columns(columns_with_dtypes)
+
+        if unique_columns:
+            df = df.unique(unique_columns)
+
         return df
 
 
-class Model(metaclass=ModelBase):
+class Model(metaclass=ModelMeta):
+    _meta: Options  # Defined to have autocompletion.
+
     def __init__(self, **kwargs):
         for column, column_value in kwargs.items():
-            if column not in self.fields:
-                raise FieldNotExistsError(
-                    f"{self} does not have column '{column}', columns are: {self.fields}")
+            if column not in self._meta.columns.get_model_columns():
+                raise ColumnNotExistsError(
+                    f"{self} does not have column '{column}', columns are: {self.columns}")
+
             setattr(self, column, column_value)
 
     def __str__(self):
         cls_name = self.__class__.__qualname__
-        return f'<{cls_name}: {cls_name} object ({", ".join(self.fields)})>'
+        return f'<{cls_name}: {cls_name} object ({", ".join(self.columns)})>'
 
-    @classmethod
-    @property
-    def fields(cls):
-        return cls._meta.fields
+    @classproperty
+    def columns(cls):
+        return cls._meta.columns.get_model_columns()
 
     @classmethod
-    def from_dict(cls, d: dict):
+    def from_dict(cls, d: dict, schema=None):
         setattr(cls, '_data_from_cls', d)
+        setattr(cls, '_schema', schema)
         return cls
 
-    def calculate_data(self):
+    def calculate_data(self) -> 'polars.DataFrame':
         raise NotImplementedError()
 
     @classmethod
-    def save(cls, to: 'Storage' = None,
+    def save(cls,
+             to: 'Storage' = None,
              format: DataFormat = None,
              table_name: str = None,
              environment: str = None,
              **kwargs):
 
         storage = cls._get_storage_or_default(to, environment=environment)
         format = cls._get_format_or_default(format)
@@ -253,8 +309,9 @@
         if storage.needs_format and not format:
             raise FormatNeededError(
                 f"Cannot save Dataframe because storage of type '{type(storage)}'"
                 " needs a format and it was not provided"
             )
 
         df = cls._get_df()
+
         storage.write_file(df, table_name, format=format, **kwargs)
```

### Comparing `datasaurus-0.0.1.dev1/datasaurus/core/storage/azure.py` & `datasaurus-0.0.1.dev2/datasaurus/core/storage/azure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import contextlib
 from io import BytesIO
 
-try:
-    from azure.storage.blob import BlobServiceClient, ContainerClient
-except:
-    pass
+with contextlib.suppress(ImportError):
+    from azure.storage.blob import BlobServiceClient
+
 from datasaurus.core.storage.base import Storage, AUTO_RESOLVE
 
 
 class AzureBlobStorage(Storage):
     __slots__ = ('connect_str', 'container_name', 'encoding', 'container_client')
 
     def __init__(self,
```

### Comparing `datasaurus-0.0.1.dev1/datasaurus/core/storage/base.py` & `datasaurus-0.0.1.dev2/datasaurus/core/storage/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import logging
 import os
 from abc import abstractmethod, ABC
 from typing import Union
 
 import polars
 
-from datasaurus.core.models.format import DataFormat, FormatNotSet
+from datasaurus.core.models.base import classproperty
+from datasaurus.core.storage.format import DataFormat, FormatNotSet
 
 
 class _auto_resolve:
     def __str__(self):
         return 'AUTO_RESOLVE'
 
 
@@ -51,15 +51,15 @@
 
     def supports_format(self, format: DataFormat):
         return format in self.supported_formats
 
     def __set_name__(self, owner, name):
         self.storage_group = owner
         if not isinstance(owner(), StorageGroup):
-            raise Exception('Cannot register') # Todo refactor exception
+            raise Exception('Cannot register')  # Todo refactor exception
 
         if self.environment == AUTO_RESOLVE:
             self.environment = name
 
     def __str__(self):
         return f'{self.__class__.__qualname__}<environment={self.environment}>'
 
@@ -75,19 +75,19 @@
             if isinstance(element, Storage)
         ]
 
     @classmethod
     def with_env(cls, environment):
         if environment not in cls.environments:
             raise Exception(
-                f"Storage Group '{cls}' does not have environment {environment}, declared enviroinmentes are : {cls.environments}")
+                f"Storage Group '{cls}' does not have environment {environment},"
+                f" declared enviroinmentes are : {cls.environments}")
         return getattr(cls, environment)
 
-    @classmethod
-    @property
+    @classproperty
     def from_env(cls) -> Storage:
         """
         Tries to infer the environment from two different env variables.
 
         - {SERVICENAME}_ENVIRONMENT (1)
         - DATASAURUS_ENVIRONMENT (2)
 
@@ -100,9 +100,10 @@
         datasaurus_env_key = os.getenv('DATASAURUS_ENVIRONMENT')
         service_env_key = os.getenv(f'{cls.__name__}_ENVIRONMENT')
 
         if env_key := datasaurus_env_key or service_env_key:
             return getattr(cls, env_key)
 
         raise CannotResolveEnvironmentException(
-            f'Neither DATASAURUS_ENVIRONMENT nor {cls.__name__}_ENVIRONMENT are defined but "from_env" needs any of these two defined in order to resolve the right storage.'
+            f'Neither DATASAURUS_ENVIRONMENT nor {cls.__name__}_ENVIRONMENT are defined but '
+            f'"from_env" needs any of these two defined in order to resolve the right storage.'
         )
```

### Comparing `datasaurus-0.0.1.dev1/datasaurus/core/storage/mixins.py` & `datasaurus-0.0.1.dev2/datasaurus/core/storage/mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,91 @@
 import pathlib
+from abc import ABC, abstractmethod
+from typing import List
 
 import polars as pl
 
 from datasaurus.core.loggers import datasaurus_logger
-from datasaurus.core.models.format import FileFormat
+from datasaurus.core.storage.format import FileFormat
 
 
-def list_to_sql_columns(l: list[str]) -> str:
+class StorageOperationMixinBase(ABC):
+    """Simple abc to stop me from messing it up when creating new Mixins"""
+
+    @abstractmethod
+    def read_file(self, file_name, columns, format): ...
+
+    @abstractmethod
+    def write_file(self, df, file_name, format, **kwargs): ...
+
+    @abstractmethod
+    def file_exists(self, file_name, format: FileFormat): ...
+
+
+def list_to_sql_columns(input_list: List[str]) -> str:
     """
     Transforms ["id", "username"...] into '(id, username)'
     """
-    return str(l).replace('[', '').replace(']', '').replace("'", "")
+    return str(input_list).replace('[', '').replace(']', '').replace("'", "")
 
 
-class SQLStorageOperationsMixin:
-    def read_file(self, file_name: str, columns: list):
+class SQLStorageOperationsMixin(StorageOperationMixinBase):
+    EXISTS_QUERY = 'SELECT * FROM `{table_name}` LIMIT 1'
+
+    def read_file(self, file_name: str, columns: list, format=None):
         datasaurus_logger.debug(f'Trying to read {file_name}')
         query = f'SELECT {list_to_sql_columns(columns)} FROM "{file_name}"'
         datasaurus_logger.debug(f'query: {query}')
         datasaurus_logger.debug(f'uri: {self.get_uri()}')
         return pl.read_database(query, self.get_uri())
 
-    def write_file(self, df: pl.DataFrame, file_name: str, **kwargs):
+    def write_file(self, df: pl.DataFrame, file_name: str, format: FileFormat, **kwargs):
         if_exists = 'append' if self.file_exists(file_name) else 'replace'
         datasaurus_logger.debug(f'Attempting to write: {df}')
         datasaurus_logger.debug(
-            f'Write configuration: { {"table_name": file_name, "connection_uri": self.get_uri(), "if_exists": if_exists} }'
+            f'Write configuration:'
+            f' { {"table_name": file_name, "connection_uri": self.get_uri(), "if_exists": if_exists} }'
         )
         df.write_database(
             table_name=file_name,
             connection_uri=self.get_uri(),
             if_exists=if_exists,
         )
         datasaurus_logger.debug(f'{file_name} written correctly.')
 
-    def file_exists(self, table_name) -> bool:
-        query = f'SELECT * FROM "{table_name}" LIMIT 1'
-        datasaurus_logger.debug(f'Checking if file "{table_name}" exists, running query "{query}"')
+    def file_exists(self, file_name, format: FileFormat = None) -> bool:
+        query = self.EXISTS_QUERY.format(table_name=file_name)
+        datasaurus_logger.debug(f'Checking if file "{file_name}" exists, running query "{query}"')
         datasaurus_logger.debug(f'uri {self.get_uri()}')
         try:
             pl.read_database(query, self.get_uri())
-        except RuntimeError as e:
+        except RuntimeError:
             # This is very dirty, fixme
             return False
         return True
 
 
-class LocalStorageOperationsMixin:
+class LocalStorageOperationsMixin(StorageOperationMixinBase):
     supported_formats = FileFormat
     needs_format = True
 
-    def file_exists(self, file_name) -> bool:
-        return pathlib.Path(self.get_uri()).exists()
+    def file_exists(self, file_name, format: FileFormat) -> bool:
+        return pathlib.Path(f'{self.get_uri()}/{file_name}.{format.name}').exists()
+
+    def write_file(self, df: pl.DataFrame, file_name: str, format: FileFormat, **kwargs):
+        full_path = (pathlib.Path(self.path) / file_name).with_suffix(suffix=format.suffix)
+
+        if not full_path.exists():
+            full_path.parent.mkdir(parents=True, exist_ok=True)
 
-    def write_file(self, data: pl.DataFrame, file_name: str, format: FileFormat, **kwargs):
-        full_path = f'{self.path}{file_name}.{format.name}' if format else file_name
-        _write_func = getattr(data, f'write_{format.name}')
+        _write_func = getattr(df, f'write_{format.name}')
         return _write_func(full_path, **kwargs)
 
     def read_file(self, file_name, columns, format: FileFormat = None, **kwargs):
-        srcdir = pathlib.Path(self.path)
-        full_path = (srcdir / file_name).with_suffix(f'.{format.name}')
+        full_path = (pathlib.Path(self.path) / file_name).with_suffix(format.suffix)
 
         if not full_path.exists():
             raise ValueError(f"Cannot find '{full_path}'")
 
         _read_func = getattr(pl, f'read_{format.name}')
 
         return _read_func(full_path)
```

### Comparing `datasaurus-0.0.1.dev1/pyproject.toml` & `datasaurus-0.0.1.dev2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 [tool.poetry]
 name = "datasaurus"
-version = "0.0.1dev1"
+version = "0.0.1dev2"
 description = "Data Engineering framework based on Polars.rs"
 repository = "https://www.github.com/surister/datasaurus"
 authors = ["surister <surister98@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["python3", "data", "polars", "dataframes", "framework", "OOP"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Topic :: Software Development :: Libraries"
-
-]
-packages = [
-    { include = "datasaurus" }
 ]
 
+
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 polars = "^0.17.15"
-connectorx = "^0.3.1"
+connectorx = [
+    {version = "^0.3.1", python="^3.8"},
+    {version= "^0.3.2a6", python="^3.11"}
+]
 pyarrow = "^12.0.0"
-adbc-driver-sqlite = "^0.4.0"
 pandas = "^2.0.2"
 sqlalchemy = "^2.0.15"
 
 
 [tool.poetry.group.azure.dependencies]
 azure-storage-blob = "^12.16.0"
 azure-identity = "^1.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.group.test.dependencies]
 factory-boy = "^3.2.1"
 
+[tool.poetry.group.mysql.dependencies]
+mysql-connector-python = "^8.0.33"
+mysqlclient = "^2.1.1"
+pymysql = "^1.0.3"
+
+
+[tool.poetry.group.postgres.dependencies]
+psycopg2 = "^2.9.6"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `datasaurus-0.0.1.dev1/PKG-INFO` & `datasaurus-0.0.1.dev2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: datasaurus
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Data Engineering framework based on Polars.rs
 Home-page: https://www.github.com/surister/datasaurus
 License: MIT
 Keywords: python3,data,polars,dataframes,framework,OOP
 Author: surister
 Author-email: surister98@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: adbc-driver-sqlite (>=0.4.0,<0.5.0)
-Requires-Dist: connectorx (>=0.3.1,<0.4.0)
+Requires-Dist: connectorx (>=0.3.1,<0.4.0) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: connectorx (>=0.3.2a6,<0.4.0) ; python_version >= "3.11" and python_version < "4.0"
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: polars (>=0.17.15,<0.18.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0)
 Project-URL: Repository, https://www.github.com/surister/datasaurus
 Description-Content-Type: text/markdown
 
 Datasaurus is a Data Engineering framework written in Python 3.7+
 
 It is based in Polars and heavily influenced by Django.
 
-The intention is to offer an opinionated, feature-rich and powerful framework to help you write
+Datasaurus offers an opinionated, feature-rich and powerful framework to help you write
 data pipelines, ETLs or data manipulation programs.
 
 [Documentation]() (TODO)
 ## It supports:
 - ✅ Fully support read/write operations.
 - ⭕ Not yet but will be implemented.
 - 💀 Won't be implemented in the near future.
 
 ### Storages:
 - Sqlite ✅
 - PostgresSQL ✅
-- MySQL/MariaDB ⭕
+- MySQL ✅
+- Mariadb ✅
 - Local Storage ✅
 - Azure blob storage ⭕
 - AWS S3 ⭕
 
 
 ### Formats:
 - CSV ✅
@@ -58,33 +61,32 @@
 - Delta Tables ⭕
 - Field validations ⭕
 
 ## Simple example
 ```python
 # settings.py 
 from datasaurus.core.storage import PostgresStorage, StorageGroup, SqliteStorage
-from datasaurus.core.models import StringField, IntegerField
+from datasaurus.core.models import StringColumn, IntegerColumn
 
 # We set the environment that will be used.
 os.environ['DATASAURUS_ENVIRONMENT'] = 'dev'
 
 class ProfilesData(StorageGroup):
     dev = SqliteStorage(path='/data/data.sqlite')
     live = PostgresStorage(username='user', password='user', host='localhost', database='postgres')
 
     
 # models.py
-from datasaurus.core.models import Model
-from datasaurus.core.models import StringField, IntegerField
+from datasaurus.core.models import Model, StringColumn, IntegerColumn
 
 class ProfileModel(Model):
-    id = IntegerField()
-    username = StringField()
-    mail = StringField()
-    sex = StringField()
+    id = IntegerColumn()
+    username = StringColumn()
+    mail = StringColumn()
+    sex = StringColumn()
 
     class Meta:
         storage = ProfilesData
         table_name = 'PROFILE'
 
 ```
```

