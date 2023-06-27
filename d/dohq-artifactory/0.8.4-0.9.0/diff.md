# Comparing `tmp/dohq-artifactory-0.8.4.tar.gz` & `tmp/dohq-artifactory-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/artifactory/artifactory/dist/.tmp-iyun88af/dohq-artifactory-0.8.4.tar", last modified: Tue Dec  6 04:31:00 2022, max compression
+gzip compressed data, was "/home/runner/work/artifactory/artifactory/dist/.tmp-kteu74_p/dohq-artifactory-0.9.0.tar", last modified: Tue Jun 27 06:46:02 2023, max compression
```

## Comparing `dohq-artifactory-0.8.4.tar` & `dohq-artifactory-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-06 04:30:50.000000 dohq-artifactory-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 04:30:50.000000 dohq-artifactory-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      974 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43943 2022-12-06 04:30:50.000000 dohq-artifactory-0.8.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    87301 2022-12-06 04:30:50.000000 dohq-artifactory-0.8.4/artifactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/dohq_artifactory/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-06 04:30:50.000000 dohq-artifactory-0.8.4/dohq_artifactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47514 2022-12-06 04:30:50.000000 dohq-artifactory-0.8.4/dohq_artifactory/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2022-12-06 04:30:50.000000 dohq-artifactory-0.8.4/dohq_artifactory/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-12-06 04:30:50.000000 dohq-artifactory-0.8.4/dohq_artifactory/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-06 04:30:50.000000 dohq-artifactory-0.8.4/dohq_artifactory/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/dohq_artifactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/dohq_artifactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/dohq_artifactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/dohq_artifactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/dohq_artifactory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/dohq_artifactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/dohq_artifactory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-06 04:31:00.000000 dohq-artifactory-0.8.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1910 2022-12-06 04:30:50.000000 dohq-artifactory-0.8.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-06 04:30:53.000000 dohq-artifactory-0.8.4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-27 06:45:48.000000 dohq-artifactory-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 06:45:48.000000 dohq-artifactory-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    44027 2023-06-27 06:45:48.000000 dohq-artifactory-0.9.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    89900 2023-06-27 06:45:48.000000 dohq-artifactory-0.9.0/artifactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/dohq_artifactory/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 06:45:48.000000 dohq-artifactory-0.9.0/dohq_artifactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47514 2023-06-27 06:45:48.000000 dohq-artifactory-0.9.0/dohq_artifactory/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-27 06:45:48.000000 dohq-artifactory-0.9.0/dohq_artifactory/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-27 06:45:48.000000 dohq-artifactory-0.9.0/dohq_artifactory/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-27 06:45:48.000000 dohq-artifactory-0.9.0/dohq_artifactory/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/dohq_artifactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/dohq_artifactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/dohq_artifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/dohq_artifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/dohq_artifactory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/dohq_artifactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/dohq_artifactory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 06:46:02.000000 dohq-artifactory-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2036 2023-06-27 06:45:48.000000 dohq-artifactory-0.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 06:45:56.000000 dohq-artifactory-0.9.0/version.txt
```

### Comparing `dohq-artifactory-0.8.4/LICENSE` & `dohq-artifactory-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dohq-artifactory-0.8.4/PKG-INFO` & `dohq-artifactory-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dohq-artifactory
-Version: 0.8.4
+Version: 0.9.0
 Summary: A Python interface to Artifactory
 Home-page: https://devopshq.github.io/artifactory/
 Download-URL: https://github.com/devopshq/artifactory
 Author: Alexey Burov
 Author-email: aburov@ptsecurity.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,11 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
+Provides-Extra: tests
 License-File: LICENSE
 
 See full documentation here: https://devopshq.github.io/artifactory/
```

### Comparing `dohq-artifactory-0.8.4/README.md` & `dohq-artifactory-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1405,18 +1405,18 @@
     "http://my-artifactory/artifactory/myrepo/restricted-path", apikey="MY_API_KEY"
 )
 ```
 
 
 ## Global Configuration File ##
 
-Artifactory Python module also can specify all connection-related settings in a central file, 
-```~/.artifactory_python.cfg``` that is read upon the creation of first ```ArtifactoryPath``` object and is stored 
-globally. For instance, you can specify per-instance settings of authentication tokens, so that you won't need to 
-explicitly pass ```auth``` parameter to ```ArtifactoryPath```.
+Artifactory Python module also can specify all connection-related settings in a central file, given by environment
+variable ```$DOHQ_ARTIFACTORY_PYTHON_CFG``` (default if not set: ```~/.artifactory_python.cfg```) that is read upon
+the creation of first ```ArtifactoryPath``` object and is stored globally. For instance, you can specify per-instance
+settings of authentication tokens, so that you won't need to explicitly pass ```auth``` parameter to ```ArtifactoryPath```.
 
 Example:
 
 ```ini
 [DEFAULT]
 username = nameforallinstances
