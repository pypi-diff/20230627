# Comparing `tmp/autopack_tools-0.1.3.tar.gz` & `tmp/autopack_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.1.3.tar", max compression
+gzip compressed data, was "autopack_tools-0.1.4.tar", max compression
```

## Comparing `autopack_tools-0.1.3.tar` & `autopack_tools-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.1.3/LICENSE
--rw-r--r--   0        0        0     2920 2023-06-25 23:21:07.938300 autopack_tools-0.1.3/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.1.3/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-25 23:21:01.956387 autopack_tools-0.1.3/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.1.3/autopack/__main__.py
--rw-r--r--   0        0        0     1427 2023-06-25 23:21:07.938595 autopack_tools-0.1.3/autopack/api.py
--rw-r--r--   0        0        0      864 2023-06-25 23:21:01.957129 autopack_tools-0.1.3/autopack/cli.py
--rw-r--r--   0        0        0      258 2023-06-25 23:21:01.957337 autopack_tools-0.1.3/autopack/errors.py
--rw-r--r--   0        0        0     4459 2023-06-25 23:21:01.957572 autopack_tools-0.1.3/autopack/get_pack.py
--rw-r--r--   0        0        0     2679 2023-06-25 23:21:01.957868 autopack_tools-0.1.3/autopack/installation.py
--rw-r--r--   0        0        0      883 2023-06-25 23:23:14.408748 autopack_tools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3576 1970-01-01 00:00:00.000000 autopack_tools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2920 2023-06-25 23:21:07.938300 autopack_tools-0.1.4/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.1.4/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-25 23:21:01.956387 autopack_tools-0.1.4/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.1.4/autopack/__main__.py
+-rw-r--r--   0        0        0     2245 2023-06-26 23:28:38.418992 autopack_tools-0.1.4/autopack/api.py
+-rw-r--r--   0        0        0      864 2023-06-25 23:21:01.957129 autopack_tools-0.1.4/autopack/cli.py
+-rw-r--r--   0        0        0      258 2023-06-25 23:21:01.957337 autopack_tools-0.1.4/autopack/errors.py
+-rw-r--r--   0        0        0     4729 2023-06-26 23:45:40.137477 autopack_tools-0.1.4/autopack/get_pack.py
+-rw-r--r--   0        0        0     2780 2023-06-26 23:38:47.664538 autopack_tools-0.1.4/autopack/installation.py
+-rw-r--r--   0        0        0      951 2023-06-26 23:46:16.871143 autopack_tools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 autopack_tools-0.1.4/PKG-INFO
```

### Comparing `autopack_tools-0.1.3/LICENSE` & `autopack_tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.3/README.md` & `autopack_tools-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.3/autopack/api.py` & `autopack_tools-0.1.4/autopack/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import requests
 from dataclasses_json import dataclass_json
 from marshmallow import ValidationError
 
 from autopack.errors import AutoPackFetchError
 
-API_URL = os.environ.get("API_URL", "https://autopack.ai")
+API_URL = os.environ.get("API_URL", "https://autopack.ai/")
 
 
 @dataclass_json
 @dataclass
 class PackResponse:
     pack_id: str
     author: str
@@ -22,19 +22,20 @@
     description: str
     name: str
     dependencies: list[str]
     source: str
     arguments: dict[str, Any]
 
     def pack_path(self) -> str:
-        return f"{self.author}-{self.repository}-{self.name}"
+        return f"{self.author}_{self.repository}_{self.name}".replace("-", "_")
 
 
-def get_pack_data(pack_id: str) -> Union[PackResponse, None]:
-    endpoint = "/packs/get"
+def get_pack_details(pack_id: str) -> Union[PackResponse, None]:
+    endpoint = "/api/details"
+
     url = urljoin(API_URL, endpoint)
     params = {"id": pack_id}
 
     response = requests.get(url, params=params)
     if response.status_code == 200:
         data = response.json()
 
@@ -48,7 +49,32 @@
     elif response.status_code <= 500:
         print(f"Error: {response.status_code}")
         return None
     else:
         print(f"Error: {response.status_code}")
         error_message = f"Error: {response.status_code}"
         raise AutoPackFetchError(error_message)
+
+
+def pack_search(query: str) -> list[PackResponse]:
+    endpoint = "/api/search"
+    url = urljoin(API_URL, endpoint)
+    params = {"query": query}
+
+    response = requests.get(url, params=params)
+    if response.status_code == 200:
+        data = response.json()
+
+        try:
+            return [PackResponse(*datum) for datum in data]
+        except (ValidationError, TypeError) as e:
+            message = f"Pack fetch received invalid data: {e}"
+            print(message)
+            raise AutoPackFetchError(message)
+
+    elif response.status_code <= 500:
+        print(f"Error: {response.status_code}")
+        return []
+    else:
+        print(f"Error: {response.status_code}")
+        error_message = f"Error: {response.status_code}"
+        raise AutoPackFetchError(error_message)
```

### Comparing `autopack_tools-0.1.3/autopack/cli.py` & `autopack_tools-0.1.4/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.3/autopack/get_pack.py` & `autopack_tools-0.1.4/autopack/get_pack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 import importlib
 import inspect
 import os
 import sys
