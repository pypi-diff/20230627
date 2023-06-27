# Comparing `tmp/nonebot_plugin_songpicker2-0.2.4.tar.gz` & `tmp/nonebot_plugin_songpicker2-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_songpicker2-0.2.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_songpicker2-0.2.5.tar", max compression
```

## Comparing `nonebot_plugin_songpicker2-0.2.4.tar` & `nonebot_plugin_songpicker2-0.2.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35148 2023-06-26 15:32:50.796663 nonebot_plugin_songpicker2-0.2.4/LICENSE
--rw-r--r--   0        0        0     2151 2023-06-26 15:36:22.932663 nonebot_plugin_songpicker2-0.2.4/nonebot_plugin_songpicker2/__init__.py
--rwxr-xr-x   0        0        0     5524 2023-06-26 15:32:50.796663 nonebot_plugin_songpicker2-0.2.4/nonebot_plugin_songpicker2/data_source.py
--rw-r--r--   0        0        0      559 2023-06-26 15:42:36.352663 nonebot_plugin_songpicker2-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 nonebot_plugin_songpicker2-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-26 15:32:50.796663 nonebot_plugin_songpicker2-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2175 2023-06-27 08:34:01.498803 nonebot_plugin_songpicker2-0.2.5/nonebot_plugin_songpicker2/__init__.py
+-rwxr-xr-x   0        0        0     5524 2023-06-26 15:32:50.796663 nonebot_plugin_songpicker2-0.2.5/nonebot_plugin_songpicker2/data_source.py
+-rw-r--r--   0        0        0      559 2023-06-27 08:34:32.878803 nonebot_plugin_songpicker2-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 nonebot_plugin_songpicker2-0.2.5/PKG-INFO
```

### Comparing `nonebot_plugin_songpicker2-0.2.4/LICENSE` & `nonebot_plugin_songpicker2-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_songpicker2-0.2.4/nonebot_plugin_songpicker2/__init__.py` & `nonebot_plugin_songpicker2-0.2.5/nonebot_plugin_songpicker2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .data_source import DataGet, DataProcess
 
 __plugin_meta__ = PluginMetadata(
     name="songpicker2",
     description="点播歌曲，支持候选菜单、热评显示，数据源为网易云",
     usage="点歌吧大概",
+    type="application",
     extra={},
 )
 
 songpicker = on_command("点歌")
 
 dataGet = DataGet()
```

### Comparing `nonebot_plugin_songpicker2-0.2.4/nonebot_plugin_songpicker2/data_source.py` & `nonebot_plugin_songpicker2-0.2.5/nonebot_plugin_songpicker2/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_songpicker2-0.2.4/pyproject.toml` & `nonebot_plugin_songpicker2-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_songpicker2"
-version = "0.2.4"
+version = "0.2.5"
 description = "点播歌曲，支持候选菜单、热评显示，数据源为网易云"
 authors = ["Maximilian Wu <me@maxng.cc>"]
 repository = "https://github.com/maxesisn/nonebot_plugin_songpicker2"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0"
```

### Comparing `nonebot_plugin_songpicker2-0.2.4/PKG-INFO` & `nonebot_plugin_songpicker2-0.2.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-songpicker2
-Version: 0.2.4
+Version: 0.2.5
 Summary: 点播歌曲，支持候选菜单、热评显示，数据源为网易云
 Home-page: https://github.com/maxesisn/nonebot_plugin_songpicker2
 Author: Maximilian Wu
 Author-email: me@maxng.cc
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