```

### Comparing `dohq-artifactory-0.8.4/artifactory.py` & `dohq-artifactory-0.9.0/artifactory.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 import os
 import pathlib
 import platform
 import re
 import sys
 import urllib.parse
 from itertools import islice
+from warnings import warn
 
 import dateutil.parser
 import requests
 
 from dohq_artifactory.admin import Group
 from dohq_artifactory.admin import PermissionTarget
 from dohq_artifactory.admin import Project
@@ -59,17 +60,20 @@
 except ImportError:
     import urllib3
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 
-default_config_path = "~/.artifactory_python.cfg"
-if platform.system() == "Windows":
+if "DOHQ_ARTIFACTORY_PYTHON_CFG" in os.environ:
+    default_config_path = os.environ["DOHQ_ARTIFACTORY_PYTHON_CFG"]
+elif platform.system() == "Windows":
     default_config_path = "~\\.artifactory_python.cfg"
+else:
+    default_config_path = "~/.artifactory_python.cfg"
 global_config = None
 
 
 def read_config(config_path=default_config_path):
     """
     Read configuration file and produce a dictionary of the following structure:
 
@@ -311,29 +315,39 @@
     def __len__(self):
         """
         __len__ will be used by requests to determine stream size
         """
         return int(self.getheader("content-length"))
 
 
-def encode_matrix_parameters(parameters):
+def encode_matrix_parameters(parameters, quote_parameters):
     """
     Performs encoding of url matrix parameters from dictionary to
     a string.
     See http://www.w3.org/DesignIssues/MatrixURIs.html for specs.
+    If quote_parameters is true, then apply URL quoting to the values and the parameter names.
     """
     result = []
 
     for param in iter(sorted(parameters)):
-        if isinstance(parameters[param], (list, tuple)):
-            value = f";{param}=".join(parameters[param])
+        raw_value = parameters[param]
+
+        resolved_param = urllib.parse.quote(param) if quote_parameters else param
+
+        if isinstance(raw_value, (list, tuple)):
+            values = (
+                [urllib.parse.quote(v) for v in raw_value]
+                if quote_parameters
+                else raw_value
+            )
+            value = f";{resolved_param}=".join(values)
         else:
-            value = parameters[param]
+            value = urllib.parse.quote(raw_value) if quote_parameters else raw_value
 
-        result.append("=".join((param, value)))
+        result.append("=".join((resolved_param, value)))
 
     return ";".join(result)
 
 
 def escape_chars(s):
     """
     Performs character escaping of comma, pipe and equals characters
@@ -1127,14 +1141,15 @@
         sha1=None,
         sha256=None,
         parameters=None,
         explode_archive=None,
         explode_archive_atomic=None,
         checksum=None,
         by_checksum=False,
+        quote_parameters=None,  # TODO: v0.10.0: change default to True
     ):
         """
         Uploads a given file-like object
         HTTP chunked encoding will be attempted
 
         If by_checksum is True, fobj should be None
 
@@ -1144,26 +1159,38 @@
         :param sha1: (str) SHA1 checksum value
         :param sha256: (str) SHA256 checksum value
         :param parameters: Artifact properties
         :param explode_archive: (bool) if True, archive will be exploded upon deployment
         :param explode_archive_atomic: (bool) if True, archive will be exploded in an atomic operation upon deployment
         :param checksum: sha1Value or sha256Value
         :param by_checksum: (bool) if True, deploy artifact by checksum, default False
+        :param quote_parameters: (bool) if True, apply URL quoting to matrix parameter names and values,
+            default False until v0.10.0
         """
 
