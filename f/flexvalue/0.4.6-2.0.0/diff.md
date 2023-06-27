# Comparing `tmp/flexvalue-0.4.6.tar.gz` & `tmp/flexvalue-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexvalue-0.4.6.tar", last modified: Mon Oct  3 18:47:44 2022, max compression
+gzip compressed data, was "flexvalue-2.0.0.tar", last modified: Tue Jun 27 21:40:40 2023, max compression
```

## Comparing `flexvalue-0.4.6.tar` & `flexvalue-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 18:47:44.861620 flexvalue-0.4.6/
--rw-r--r--   0 root         (0) root         (0)      644 2022-10-03 18:47:44.861620 flexvalue-0.4.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    13635 2022-03-02 19:25:22.000000 flexvalue-0.4.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 18:47:44.857620 flexvalue-0.4.6/flexvalue/
--rw-rw-r--   0 root         (0) root         (0)     1221 2021-11-30 19:20:02.000000 flexvalue-0.4.6/flexvalue/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      984 2022-10-03 18:45:31.000000 flexvalue-0.4.6/flexvalue/__version__.py
--rw-rw-r--   0 root         (0) root         (0)    28710 2022-10-03 17:58:51.000000 flexvalue-0.4.6/flexvalue/calculations.py
--rw-rw-r--   0 root         (0) root         (0)    14642 2021-11-30 19:20:02.000000 flexvalue-0.4.6/flexvalue/cet_flexvalue_compare.py
--rw-rw-r--   0 root         (0) root         (0)    10124 2022-05-02 14:18:46.000000 flexvalue-0.4.6/flexvalue/cli.py
--rw-rw-r--   0 root         (0) root         (0)     7394 2022-05-02 14:18:46.000000 flexvalue-0.4.6/flexvalue/db.py
--rw-rw-r--   0 root         (0) root         (0)     3440 2022-03-02 19:25:22.000000 flexvalue-0.4.6/flexvalue/examples.py
--rw-rw-r--   0 root         (0) root         (0)    36982 2022-05-02 14:18:46.000000 flexvalue-0.4.6/flexvalue/plots.py
--rw-rw-r--   0 root         (0) root         (0)     2198 2021-11-30 19:20:02.000000 flexvalue-0.4.6/flexvalue/report.py
--rw-rw-r--   0 root         (0) root         (0)     1446 2022-10-03 18:02:56.000000 flexvalue-0.4.6/flexvalue/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 18:47:44.861620 flexvalue-0.4.6/flexvalue.egg-info/
--rw-r--r--   0 root         (0) root         (0)      644 2022-10-03 18:47:44.000000 flexvalue-0.4.6/flexvalue.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2022-10-03 18:47:44.000000 flexvalue-0.4.6/flexvalue.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-03 18:47:44.000000 flexvalue-0.4.6/flexvalue.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-10-03 18:47:44.000000 flexvalue-0.4.6/flexvalue.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      168 2022-10-03 18:47:44.000000 flexvalue-0.4.6/flexvalue.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-10-03 18:47:44.000000 flexvalue-0.4.6/flexvalue.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       63 2022-10-03 18:47:44.861620 flexvalue-0.4.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3169 2022-10-03 18:24:00.000000 flexvalue-0.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 21:40:40.858255 flexvalue-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-27 21:40:40.858255 flexvalue-2.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    30648 2023-06-27 21:15:27.000000 flexvalue-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 21:40:40.858255 flexvalue-2.0.0/flexvalue/
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-06-27 21:15:27.000000 flexvalue-2.0.0/flexvalue/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      984 2023-06-27 21:21:05.000000 flexvalue-2.0.0/flexvalue/__version__.py
+-rw-rw-r--   0 root         (0) root         (0)    14642 2023-01-19 00:54:27.000000 flexvalue-2.0.0/flexvalue/cet_flexvalue_compare.py
+-rw-rw-r--   0 root         (0) root         (0)    10248 2023-06-27 21:15:27.000000 flexvalue-2.0.0/flexvalue/cli.py
+-rw-rw-r--   0 root         (0) root         (0)     6030 2023-06-27 21:15:27.000000 flexvalue-2.0.0/flexvalue/config.py
+-rw-rw-r--   0 root         (0) root         (0)    50275 2023-06-27 21:15:27.000000 flexvalue-2.0.0/flexvalue/db.py
+-rw-rw-r--   0 root         (0) root         (0)     3440 2023-01-19 00:54:27.000000 flexvalue-2.0.0/flexvalue/examples.py
+-rw-rw-r--   0 root         (0) root         (0)     3152 2023-06-27 21:15:27.000000 flexvalue-2.0.0/flexvalue/flexvalue.py
+-rw-rw-r--   0 root         (0) root         (0)     2198 2023-01-31 00:43:43.000000 flexvalue-2.0.0/flexvalue/report.py
+-rw-rw-r--   0 root         (0) root         (0)     1446 2023-01-19 00:54:27.000000 flexvalue-2.0.0/flexvalue/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 21:40:40.858255 flexvalue-2.0.0/flexvalue.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-27 21:40:40.000000 flexvalue-2.0.0/flexvalue.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-27 21:40:40.000000 flexvalue-2.0.0/flexvalue.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 21:40:40.000000 flexvalue-2.0.0/flexvalue.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-27 21:40:40.000000 flexvalue-2.0.0/flexvalue.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-27 21:40:40.000000 flexvalue-2.0.0/flexvalue.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-27 21:40:40.000000 flexvalue-2.0.0/flexvalue.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       63 2023-06-27 21:40:40.862255 flexvalue-2.0.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3336 2023-06-27 21:15:27.000000 flexvalue-2.0.0/setup.py
```

### Comparing `flexvalue-0.4.6/PKG-INFO` & `flexvalue-2.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: flexvalue
-Version: 0.4.6
+Version: 2.0.0
 Summary: FLEXvalue: a tool for calculating avoided costs
 Home-page: http://github.com/recurve-methods/flexvalue
 Author: Recurve Analytics, Inc.
 Author-email: support@recurve.com
 License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `flexvalue-0.4.6/flexvalue/__init__.py` & `flexvalue-2.0.0/flexvalue/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,26 +14,26 @@
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 """
 
-import logging
+# import logging
+import flexvalue.flexvalue
+# from .__version__ import __title__, __description__, __url__, __version__
+# from .__version__ import __author__, __author_email__, __license__
+# from .__version__ import __copyright__
+# #from .calculations import FlexValueProject, FlexValueRun
+# # from .plots import plot_results
+# # from .db import (
+# #     get_all_valid_deer_load_shapes,
+# #     get_all_valid_utility_climate_zone_combinations,
+# # )
 
-from .__version__ import __title__, __description__, __url__, __version__
-from .__version__ import __author__, __author_email__, __license__
-from .__version__ import __copyright__
-from .calculations import FlexValueProject, FlexValueRun
-from .plots import plot_results
-from .db import (
-    get_all_valid_deer_load_shapes,
-    get_all_valid_utility_climate_zone_combinations,
-)
 
+# def get_version():
+#     return __version__
 
-def get_version():
-    return __version__
 
-
-# Set default logging handler to avoid "No handler found" warnings.
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+# # Set default logging handler to avoid "No handler found" warnings.
+# logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `flexvalue-0.4.6/flexvalue/__version__.py` & `flexvalue-2.0.0/flexvalue/__version__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,12 +16,12 @@
    See the License for the specific language governing permissions and
    limitations under the License.
 
 """
 __title__ = "FLEXvalue"
 __description__ = "FLEXvalue: a tool for calculating avoided costs"
 __url__ = "http://github.com/recurve-methods/flexvalue"
-__version__ = "0.4.6"
+__version__ = "2.0.0"
 __author__ = "Recurve Analytics, Inc."
 __author_email__ = "support@recurve.com"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright 2021 Recurve Analytics, Inc."
```

### Comparing `flexvalue-0.4.6/flexvalue/cet_flexvalue_compare.py` & `flexvalue-2.0.0/flexvalue/cet_flexvalue_compare.py`

 * *Files identical despite different names*

### Comparing `flexvalue-0.4.6/flexvalue/examples.py` & `flexvalue-2.0.0/flexvalue/examples.py`

 * *Files identical despite different names*

### Comparing `flexvalue-0.4.6/flexvalue/report.py` & `flexvalue-2.0.0/flexvalue/report.py`

 * *Files identical despite different names*

### Comparing `flexvalue-0.4.6/flexvalue/settings.py` & `flexvalue-2.0.0/flexvalue/settings.py`

 * *Files identical despite different names*

### Comparing `flexvalue-0.4.6/flexvalue.egg-info/PKG-INFO` & `flexvalue-2.0.0/flexvalue.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: flexvalue
-Version: 0.4.6
+Version: 2.0.0
 Summary: FLEXvalue: a tool for calculating avoided costs
 Home-page: http://github.com/recurve-methods/flexvalue
 Author: Recurve Analytics, Inc.
 Author-email: support@recurve.com
 License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `flexvalue-0.4.6/setup.py` & `flexvalue-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,34 +18,39 @@
 
 """
 # This setup.py inspired by https://github.com/kennethreitz/setup.py
 
 # Note: To use the 'upload' functionality of this file, you must:
 #   $ pip install twine
 
-import io
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 NAME = "flexvalue"
+
+# TODO: fix psycopg-binary; use correct dependency for distributing
 INSTALL_REQUIRES = [
     "click==8.0.3",
+    "toml==0.10.2",
     "pandas==1.3.4",
     "statsmodels==0.13.1",
     "scipy==1.7.2",
     "seaborn==0.11.2",
-    "sqlalchemy<1.4.0",
+    "sqlalchemy==2.0",
     "nbformat==5.1.3",
     "nbconvert==6.3.0",
     "jinja2==3.0.3",
     "matplotlib<3.6",
     "numpy<1.23.0",
+    "psycopg[binary]==3.1.8",
+    "google-cloud-bigquery==3.6.0",
+    "db-dtypes>=1.0.5"
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Load the package's __version__.py module as a dictionary.
 about = {}
 with open(os.path.join(here, NAME, "__version__.py")) as f:
```

