# Comparing `tmp/micado-client-0.12.1.tar.gz` & `tmp/micado-client-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micado-client-0.12.1.tar", last modified: Sun Jun 11 08:42:12 2023, max compression
+gzip compressed data, was "micado-client-0.12.2.tar", last modified: Tue Jun 27 10:09:03 2023, max compression
```

## Comparing `micado-client-0.12.1.tar` & `micado-client-0.12.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.840510 micado-client-0.12.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 08:41:56.000000 micado-client-0.12.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-11 08:42:12.840510 micado-client-0.12.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-11 08:41:56.000000 micado-client-0.12.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.832509 micado-client-0.12.1/micado/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.832509 micado-client-0.12.1/micado/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/api/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.832509 micado-client-0.12.1/micado/installer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/installer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.832509 micado-client-0.12.1/micado/installer/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/installer/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/installer/ansible/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/installer/ansible/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.832509 micado-client-0.12.1/micado/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.836509 micado-client-0.12.1/micado/launcher/cloudbroker/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/cloudbroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/cloudbroker/cloudbroker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.836509 micado-client-0.12.1/micado/launcher/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/openstack/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/launcher/openstack/openstack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.836509 micado-client-0.12.1/micado/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/models/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/models/micado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.836509 micado-client-0.12.1/micado/types/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/types/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/types/micado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.836509 micado-client-0.12.1/micado/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-11 08:41:56.000000 micado-client-0.12.1/micado/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.840510 micado-client-0.12.1/micado_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 08:42:12.000000 micado-client-0.12.1/micado_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 08:42:12.840510 micado-client-0.12.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-11 08:41:56.000000 micado-client-0.12.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 08:42:12.840510 micado-client-0.12.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-11 08:41:56.000000 micado-client-0.12.1/tests/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.234766 micado-client-0.12.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 10:08:49.000000 micado-client-0.12.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-27 10:09:03.230766 micado-client-0.12.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-27 10:08:49.000000 micado-client-0.12.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.226766 micado-client-0.12.2/micado/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.226766 micado-client-0.12.2/micado/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/api/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.226766 micado-client-0.12.2/micado/installer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/installer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.226766 micado-client-0.12.2/micado/installer/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/installer/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/installer/ansible/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/installer/ansible/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.230766 micado-client-0.12.2/micado/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/launcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.230766 micado-client-0.12.2/micado/launcher/cloudbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/launcher/cloudbroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/launcher/cloudbroker/cloudbroker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.230766 micado-client-0.12.2/micado/launcher/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/launcher/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/launcher/openstack/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/launcher/openstack/openstack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.230766 micado-client-0.12.2/micado/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/models/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/models/micado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.230766 micado-client-0.12.2/micado/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/types/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/types/micado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.230766 micado-client-0.12.2/micado/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-27 10:08:49.000000 micado-client-0.12.2/micado/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.230766 micado-client-0.12.2/micado_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-27 10:09:03.000000 micado-client-0.12.2/micado_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-27 10:09:03.000000 micado-client-0.12.2/micado_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:09:03.000000 micado-client-0.12.2/micado_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-27 10:09:03.000000 micado-client-0.12.2/micado_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-27 10:09:03.000000 micado-client-0.12.2/micado_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 10:09:03.000000 micado-client-0.12.2/micado_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 10:09:03.234766 micado-client-0.12.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-27 10:08:49.000000 micado-client-0.12.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:03.230766 micado-client-0.12.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-27 10:08:49.000000 micado-client-0.12.2/tests/test_auth.py
```

### Comparing `micado-client-0.12.1/LICENSE` & `micado-client-0.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/PKG-INFO` & `micado-client-0.12.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micado-client
-Version: 0.12.1
+Version: 0.12.2
 Summary: A Python Client Library for MiCADO
 Home-page: https://github.com/micado-scale/micado-client
 Author: Márk Emődi & Jay DesLauriers
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/micado-scale/micado-client/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `micado-client-0.12.1/micado/api/application.py` & `micado-client-0.12.2/micado/api/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 
 Low-level methods for managing applications in MiCADO
 
 """
+import json
+
 from micado.types import ApplicationInfo
 from micado.exceptions import detailed_raise_for_status
 
 class ApplicationMixin:
     def applications(self):
         """Lists the currently running applications
 
@@ -62,16 +64,21 @@
         if app_id:
             url = self._url(f"/applications/{app_id}/")
         else:
             url = self._url("/applications/")
 
         json_data = ApplicationInfo(adt, url, params, dryrun)
         if file:
+            form_data = {
+                k: json.dumps(v) if isinstance(v, dict) 
+                else str(v) 
+                for k, v in json_data.items()
+            }
             file_data = {"adt": file}
-            resp = self.post(url, files=file_data, json=json_data)
+            resp = self.post(url, files=file_data, data=form_data)
         else:
             resp = self.post(url, json=json_data)
         detailed_raise_for_status(resp)
         return resp.json()
 
     def delete_app(self, app_id, force=False):
         """Delete an application in MiCADO
```

