# Comparing `tmp/amocrm_api-2.6.0.tar.gz` & `tmp/amocrm_api-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amocrm_api-2.6.0.tar", last modified: Tue Jun 20 19:49:10 2023, max compression
+gzip compressed data, was "amocrm_api-2.6.1.tar", last modified: Tue Jun 27 05:41:45 2023, max compression
```

## Comparing `amocrm_api-2.6.0.tar` & `amocrm_api-2.6.1.tar`

### file list

```diff
@@ -1,54 +1,47 @@
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.553098 amocrm_api-2.6.0/
--rw-r--r--   0 pandadoc   (501) staff       (20)     1081 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/LICENSE.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)     6723 2023-06-20 19:49:10.553216 amocrm_api-2.6.0/PKG-INFO
--rw-r--r--   0 pandadoc   (501) staff       (20)     5875 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/README.rst
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.541085 amocrm_api-2.6.0/amocrm/
--rw-r--r--   0 pandadoc   (501) staff       (20)      466 2023-06-20 19:45:32.000000 amocrm_api-2.6.0/amocrm/__init__.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.545102 amocrm_api-2.6.0/amocrm/v2/
--rw-r--r--   0 pandadoc   (501) staff       (20)      429 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/amocrm/v2/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1524 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/account.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4638 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/cli.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.549187 amocrm_api-2.6.0/amocrm/v2/entity/
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2493 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/call.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1086 2022-08-28 19:28:40.000000 amocrm_api-2.6.0/amocrm/v2/entity/company.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1082 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/amocrm/v2/entity/contact.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     8199 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/custom_field.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1582 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/amocrm/v2/entity/customer.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4932 2022-08-28 19:28:37.000000 amocrm_api-2.6.0/amocrm/v2/entity/events.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1959 2022-08-28 19:28:40.000000 amocrm_api-2.6.0/amocrm/v2/entity/lead.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      908 2023-06-20 19:44:04.000000 amocrm_api-2.6.0/amocrm/v2/entity/list.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2520 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/note.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1901 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/pipeline.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1852 2023-06-20 19:44:04.000000 amocrm_api-2.6.0/amocrm/v2/entity/tag.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2125 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/amocrm/v2/entity/task.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      994 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/user.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1011 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/exceptions.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4945 2022-08-28 19:52:07.000000 amocrm_api-2.6.0/amocrm/v2/fields.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2150 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/amocrm/v2/filters.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     5075 2023-06-20 19:44:04.000000 amocrm_api-2.6.0/amocrm/v2/interaction.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      885 2023-06-20 19:44:04.000000 amocrm_api-2.6.0/amocrm/v2/links.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1120 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/manager.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2286 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/model.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      377 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/register.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     5626 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/tokens.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.550663 amocrm_api-2.6.0/amocrm_api.egg-info/
--rw-r--r--   0 pandadoc   (501) staff       (20)     6723 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/PKG-INFO
--rw-r--r--   0 pandadoc   (501) staff       (20)     1082 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/SOURCES.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/dependency_links.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)       48 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/entry_points.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)       37 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/requires.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)       13 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/top_level.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)       80 2023-06-20 19:49:10.553587 amocrm_api-2.6.0/setup.cfg
--rw-r--r--   0 pandadoc   (501) staff       (20)     1452 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/setup.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.551905 amocrm_api-2.6.0/tests/
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      688 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/conftest.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.552865 amocrm_api-2.6.0/tests/data/
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/data/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      683 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/data/companies.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4540 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/data/contacts.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1440 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/data/users.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2993 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/tests/test_contacts.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      512 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/test_user.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      554 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/test_utils.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-27 05:41:45.842696 amocrm_api-2.6.1/
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1081 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/LICENSE.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)     6774 2023-06-27 05:41:45.842860 amocrm_api-2.6.1/PKG-INFO
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5875 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/README.rst
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-27 05:41:45.827834 amocrm_api-2.6.1/amocrm/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      466 2023-06-27 05:33:23.000000 amocrm_api-2.6.1/amocrm/__init__.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-27 05:41:45.830137 amocrm_api-2.6.1/amocrm/v2/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      429 2022-08-28 20:10:58.000000 amocrm_api-2.6.1/amocrm/v2/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1524 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/account.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4638 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/cli.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-27 05:41:45.832734 amocrm_api-2.6.1/amocrm/v2/entity/
+-rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/entity/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2493 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/entity/call.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1086 2022-08-28 19:28:40.000000 amocrm_api-2.6.1/amocrm/v2/entity/company.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1082 2022-08-28 20:10:58.000000 amocrm_api-2.6.1/amocrm/v2/entity/contact.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     8199 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/entity/custom_field.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1582 2022-08-28 20:10:58.000000 amocrm_api-2.6.1/amocrm/v2/entity/customer.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5214 2023-06-27 05:32:52.000000 amocrm_api-2.6.1/amocrm/v2/entity/events.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1959 2022-08-28 19:28:40.000000 amocrm_api-2.6.1/amocrm/v2/entity/lead.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      908 2023-06-20 19:44:04.000000 amocrm_api-2.6.1/amocrm/v2/entity/list.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2520 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/entity/note.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1901 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/entity/pipeline.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1852 2023-06-20 19:44:04.000000 amocrm_api-2.6.1/amocrm/v2/entity/tag.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2125 2022-08-28 20:10:58.000000 amocrm_api-2.6.1/amocrm/v2/entity/task.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      994 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/entity/user.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1011 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/exceptions.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4945 2022-08-28 19:52:07.000000 amocrm_api-2.6.1/amocrm/v2/fields.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2150 2022-08-28 20:10:58.000000 amocrm_api-2.6.1/amocrm/v2/filters.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5075 2023-06-20 19:44:04.000000 amocrm_api-2.6.1/amocrm/v2/interaction.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      885 2023-06-20 19:44:04.000000 amocrm_api-2.6.1/amocrm/v2/links.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1120 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/manager.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2286 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/model.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      377 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/register.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5626 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/amocrm/v2/tokens.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-27 05:41:45.841204 amocrm_api-2.6.1/amocrm_api.egg-info/
+-rw-r--r--   0 pandadoc   (501) staff       (20)     6774 2023-06-27 05:41:45.000000 amocrm_api-2.6.1/amocrm_api.egg-info/PKG-INFO
+-rw-r--r--   0 pandadoc   (501) staff       (20)      956 2023-06-27 05:41:45.000000 amocrm_api-2.6.1/amocrm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-06-27 05:41:45.000000 amocrm_api-2.6.1/amocrm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)       48 2023-06-27 05:41:45.000000 amocrm_api-2.6.1/amocrm_api.egg-info/entry_points.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)       37 2023-06-27 05:41:45.000000 amocrm_api-2.6.1/amocrm_api.egg-info/requires.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)        7 2023-06-27 05:41:45.000000 amocrm_api-2.6.1/amocrm_api.egg-info/top_level.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)       80 2023-06-27 05:41:45.843466 amocrm_api-2.6.1/setup.cfg
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1530 2023-06-27 05:41:23.000000 amocrm_api-2.6.1/setup.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-27 05:41:45.842328 amocrm_api-2.6.1/tests/
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2993 2022-08-28 20:10:58.000000 amocrm_api-2.6.1/tests/test_contacts.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      512 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/tests/test_user.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      554 2022-05-31 17:55:19.000000 amocrm_api-2.6.1/tests/test_utils.py
```

### Comparing `amocrm_api-2.6.0/LICENSE.txt` & `amocrm_api-2.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/PKG-INFO` & `amocrm_api-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: amocrm_api
-Version: 2.6.0
+Version: 2.6.1
 Summary: Python API for Amocrm
 Home-page: https://github.com/Krukov/amocrm_api
