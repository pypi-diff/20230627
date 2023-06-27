# Comparing `tmp/endi_celery-6.6.4.tar.gz` & `tmp/endi_celery-6.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endi_celery-6.6.4.tar", last modified: Mon Jun 26 11:44:21 2023, max compression
+gzip compressed data, was "endi_celery-6.6.5.tar", last modified: Tue Jun 27 17:21:26 2023, max compression
```

## Comparing `endi_celery-6.6.4.tar` & `endi_celery-6.6.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:44:21.337160 endi_celery-6.6.4/
--rw-r--r--   0 gas       (1000) gas       (1000)        6 2023-06-26 11:44:11.000000 endi_celery-6.6.4/CURRENT_VERSION
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 endi_celery-6.6.4/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      186 2020-06-24 14:37:06.000000 endi_celery-6.6.4/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-06-26 11:44:21.337160 endi_celery-6.6.4/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     2601 2023-04-24 10:03:13.000000 endi_celery-6.6.4/README.rst
--rw-r--r--   0 gas       (1000) gas       (1000)     5047 2023-05-25 15:22:08.000000 endi_celery-6.6.4/development.ini
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:44:21.330160 endi_celery-6.6.4/endi_celery/
--rw-r--r--   0 gas       (1000) gas       (1000)     4535 2023-04-24 10:04:13.000000 endi_celery-6.6.4/endi_celery/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1787 2023-01-11 11:06:17.000000 endi_celery-6.6.4/endi_celery/conf.py
--rw-r--r--   0 gas       (1000) gas       (1000)      585 2023-01-11 11:00:06.000000 endi_celery-6.6.4/endi_celery/exception.py
--rw-r--r--   0 gas       (1000) gas       (1000)      504 2021-09-10 16:39:28.000000 endi_celery-6.6.4/endi_celery/hacks.py
--rw-r--r--   0 gas       (1000) gas       (1000)      753 2023-01-11 11:00:06.000000 endi_celery-6.6.4/endi_celery/interfaces.py
--rw-r--r--   0 gas       (1000) gas       (1000)      482 2023-01-11 11:48:27.000000 endi_celery-6.6.4/endi_celery/locks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5742 2022-12-09 15:12:22.000000 endi_celery-6.6.4/endi_celery/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     7225 2022-12-09 15:12:22.000000 endi_celery-6.6.4/endi_celery/models.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:44:21.333160 endi_celery-6.6.4/endi_celery/parsers/
--rw-r--r--   0 gas       (1000) gas       (1000)     2162 2023-01-12 14:56:56.000000 endi_celery-6.6.4/endi_celery/parsers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2870 2023-05-11 15:37:23.000000 endi_celery-6.6.4/endi_celery/parsers/isacompta.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3288 2023-01-18 08:46:47.000000 endi_celery-6.6.4/endi_celery/parsers/quadra.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3103 2023-06-15 14:04:15.000000 endi_celery-6.6.4/endi_celery/parsers/sage.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3891 2023-04-24 10:04:13.000000 endi_celery-6.6.4/endi_celery/parsers/sage_generation_expert.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:44:21.334160 endi_celery-6.6.4/endi_celery/schedulers/
--rw-r--r--   0 gas       (1000) gas       (1000)       29 2020-06-24 14:37:06.000000 endi_celery-6.6.4/endi_celery/schedulers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)      427 2022-12-09 15:12:22.000000 endi_celery-6.6.4/endi_celery/schedulers/tasks.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:44:21.336160 endi_celery-6.6.4/endi_celery/tasks/
--rw-r--r--   0 gas       (1000) gas       (1000)    10123 2023-06-26 11:42:34.000000 endi_celery-6.6.4/endi_celery/tasks/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)    39473 2023-05-25 15:25:03.000000 endi_celery-6.6.4/endi_celery/tasks/accounting_measure_compute.py
--rw-r--r--   0 gas       (1000) gas       (1000)    12003 2023-01-17 16:14:55.000000 endi_celery-6.6.4/endi_celery/tasks/accounting_parser.py
--rw-r--r--   0 gas       (1000) gas       (1000)    29193 2023-01-12 16:49:34.000000 endi_celery-6.6.4/endi_celery/tasks/csv_import.py
--rw-r--r--   0 gas       (1000) gas       (1000)    16393 2023-06-26 11:09:42.000000 endi_celery-6.6.4/endi_celery/tasks/export.py
--rw-r--r--   0 gas       (1000) gas       (1000)     4856 2022-12-09 15:12:23.000000 endi_celery-6.6.4/endi_celery/tasks/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1064 2023-05-25 15:25:03.000000 endi_celery-6.6.4/endi_celery/tasks/notification.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3267 2022-03-03 10:44:16.000000 endi_celery-6.6.4/endi_celery/tasks/tasks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     6687 2022-12-09 15:12:23.000000 endi_celery-6.6.4/endi_celery/tasks/utils.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2765 2022-03-03 10:44:16.000000 endi_celery-6.6.4/endi_celery/transactional_task.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-26 11:44:21.332160 endi_celery-6.6.4/endi_celery.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-06-26 11:44:20.000000 endi_celery-6.6.4/endi_celery.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     1106 2023-06-26 11:44:21.000000 endi_celery-6.6.4/endi_celery.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-06-26 11:44:20.000000 endi_celery-6.6.4/endi_celery.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       82 2023-06-26 11:44:21.000000 endi_celery-6.6.4/endi_celery.egg-info/entry_points.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-11-23 12:28:56.000000 endi_celery-6.6.4/endi_celery.egg-info/not-zip-safe
--rw-r--r--   0 gas       (1000) gas       (1000)       80 2023-06-26 11:44:21.000000 endi_celery-6.6.4/endi_celery.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       12 2023-06-26 11:44:21.000000 endi_celery-6.6.4/endi_celery.egg-info/top_level.txt
--rw-r--r--   0 gas       (1000) gas       (1000)     2934 2021-03-25 17:57:51.000000 endi_celery-6.6.4/prod_example.ini
--rw-r--r--   0 gas       (1000) gas       (1000)       53 2020-06-24 14:37:06.000000 endi_celery-6.6.4/pytest.ini
--rw-r--r--   0 gas       (1000) gas       (1000)       81 2022-01-12 14:56:54.000000 endi_celery-6.6.4/requirements.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       38 2023-06-26 11:44:21.337160 endi_celery-6.6.4/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1326 2023-01-17 16:18:35.000000 endi_celery-6.6.4/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-27 17:21:26.615597 endi_celery-6.6.5/
+-rw-r--r--   0 gas       (1000) gas       (1000)        6 2023-06-27 17:20:21.000000 endi_celery-6.6.5/CURRENT_VERSION
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 endi_celery-6.6.5/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      186 2020-06-24 14:37:06.000000 endi_celery-6.6.5/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-06-27 17:21:26.614597 endi_celery-6.6.5/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     2601 2023-04-24 10:03:13.000000 endi_celery-6.6.5/README.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)     5047 2023-05-25 15:22:08.000000 endi_celery-6.6.5/development.ini
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-27 17:21:26.605597 endi_celery-6.6.5/endi_celery/
+-rw-r--r--   0 gas       (1000) gas       (1000)     4535 2023-04-24 10:04:13.000000 endi_celery-6.6.5/endi_celery/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1787 2023-01-11 11:06:17.000000 endi_celery-6.6.5/endi_celery/conf.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      585 2023-01-11 11:00:06.000000 endi_celery-6.6.5/endi_celery/exception.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      504 2021-09-10 16:39:28.000000 endi_celery-6.6.5/endi_celery/hacks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      753 2023-01-11 11:00:06.000000 endi_celery-6.6.5/endi_celery/interfaces.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      482 2023-01-11 11:48:27.000000 endi_celery-6.6.5/endi_celery/locks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5742 2022-12-09 15:12:22.000000 endi_celery-6.6.5/endi_celery/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     7225 2022-12-09 15:12:22.000000 endi_celery-6.6.5/endi_celery/models.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-27 17:21:26.608597 endi_celery-6.6.5/endi_celery/parsers/
+-rw-r--r--   0 gas       (1000) gas       (1000)     2162 2023-01-12 14:56:56.000000 endi_celery-6.6.5/endi_celery/parsers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2870 2023-05-11 15:37:23.000000 endi_celery-6.6.5/endi_celery/parsers/isacompta.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3288 2023-01-18 08:46:47.000000 endi_celery-6.6.5/endi_celery/parsers/quadra.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3103 2023-06-15 14:04:15.000000 endi_celery-6.6.5/endi_celery/parsers/sage.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3891 2023-04-24 10:04:13.000000 endi_celery-6.6.5/endi_celery/parsers/sage_generation_expert.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-27 17:21:26.609597 endi_celery-6.6.5/endi_celery/schedulers/
+-rw-r--r--   0 gas       (1000) gas       (1000)       29 2020-06-24 14:37:06.000000 endi_celery-6.6.5/endi_celery/schedulers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      427 2022-12-09 15:12:22.000000 endi_celery-6.6.5/endi_celery/schedulers/tasks.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-27 17:21:26.613597 endi_celery-6.6.5/endi_celery/tasks/
+-rw-r--r--   0 gas       (1000) gas       (1000)    10123 2023-06-27 17:18:27.000000 endi_celery-6.6.5/endi_celery/tasks/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    39645 2023-06-26 14:16:53.000000 endi_celery-6.6.5/endi_celery/tasks/accounting_measure_compute.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    12003 2023-01-17 16:14:55.000000 endi_celery-6.6.5/endi_celery/tasks/accounting_parser.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    29193 2023-01-12 16:49:34.000000 endi_celery-6.6.5/endi_celery/tasks/csv_import.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    16393 2023-06-26 11:09:42.000000 endi_celery-6.6.5/endi_celery/tasks/export.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     4856 2022-12-09 15:12:23.000000 endi_celery-6.6.5/endi_celery/tasks/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1064 2023-05-25 15:25:03.000000 endi_celery-6.6.5/endi_celery/tasks/notification.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3267 2022-03-03 10:44:16.000000 endi_celery-6.6.5/endi_celery/tasks/tasks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     6687 2022-12-09 15:12:23.000000 endi_celery-6.6.5/endi_celery/tasks/utils.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2765 2022-03-03 10:44:16.000000 endi_celery-6.6.5/endi_celery/transactional_task.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-27 17:21:26.607597 endi_celery-6.6.5/endi_celery.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)     3178 2023-06-27 17:21:25.000000 endi_celery-6.6.5/endi_celery.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     1106 2023-06-27 17:21:26.000000 endi_celery-6.6.5/endi_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-06-27 17:21:25.000000 endi_celery-6.6.5/endi_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       82 2023-06-27 17:21:26.000000 endi_celery-6.6.5/endi_celery.egg-info/entry_points.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2020-11-23 12:28:56.000000 endi_celery-6.6.5/endi_celery.egg-info/not-zip-safe
+-rw-r--r--   0 gas       (1000) gas       (1000)       80 2023-06-27 17:21:26.000000 endi_celery-6.6.5/endi_celery.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       12 2023-06-27 17:21:26.000000 endi_celery-6.6.5/endi_celery.egg-info/top_level.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)     2934 2021-03-25 17:57:51.000000 endi_celery-6.6.5/prod_example.ini
+-rw-r--r--   0 gas       (1000) gas       (1000)       53 2020-06-24 14:37:06.000000 endi_celery-6.6.5/pytest.ini
+-rw-r--r--   0 gas       (1000) gas       (1000)       81 2022-01-12 14:56:54.000000 endi_celery-6.6.5/requirements.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       38 2023-06-27 17:21:26.615597 endi_celery-6.6.5/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1326 2023-06-26 11:47:38.000000 endi_celery-6.6.5/setup.py
```

### Comparing `endi_celery-6.6.4/LICENSE.txt` & `endi_celery-6.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/PKG-INFO` & `endi_celery-6.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endi_celery
-Version: 6.6.4
+Version: 6.6.5
 Summary: endi_celery
 Home-page: https://framagit.org/endi/endi_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `endi_celery-6.6.4/README.rst` & `endi_celery-6.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/development.ini` & `endi_celery-6.6.5/development.ini`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/__init__.py` & `endi_celery-6.6.5/endi_celery/__init__.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/conf.py` & `endi_celery-6.6.5/endi_celery/conf.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/exception.py` & `endi_celery-6.6.5/endi_celery/exception.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/interfaces.py` & `endi_celery-6.6.5/endi_celery/interfaces.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/mail.py` & `endi_celery-6.6.5/endi_celery/mail.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/models.py` & `endi_celery-6.6.5/endi_celery/models.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/parsers/__init__.py` & `endi_celery-6.6.5/endi_celery/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/parsers/isacompta.py` & `endi_celery-6.6.5/endi_celery/parsers/isacompta.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/parsers/quadra.py` & `endi_celery-6.6.5/endi_celery/parsers/quadra.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/parsers/sage.py` & `endi_celery-6.6.5/endi_celery/parsers/sage.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/parsers/sage_generation_expert.py` & `endi_celery-6.6.5/endi_celery/parsers/sage_generation_expert.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/tasks/__init__.py` & `endi_celery-6.6.5/endi_celery/tasks/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -304,24 +304,24 @@
             "hook_add_row": _add_supplier_invoice_data,
             "foreign_key_name": "supplier_invoice_id",
             "excludes": (
                 "name",
                 "created_at",
                 "updated_at",
                 "type_",
-                "payer",
                 "supplier_orders",
                 "lines",
                 "exports",
                 "exported",
             ),
             "order": (
                 "company",
                 "supplier",
                 "date",
                 "official_number",
                 "remote_invoice_number",
                 "exported",
                 "cae_percentage",
+                "payer",
             ),
         },
     )
