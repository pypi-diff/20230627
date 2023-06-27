# Comparing `tmp/mypy-boto3-kinesisvideo-1.26.28.tar.gz` & `tmp/mypy-boto3-kinesisvideo-1.26.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisvideo-1.26.28.tar", last modified: Mon Dec 12 20:27:27 2022, max compression
+gzip compressed data, was "mypy-boto3-kinesisvideo-1.26.33.tar", last modified: Mon Dec 19 20:27:39 2022, max compression
```

## Comparing `mypy-boto3-kinesisvideo-1.26.28.tar` & `mypy-boto3-kinesisvideo-1.26.33.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.859752 mypy-boto3-kinesisvideo-1.26.28/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-12 20:26:47.000000 mypy-boto3-kinesisvideo-1.26.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15759 2022-12-12 20:27:27.859752 mypy-boto3-kinesisvideo-1.26.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14252 2022-12-12 20:26:47.000000 mypy-boto3-kinesisvideo-1.26.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.855752 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-12 20:26:47.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2022-12-12 20:26:47.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-12 20:26:47.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20526 2022-12-12 20:26:48.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20492 2022-12-12 20:26:48.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2022-12-12 20:26:48.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2022-12-12 20:26:48.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2022-12-12 20:26:48.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2022-12-12 20:26:48.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 20:26:47.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22376 2022-12-12 20:26:48.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22343 2022-12-12 20:26:48.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-12 20:26:47.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.855752 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15759 2022-12-12 20:27:27.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-12 20:27:27.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 20:27:27.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 20:27:27.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-12 20:27:27.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-12 20:27:27.000000 mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 20:27:27.859752 mypy-boto3-kinesisvideo-1.26.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2022-12-12 20:26:47.000000 mypy-boto3-kinesisvideo-1.26.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:27:39.495972 mypy-boto3-kinesisvideo-1.26.33/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16547 2022-12-19 20:27:39.495972 mypy-boto3-kinesisvideo-1.26.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15040 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:27:39.495972 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23103 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23065 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25175 2022-12-19 20:26:51.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2022-12-19 20:26:51.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:27:39.495972 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16547 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 20:27:39.495972 mypy-boto3-kinesisvideo-1.26.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/setup.py
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/LICENSE` & `mypy-boto3-kinesisvideo-1.26.33/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.26.28/PKG-INFO` & `mypy-boto3-kinesisvideo-1.26.33/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.26.28
-Summary: Type annotations for boto3.KinesisVideo 1.26.28 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.33
+Summary: Type annotations for boto3.KinesisVideo 1.26.33 service generated with mypy-boto3-builder 7.12.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisvideo?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.26.33](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -279,20 +279,27 @@
 `mypy_boto3_kinesisvideo.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kinesisvideo import KinesisVideoClient
-from mypy_boto3_kinesisvideo.paginator import ListSignalingChannelsPaginator, ListStreamsPaginator
+from mypy_boto3_kinesisvideo.paginator import (
+    DescribeMappedResourceConfigurationPaginator,
+    ListSignalingChannelsPaginator,
+    ListStreamsPaginator,
+)
 
 client: KinesisVideoClient = Session().client("kinesisvideo")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = (
+    client.get_paginator("describe_mapped_resource_configuration")
+)
 list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator(
     "list_signaling_channels"
 )
 list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
 ```
 
 <a id="literals"></a>
@@ -306,19 +313,21 @@
 from mypy_boto3_kinesisvideo.literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ComparisonOperatorType,
     ConfigurationStatusType,
+    DescribeMappedResourceConfigurationPaginatorName,
     FormatConfigKeyType,
     FormatType,
     ImageSelectorTypeType,
     ListSignalingChannelsPaginatorName,
     ListStreamsPaginatorName,
+    MediaStorageConfigurationStatusType,
     MediaUriTypeType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
     KinesisVideoServiceName,
     ServiceName,
@@ -347,23 +356,27 @@
     ResponseMetadataTypeDef,
     CreateStreamInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    DescribeMappedResourceConfigurationInputRequestTypeDef,
+    MappedResourceConfigurationListItemTypeDef,
+    DescribeMediaStorageConfigurationInputRequestTypeDef,
+    MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     GetDataEndpointInputRequestTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
     ImageGenerationDestinationConfigTypeDef,
-    PaginatorConfigTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     MediaSourceConfigTypeDef,
     NotificationDestinationConfigTypeDef,
     ScheduleConfigTypeDef,
     TagStreamInputRequestTypeDef,
@@ -378,20 +391,24 @@
     TagResourceInputRequestTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamOutputTypeDef,
     GetDataEndpointOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
+    DescribeMappedResourceConfigurationOutputTypeDef,
+    DescribeMediaStorageConfigurationOutputTypeDef,
+    UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/README.md` & `mypy-boto3-kinesisvideo-1.26.33/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisvideo?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.26.33](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -247,20 +247,27 @@
 `mypy_boto3_kinesisvideo.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kinesisvideo import KinesisVideoClient
-from mypy_boto3_kinesisvideo.paginator import ListSignalingChannelsPaginator, ListStreamsPaginator
+from mypy_boto3_kinesisvideo.paginator import (
+    DescribeMappedResourceConfigurationPaginator,
+    ListSignalingChannelsPaginator,
+    ListStreamsPaginator,
+)
 
 client: KinesisVideoClient = Session().client("kinesisvideo")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = (
+    client.get_paginator("describe_mapped_resource_configuration")
+)
 list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator(
     "list_signaling_channels"
 )
 list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
 ```
 
 <a id="literals"></a>
@@ -274,19 +281,21 @@
 from mypy_boto3_kinesisvideo.literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ComparisonOperatorType,
     ConfigurationStatusType,
+    DescribeMappedResourceConfigurationPaginatorName,
     FormatConfigKeyType,
     FormatType,
     ImageSelectorTypeType,
     ListSignalingChannelsPaginatorName,
     ListStreamsPaginatorName,
+    MediaStorageConfigurationStatusType,
     MediaUriTypeType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
     KinesisVideoServiceName,
     ServiceName,
@@ -315,23 +324,27 @@
     ResponseMetadataTypeDef,
     CreateStreamInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    DescribeMappedResourceConfigurationInputRequestTypeDef,
+    MappedResourceConfigurationListItemTypeDef,
+    DescribeMediaStorageConfigurationInputRequestTypeDef,
+    MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     GetDataEndpointInputRequestTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
     ImageGenerationDestinationConfigTypeDef,
-    PaginatorConfigTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     MediaSourceConfigTypeDef,
     NotificationDestinationConfigTypeDef,
     ScheduleConfigTypeDef,
     TagStreamInputRequestTypeDef,
@@ -346,20 +359,24 @@
     TagResourceInputRequestTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamOutputTypeDef,
     GetDataEndpointOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
+    DescribeMappedResourceConfigurationOutputTypeDef,
+    DescribeMediaStorageConfigurationOutputTypeDef,
+    UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/__main__.py` & `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideo 1.26.28\nVersion:         1.26.28\nBuilder"
+        "Type annotations for boto3.KinesisVideo 1.26.33\nVersion:         1.26.33\nBuilder"
         " version: 7.12.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.28")
