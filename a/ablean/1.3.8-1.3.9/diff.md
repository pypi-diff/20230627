# Comparing `tmp/ablean-1.3.8.tar.gz` & `tmp/ablean-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablean-1.3.8.tar", last modified: Tue Jun 27 01:25:05 2023, max compression
+gzip compressed data, was "ablean-1.3.9.tar", last modified: Tue Jun 27 02:30:53 2023, max compression
```

## Comparing `ablean-1.3.8.tar` & `ablean-1.3.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.309051 ablean-1.3.8/
--rw-rw-rw-   0        0        0     2184 2022-06-06 10:43:40.000000 ablean-1.3.8/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.257661 ablean-1.3.8/.vscode/
--rw-rw-rw-   0        0        0     1442 2023-04-20 14:13:20.000000 ablean-1.3.8/.vscode/launch.json
--rw-rw-rw-   0        0        0    55778 2023-06-27 01:25:05.309051 ablean-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    53240 2022-06-05 03:11:14.000000 ablean-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.263335 ablean-1.3.8/ablean/
--rw-rw-rw-   0        0        0      930 2023-06-26 09:01:52.000000 ablean-1.3.8/ablean/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.284410 ablean-1.3.8/ablean/commands/
--rw-rw-rw-   0        0        0     1273 2022-06-06 09:45:38.000000 ablean-1.3.8/ablean/commands/__init__.py
--rw-rw-rw-   0        0        0    12597 2023-06-21 04:52:15.000000 ablean-1.3.8/ablean/commands/backtest.py
--rw-rw-rw-   0        0        0    11132 2023-06-26 09:01:36.000000 ablean-1.3.8/ablean/commands/create_project.py
--rw-rw-rw-   0        0        0     1322 2022-06-10 02:17:02.000000 ablean-1.3.8/ablean/commands/download.py
--rw-rw-rw-   0        0        0     2098 2022-06-06 10:41:51.000000 ablean-1.3.8/ablean/commands/init.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.286463 ablean-1.3.8/ablean/components/
--rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.292185 ablean-1.3.8/ablean/components/config/
--rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/config/__init__.py
--rw-rw-rw-   0        0        0     2786 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/config/cli_config_manager.py
--rw-rw-rw-   0        0        0    14072 2023-06-21 01:14:02.000000 ablean-1.3.8/ablean/components/config/lean_config_manager.py
--rw-rw-rw-   0        0        0     5417 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/config/output_config_manager.py
--rw-rw-rw-   0        0        0     2435 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/config/project_config_manager.py
--rw-rw-rw-   0        0        0     3279 2022-06-05 07:48:48.000000 ablean-1.3.8/ablean/components/config/storage.py
--rw-rw-rw-   0        0        0     5080 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/lean_runner.py
--rw-rw-rw-   0        0        0     2787 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/module_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.299835 ablean-1.3.8/ablean/components/util/
--rw-rw-rw-   0        0        0      676 2022-06-05 08:19:14.000000 ablean-1.3.8/ablean/components/util/__init__.py
--rw-rw-rw-   0        0        0     6356 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/logger.py
--rw-rw-rw-   0        0        0     1368 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/name_extraction.py
--rw-rw-rw-   0        0        0     3205 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/name_generator.py
--rw-rw-rw-   0        0        0     3261 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/path_manager.py
--rw-rw-rw-   0        0        0     4584 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/platform_manager.py
--rw-rw-rw-   0        0        0    21926 2022-06-05 04:02:32.000000 ablean-1.3.8/ablean/components/util/project_manager.py
--rw-rw-rw-   0        0        0     1689 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/temp_manager.py
--rw-rw-rw-   0        0        0     1680 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/xml_manager.py
--rw-rw-rw-   0        0        0     4485 2023-06-21 00:58:59.000000 ablean-1.3.8/ablean/constants.py
--rw-rw-rw-   0        0        0     3838 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/container.py
--rw-rw-rw-   0        0        0     8436 2022-06-22 06:13:42.000000 ablean-1.3.8/ablean/data_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.301080 ablean-1.3.8/ablean/icons/
--rw-rw-rw-   0        0        0    34808 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/icons/icon.icns
--rw-rw-rw-   0        0        0    14816 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/icons/icon.ico
--rw-rw-rw-   0        0        0     5968 2022-06-06 09:47:56.000000 ablean-1.3.8/ablean/main.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.307067 ablean-1.3.8/ablean/models/
--rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/__init__.py
--rw-rw-rw-   0        0        0     2305 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/errors.py
--rw-rw-rw-   0        0        0     1555 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/modules.py
--rw-rw-rw-   0        0        0     4037 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/options.py
--rw-rw-rw-   0        0        0     1507 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/pydantic.py
--rw-rw-rw-   0        0        0     1456 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/utils.py
--rw-rw-rw-   0        0        0     9966 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/myclick.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.279923 ablean-1.3.8/ablean.egg-info/
--rw-rw-rw-   0        0        0    55778 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1428 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      302 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      920 2023-06-22 13:16:53.000000 ablean-1.3.8/pub.ps1
-drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.308049 ablean-1.3.8/scripts/
--rw-rw-rw-   0        0        0     3900 2022-06-05 03:31:44.000000 ablean-1.3.8/scripts/readme.py
--rw-rw-rw-   0        0        0       42 2023-06-27 01:25:05.310049 ablean-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     3443 2022-06-05 05:42:03.000000 ablean-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.536448 ablean-1.3.9/
+-rw-rw-rw-   0        0        0     2184 2022-06-06 10:43:40.000000 ablean-1.3.9/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.482575 ablean-1.3.9/.vscode/
+-rw-rw-rw-   0        0        0     1491 2023-06-27 02:08:37.000000 ablean-1.3.9/.vscode/launch.json
+-rw-rw-rw-   0        0        0    55778 2023-06-27 02:30:53.535448 ablean-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    53240 2022-06-05 03:11:14.000000 ablean-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.486574 ablean-1.3.9/ablean/
+-rw-rw-rw-   0        0        0      930 2023-06-27 02:30:24.000000 ablean-1.3.9/ablean/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.512268 ablean-1.3.9/ablean/commands/
+-rw-rw-rw-   0        0        0     1273 2022-06-06 09:45:38.000000 ablean-1.3.9/ablean/commands/__init__.py
+-rw-rw-rw-   0        0        0    12597 2023-06-21 04:52:15.000000 ablean-1.3.9/ablean/commands/backtest.py
+-rw-rw-rw-   0        0        0    10673 2023-06-27 02:17:54.000000 ablean-1.3.9/ablean/commands/create_project.py
+-rw-rw-rw-   0        0        0     1322 2022-06-10 02:17:02.000000 ablean-1.3.9/ablean/commands/download.py
+-rw-rw-rw-   0        0        0     2098 2022-06-06 10:41:51.000000 ablean-1.3.9/ablean/commands/init.py
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.513314 ablean-1.3.9/ablean/components/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.518860 ablean-1.3.9/ablean/components/config/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/config/__init__.py
+-rw-rw-rw-   0        0        0     2786 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/config/cli_config_manager.py
+-rw-rw-rw-   0        0        0    14059 2023-06-27 01:51:39.000000 ablean-1.3.9/ablean/components/config/lean_config_manager.py
+-rw-rw-rw-   0        0        0     5417 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/config/output_config_manager.py
+-rw-rw-rw-   0        0        0     2435 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/config/project_config_manager.py
+-rw-rw-rw-   0        0        0     3279 2023-06-27 01:46:04.000000 ablean-1.3.9/ablean/components/config/storage.py
+-rw-rw-rw-   0        0        0     5080 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/lean_runner.py
+-rw-rw-rw-   0        0        0     2787 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/module_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.526630 ablean-1.3.9/ablean/components/util/
+-rw-rw-rw-   0        0        0      676 2022-06-05 08:19:14.000000 ablean-1.3.9/ablean/components/util/__init__.py
+-rw-rw-rw-   0        0        0     6356 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/util/logger.py
+-rw-rw-rw-   0        0        0     1368 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/util/name_extraction.py
+-rw-rw-rw-   0        0        0     3205 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/util/name_generator.py
+-rw-rw-rw-   0        0        0     3261 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/util/path_manager.py
+-rw-rw-rw-   0        0        0     4584 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/util/platform_manager.py
+-rw-rw-rw-   0        0        0    21926 2022-06-05 04:02:32.000000 ablean-1.3.9/ablean/components/util/project_manager.py
+-rw-rw-rw-   0        0        0     1689 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/util/temp_manager.py
+-rw-rw-rw-   0        0        0     1680 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/components/util/xml_manager.py
+-rw-rw-rw-   0        0        0     4485 2023-06-21 00:58:59.000000 ablean-1.3.9/ablean/constants.py
+-rw-rw-rw-   0        0        0     3838 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/container.py
+-rw-rw-rw-   0        0        0     8436 2022-06-22 06:13:42.000000 ablean-1.3.9/ablean/data_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.527996 ablean-1.3.9/ablean/icons/
+-rw-rw-rw-   0        0        0    34808 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/icons/icon.icns
+-rw-rw-rw-   0        0        0    14816 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/icons/icon.ico
+-rw-rw-rw-   0        0        0     5968 2022-06-06 09:47:56.000000 ablean-1.3.9/ablean/main.py
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.533442 ablean-1.3.9/ablean/models/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/models/__init__.py
+-rw-rw-rw-   0        0        0     2305 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/models/errors.py
+-rw-rw-rw-   0        0        0     1555 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/models/modules.py
+-rw-rw-rw-   0        0        0     4037 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/models/options.py
+-rw-rw-rw-   0        0        0     1507 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/models/pydantic.py
+-rw-rw-rw-   0        0        0     1456 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/models/utils.py
+-rw-rw-rw-   0        0        0     9966 2022-06-05 03:11:14.000000 ablean-1.3.9/ablean/myclick.py
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.508079 ablean-1.3.9/ablean.egg-info/
+-rw-rw-rw-   0        0        0    55778 2023-06-27 02:30:53.000000 ablean-1.3.9/ablean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1428 2023-06-27 02:30:53.000000 ablean-1.3.9/ablean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 02:30:53.000000 ablean-1.3.9/ablean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-27 02:30:53.000000 ablean-1.3.9/ablean.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      302 2023-06-27 02:30:53.000000 ablean-1.3.9/ablean.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 02:30:53.000000 ablean-1.3.9/ablean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      920 2023-06-22 13:16:53.000000 ablean-1.3.9/pub.ps1
+drwxrwxrwx   0        0        0        0 2023-06-27 02:30:53.534448 ablean-1.3.9/scripts/
+-rw-rw-rw-   0        0        0     3900 2022-06-05 03:31:44.000000 ablean-1.3.9/scripts/readme.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 02:30:53.536448 ablean-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     3443 2022-06-05 05:42:03.000000 ablean-1.3.9/setup.py
```

### Comparing `ablean-1.3.8/.gitignore` & `ablean-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/.vscode/launch.json` & `ablean-1.3.9/.vscode/launch.json`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,21 @@
         {
             "name": "ablean",
             "type": "python",
             "request": "launch",
             "program": "${workspaceFolder}${pathSeparator}ablean${pathSeparator}main.py",
             "args": [
                 // "init",
-                "backtest",
+                // "backtest",
+                "create-project", "demo2"
                 // "download",
                 // "--market", "deribit"
                 // "--date-start", "2022-06-03",
                 // "--date-end", "2022-06-04",
-                "c:/work/repos/lean/demo1/deribit_backtest.py",
+                // "c:/work/repos/lean/demo1/deribit_backtest.py",
                 // "--download-data",
                 // "--debug",
                 // "-h", "119.8.180.153",
                 // "-u", "data_sync",
                 // "-w", "5@peksync"
             ],
             "cwd": "${workspaceFolder}/temp",
```

