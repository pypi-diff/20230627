# Comparing `tmp/openshift-client-1.0.8.tar.gz` & `tmp/openshift-client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openshift-client-1.0.8.tar", last modified: Mon Nov  2 15:46:13 2020, max compression
+gzip compressed data, was "dist/openshift-client-1.0.9.tar", last modified: Fri Nov 20 20:56:52 2020, max compression
```

## Comparing `openshift-client-1.0.8.tar` & `openshift-client-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 brawilli  (1000) brawilli  (1000)        0 2020-11-02 15:46:13.852547 openshift-client-1.0.8/
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    10759 2020-02-13 15:09:29.000000 openshift-client-1.0.8/LICENSE
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    29901 2020-11-02 15:46:13.852547 openshift-client-1.0.8/PKG-INFO
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    24304 2020-04-23 19:33:58.000000 openshift-client-1.0.8/README.md
-drwxrwxr-x   0 brawilli  (1000) brawilli  (1000)        0 2020-11-02 15:46:13.849547 openshift-client-1.0.8/packages/
-drwxrwxr-x   0 brawilli  (1000) brawilli  (1000)        0 2020-11-02 15:46:13.851547 openshift-client-1.0.8/packages/openshift/
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      652 2020-11-02 15:45:46.000000 openshift-client-1.0.8/packages/openshift/__init__.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    14910 2020-04-16 21:16:49.000000 openshift-client-1.0.8/packages/openshift/action.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      608 2019-07-30 13:42:05.000000 openshift-client-1.0.8/packages/openshift/ansible.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    36363 2020-08-26 13:53:53.000000 openshift-client-1.0.8/packages/openshift/apiobject.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    60805 2020-11-02 15:37:33.000000 openshift-client-1.0.8/packages/openshift/base_verbs.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     7577 2020-04-16 21:16:49.000000 openshift-client-1.0.8/packages/openshift/config.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    21825 2020-06-03 15:29:49.000000 openshift-client-1.0.8/packages/openshift/context.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     9231 2020-07-20 15:26:16.000000 openshift-client-1.0.8/packages/openshift/model.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    23921 2020-04-16 21:16:49.000000 openshift-client-1.0.8/packages/openshift/naming.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     3360 2020-04-16 21:16:49.000000 openshift-client-1.0.8/packages/openshift/result.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    33322 2020-10-26 14:33:46.000000 openshift-client-1.0.8/packages/openshift/selector.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     2136 2020-04-16 21:16:49.000000 openshift-client-1.0.8/packages/openshift/status.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      373 2020-06-05 21:45:18.000000 openshift-client-1.0.8/packages/openshift/test_apiobject.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    12516 2020-07-20 15:26:16.000000 openshift-client-1.0.8/packages/openshift/test_model.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     2281 2020-04-16 21:16:49.000000 openshift-client-1.0.8/packages/openshift/test_selector.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     1428 2020-04-16 21:16:49.000000 openshift-client-1.0.8/packages/openshift/test_util.py
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     5313 2020-06-03 15:45:50.000000 openshift-client-1.0.8/packages/openshift/util.py
-drwxrwxr-x   0 brawilli  (1000) brawilli  (1000)        0 2020-11-02 15:46:13.851547 openshift-client-1.0.8/packages/openshift_client.egg-info/
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    29901 2020-11-02 15:46:13.000000 openshift-client-1.0.8/packages/openshift_client.egg-info/PKG-INFO
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      822 2020-11-02 15:46:13.000000 openshift-client-1.0.8/packages/openshift_client.egg-info/SOURCES.txt
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)        1 2020-11-02 15:46:13.000000 openshift-client-1.0.8/packages/openshift_client.egg-info/dependency_links.txt
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)       20 2020-11-02 15:46:13.000000 openshift-client-1.0.8/packages/openshift_client.egg-info/requires.txt
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)       10 2020-11-02 15:46:13.000000 openshift-client-1.0.8/packages/openshift_client.egg-info/top_level.txt
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      114 2020-04-16 21:16:49.000000 openshift-client-1.0.8/requirements.txt
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      102 2020-11-02 15:46:13.852547 openshift-client-1.0.8/setup.cfg
--rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     2229 2020-04-23 16:05:36.000000 openshift-client-1.0.8/setup.py
+drwxrwxr-x   0 brawilli  (1000) brawilli  (1000)        0 2020-11-20 20:56:52.739878 openshift-client-1.0.9/
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    10759 2020-02-13 15:09:29.000000 openshift-client-1.0.9/LICENSE
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    29901 2020-11-20 20:56:52.739878 openshift-client-1.0.9/PKG-INFO
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    24304 2020-04-23 19:33:58.000000 openshift-client-1.0.9/README.md
+drwxrwxr-x   0 brawilli  (1000) brawilli  (1000)        0 2020-11-20 20:56:52.735878 openshift-client-1.0.9/packages/
+drwxrwxr-x   0 brawilli  (1000) brawilli  (1000)        0 2020-11-20 20:56:52.738878 openshift-client-1.0.9/packages/openshift/
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      652 2020-11-20 20:55:23.000000 openshift-client-1.0.9/packages/openshift/__init__.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    14910 2020-04-16 21:16:49.000000 openshift-client-1.0.9/packages/openshift/action.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      608 2019-07-30 13:42:05.000000 openshift-client-1.0.9/packages/openshift/ansible.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    36562 2020-11-20 20:52:09.000000 openshift-client-1.0.9/packages/openshift/apiobject.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    60805 2020-11-02 15:37:33.000000 openshift-client-1.0.9/packages/openshift/base_verbs.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     7577 2020-04-16 21:16:49.000000 openshift-client-1.0.9/packages/openshift/config.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    21825 2020-06-03 15:29:49.000000 openshift-client-1.0.9/packages/openshift/context.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     9231 2020-07-20 15:26:16.000000 openshift-client-1.0.9/packages/openshift/model.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    23921 2020-04-16 21:16:49.000000 openshift-client-1.0.9/packages/openshift/naming.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     3360 2020-04-16 21:16:49.000000 openshift-client-1.0.9/packages/openshift/result.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    33586 2020-11-20 20:52:09.000000 openshift-client-1.0.9/packages/openshift/selector.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     2136 2020-04-16 21:16:49.000000 openshift-client-1.0.9/packages/openshift/status.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      373 2020-06-05 21:45:18.000000 openshift-client-1.0.9/packages/openshift/test_apiobject.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    12516 2020-07-20 15:26:16.000000 openshift-client-1.0.9/packages/openshift/test_model.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     2281 2020-04-16 21:16:49.000000 openshift-client-1.0.9/packages/openshift/test_selector.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     1428 2020-04-16 21:16:49.000000 openshift-client-1.0.9/packages/openshift/test_util.py
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     5313 2020-06-03 15:45:50.000000 openshift-client-1.0.9/packages/openshift/util.py
+drwxrwxr-x   0 brawilli  (1000) brawilli  (1000)        0 2020-11-20 20:56:52.738878 openshift-client-1.0.9/packages/openshift_client.egg-info/
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)    29901 2020-11-20 20:56:52.000000 openshift-client-1.0.9/packages/openshift_client.egg-info/PKG-INFO
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      822 2020-11-20 20:56:52.000000 openshift-client-1.0.9/packages/openshift_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)        1 2020-11-20 20:56:52.000000 openshift-client-1.0.9/packages/openshift_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)       20 2020-11-20 20:56:52.000000 openshift-client-1.0.9/packages/openshift_client.egg-info/requires.txt
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)       10 2020-11-20 20:56:52.000000 openshift-client-1.0.9/packages/openshift_client.egg-info/top_level.txt
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      114 2020-04-16 21:16:49.000000 openshift-client-1.0.9/requirements.txt
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)      102 2020-11-20 20:56:52.739878 openshift-client-1.0.9/setup.cfg
+-rw-rw-r--   0 brawilli  (1000) brawilli  (1000)     2229 2020-04-23 16:05:36.000000 openshift-client-1.0.9/setup.py
```

### Comparing `openshift-client-1.0.8/LICENSE` & `openshift-client-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/PKG-INFO` & `openshift-client-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: OpenShift python client
 Home-page: https://github.com/openshift/openshift-client-python
 Author: Justin Pierce
 Author-email: jupierce@redhat.com
 Maintainer: Brad Williams
 Maintainer-email: brawilli@redhat.com
 License: UNKNOWN