-Download-URL: https://github.com/Krukov/amocrm_api/tarball/2.6.0
+Download-URL: https://github.com/Krukov/amocrm_api/tarball/2.6.1
 Author: Dmitry Kryukov
 Author-email: glebov.ru@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Provides-Extra: cli
 License-File: LICENSE.txt
 
 ===============================
 AmoCRM python API. V2
```

### Comparing `amocrm_api-2.6.0/README.rst` & `amocrm_api-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/account.py` & `amocrm_api-2.6.1/amocrm/v2/account.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/cli.py` & `amocrm_api-2.6.1/amocrm/v2/cli.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/call.py` & `amocrm_api-2.6.1/amocrm/v2/entity/call.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/company.py` & `amocrm_api-2.6.1/amocrm/v2/entity/company.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/contact.py` & `amocrm_api-2.6.1/amocrm/v2/entity/contact.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/custom_field.py` & `amocrm_api-2.6.1/amocrm/v2/entity/custom_field.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/customer.py` & `amocrm_api-2.6.1/amocrm/v2/entity/customer.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/events.py` & `amocrm_api-2.6.1/amocrm/v2/entity/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     "contact_linked",
     "contact_unlinked",
     "lead_linked",
     "lead_unlinked",
     "entity_linked",
     "entity_unlinked",
 )