```

### Comparing `endi_celery-6.6.4/endi_celery/tasks/accounting_measure_compute.py` & `endi_celery-6.6.5/endi_celery/tasks/accounting_measure_compute.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,17 @@
 
         self.all_type_ids = [t.id for t in self.common_measure_types]
         for types in self.computed_measure_types.values():
             self.all_type_ids.extend([t.id for t in types])
 
         self.processed_grids = []
 
+    def get_message(self, grids: list) -> str:
+        return ""
+
     def _get_active_type_query(self):
         """
         Build a query to list active measure types
         :returns: An sqlalchemy query object
         """
         if self.measure_type_category_class:
             return (
@@ -487,25 +490,27 @@
         self.session.flush()
         self._cache_grid_totals()
         self._process_computed_measures()
         self.session.flush()
         return [griditem.grid for griditem in self.processed_grids]
 
     def _get_date_to_use_for_grid(self):
-        date_to_use = self.upload.updated_at.date()
         this_year = datetime.datetime.today().year
 
-        # If synchronized accounting and écritures from last year
+        # Si c'est une remontée par api et les écritures datent d'avant cette année
         if (
             self.upload.filetype == AccountingOperationUpload.SYNCHRONIZED_ACCOUNTING
             and self.upload.date.year < this_year
         ):
-            # Only works for 31/12 exercice closure, not a problem as long as
-            # synchronized accounting works year by year
+            # Ne fonctionne que pour les clôtures au 31/12
+            # Fonctionne car les upload se font par année
             date_to_use = datetime.date(day=31, month=12, year=self.upload.date.year)
+        else:
+            # On utilise la date de dépôt des données
+            date_to_use = self.upload.updated_at.date()
 
         return date_to_use
 
 
 class BalanceSheetMeasureCompiler(BaseMeasureCompiler):
     measure_type_class = BalanceSheetMeasureType
     measure_type_category_class = None
@@ -1083,40 +1088,43 @@
 
     operations = collect_operations(compiler_type, upload)
     if not operations:
         logger.error("Can't find any operation")
         transaction.abort()
         return False
 
-    factory = GRID_COMPILERS[compiler_type]
-    try:
-        compiler = factory(upload, operations)
-        grids = compiler.process_datas()
-        messages.append(compiler.get_message(grids))
-    except Exception as exc:
-        logger.exception("Error while generating measures")
-        transaction.abort()
-        message = getattr(exc, "message", str(exc))
-        send_error(
-            request,
-            mail_addresses,
-            factory.label,
-            message,
-        )
-        return False
-    else:
-        logger.info("{0} measure grids were handled".format(len(grids)))
-        if mail:
-            send_success(
+    factories = get_measure_compilers(compiler_type)
+    for factory in factories:
+        try:
+            compiler = factory(upload, operations)
+            grids = compiler.process_datas()
+            messages.append(compiler.get_message(grids))
+        except Exception as exc:
+            logger.exception("Error while generating measures")
+            transaction.abort()
+            message = getattr(exc, "message", str(exc))
+            send_error(
                 request,
                 mail_addresses,
-                compiler.label,
-                compiler.get_message(grids),
+                factory.label,
+                message,
             )
-            logger.info("A success email has been sent to {0}".format(mail_addresses))
+            return False
+        else:
+            logger.info("{0} measure grids were handled".format(len(grids)))
+            if mail:
+                send_success(
+                    request,
+                    mail_addresses,
+                    compiler.label,
+                    compiler.get_message(grids),
+                )
+                logger.info(
+                    "A success email has been sent to {0}".format(mail_addresses)
+                )
 
     transaction.commit()
     logger.info("The transaction has been commited")
     return True
 
 
 LOCK_NAME = "measure_compute"
@@ -1133,20 +1141,15 @@
     logger.info(f"Compiling Accounting States for upload {upload_id}")
     if is_locked(LOCK_NAME):
         logger.error("Other task is running : Cancel")
         return False
 
     acquire_lock(LOCK_NAME)
     try:
-        if grid_type is not None:
-            logger.info(f"  + Only compiling {grid_type} grids")
-            grid_types = [grid_type]
-        else:
-            grid_types = list(GRID_COMPILERS.keys())
-
+        grid_types = get_measure_compilers(grid_type)
         for grid_type in grid_types:
             run_compiler(grid_type, upload_id, mail)
     except Exception:
         logger.exception("Erreur inconnue")
 
     release_lock(LOCK_NAME)
     return True
```

### Comparing `endi_celery-6.6.4/endi_celery/tasks/accounting_parser.py` & `endi_celery-6.6.5/endi_celery/tasks/accounting_parser.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/tasks/csv_import.py` & `endi_celery-6.6.5/endi_celery/tasks/csv_import.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/tasks/export.py` & `endi_celery-6.6.5/endi_celery/tasks/export.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/tasks/mail.py` & `endi_celery-6.6.5/endi_celery/tasks/mail.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/tasks/notification.py` & `endi_celery-6.6.5/endi_celery/tasks/notification.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/tasks/tasks.py` & `endi_celery-6.6.5/endi_celery/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/tasks/utils.py` & `endi_celery-6.6.5/endi_celery/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery/transactional_task.py` & `endi_celery-6.6.5/endi_celery/transactional_task.py`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/endi_celery.egg-info/PKG-INFO` & `endi_celery-6.6.5/endi_celery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endi-celery
-Version: 6.6.4
+Version: 6.6.5
 Summary: endi_celery
 Home-page: https://framagit.org/endi/endi_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `endi_celery-6.6.4/endi_celery.egg-info/SOURCES.txt` & `endi_celery-6.6.5/endi_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/prod_example.ini` & `endi_celery-6.6.5/prod_example.ini`

 * *Files identical despite different names*

### Comparing `endi_celery-6.6.4/setup.py` & `endi_celery-6.6.5/setup.py`

 * *Files identical despite different names*

