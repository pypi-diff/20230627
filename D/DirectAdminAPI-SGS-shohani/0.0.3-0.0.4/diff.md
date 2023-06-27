# Comparing `tmp/directadminapi_sgs_shohani-0.0.3.tar.gz` & `tmp/directadminapi_sgs_shohani-0.0.4.tar.gz`

## Comparing `directadminapi_sgs_shohani-0.0.3.tar` & `directadminapi_sgs_shohani-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.3/build_upload.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.3/src/DirectAdminAPI_SGS_shohani/__init__.py
--rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.3/src/DirectAdminAPI_SGS_shohani/api.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.3/tests/test.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.3/LICENSE
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.3/README.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.4/build_upload.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.4/src/DirectAdminAPI_SGS_shohani/__init__.py
+-rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.4/src/DirectAdminAPI_SGS_shohani/api.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.4/tests/test.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.4/LICENSE
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.4/README.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.4/PKG-INFO
```

### Comparing `directadminapi_sgs_shohani-0.0.3/src/DirectAdminAPI_SGS_shohani/api.py` & `directadminapi_sgs_shohani-0.0.4/src/DirectAdminAPI_SGS_shohani/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,8 +238,17 @@
 
     def get_ssl_certificates(self, domain):
         '''Get ssl certificates'''
         return self.cmd_api_ssl(
             domain=domain,
             dnsproviders='no',
             GET_METHOD = True
+        )
+    
+    def get_all_users_with_quota(self):
+        '''Get protected directory users list'''
+        return self.cmd_all_user_show(
+            page=1,            
+            ipp=1000 ,#item per page
+            bytes='yes',
+            GET_METHOD = True
         )
```

### Comparing `directadminapi_sgs_shohani-0.0.3/tests/test.py` & `directadminapi_sgs_shohani-0.0.4/tests/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from src.DirectAdminAPI_SGS_shohani.api import PrettyAPI
 from getpass import getpass
 
 api = PrettyAPI(username=input("admin_da_user:"),password=getpass("admin_da_pwd:"),server=input("Enter DA url:"),json=True)
 
 #res_certs = api.get_ssl_certificates('androidsoftware.ir')
 #res_disable = api.disable_ssl('androidsoftware.ir')
-res_enable = api.enable_ssl('androidsoftware.ir')
-res = api.enable_letsencrypt_ssl('androidsoftware.ir','name','sadegh.tkd@gmail.com',["androidsoftware.ir","www.androidsoftware.ir","mail.androidsoftware.ir"])
+#res_enable = api.enable_ssl('androidsoftware.ir')
+#res = api.enable_letsencrypt_ssl('androidsoftware.ir','name','sadegh.tkd@gmail.com',["androidsoftware.ir","www.androidsoftware.ir","mail.androidsoftware.ir"])
 
-da_files = api.search_files(input('Enter path to list files:'),'a.txt' , recursive=True)
+#da_files = api.search_files(input('Enter path to list files:'),'a.txt' , recursive=True)
 
-for key in da_files:
-    print(da_files[key])
+#for key in da_files:
+    #print(da_files[key])
+res = api.get_all_users_with_quota()
+print(res)
```

### Comparing `directadminapi_sgs_shohani-0.0.3/LICENSE` & `directadminapi_sgs_shohani-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `directadminapi_sgs_shohani-0.0.3/README.md` & `directadminapi_sgs_shohani-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `directadminapi_sgs_shohani-0.0.3/pyproject.toml` & `directadminapi_sgs_shohani-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "DirectAdminAPI_SGS_shohani"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Sadegh Ghanbari Shohani", email="sadegh.tkd@gmail.com" },
 ]
 description = "DirectAdmin API for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `directadminapi_sgs_shohani-0.0.3/PKG-INFO` & `directadminapi_sgs_shohani-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DirectAdminAPI_SGS_shohani
-Version: 0.0.3
+Version: 0.0.4
 Summary: DirectAdmin API for Python
 Project-URL: Homepage, https://github.com/sadeghtkd/DirectAdminAPI_SGS
 Project-URL: Bug Tracker, https://github.com/sadeghtkd/DirectAdminAPI_SGS/issues
 Author-email: Sadegh Ghanbari Shohani <sadegh.tkd@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