+    print("1.26.33")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/client.py` & `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,39 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import APINameType, ChannelTypeType, UpdateDataRetentionOperationType
-from .paginator import ListSignalingChannelsPaginator, ListStreamsPaginator
+from .paginator import (
+    DescribeMappedResourceConfigurationPaginator,
+    ListSignalingChannelsPaginator,
+    ListStreamsPaginator,
+)
 from .type_defs import (
     ChannelNameConditionTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamOutputTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
+    DescribeMappedResourceConfigurationOutputTypeDef,
+    DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
+    MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     SingleMasterConfigurationTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
     StreamNameConditionTypeDef,
     TagTypeDef,
 )
@@ -181,14 +188,39 @@
         """
         Gets the `ImageGenerationConfiguration` for a given Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_image_generation_configuration)
         """
 
+    def describe_mapped_resource_configuration(
+        self,
+        *,
+        StreamName: str = ...,
+        StreamARN: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeMappedResourceConfigurationOutputTypeDef:
+        """
+        Returns the most current information about the stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_mapped_resource_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_mapped_resource_configuration)
+        """
+
+    def describe_media_storage_configuration(
+        self, *, ChannelName: str = ..., ChannelARN: str = ...
+    ) -> DescribeMediaStorageConfigurationOutputTypeDef:
+        """
+        Returns the most current information about the channel.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_media_storage_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_media_storage_configuration)
+        """
+
     def describe_notification_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeNotificationConfigurationOutputTypeDef:
         """
         Gets the `NotificationConfiguration` for a given Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_notification_configuration)
@@ -374,14 +406,24 @@
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_image_generation_configuration)
         """
 
+    def update_media_storage_configuration(
+        self, *, ChannelARN: str, MediaStorageConfiguration: MediaStorageConfigurationTypeDef
+    ) -> Dict[str, Any]:
+        """
+        Associates a `SignalingChannel` to a stream to store the media.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_media_storage_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_media_storage_configuration)
+        """
+
     def update_notification_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
@@ -420,14 +462,23 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_stream)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_mapped_resource_configuration"]
+    ) -> DescribeMappedResourceConfigurationPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_signaling_channels"]
     ) -> ListSignalingChannelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/client.pyi` & `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,39 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import APINameType, ChannelTypeType, UpdateDataRetentionOperationType
