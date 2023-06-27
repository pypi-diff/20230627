# Comparing `tmp/types-Flask-Cors-3.0.9.tar.gz` & `tmp/types-Flask-Cors-4.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Flask-Cors-3.0.9.tar", last modified: Thu Jul  7 12:38:39 2022, max compression
+gzip compressed data, was "types-Flask-Cors-4.0.0.0.tar", last modified: Tue Jun 27 01:42:56 2023, max compression
```

## Comparing `types-Flask-Cors-3.0.9.tar` & `types-Flask-Cors-4.0.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 12:38:39.560135 types-Flask-Cors-3.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-07-07 12:38:38.000000 types-Flask-Cors-3.0.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-07 12:38:38.000000 types-Flask-Cors-3.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-07-07 12:38:39.560135 types-Flask-Cors-3.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 12:38:39.560135 types-Flask-Cors-3.0.9/flask_cors-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-07 12:38:38.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-07-07 12:38:30.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2711 2022-07-07 12:38:30.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-07 12:38:30.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-07-07 12:38:30.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-07 12:38:30.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-07 12:38:39.560135 types-Flask-Cors-3.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-07-07 12:38:38.000000 types-Flask-Cors-3.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 12:38:39.560135 types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-07-07 12:38:39.000000 types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-07-07 12:38:39.000000 types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-07 12:38:39.000000 types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-07 12:38:39.000000 types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:42:56.813929 types-Flask-Cors-4.0.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-27 01:42:55.000000 types-Flask-Cors-4.0.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 01:42:55.000000 types-Flask-Cors-4.0.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-27 01:42:56.813929 types-Flask-Cors-4.0.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:42:56.813929 types-Flask-Cors-4.0.0.0/flask_cors-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-27 01:42:55.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 01:42:44.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-27 01:42:44.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-27 01:42:44.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-27 01:42:44.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 01:42:44.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 01:42:56.813929 types-Flask-Cors-4.0.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-27 01:42:55.000000 types-Flask-Cors-4.0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:42:56.813929 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-27 01:42:56.000000 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-27 01:42:56.000000 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 01:42:56.000000 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 01:42:56.000000 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 01:42:56.000000 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/top_level.txt
```

### Comparing `types-Flask-Cors-3.0.9/PKG-INFO` & `types-Flask-Cors-4.0.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: types-Flask-Cors
-Version: 3.0.9
+Version: 4.0.0.0
 Summary: Typing stubs for Flask-Cors
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for Flask-Cors
 