### Comparing `ablean-1.3.8/PKG-INFO` & `ablean-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablean
-Version: 1.3.8
+Version: 1.3.9
 Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
 Home-page: https://lean.io/cli
 Author: abl
 Author-email: support@quantconnect.com
 Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
 Project-URL: Source, https://github.com/QuantConnect/lean-cli
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ablean-1.3.8/README.md` & `ablean-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/__init__.py` & `ablean-1.3.9/ablean/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # The version is always set to "dev" in the Git repository. When a new release is ready,
 # a maintainer will push a new Git tag which will trigger GitHub Actions to publish a new
 # package to PyPI with the version of the tag.
-__version__ = "1.3.8"
+__version__ = "1.3.9"
```

### Comparing `ablean-1.3.8/ablean/commands/__init__.py` & `ablean-1.3.9/ablean/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/commands/backtest.py` & `ablean-1.3.9/ablean/commands/backtest.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/commands/create_project.py` & `ablean-1.3.9/ablean/commands/create_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,39 +68,31 @@
 )
 
 DEFAULT_PYTHON_NOTEBOOK = (
     """
 {
     "cells": [
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "![QuantConnect Logo](https://cdn.quantconnect.com/web/i/icon.png)\\n",
-                "<hr>"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "%run \"#LEAN_ROOT_PATH#/launcher/start.py\""
+                "%run \\"#LEAN_ROOT_PATH#/launcher/start.py\\""
             ]
         },        
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# QuantBook Analysis Tool\\n",
                 "# For more information see https://www.quantconnect.com/docs/research/overview\\n",
-                "from AlgorithmImports import *\\n"
+                "from AlgorithmImports import *\\n",
                 "qb = QuantBook()\\n",
                 "spy = qb.AddEquity(\\"SPY\\")\\n",
                 "history = qb.History(qb.Securities.Keys, 360, Resolution.Daily)\\n",
                 "\\n",
                 "# Indicator Analysis\\n",
                 "ema = qb.Indicator(ExponentialMovingAverage(10), spy.Symbol, 360, Resolution.Daily)\\n",
                 "ema.plot()"
@@ -206,22 +198,14 @@
 )
 
 DEFAULT_CSHARP_NOTEBOOK = (
     """
 {
     "cells": [
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "![QuantConnect Logo](https://cdn.quantconnect.com/web/i/icon.png)\\n",
-                "<hr>"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "// We need to load assemblies at the start in their own cell\\n",
                 "#load \\"../Initialize.csx\\""
@@ -349,15 +333,15 @@
         file.write(
             main_content.replace("$CLASS_NAME$", class_name).replace(
                 "$PROJECT_NAME$", full_path.name
             )
         )
 
     with (full_path / "research.ipynb").open("w+", encoding="utf-8") as file:
-        content = DEFAULT_PYTHON_NOTEBOOK.replace("#LEAN_ROOT_PATH#", cli_root)
+        content = DEFAULT_PYTHON_NOTEBOOK.replace("#LEAN_ROOT_PATH#", str(cli_root).replace('\\', '/'))
         file.write(content if language == "python" else DEFAULT_CSHARP_NOTEBOOK)
 
     if language == "python":
         pandas_mapper = cli_root / "launcher" / "PandasMapper.py"
         shutil.copyfile(pandas_mapper, full_path / "PandasMapper.py")
 
     logger = container.logger()
```

### Comparing `ablean-1.3.8/ablean/commands/download.py` & `ablean-1.3.9/ablean/commands/download.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/commands/init.py` & `ablean-1.3.9/ablean/commands/init.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/__init__.py` & `ablean-1.3.9/ablean/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/config/__init__.py` & `ablean-1.3.9/ablean/components/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/config/cli_config_manager.py` & `ablean-1.3.9/ablean/components/config/cli_config_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/config/lean_config_manager.py` & `ablean-1.3.9/ablean/components/config/lean_config_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
         if self._lean_config_path is not None:
             return self._lean_config_path
 
         # Recurse upwards in the directory tree until we find a Lean config file
         list = self.get_search_paths()
         for current_dir in list:
-            target_file = os.path.join(current_dir, DEFAULT_LEAN_CONFIG_FILE_NAME)
+            target_file = current_dir / DEFAULT_LEAN_CONFIG_FILE_NAME
             if target_file.exists():
                 self._lean_config_path = target_file
                 self.store_known_lean_config_path(self._lean_config_path)
                 return self._lean_config_path
             
         raise MoreInfoError(
             f"'{DEFAULT_LEAN_CONFIG_FILE_NAME}' not found",
```

### Comparing `ablean-1.3.8/ablean/components/config/output_config_manager.py` & `ablean-1.3.9/ablean/components/config/output_config_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/config/project_config_manager.py` & `ablean-1.3.9/ablean/components/config/project_config_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/config/storage.py` & `ablean-1.3.9/ablean/components/config/storage.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/lean_runner.py` & `ablean-1.3.9/ablean/components/lean_runner.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/module_manager.py` & `ablean-1.3.9/ablean/components/module_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/util/__init__.py` & `ablean-1.3.9/ablean/components/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/util/logger.py` & `ablean-1.3.9/ablean/components/util/logger.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/util/name_extraction.py` & `ablean-1.3.9/ablean/components/util/name_extraction.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/util/name_generator.py` & `ablean-1.3.9/ablean/components/util/name_generator.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/util/path_manager.py` & `ablean-1.3.9/ablean/components/util/path_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/util/platform_manager.py` & `ablean-1.3.9/ablean/components/util/platform_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/util/project_manager.py` & `ablean-1.3.9/ablean/components/util/project_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/util/temp_manager.py` & `ablean-1.3.9/ablean/components/util/temp_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/components/util/xml_manager.py` & `ablean-1.3.9/ablean/components/util/xml_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/constants.py` & `ablean-1.3.9/ablean/constants.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/container.py` & `ablean-1.3.9/ablean/container.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/data_manager.py` & `ablean-1.3.9/ablean/data_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/icons/icon.icns` & `ablean-1.3.9/ablean/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/icons/icon.ico` & `ablean-1.3.9/ablean/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/main.py` & `ablean-1.3.9/ablean/main.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/models/__init__.py` & `ablean-1.3.9/ablean/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/models/errors.py` & `ablean-1.3.9/ablean/models/errors.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/models/modules.py` & `ablean-1.3.9/ablean/models/modules.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/models/options.py` & `ablean-1.3.9/ablean/models/options.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/models/pydantic.py` & `ablean-1.3.9/ablean/models/pydantic.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/models/utils.py` & `ablean-1.3.9/ablean/models/utils.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean/myclick.py` & `ablean-1.3.9/ablean/myclick.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/ablean.egg-info/PKG-INFO` & `ablean-1.3.9/ablean.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablean
-Version: 1.3.8
+Version: 1.3.9
 Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
 Home-page: https://lean.io/cli
 Author: abl
 Author-email: support@quantconnect.com
 Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
 Project-URL: Source, https://github.com/QuantConnect/lean-cli
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ablean-1.3.8/ablean.egg-info/SOURCES.txt` & `ablean-1.3.9/ablean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/pub.ps1` & `ablean-1.3.9/pub.ps1`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/scripts/readme.py` & `ablean-1.3.9/scripts/readme.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.8/setup.py` & `ablean-1.3.9/setup.py`

 * *Files identical despite different names*