-from .paginator import ListSignalingChannelsPaginator, ListStreamsPaginator
+from .paginator import (
+    DescribeMappedResourceConfigurationPaginator,
+    ListSignalingChannelsPaginator,
+    ListStreamsPaginator,
+)
 from .type_defs import (
     ChannelNameConditionTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamOutputTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
+    DescribeMappedResourceConfigurationOutputTypeDef,
+    DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
+    MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     SingleMasterConfigurationTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
     StreamNameConditionTypeDef,
     TagTypeDef,
 )
@@ -168,14 +175,37 @@
     ) -> DescribeImageGenerationConfigurationOutputTypeDef:
         """
         Gets the `ImageGenerationConfiguration` for a given Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_image_generation_configuration)
         """
+    def describe_mapped_resource_configuration(
+        self,
+        *,
+        StreamName: str = ...,
+        StreamARN: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeMappedResourceConfigurationOutputTypeDef:
+        """
+        Returns the most current information about the stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_mapped_resource_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_mapped_resource_configuration)
+        """
+    def describe_media_storage_configuration(
+        self, *, ChannelName: str = ..., ChannelARN: str = ...
+    ) -> DescribeMediaStorageConfigurationOutputTypeDef:
+        """
+        Returns the most current information about the channel.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_media_storage_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_media_storage_configuration)
+        """
     def describe_notification_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeNotificationConfigurationOutputTypeDef:
         """
         Gets the `NotificationConfiguration` for a given Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_notification_configuration)
@@ -344,14 +374,23 @@
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_image_generation_configuration)
         """
+    def update_media_storage_configuration(
+        self, *, ChannelARN: str, MediaStorageConfiguration: MediaStorageConfigurationTypeDef
+    ) -> Dict[str, Any]:
+        """
+        Associates a `SignalingChannel` to a stream to store the media.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_media_storage_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_media_storage_configuration)
+        """
     def update_notification_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
@@ -387,14 +426,22 @@
         Updates stream metadata, such as the device name and media type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_stream)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_mapped_resource_configuration"]
+    ) -> DescribeMappedResourceConfigurationPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_signaling_channels"]
     ) -> ListSignalingChannelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
         """
     @overload
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/literals.py` & `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,21 @@
 __all__ = (
     "APINameType",
     "ChannelProtocolType",
     "ChannelRoleType",
     "ChannelTypeType",
     "ComparisonOperatorType",
     "ConfigurationStatusType",
+    "DescribeMappedResourceConfigurationPaginatorName",
     "FormatConfigKeyType",
     "FormatType",
     "ImageSelectorTypeType",
     "ListSignalingChannelsPaginatorName",
     "ListStreamsPaginatorName",
+    "MediaStorageConfigurationStatusType",
     "MediaUriTypeType",
     "StatusType",
     "StrategyOnFullSizeType",
     "SyncStatusType",
     "UpdateDataRetentionOperationType",
     "KinesisVideoServiceName",
     "ServiceName",
@@ -50,24 +52,26 @@
     "GET_HLS_STREAMING_SESSION_URL",
     "GET_IMAGES",
     "GET_MEDIA",
     "GET_MEDIA_FOR_FRAGMENT_LIST",
     "LIST_FRAGMENTS",
     "PUT_MEDIA",
 ]
-ChannelProtocolType = Literal["HTTPS", "WSS"]
+ChannelProtocolType = Literal["HTTPS", "WEBRTC", "WSS"]
 ChannelRoleType = Literal["MASTER", "VIEWER"]
 ChannelTypeType = Literal["FULL_MESH", "SINGLE_MASTER"]
 ComparisonOperatorType = Literal["BEGINS_WITH"]
 ConfigurationStatusType = Literal["DISABLED", "ENABLED"]
+DescribeMappedResourceConfigurationPaginatorName = Literal["describe_mapped_resource_configuration"]
 FormatConfigKeyType = Literal["JPEGQuality"]
 FormatType = Literal["JPEG", "PNG"]
 ImageSelectorTypeType = Literal["PRODUCER_TIMESTAMP", "SERVER_TIMESTAMP"]
 ListSignalingChannelsPaginatorName = Literal["list_signaling_channels"]
 ListStreamsPaginatorName = Literal["list_streams"]
+MediaStorageConfigurationStatusType = Literal["DISABLED", "ENABLED"]
 MediaUriTypeType = Literal["FILE_URI", "RTSP_URI"]
 StatusType = Literal["ACTIVE", "CREATING", "DELETING", "UPDATING"]
 StrategyOnFullSizeType = Literal["DELETE_OLDEST_MEDIA", "DENY_NEW_MEDIA"]
 SyncStatusType = Literal[
     "ACKNOWLEDGED", "DELETE_FAILED", "DELETING", "IN_SYNC", "SYNCING", "SYNC_FAILED"
 ]
 UpdateDataRetentionOperationType = Literal["DECREASE_DATA_RETENTION", "INCREASE_DATA_RETENTION"]
@@ -241,14 +245,15 @@
     "kafkaconnect",
     "kendra",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
@@ -416,15 +421,17 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal["list_signaling_channels", "list_streams"]
+PaginatorName = Literal[
+    "describe_mapped_resource_configuration", "list_signaling_channels", "list_streams"
+]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/literals.pyi` & `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,21 @@
 __all__ = (
     "APINameType",
     "ChannelProtocolType",
     "ChannelRoleType",
     "ChannelTypeType",
     "ComparisonOperatorType",
     "ConfigurationStatusType",
+    "DescribeMappedResourceConfigurationPaginatorName",
     "FormatConfigKeyType",
     "FormatType",
     "ImageSelectorTypeType",
     "ListSignalingChannelsPaginatorName",
     "ListStreamsPaginatorName",
+    "MediaStorageConfigurationStatusType",
     "MediaUriTypeType",
     "StatusType",
     "StrategyOnFullSizeType",
     "SyncStatusType",
     "UpdateDataRetentionOperationType",
     "KinesisVideoServiceName",
     "ServiceName",
@@ -48,24 +50,26 @@
     "GET_HLS_STREAMING_SESSION_URL",
     "GET_IMAGES",
     "GET_MEDIA",
     "GET_MEDIA_FOR_FRAGMENT_LIST",
     "LIST_FRAGMENTS",
     "PUT_MEDIA",
 ]
-ChannelProtocolType = Literal["HTTPS", "WSS"]
+ChannelProtocolType = Literal["HTTPS", "WEBRTC", "WSS"]
 ChannelRoleType = Literal["MASTER", "VIEWER"]
 ChannelTypeType = Literal["FULL_MESH", "SINGLE_MASTER"]
 ComparisonOperatorType = Literal["BEGINS_WITH"]
 ConfigurationStatusType = Literal["DISABLED", "ENABLED"]
+DescribeMappedResourceConfigurationPaginatorName = Literal["describe_mapped_resource_configuration"]
 FormatConfigKeyType = Literal["JPEGQuality"]
 FormatType = Literal["JPEG", "PNG"]
 ImageSelectorTypeType = Literal["PRODUCER_TIMESTAMP", "SERVER_TIMESTAMP"]
 ListSignalingChannelsPaginatorName = Literal["list_signaling_channels"]
 ListStreamsPaginatorName = Literal["list_streams"]
+MediaStorageConfigurationStatusType = Literal["DISABLED", "ENABLED"]
 MediaUriTypeType = Literal["FILE_URI", "RTSP_URI"]
 StatusType = Literal["ACTIVE", "CREATING", "DELETING", "UPDATING"]
 StrategyOnFullSizeType = Literal["DELETE_OLDEST_MEDIA", "DENY_NEW_MEDIA"]
 SyncStatusType = Literal[
     "ACKNOWLEDGED", "DELETE_FAILED", "DELETING", "IN_SYNC", "SYNCING", "SYNC_FAILED"
 ]
 UpdateDataRetentionOperationType = Literal["DECREASE_DATA_RETENTION", "INCREASE_DATA_RETENTION"]
@@ -239,14 +243,15 @@
     "kafkaconnect",
     "kendra",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
@@ -414,15 +419,17 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal["list_signaling_channels", "list_streams"]
+PaginatorName = Literal[
+    "describe_mapped_resource_configuration", "list_signaling_channels", "list_streams"
+]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/type_defs.py` & `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
     FormatType,
     ImageSelectorTypeType,
+    MediaStorageConfigurationStatusType,
     MediaUriTypeType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
 )
 
@@ -47,23 +48,27 @@
     "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "DescribeMappedResourceConfigurationInputRequestTypeDef",
+    "MappedResourceConfigurationListItemTypeDef",
+    "DescribeMediaStorageConfigurationInputRequestTypeDef",
+    "MediaStorageConfigurationTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
     "GetDataEndpointInputRequestTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "MediaSourceConfigTypeDef",
     "NotificationDestinationConfigTypeDef",
     "ScheduleConfigTypeDef",
     "TagStreamInputRequestTypeDef",
@@ -78,20 +83,24 @@
     "TagResourceInputRequestTypeDef",
     "CreateSignalingChannelOutputTypeDef",
     "CreateStreamOutputTypeDef",
     "GetDataEndpointOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamOutputTypeDef",
     "DeletionConfigTypeDef",
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    "DescribeMappedResourceConfigurationOutputTypeDef",
+    "DescribeMediaStorageConfigurationOutputTypeDef",
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
@@ -232,14 +241,74 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+DescribeMappedResourceConfigurationInputRequestTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+MappedResourceConfigurationListItemTypeDef = TypedDict(
+    "MappedResourceConfigurationListItemTypeDef",
+    {
+        "Type": str,
+        "ARN": str,
+    },
+    total=False,
+)
+
+DescribeMediaStorageConfigurationInputRequestTypeDef = TypedDict(
+    "DescribeMediaStorageConfigurationInputRequestTypeDef",
+    {
+        "ChannelName": str,
+        "ChannelARN": str,
+    },
+    total=False,
+)
+
+_RequiredMediaStorageConfigurationTypeDef = TypedDict(
+    "_RequiredMediaStorageConfigurationTypeDef",
+    {
+        "Status": MediaStorageConfigurationStatusType,
+    },
+)
+_OptionalMediaStorageConfigurationTypeDef = TypedDict(
+    "_OptionalMediaStorageConfigurationTypeDef",
+    {
+        "StreamARN": str,
+    },
+    total=False,
+)
+
+
+class MediaStorageConfigurationTypeDef(
+    _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
+):
+    pass
+
+
 DescribeNotificationConfigurationInputRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
@@ -323,24 +392,14 @@
     "ImageGenerationDestinationConfigTypeDef",
     {
         "Uri": str,
         "DestinationRegion": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 StreamNameConditionTypeDef = TypedDict(
     "StreamNameConditionTypeDef",
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
@@ -627,14 +686,58 @@
         "EdgeRetentionInHours": int,
         "LocalSizeConfig": LocalSizeConfigTypeDef,
         "DeleteAfterUpload": bool,
     },
     total=False,
 )
 
+DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    {
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeMappedResourceConfigurationOutputTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationOutputTypeDef",
+    {
+        "MappedResourceConfigurationList": List[MappedResourceConfigurationListItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeMediaStorageConfigurationOutputTypeDef = TypedDict(
+    "DescribeMediaStorageConfigurationOutputTypeDef",
+    {
+        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
+    {
+        "ChannelARN": str,
+        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
+    },
+)
+
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamInfo": StreamInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -701,23 +804,14 @@
 
 class ImageGenerationConfigurationTypeDef(
     _RequiredImageGenerationConfigurationTypeDef, _OptionalImageGenerationConfigurationTypeDef
 ):
     pass
 
 
-ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    {
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo/type_defs.pyi` & `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
     FormatType,
     ImageSelectorTypeType,
+    MediaStorageConfigurationStatusType,
     MediaUriTypeType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
 )
 
@@ -46,23 +47,27 @@
     "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "DescribeMappedResourceConfigurationInputRequestTypeDef",
+    "MappedResourceConfigurationListItemTypeDef",
+    "DescribeMediaStorageConfigurationInputRequestTypeDef",
+    "MediaStorageConfigurationTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
     "GetDataEndpointInputRequestTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
     "MediaSourceConfigTypeDef",
     "NotificationDestinationConfigTypeDef",
     "ScheduleConfigTypeDef",
     "TagStreamInputRequestTypeDef",
@@ -77,20 +82,24 @@
     "TagResourceInputRequestTypeDef",
     "CreateSignalingChannelOutputTypeDef",
     "CreateStreamOutputTypeDef",
     "GetDataEndpointOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamOutputTypeDef",
     "DeletionConfigTypeDef",
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    "DescribeMappedResourceConfigurationOutputTypeDef",
+    "DescribeMediaStorageConfigurationOutputTypeDef",
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
@@ -225,14 +234,72 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+DescribeMappedResourceConfigurationInputRequestTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+MappedResourceConfigurationListItemTypeDef = TypedDict(
+    "MappedResourceConfigurationListItemTypeDef",
+    {
+        "Type": str,
+        "ARN": str,
+    },
+    total=False,
+)
+
+DescribeMediaStorageConfigurationInputRequestTypeDef = TypedDict(
+    "DescribeMediaStorageConfigurationInputRequestTypeDef",
+    {
+        "ChannelName": str,
+        "ChannelARN": str,
+    },
+    total=False,
+)
+
+_RequiredMediaStorageConfigurationTypeDef = TypedDict(
+    "_RequiredMediaStorageConfigurationTypeDef",
+    {
+        "Status": MediaStorageConfigurationStatusType,
+    },
+)
+_OptionalMediaStorageConfigurationTypeDef = TypedDict(
+    "_OptionalMediaStorageConfigurationTypeDef",
+    {
+        "StreamARN": str,
+    },
+    total=False,
+)
+
+class MediaStorageConfigurationTypeDef(
+    _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
+):
+    pass
+
 DescribeNotificationConfigurationInputRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
@@ -314,24 +381,14 @@
     "ImageGenerationDestinationConfigTypeDef",
     {
         "Uri": str,
         "DestinationRegion": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 StreamNameConditionTypeDef = TypedDict(
     "StreamNameConditionTypeDef",
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
@@ -604,14 +661,58 @@
         "EdgeRetentionInHours": int,
         "LocalSizeConfig": LocalSizeConfigTypeDef,
         "DeleteAfterUpload": bool,
     },
     total=False,
 )
 
+DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    {
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeMappedResourceConfigurationOutputTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationOutputTypeDef",
+    {
+        "MappedResourceConfigurationList": List[MappedResourceConfigurationListItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeMediaStorageConfigurationOutputTypeDef = TypedDict(
+    "DescribeMediaStorageConfigurationOutputTypeDef",
+    {
+        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
+    "UpdateMediaStorageConfigurationInputRequestTypeDef",
+    {
+        "ChannelARN": str,
+        "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
+    },
+)
+
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamInfo": StreamInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -674,23 +775,14 @@
 )
 
 class ImageGenerationConfigurationTypeDef(
     _RequiredImageGenerationConfigurationTypeDef, _OptionalImageGenerationConfigurationTypeDef
 ):
     pass
 
-ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    {
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo.egg-info/PKG-INFO` & `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.26.28
-Summary: Type annotations for boto3.KinesisVideo 1.26.28 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.33
+Summary: Type annotations for boto3.KinesisVideo 1.26.33 service generated with mypy-boto3-builder 7.12.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisvideo?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.26.33](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -279,20 +279,27 @@
 `mypy_boto3_kinesisvideo.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kinesisvideo import KinesisVideoClient
-from mypy_boto3_kinesisvideo.paginator import ListSignalingChannelsPaginator, ListStreamsPaginator
+from mypy_boto3_kinesisvideo.paginator import (
+    DescribeMappedResourceConfigurationPaginator,
+    ListSignalingChannelsPaginator,
+    ListStreamsPaginator,
+)
 
 client: KinesisVideoClient = Session().client("kinesisvideo")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = (
+    client.get_paginator("describe_mapped_resource_configuration")
+)
 list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator(
     "list_signaling_channels"
 )
 list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
 ```
 
 <a id="literals"></a>
@@ -306,19 +313,21 @@
 from mypy_boto3_kinesisvideo.literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ComparisonOperatorType,
     ConfigurationStatusType,
+    DescribeMappedResourceConfigurationPaginatorName,
     FormatConfigKeyType,
     FormatType,
     ImageSelectorTypeType,
     ListSignalingChannelsPaginatorName,
     ListStreamsPaginatorName,
+    MediaStorageConfigurationStatusType,
     MediaUriTypeType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
     KinesisVideoServiceName,
     ServiceName,
@@ -347,23 +356,27 @@
     ResponseMetadataTypeDef,
     CreateStreamInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    DescribeMappedResourceConfigurationInputRequestTypeDef,
+    MappedResourceConfigurationListItemTypeDef,
+    DescribeMediaStorageConfigurationInputRequestTypeDef,
+    MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     GetDataEndpointInputRequestTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
     ImageGenerationDestinationConfigTypeDef,
-    PaginatorConfigTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForStreamInputRequestTypeDef,
     MediaSourceConfigTypeDef,
     NotificationDestinationConfigTypeDef,
     ScheduleConfigTypeDef,
     TagStreamInputRequestTypeDef,
@@ -378,20 +391,24 @@
     TagResourceInputRequestTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamOutputTypeDef,
     GetDataEndpointOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
+    DescribeMappedResourceConfigurationOutputTypeDef,
+    DescribeMediaStorageConfigurationOutputTypeDef,
+    UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
```

### Comparing `mypy-boto3-kinesisvideo-1.26.28/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt` & `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.26.28/setup.py` & `mypy-boto3-kinesisvideo-1.26.33/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-kinesisvideo",
-    version="1.26.28",
+    version="1.26.33",
     packages=["mypy_boto3_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideo 1.26.28 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.KinesisVideo 1.26.33 service generated with mypy-boto3-builder"
         " 7.12.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