+        if quote_parameters is None:
+            warn(
+                "The current default value of quote_parameters (False) will change to True in v0.10.0.\n"
+                "To ensure consistent behavior and remove this warning, explicitly set a value for quote_parameters.\n"
+                "For more details see https://github.com/devopshq/artifactory/issues/408."
+            )
+            quote_parameters = False
+
         if fobj and by_checksum:
             raise ArtifactoryException("Either fobj or by_checksum, but not both")
 
         if isinstance(fobj, urllib3.response.HTTPResponse):
             fobj = HTTPResponseWrapper(fobj)
 
         url = str(pathobj)
 
         matrix_parameters = (
-            f";{encode_matrix_parameters(parameters)}" if parameters else None
+            f";{encode_matrix_parameters(parameters, quote_parameters=quote_parameters)}"
+            if parameters
+            else None
         )
         headers = {}
 
         if md5:
             headers["X-Checksum-Md5"] = md5
         if sha1:
             headers["X-Checksum-Sha1"] = sha1
@@ -1786,15 +1813,19 @@
         :param data (bytes): Data to be written to file
         """
         md5 = hashlib.md5(data).hexdigest()
         sha1 = hashlib.sha1(data).hexdigest()
         sha256 = hashlib.sha256(data).hexdigest()
 
         fobj = io.BytesIO(data)
-        self.deploy(fobj, md5=md5, sha1=sha1, sha256=sha256)
+        self.deploy(fobj, md5=md5, sha1=sha1, sha256=sha256, quote_parameters=False)
+        # TODO: v0.10.0 - possibly remove quote_parameters explicit setting
+        # Because this call never has parameters, it should not matter what it's set to.
+        # In this version, we set it explicitly to avoid the warning.
+        # In 0.10.0 or later, we can either keep it explicitly set to False, or remove it entirely.
         return len(data)
 
     def write_text(self, data, encoding="utf-8", errors="strict"):
         """
         Write file content as text
         :param data (str): Text to be written to file
         """
@@ -1931,38 +1962,41 @@
         fobj,
         md5=None,
         sha1=None,
         sha256=None,
         parameters={},
         explode_archive=None,
         explode_archive_atomic=None,
+        quote_parameters=None,
     ):
         """
         Upload the given file object to this path
         """
         return self._accessor.deploy(
             self,
             fobj,
             md5=md5,
             sha1=sha1,
             sha256=sha256,
             parameters=parameters,
             explode_archive=explode_archive,
             explode_archive_atomic=explode_archive_atomic,
+            quote_parameters=quote_parameters,
         )
 
     def deploy_file(
         self,
         file_name,
         calc_md5=True,
         calc_sha1=True,
         calc_sha256=True,
         parameters={},
         explode_archive=False,
         explode_archive_atomic=False,
+        quote_parameters=None,
     ):
         """
         Upload the given file to this path
         """
         md5 = md5sum(file_name) if calc_md5 else None
         sha1 = sha1sum(file_name) if calc_sha1 else None
         sha256 = sha256sum(file_name) if calc_sha256 else None
@@ -1977,22 +2011,24 @@
                 fobj,
                 md5=md5,
                 sha1=sha1,
                 sha256=sha256,
                 parameters=parameters,
                 explode_archive=explode_archive,
                 explode_archive_atomic=explode_archive_atomic,
+                quote_parameters=quote_parameters,
             )
 
     def deploy_by_checksum(
         self,
         sha1=None,
         sha256=None,
         checksum=None,
         parameters={},
+        quote_parameters=None,
     ):
         """
         Deploy an artifact to the specified destination by checking if the
         artifact content already exists in Artifactory.
 
         :param pathobj: ArtifactoryPath object
         :param sha1: sha1Value
@@ -2003,37 +2039,47 @@
             self,
             fobj=None,
             sha1=sha1,
             sha256=sha256,
             checksum=checksum,
             by_checksum=True,
             parameters=parameters,
+            quote_parameters=quote_parameters,
         )
 
     def deploy_deb(
-        self, file_name, distribution, component, architecture, parameters={}
+        self,
+        file_name,
+        distribution,
+        component,
+        architecture,
+        parameters={},
+        quote_parameters=None,
     ):
         """
         Convenience method to deploy .deb packages
 
         Keyword arguments:
         file_name -- full path to local file that will be deployed
         distribution -- debian distribution (e.g. 'wheezy')
         component -- repository component (e.g. 'main')
         architecture -- package architecture (e.g. 'i386')
         parameters -- attach any additional metadata
+        quote_parameters -- URL quote parameter values and names
         """
         params = {
             "deb.distribution": distribution,
             "deb.component": component,
             "deb.architecture": architecture,
         }
         params.update(parameters)
 