+EVENT_REQUEST_LIMIT = 100
 
 
 class _EventValueField(fields._UnEditableField):
     def on_get_instance(self, instance, value):
         """
         value here is what we have in value_after/value_before field
         For example
@@ -111,14 +112,17 @@
             return datetime.utcfromtimestamp(float(value[0]["task_deadline"]["timestamp"]))
         return value
 
 
 class EventsInteraction(GenericInteraction):
     path = "events"
 
+    def get_all(self, include=None, query=None, filters=(), order=None):
+        for data in self._all(self._get_path(), include=include, query=query, filters=filters, order=order, limit=EVENT_REQUEST_LIMIT):
+            yield from data[self._get_field()]
 
 class Event(model.Model):
     type = fields._Field("type")
     entity_id = fields._UnEditableField("entity_id")
     entity_type = fields._UnEditableField("entity_type")
     created_by = fields._Link("created_by", "User")
     created_at = fields._DateTimeField("created_at")
```

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/lead.py` & `amocrm_api-2.6.1/amocrm/v2/entity/lead.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/list.py` & `amocrm_api-2.6.1/amocrm/v2/entity/list.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/note.py` & `amocrm_api-2.6.1/amocrm/v2/entity/note.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/pipeline.py` & `amocrm_api-2.6.1/amocrm/v2/entity/pipeline.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/tag.py` & `amocrm_api-2.6.1/amocrm/v2/entity/tag.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/task.py` & `amocrm_api-2.6.1/amocrm/v2/entity/task.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/entity/user.py` & `amocrm_api-2.6.1/amocrm/v2/entity/user.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/exceptions.py` & `amocrm_api-2.6.1/amocrm/v2/exceptions.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/fields.py` & `amocrm_api-2.6.1/amocrm/v2/fields.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/filters.py` & `amocrm_api-2.6.1/amocrm/v2/filters.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/interaction.py` & `amocrm_api-2.6.1/amocrm/v2/interaction.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/links.py` & `amocrm_api-2.6.1/amocrm/v2/links.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/manager.py` & `amocrm_api-2.6.1/amocrm/v2/manager.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/model.py` & `amocrm_api-2.6.1/amocrm/v2/model.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm/v2/tokens.py` & `amocrm_api-2.6.1/amocrm/v2/tokens.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/amocrm_api.egg-info/PKG-INFO` & `amocrm_api-2.6.1/amocrm_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: amocrm-api
-Version: 2.6.0
+Version: 2.6.1
 Summary: Python API for Amocrm
 Home-page: https://github.com/Krukov/amocrm_api
-Download-URL: https://github.com/Krukov/amocrm_api/tarball/2.6.0
+Download-URL: https://github.com/Krukov/amocrm_api/tarball/2.6.1
 Author: Dmitry Kryukov
 Author-email: glebov.ru@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Provides-Extra: cli
 License-File: LICENSE.txt
 
 ===============================
 AmoCRM python API. V2
```

### Comparing `amocrm_api-2.6.0/tests/test_contacts.py` & `amocrm_api-2.6.1/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/tests/test_user.py` & `amocrm_api-2.6.1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.6.0/tests/test_utils.py` & `amocrm_api-2.6.1/tests/test_utils.py`

 * *Files identical despite different names*