+from types import ModuleType
 from typing import Type, Union
 
-from autopack.api import PackResponse, get_pack_data
-from autopack.errors import (AutoPackError, AutoPackLoadError,
-                             AutoPackNotFoundError, AutoPackNotInstalledError)
+from autopack.api import PackResponse, get_pack_details
+from autopack.errors import AutoPackError, AutoPackLoadError, AutoPackNotFoundError, AutoPackNotInstalledError
 
 
-def try_get_pack(pack_id: str) -> Union[Type, None]:
+def try_get_pack(pack_id: str, quiet=False) -> Union[Type, None]:
     """
     Get a pack based on its ID, in `author/repo_name/pack_name` format. Same as `get_pack` but does not raise an
     Exception. If there is a problem finding or loading a pack it will return None.
 
     Args:
         pack_id (str): The ID of the pack to fetch.
+        quiet (bool, Optional): If True, won't print any output
 
     Returns:
         BaseTool or None: The fetched pack as a LangChain BaseTool object, None if the pack could not be loaded
     """
 
     try:
-        return get_pack(pack_id)
+        return get_pack(pack_id, quiet=quiet)
     except AutoPackError:
         return None
 
 
-def get_pack(pack_id: str) -> Type:
+def get_pack(pack_id: str, quiet=False) -> Type:
     """
     Get a pack based on its ID, in `author/repo_name/pack_name` format.
 
     Args:
         pack_id (str): The ID of the pack to fetch.
+        quiet (bool, Optional): If True, won't print any output
 
     Returns:
         BaseTool: The fetched pack as a LangChain BaseTool object
 
     Raises:
         AutoPackFetchError: If there was an error during the data fetch.
         AutoPackNotInstalledError: If the pack was found but not installed.
         AutoPackNotFoundError: If no pack matching that ID was found.
         AutoPackLoadError: If the pack was found but there was an error importing or finding the pack class.
     """
-    pack_data = get_pack_data(pack_id)
+    pack_data = get_pack_details(pack_id)
 
     if not pack_data:
         raise AutoPackNotFoundError()
 
-    return find_pack(pack_data)
+    return find_pack(pack_data, quiet=quiet)
 
 
-def find_module(module_path: str):
+def find_module(pack_data: PackResponse) -> ModuleType:
+    module_path = pack_data.module_path
+
+    # Just in case they already have it in their path for whatever reason
     try:
         return importlib.import_module(module_path)
-    except ModuleNotFoundError:
-        find_autopack_dir_and_add_to_sys_path()
-        return importlib.import_module(module_path)
+    except:
+        autopack_dir = find_or_create_autopack_dir()
+        sys.path.insert(0, autopack_dir)
 
+        try:
+            return importlib.import_module(pack_data.pack_path() + "." + module_path)
+        finally:
+            sys.path.remove(autopack_dir)
 
-def find_autopack_dir_and_add_to_sys_path(depth=0):
+
+def find_or_create_autopack_dir(depth=0) -> str:
     """Search in current and parent directories looking for .autopack"""
-    autopack_dir = os.path.abspath(
-        os.path.join(os.getcwd(), *[os.pardir] * depth, ".autopack")
-    )
+    autopack_dir = os.path.abspath(os.path.join(os.getcwd(), *[os.pardir] * depth, ".autopack"))
 
     if not os.path.exists(autopack_dir) or not os.path.isdir(autopack_dir):
         if depth > 3:
             raise ModuleNotFoundError(".autopack directory could not be found")
-        return find_autopack_dir_and_add_to_sys_path(depth=depth + 1)
-
-    sys.path.append(autopack_dir)
+        return find_or_create_autopack_dir(depth=depth + 1)
 
+    return autopack_dir
 
-def find_pack(pack_data: PackResponse) -> Type:
-    if pack_data.source == "git":
-        module_path = f"{pack_data.pack_path()}.{pack_data.module_path}"
-    else:
-        module_path = pack_data.module_path
 
+def find_pack(pack_data: PackResponse, quiet=False) -> Type:
     try:
-        module = find_module(module_path)
+        module = find_module(pack_data)
         if not module:
             message = (
                 f"Pack {pack_data.pack_id} could not be found. Either it is misconfigured or .autopack directory not "
                 f"found"
             )
             raise AutoPackNotFoundError(message)
 
         for _, obj in inspect.getmembers(module):
             if is_valid_pack(obj, pack_data.name):
                 return obj
 