### Comparing `micado-client-0.12.1/micado/api/client.py` & `micado-client-0.12.2/micado/api/client.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/cli.py` & `micado-client-0.12.2/micado/cli.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/client.py` & `micado-client-0.12.2/micado/client.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/exceptions.py` & `micado-client-0.12.2/micado/exceptions.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/installer/ansible/ansible.py` & `micado-client-0.12.2/micado/installer/ansible/ansible.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/installer/ansible/playbook.py` & `micado-client-0.12.2/micado/installer/ansible/playbook.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/launcher/cloudbroker/cloudbroker.py` & `micado-client-0.12.2/micado/launcher/cloudbroker/cloudbroker.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         Raises:
             MicadoException: Missing or incorrect data.
         """
         try:
             auth_url = None
             content = None
             with open(self.home + 'data.yml', mode='r') as f:
-                content = yaml.load(f)
+                content = yaml.safe_load(f)
             search = [i for i in content["micados"] if i.get(id, None)]
             if not search:
                 logger.debug(
                     "This {} ID can not find in the data file.".format(id))
                 pass
             else:
                 logger.debug("Remove {} record".format(search))
```

### Comparing `micado-client-0.12.1/micado/launcher/openstack/auth.py` & `micado-client-0.12.2/micado/launcher/openstack/auth.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/launcher/openstack/openstack.py` & `micado-client-0.12.2/micado/launcher/openstack/openstack.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/models/application.py` & `micado-client-0.12.2/micado/models/application.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/models/base.py` & `micado-client-0.12.2/micado/models/base.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/models/micado.py` & `micado-client-0.12.2/micado/models/micado.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado/types/applications.py` & `micado-client-0.12.2/micado/types/applications.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 
 
 class ApplicationInfo(dict):
-    def __init__(self, adt=None, url=None, params={}, dryrun=False):
+    def __init__(self, adt=None, url=None, params=None, dryrun=False):
         """Creates required JSON parameters for create_app
 
         Args:
             adt (dict, optional): YAML dict of Application Description
                 Template. Required is URL is empty. Defaults to None.
             url (string, optional): URL of YAML ADT. Required if ADT is empty.
                 Defaults to None.
```

### Comparing `micado-client-0.12.1/micado/utils/utils.py` & `micado-client-0.12.2/micado/utils/utils.py`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/micado_client.egg-info/PKG-INFO` & `micado-client-0.12.2/micado_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micado-client
-Version: 0.12.1
+Version: 0.12.2
 Summary: A Python Client Library for MiCADO
 Home-page: https://github.com/micado-scale/micado-client
 Author: Márk Emődi & Jay DesLauriers
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/micado-scale/micado-client/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `micado-client-0.12.1/micado_client.egg-info/SOURCES.txt` & `micado-client-0.12.2/micado_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micado-client-0.12.1/setup.py` & `micado-client-0.12.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "ansible-runner",
     "click",
     "dicttoxml",
 ]
 
 setup(
     name="micado-client",
-    version="0.12.1",
+    version="0.12.2",
     description="A Python Client Library for MiCADO",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Márk Emődi & Jay DesLauriers",
     python_requires=">=3.8",
     url="https://github.com/micado-scale/micado-client",
     packages=find_packages(exclude=["tests"]),
```

### Comparing `micado-client-0.12.1/tests/test_auth.py` & `micado-client-0.12.2/tests/test_auth.py`

 * *Files identical despite different names*