-This is a PEP 561 type stub package for the `Flask-Cors` package.
-It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
-that uses `Flask-Cors`. The source for this package can be found at
-https://github.com/python/typeshed/tree/master/stubs/Flask-Cors. All fixes for
+This is a PEP 561 type stub package for the `Flask-Cors` package. It
+can be used by type-checking tools like
+[mypy](https://github.com/python/mypy/),
+[pyright](https://github.com/microsoft/pyright),
+[pytype](https://github.com/google/pytype/),
+PyCharm, etc. to check code that uses
+`Flask-Cors`. The source for this package can be found at
+https://github.com/python/typeshed/tree/main/stubs/Flask-Cors. All fixes for
 types and metadata should be contributed there.
 
-See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `9ccf4589a0cc8f0c5a8cc2c07c485da6d7118767`.
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
 
 
+See https://github.com/python/typeshed/blob/main/README.md for more details.
+This package was generated from typeshed commit `b8ab395d4bafd6352560e74b636744d49a9bcd6e` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
+pytype 2023.6.2.
```

### Comparing `types-Flask-Cors-3.0.9/flask_cors-stubs/core.pyi` & `types-Flask-Cors-4.0.0.0/flask_cors-stubs/core.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from collections.abc import Iterable
 from datetime import timedelta
 from logging import Logger
-from typing import Any, Pattern, TypeVar, overload
+from re import Pattern
+from typing import Any, TypeVar, overload
 from typing_extensions import TypeAlias, TypedDict
 
+import flask
+
 _IterableT = TypeVar("_IterableT", bound=Iterable[Any])
 _T = TypeVar("_T")
-_App: TypeAlias = Any  # flask is not part of typeshed
-_Response: TypeAlias = Any  # flask is not part of typeshed
 _MultiDict: TypeAlias = Any  # werkzeug is not part of typeshed
 
 class _Options(TypedDict, total=False):
     resources: dict[str, dict[str, Any]] | list[str] | str | None
     origins: str | list[str] | None
     methods: str | list[str] | None
     expose_headers: str | list[str] | None
@@ -40,23 +41,23 @@
 DEFAULT_OPTIONS: _Options
 
 def parse_resources(resources: dict[str, _Options] | Iterable[str] | str | Pattern[str]) -> list[tuple[str, _Options]]: ...
 def get_regexp_pattern(regexp: str | Pattern[str]) -> str: ...
 def get_cors_origins(options: _Options, request_origin: str | None) -> list[str] | None: ...
 def get_allow_headers(options: _Options, acl_request_headers: str | None) -> str | None: ...
 def get_cors_headers(options: _Options, request_headers: dict[str, Any], request_method: str) -> _MultiDict: ...
-def set_cors_headers(resp: _Response, options: _Options) -> _Response: ...
+def set_cors_headers(resp: flask.Response, options: _Options) -> flask.Response: ...
 def probably_regex(maybe_regex: str | Pattern[str]) -> bool: ...
 def re_fix(reg: str) -> str: ...
 def try_match_any(inst: str, patterns: Iterable[str | Pattern[str]]) -> bool: ...
 def try_match(request_origin: str, maybe_regex: str | Pattern[str]) -> bool: ...
-def get_cors_options(appInstance: _App | None, *dicts: _Options) -> _Options: ...
-def get_app_kwarg_dict(appInstance: _App | None = ...) -> _Options: ...
+def get_cors_options(appInstance: flask.Flask | None, *dicts: _Options) -> _Options: ...
+def get_app_kwarg_dict(appInstance: flask.Flask | None = None) -> _Options: ...
 def flexible_str(obj: object) -> str | None: ...
-def serialize_option(options_dict: _Options, key: str, upper: bool = ...) -> None: ...
+def serialize_option(options_dict: _Options, key: str, upper: bool = False) -> None: ...
 @overload
 def ensure_iterable(inst: str) -> list[str]: ...  # type: ignore[misc]
 @overload
 def ensure_iterable(inst: _IterableT) -> _IterableT: ...
 @overload
 def ensure_iterable(inst: _T) -> list[_T]: ...
 def sanitize_regex_param(param: str | list[str]) -> list[str]: ...
```

### Comparing `types-Flask-Cors-3.0.9/flask_cors-stubs/decorator.pyi` & `types-Flask-Cors-4.0.0.0/flask_cors-stubs/decorator.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections.abc import Callable, Iterable
 from datetime import timedelta
 from logging import Logger
-from typing import Any, Pattern
+from re import Pattern
+from typing import Any
 from typing_extensions import ParamSpec
 
 _P = ParamSpec("_P")
 
 LOG: Logger
 
 def cross_origin(
```

### Comparing `types-Flask-Cors-3.0.9/flask_cors-stubs/extension.pyi` & `types-Flask-Cors-4.0.0.0/flask_cors-stubs/extension.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
+from _typeshed import Incomplete
 from collections.abc import Callable, Iterable
 from datetime import timedelta
 from logging import Logger
 from typing import Any
-from typing_extensions import TypeAlias
 
-_App: TypeAlias = Any  # flask is not part of typeshed
+import flask
 
 LOG: Logger
 
 class CORS:
     def __init__(
         self,
-        app: Any | None = ...,
+        app: Incomplete | None = None,
         *,
         resources: dict[str, dict[str, Any]] | list[str] | str | None = ...,
         origins: str | list[str] | None = ...,
         methods: str | list[str] | None = ...,
         expose_headers: str | list[str] | None = ...,
         allow_headers: str | list[str] | None = ...,
         supports_credentials: bool | None = ...,
         max_age: timedelta | int | str | None = ...,
         send_wildcard: bool | None = ...,
         vary_header: bool | None = ...,
         **kwargs: Any,
     ) -> None: ...
     def init_app(
         self,
-        app: _App,
+        app: flask.Flask,
         *,
         resources: dict[str, dict[str, Any]] | list[str] | str = ...,
         origins: str | list[str] = ...,
         methods: str | list[str] = ...,
         expose_headers: str | list[str] = ...,
         allow_headers: str | list[str] = ...,
         supports_credentials: bool = ...,
```

### Comparing `types-Flask-Cors-3.0.9/setup.py` & `types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-from setuptools import setup
+Metadata-Version: 2.1
+Name: types-Flask-Cors
+Version: 4.0.0.0
+Summary: Typing stubs for Flask-Cors
+Home-page: https://github.com/python/typeshed
+License: Apache-2.0 license
+Project-URL: GitHub, https://github.com/python/typeshed
+Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md
+Project-URL: Issue tracker, https://github.com/python/typeshed/issues
+Project-URL: Chat, https://gitter.im/python/typing
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Typing :: Stubs Only
+Description-Content-Type: text/markdown
 
-name = "types-Flask-Cors"
-description = "Typing stubs for Flask-Cors"
-long_description = '''
 ## Typing stubs for Flask-Cors
 
-This is a PEP 561 type stub package for the `Flask-Cors` package.
-It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
-that uses `Flask-Cors`. The source for this package can be found at
-https://github.com/python/typeshed/tree/master/stubs/Flask-Cors. All fixes for
+This is a PEP 561 type stub package for the `Flask-Cors` package. It
+can be used by type-checking tools like
+[mypy](https://github.com/python/mypy/),
+[pyright](https://github.com/microsoft/pyright),
+[pytype](https://github.com/google/pytype/),
+PyCharm, etc. to check code that uses
+`Flask-Cors`. The source for this package can be found at
+https://github.com/python/typeshed/tree/main/stubs/Flask-Cors. All fixes for
 types and metadata should be contributed there.
 
-See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `9ccf4589a0cc8f0c5a8cc2c07c485da6d7118767`.
-'''.lstrip()
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
 
-setup(name=name,
-      version="3.0.9",
-      description=description,
-      long_description=long_description,
-      long_description_content_type="text/markdown",
-      url="https://github.com/python/typeshed",
-      project_urls={
-          "GitHub": "https://github.com/python/typeshed",
-          "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md",
-          "Issue tracker": "https://github.com/python/typeshed/issues",
-          "Chat": "https://gitter.im/python/typing",
-      },
-      install_requires=[],
-      packages=['flask_cors-stubs'],
-      package_data={'flask_cors-stubs': ['__init__.pyi', 'core.pyi', 'decorator.pyi', 'extension.pyi', 'version.pyi', 'METADATA.toml']},
-      license="Apache-2.0 license",
-      classifiers=[
-          "License :: OSI Approved :: Apache Software License",
-          "Programming Language :: Python :: 3",
-          "Typing :: Stubs Only",
-      ]
-)
+
+See https://github.com/python/typeshed/blob/main/README.md for more details.
+This package was generated from typeshed commit `b8ab395d4bafd6352560e74b636744d49a9bcd6e` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
+pytype 2023.6.2.
```