```

### Comparing `openshift-client-1.0.8/README.md` & `openshift-client-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/__init__.py` & `openshift-client-1.0.9/packages/openshift/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .apiobject import *
 from . import naming
 from . import status
 from . import config
 from .ansible import ansible
 
 # Single source for module version
-__VERSION__ = '1.0.8'
+__VERSION__ = '1.0.9'
 
 null = None  # Allow scripts to specify null in object definitions
 
 
 # Allows modules to trigger errors
 def error(msg, **kwargs):
     raise OpenShiftPythonException(msg, **kwargs)
```

### Comparing `openshift-client-1.0.8/packages/openshift/action.py` & `openshift-client-1.0.9/packages/openshift/action.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/ansible.py` & `openshift-client-1.0.9/packages/openshift/ansible.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/apiobject.py` & `openshift-client-1.0.9/packages/openshift/apiobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -662,16 +662,17 @@
         base_args.append("--patch=" + patch_def)
         r.add_action(oc_action(self.context, "patch", cmd_args=[base_args, cmd_args],
                                namespace=self.namespace(if_missing=None)))
 
         r.fail_if("Error running patch on objects")
         return r
 
-    def elements(self):
+    def elements(self, cls=None):
         """
+        :param cls A custom subclass of APIObject to return in place of APIObjects
         :return: Returns a python list of APIObjects. If receiver is an OpenShift 'List', each element will be
         added to the returned list. If the receiver is not of kind List, the [self] will be returned.
         """
         self_kind = self.kind(lowercase=False)
         if self_kind.endswith('List'):  # e.g. "List", "PodList", "NodeList"
             item_kind = self_kind[
                         :-4]  # strip 'List' off the end. This may leave '' or the kind of elements in the list