-        self.deploy_file(file_name, parameters=params)
+        self.deploy_file(
+            file_name, parameters=params, quote_parameters=quote_parameters
+        )
 
     def copy(self, dst, suppress_layouts=False, fail_fast=False, dry_run=False):
         """
         Copy artifact from this path to destination.
         If files are on the same instance of artifactory, lightweight (local)
         copying will be attempted.
 
@@ -2103,15 +2149,25 @@
             if dry_run:
                 logger.debug(
                     "Artifactory drive is different. Will do a standard upload"
                 )
                 return
 
             with self.open() as fobj:
-                dst.deploy(fobj, md5=stat.md5, sha1=stat.sha1, sha256=stat.sha256)
+                dst.deploy(
+                    fobj,
+                    md5=stat.md5,
+                    sha1=stat.sha1,
+                    sha256=stat.sha256,
+                    quote_parameters=False,
+                )
+                # TODO: v0.10.0 - possibly remove quote_parameters explicit setting
+                # Because this call never has parameters, it should not matter what it's set to.
+                # In this version, we set it explicitly to avoid the warning.
+                # In 0.10.0 or later, we can either keep it explicitly set to False, or remove it entirely.
 
     def move(self, dst, suppress_layouts=False, fail_fast=False, dry_run=False):
         """
         Move artifact from this path to destination.
 
         The suppress_layouts parameter, when set to True, will allow artifacts
         from one path to be moved directly into another path without enforcing
```

### Comparing `dohq-artifactory-0.8.4/dohq_artifactory/admin.py` & `dohq-artifactory-0.9.0/dohq_artifactory/admin.py`

 * *Files identical despite different names*

### Comparing `dohq-artifactory-0.8.4/dohq_artifactory/auth.py` & `dohq-artifactory-0.9.0/dohq_artifactory/auth.py`

 * *Files identical despite different names*

### Comparing `dohq-artifactory-0.8.4/dohq_artifactory/exception.py` & `dohq-artifactory-0.9.0/dohq_artifactory/exception.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     try:
         response.raise_for_status()
     except requests.HTTPError as exception:
         # start processing HTTP error and try to extract meaningful data from it
         try:
             response_json = exception.response.json()
             error_list = response_json.pop("errors", None)
-        except requests.compat.JSONDecodeError:
+        except (requests.compat.JSONDecodeError, requests.exceptions.JSONDecodeError):
             # not a JSON response
             raise ArtifactoryException(str(exception)) from exception
 
         if not isinstance(error_list, list) or not error_list:
             # no standard error list in the exception
             raise ArtifactoryException(str(exception)) from exception
```

### Comparing `dohq-artifactory-0.8.4/dohq_artifactory.egg-info/PKG-INFO` & `dohq-artifactory-0.9.0/dohq_artifactory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dohq-artifactory
-Version: 0.8.4
+Version: 0.9.0
 Summary: A Python interface to Artifactory
 Home-page: https://devopshq.github.io/artifactory/
 Download-URL: https://github.com/devopshq/artifactory
 Author: Alexey Burov
 Author-email: aburov@ptsecurity.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,11 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
+Provides-Extra: tests
 License-File: LICENSE
 
 See full documentation here: https://devopshq.github.io/artifactory/
```

### Comparing `dohq-artifactory-0.8.4/setup.py` & `dohq-artifactory-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 if "alpha" in __version__:
     dev_status = "3 - Alpha"
 elif "dev" in __version__:
     dev_status = "4 - Beta"
 else:
     dev_status = "5 - Production/Stable"
 
+tests_require = ["pytest>=7.0.0", "responses>=0.23.1", "mock", "flake8"]
 
 setup(
     name="dohq-artifactory",
     version=__version__,
     py_modules=["artifactory"],
     license="MIT License",
     description="A Python interface to Artifactory",
@@ -48,15 +49,16 @@
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries",
         "Topic :: System :: Filesystems",
     ],
     url="https://devopshq.github.io/artifactory/",
     download_url="https://github.com/devopshq/artifactory",
     install_requires=[
-        "requests",
+        "requests>=2.30.0",
         "python-dateutil",
         "PyJWT~=2.0",
     ],
+    extras_require={"tests": tests_require},
     zip_safe=False,
     package_data={"": ["README.md"]},
     packages=["dohq_artifactory"],
 )
```

