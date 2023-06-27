# Comparing `tmp/types-WebOb-1.8.0.0.tar.gz` & `tmp/types-WebOb-1.8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-WebOb-1.8.0.0.tar", last modified: Sun Jun 18 15:13:37 2023, max compression
+gzip compressed data, was "types-WebOb-1.8.0.1.tar", last modified: Tue Jun 27 15:17:32 2023, max compression
```

## Comparing `types-WebOb-1.8.0.0.tar` & `types-WebOb-1.8.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:13:37.153332 types-WebOb-1.8.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-18 15:13:34.000000 types-WebOb-1.8.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 15:13:34.000000 types-WebOb-1.8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-18 15:13:37.153332 types-WebOb-1.8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 15:13:37.153332 types-WebOb-1.8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-18 15:13:34.000000 types-WebOb-1.8.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:13:37.153332 types-WebOb-1.8.0.0/types_WebOb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-18 15:13:37.000000 types-WebOb-1.8.0.0/types_WebOb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-18 15:13:37.000000 types-WebOb-1.8.0.0/types_WebOb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:13:37.000000 types-WebOb-1.8.0.0/types_WebOb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 15:13:37.000000 types-WebOb-1.8.0.0/types_WebOb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:13:37.153332 types-WebOb-1.8.0.0/webob-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 15:13:34.000000 types-WebOb-1.8.0.0/webob-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/acceptparse.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/byterange.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/cachecontrol.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/datetime_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/dec.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/descriptors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/etag.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/exc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/headers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/multidict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/static.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-18 15:13:24.000000 types-WebOb-1.8.0.0/webob-stubs/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:17:32.712819 types-WebOb-1.8.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-27 15:17:29.000000 types-WebOb-1.8.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 15:17:29.000000 types-WebOb-1.8.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-27 15:17:32.712819 types-WebOb-1.8.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:17:32.712819 types-WebOb-1.8.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-27 15:17:29.000000 types-WebOb-1.8.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:17:32.708819 types-WebOb-1.8.0.1/types_WebOb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-27 15:17:32.000000 types-WebOb-1.8.0.1/types_WebOb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-27 15:17:32.000000 types-WebOb-1.8.0.1/types_WebOb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:17:32.000000 types-WebOb-1.8.0.1/types_WebOb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 15:17:32.000000 types-WebOb-1.8.0.1/types_WebOb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:17:32.712819 types-WebOb-1.8.0.1/webob-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 15:17:29.000000 types-WebOb-1.8.0.1/webob-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/acceptparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/byterange.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/cachecontrol.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/datetime_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/dec.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/descriptors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/etag.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/exc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/headers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/multidict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 15:17:13.000000 types-WebOb-1.8.0.1/webob-stubs/util.pyi
```

### Comparing `types-WebOb-1.8.0.0/PKG-INFO` & `types-WebOb-1.8.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-WebOb
-Version: 1.8.0.0
+Version: 1.8.0.1
 Summary: Typing stubs for WebOb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/WebOb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `WebOb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/WebOb. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `df795220a376ae9371afdc60dbf160392b93b6c2` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
+This package was generated from typeshed commit `93b4060cd4a6bd45a48fc70c16adc4a69edc9114` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
 pytype 2023.6.2.
```

### Comparing `types-WebOb-1.8.0.0/setup.py` & `types-WebOb-1.8.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `WebOb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/WebOb. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `df795220a376ae9371afdc60dbf160392b93b6c2` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
+This package was generated from typeshed commit `93b4060cd4a6bd45a48fc70c16adc4a69edc9114` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
 pytype 2023.6.2.
 '''.lstrip()
 
 setup(name=name,
-      version="1.8.0.0",
+      version="1.8.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/WebOb.md",
```

### Comparing `types-WebOb-1.8.0.0/types_WebOb.egg-info/PKG-INFO` & `types-WebOb-1.8.0.1/types_WebOb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-WebOb
-Version: 1.8.0.0
+Version: 1.8.0.1
 Summary: Typing stubs for WebOb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/WebOb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `WebOb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/WebOb. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `df795220a376ae9371afdc60dbf160392b93b6c2` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
+This package was generated from typeshed commit `93b4060cd4a6bd45a48fc70c16adc4a69edc9114` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
 pytype 2023.6.2.
```

### Comparing `types-WebOb-1.8.0.0/types_WebOb.egg-info/SOURCES.txt` & `types-WebOb-1.8.0.1/types_WebOb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/acceptparse.pyi` & `types-WebOb-1.8.0.1/webob-stubs/acceptparse.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/byterange.pyi` & `types-WebOb-1.8.0.1/webob-stubs/byterange.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/cachecontrol.pyi` & `types-WebOb-1.8.0.1/webob-stubs/cachecontrol.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/client.pyi` & `types-WebOb-1.8.0.1/webob-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/cookies.pyi` & `types-WebOb-1.8.0.1/webob-stubs/cookies.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/datetime_utils.pyi` & `types-WebOb-1.8.0.1/webob-stubs/datetime_utils.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/dec.pyi` & `types-WebOb-1.8.0.1/webob-stubs/dec.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/descriptors.pyi` & `types-WebOb-1.8.0.1/webob-stubs/descriptors.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/etag.pyi` & `types-WebOb-1.8.0.1/webob-stubs/etag.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/exc.pyi` & `types-WebOb-1.8.0.1/webob-stubs/exc.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/headers.pyi` & `types-WebOb-1.8.0.1/webob-stubs/headers.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/multidict.pyi` & `types-WebOb-1.8.0.1/webob-stubs/multidict.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def view_list(cls, lst: list[tuple[_KT, _VT]]) -> MultiDict[_KT, _VT]: ...
     @classmethod
     def from_fieldstorage(cls, fs: FieldStorage) -> MultiDict[str, str | FieldStorage]: ...
     def __getitem__(self, key: _KT) -> _VT: ...
     def __setitem__(self, key: _KT, value: _VT) -> None: ...
     def add(self, key: _KT, value: _VT) -> None: ...
     @overload
-    def get(self, key: _KT) -> _VT: ...
+    def get(self, key: _KT) -> _VT | None: ...
     @overload
     def get(self, key: _KT, default: _T) -> _VT | _T: ...
     def getall(self, key: _KT) -> list[_VT]: ...
     def getone(self, key: _KT) -> _VT: ...
     def mixed(self) -> dict[_KT, _VT | list[_VT]]: ...
     def dict_of_lists(self) -> dict[_KT, list[_VT]]: ...
     def __delitem__(self, key: _KT) -> None: ...
```

### Comparing `types-WebOb-1.8.0.0/webob-stubs/request.pyi` & `types-WebOb-1.8.0.1/webob-stubs/request.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/response.pyi` & `types-WebOb-1.8.0.1/webob-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `types-WebOb-1.8.0.0/webob-stubs/static.pyi` & `types-WebOb-1.8.0.1/webob-stubs/static.pyi`

 * *Files identical despite different names*