@@ -684,15 +685,20 @@
 
             # If not an empty string, set the kind in the underlying object. This is because of the odd
             # way `oc adm manage-node --list-pods <node> -o=yaml` returns yaml for each pod, but without
             # a 'kind' in the object markup. So, if we get a 'PodList', set the kind before making into apiobjects.
             if item_kind:
                 d['kind'] = item_kind
 
-            l.append(APIObject(d))
+            if cls is not None:
+                obj = cls(d)
+            else:
+                obj = APIObject(d)
+
+            l.append(obj)
 
         return l
 
     def process(self, parameters=None, cmd_args=None):
 
         """
         Assumes this APIObject is a template and runs oc process against it.
```

### Comparing `openshift-client-1.0.8/packages/openshift/base_verbs.py` & `openshift-client-1.0.9/packages/openshift/base_verbs.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/config.py` & `openshift-client-1.0.9/packages/openshift/config.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/context.py` & `openshift-client-1.0.9/packages/openshift/context.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/model.py` & `openshift-client-1.0.9/packages/openshift/model.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/naming.py` & `openshift-client-1.0.9/packages/openshift/naming.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/result.py` & `openshift-client-1.0.9/packages/openshift/result.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/selector.py` & `openshift-client-1.0.9/packages/openshift/selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,43 +387,51 @@
                 "kind": "List",
                 "metadata": {},
                 "items": []
             })
 
         return r.out()
 
-    def object(self, ignore_not_found=False):
+    def object(self, ignore_not_found=False, cls=None):
         """
         Returns a single APIObject that represents the selected resource. If multiple
         resources are being selected an exception will be thrown (use objects() when
         there is a possibility of selecting multiple objects).
         :param ignore_not_found: If True and no object exists, None will be returned instead of an exception.
+        :param cls: Custom APIObject class to return
         :return: A Model of the selected resource.
         """
-        objs = self.objects()
+        objs = self.objects(cls=cls)
         if len(objs) == 0:
             if ignore_not_found:
                 return None
             raise OpenShiftPythonException("Expected a single object, but selected 0")
         elif len(objs) > 1:
             raise OpenShiftPythonException("Expected a single object, but selected more than one")
 
         return objs[0]
 
-    def objects(self, ignore_not_found=True):
+    def objects(self, ignore_not_found=True, cls=None):
         """
         Returns a python list of APIObject objects that represent the selected resources. An
         empty is returned if nothing is selected.
         :param ignore_not_found: If true, missing named resources will not raise an exception.
+        :param cls: Custom APIObject class to return
         :return: A list of Model objects representing the receiver's selected resources.
         """
         from .apiobject import APIObject
 
         obj = json.loads(self.object_json(ignore_not_found=ignore_not_found))
-        return APIObject(obj).elements()
+
+        if cls is not None:
+            api_objects = cls(obj).elements(cls)
+        else:
+            api_objects = APIObject(obj).elements()
+
+        return api_objects
 
     def start_build(self, cmd_args=None):
         r = Selector('start_build')
 
         # Have start-build output a list of objects it creates
         base_args = list()
         base_args.append("-o=name")
```

### Comparing `openshift-client-1.0.8/packages/openshift/status.py` & `openshift-client-1.0.9/packages/openshift/status.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/test_model.py` & `openshift-client-1.0.9/packages/openshift/test_model.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/test_selector.py` & `openshift-client-1.0.9/packages/openshift/test_selector.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/test_util.py` & `openshift-client-1.0.9/packages/openshift/test_util.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift/util.py` & `openshift-client-1.0.9/packages/openshift/util.py`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/packages/openshift_client.egg-info/PKG-INFO` & `openshift-client-1.0.9/packages/openshift_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: OpenShift python client
 Home-page: https://github.com/openshift/openshift-client-python
 Author: Justin Pierce
 Author-email: jupierce@redhat.com
 Maintainer: Brad Williams
 Maintainer-email: brawilli@redhat.com
 License: UNKNOWN
```

### Comparing `openshift-client-1.0.8/packages/openshift_client.egg-info/SOURCES.txt` & `openshift-client-1.0.9/packages/openshift_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openshift-client-1.0.8/setup.py` & `openshift-client-1.0.9/setup.py`

 * *Files identical despite different names*