-        message = (
-            f"Pack {pack_data.pack_id} found, but {pack_data.name} is not found in its module, "
-            f"{module_path}"
-        )
+        message = f"Pack {pack_data.pack_id} found, but {pack_data.name} is not found in its module"
         raise AutoPackNotFoundError(message)
     except ModuleNotFoundError:
-        message = f"Pack {pack_data.pack_id} is available but not installed. To install: autopack install {pack_data.pack_id}"
-        print(message)
+        message = (
+            f"Pack {pack_data.pack_id} is available but not installed. To install: autopack install {pack_data.pack_id}"
+        )
+        if not quiet:
+            print(message)
         raise AutoPackNotInstalledError(message)
     except (ImportError, AttributeError) as e:
         message = f"Error loading {pack_data.pack_id}: {e}"
-        print(message)
+        if not quiet:
+            print(message)
         raise AutoPackLoadError(message)
 
 
 def is_valid_pack(klass: Type, name: str):
     if not inspect.isclass(klass):
         return False
 
     base_class_names = [k.__name__ for k in klass.__bases__]
-    roughly_adheres_to_interface = (
-        hasattr(klass, "run") or "BaseTool" in base_class_names
-    )
+    roughly_adheres_to_interface = hasattr(klass, "run") or "BaseTool" in base_class_names
     if not roughly_adheres_to_interface:
         return False
 
     # Pack name is the class name
     if name == klass.__name__:
         return True
```

### Comparing `autopack_tools-0.1.3/autopack/installation.py` & `autopack_tools-0.1.4/autopack/installation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import importlib
 import os
 import subprocess
 
 from git import Repo
 
-from autopack.api import PackResponse, get_pack_data
+from autopack.api import PackResponse, get_pack_details
 from autopack.errors import AutoPackError
-from autopack.get_pack import get_pack, try_get_pack
+from autopack.get_pack import try_get_pack
 
 
 def is_dependency_installed(dependency: str) -> bool:
     try:
         importlib.import_module(dependency)
         return True
     except ImportError:
@@ -34,17 +34,15 @@
     for dependency in dependencies:
         if is_dependency_installed(dependency):
             continue
 
         if force:
             install_dependency(dependency)
         else:
-            print(
-                f"This pack requires the dependency {dependency} to be installed. Continue?"
-            )
+            print(f"This pack requires the dependency {dependency} to be installed. Continue?")
             agree = input("[Yn]")
             if agree.lower() == "y" or agree == "":
                 install_dependency(dependency)
             else:
                 print(f"Skipping install of {dependency}")
 
 
@@ -58,36 +56,39 @@
         print("Repo already exists, pulling updates")
         Repo(pack_path).remotes.origin.pull()
     else:
         print(f"Cloning repo into {pack_path}")
         Repo.clone_from(url, pack_path)
 
 
-def install_pack(pack_id, force_dependencies=False):
+def install_pack(pack_id: str, force_dependencies=False):
     print(f"Installing pack: {pack_id}")
+    os.makedirs(".autopack", exist_ok=True)
 
-    pack = try_get_pack(pack_id)
+    pack = try_get_pack(pack_id, quiet=True)
     if pack:
         print(f"Pack {pack_id} already installed.")
         return True
 
     try:
-        pack_data = get_pack_data(pack_id)
+        pack_data = get_pack_details(pack_id)
 
+        if not pack_data:
+            return False
         ask_to_install_dependencies(pack_data.dependencies, force_dependencies)
     except AutoPackError as e:
         # Maybe do something else
         print(f"Could not install pack {e}")
         return False
     except BaseException as e:
         print(f"Could not install pack {e}")
         return False
 
     if pack_data.source == "git":
         install_from_git(pack_data)
 
-    pack = get_pack(pack_id)
+    pack = try_get_pack(pack_id, quiet=True)
     if pack:
         return True
 
-    print("Installation completed but pack could still not be found.")
+    print("Error: Installation completed but pack could still not be found.")
     return False
```

### Comparing `autopack_tools-0.1.3/pyproject.toml` & `autopack_tools-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.1.3"
+version = "0.1.4"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
 
 [tool.poetry.scripts]
 autopack = 'autopack.cli:main'
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.10.3"
 requests = "^2.31.0"
 dataclasses-json = "^0.5.8"
 urllib3 = "^1.26.16"
 gitpython = "^3.1.31"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
@@ -28,11 +28,14 @@
 pytest-mock = "^3.11.1"
 types-requests = "^2.31.0.1"
 psycopg2 = "^2.9.6"
 docopt = "^0.6.2"
 autoflake = "^2.2.0"
 types-psycopg2 = "^2.9.21.10"
 types-docopt = "^0.6.11.3"
+langchain = "^0.0.215"
+pipreqs = "^0.4.13"
+gitpython = "^3.1.31"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autopack_tools-0.1.3/PKG-INFO` & `autopack_tools-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10.3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.8,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
```

