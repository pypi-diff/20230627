# Comparing `tmp/mds_account_primanota-6.8.6.tar.gz` & `tmp/mds_account_primanota-6.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_account_primanota-6.8.6.tar", last modified: Tue Jun 27 08:43:12 2023, max compression
+gzip compressed data, was "mds_account_primanota-6.8.7.tar", last modified: Tue Jun 27 14:19:44 2023, max compression
```

## Comparing `mds_account_primanota-6.8.6.tar` & `mds_account_primanota-6.8.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 08:43:12.015759 mds_account_primanota-6.8.6/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1544 2023-06-27 08:43:12.015759 mds_account_primanota-6.8.6/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      286 2023-06-27 08:41:12.000000 mds_account_primanota-6.8.6/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      614 2023-06-19 11:32:35.000000 mds_account_primanota-6.8.6/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2688 2023-06-19 11:33:26.000000 mds_account_primanota-6.8.6/analytic.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1010 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/analytic.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 08:43:12.011759 mds_account_primanota-6.8.6/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     7464 2023-06-27 08:40:23.000000 mds_account_primanota-6.8.6/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6818 2023-06-27 08:40:23.000000 mds_account_primanota-6.8.6/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 08:43:12.015759 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1544 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      728 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      572 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/menu.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    13358 2023-06-27 08:40:23.000000 mds_account_primanota-6.8.6/primanota.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2577 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/primanota.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-27 08:43:12.015759 mds_account_primanota-6.8.6/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3703 2023-06-19 11:35:07.000000 mds_account_primanota-6.8.6/setup.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 08:43:12.011759 mds_account_primanota-6.8.6/tests/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      144 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    12585 2023-06-27 08:40:23.000000 mds_account_primanota-6.8.6/tests/test_primanota.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      134 2023-06-27 08:41:20.000000 mds_account_primanota-6.8.6/tryton.cfg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 08:43:12.011759 mds_account_primanota-6.8.6/view/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      505 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/analytic_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      377 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/analytic_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      358 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/analyticline_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      700 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/primanota_context_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2449 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/primanota_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1081 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/primanota_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      316 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/taxline_list.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 14:19:44.649130 mds_account_primanota-6.8.7/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1649 2023-06-27 14:19:44.649130 mds_account_primanota-6.8.7/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      359 2023-06-27 14:18:54.000000 mds_account_primanota-6.8.7/README.rst
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      614 2023-06-19 11:32:35.000000 mds_account_primanota-6.8.7/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2688 2023-06-19 11:33:26.000000 mds_account_primanota-6.8.7/analytic.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1010 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.7/analytic.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 14:19:44.645130 mds_account_primanota-6.8.7/locale/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7476 2023-06-27 14:17:49.000000 mds_account_primanota-6.8.7/locale/de.po
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6830 2023-06-27 14:17:49.000000 mds_account_primanota-6.8.7/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 14:19:44.649130 mds_account_primanota-6.8.7/mds_account_primanota.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1649 2023-06-27 14:19:44.000000 mds_account_primanota-6.8.7/mds_account_primanota.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      728 2023-06-27 14:19:44.000000 mds_account_primanota-6.8.7/mds_account_primanota.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-27 14:19:44.000000 mds_account_primanota-6.8.7/mds_account_primanota.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-06-27 14:19:44.000000 mds_account_primanota-6.8.7/mds_account_primanota.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-27 14:19:44.000000 mds_account_primanota-6.8.7/mds_account_primanota.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-27 14:19:44.000000 mds_account_primanota-6.8.7/mds_account_primanota.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-27 14:19:44.000000 mds_account_primanota-6.8.7/mds_account_primanota.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      572 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.7/menu.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    14032 2023-06-27 14:17:49.000000 mds_account_primanota-6.8.7/primanota.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2577 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.7/primanota.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-27 14:19:44.649130 mds_account_primanota-6.8.7/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3703 2023-06-19 11:35:07.000000 mds_account_primanota-6.8.7/setup.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 14:19:44.645130 mds_account_primanota-6.8.7/tests/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      144 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.7/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    19676 2023-06-27 14:17:49.000000 mds_account_primanota-6.8.7/tests/test_primanota.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      134 2023-06-27 14:18:21.000000 mds_account_primanota-6.8.7/tryton.cfg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.7/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 14:19:44.645130 mds_account_primanota-6.8.7/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      505 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.7/view/analytic_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      377 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.7/view/analytic_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      358 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.7/view/analyticline_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      700 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.7/view/primanota_context_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2449 2023-06-27 10:55:51.000000 mds_account_primanota-6.8.7/view/primanota_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1081 2023-06-27 10:55:52.000000 mds_account_primanota-6.8.7/view/primanota_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      316 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.7/view/taxline_list.xml
```

### Comparing `mds_account_primanota-6.8.6/PKG-INFO` & `mds_account_primanota-6.8.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mds_account_primanota
-Version: 6.8.6
+Version: 6.8.7
 Summary: Tryton module to add a primanota-view.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-account-primanota
         =====================
@@ -18,14 +18,18 @@
         Requires
         ========
         - Tryton 6.8
         
         Changes
         =======
         
+        *6.8.7 - 27.06.2023*
+        
+        - updt: field 'origin_party' --> 'origin_parties'
+        
         *6.8.6 - 27.06.2023*
         
         - add: fields - move, move_parties, origin_party
         
         *6.8.5 - 19.06.2023*
         
         - init
```

### Comparing `mds_account_primanota-6.8.6/__init__.py` & `mds_account_primanota-6.8.7/__init__.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.6/analytic.py` & `mds_account_primanota-6.8.7/analytic.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.6/analytic.xml` & `mds_account_primanota-6.8.7/analytic.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.6/locale/de.po` & `mds_account_primanota-6.8.7/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -207,21 +207,21 @@
 msgid "Parties of account move"
 msgstr "Parteien des Buchungssatzes"
 
 msgctxt "help:account_primanota.primanota,move_parties:"
 msgid "Contains the parties from the posting record lines."
 msgstr "enthält die Parteien aus den Buchungssatzzeilen."
 
-msgctxt "field:account_primanota.primanota,origin_party:"
-msgid "Party of Origin"
-msgstr "Partei der Herkunft"
-
-msgctxt "help:account_primanota.primanota,origin_party:"
-msgid "Party of the origin data record, if existing"
-msgstr "Partei des Herkunftdatensatzes, sofern existent"
+msgctxt "field:account_primanota.primanota,origin_parties:"
+msgid "Parties of Origin"
+msgstr "Parteien der Herkunft"
+
+msgctxt "help:account_primanota.primanota,origin_parties:"
+msgid "Parties of the origin data record, if existing"
+msgstr "Parteien des Herkunftdatensatzes, sofern existent"
 
 msgctxt "field:account_primanota.primanota,move:"
 msgid "Move"
 msgstr "Buchungssatz"
 
 
 #######################################
```

### Comparing `mds_account_primanota-6.8.6/locale/en.po` & `mds_account_primanota-6.8.7/locale/en.po`

 * *Files 8% similar despite different names*

```diff
@@ -202,21 +202,21 @@
 msgid "Parties of account move"
 msgstr "Parties of account move"
 
 msgctxt "help:account_primanota.primanota,move_parties:"
 msgid "Contains the parties from the posting record lines."
 msgstr "Contains the parties from the posting record lines."
 
-msgctxt "field:account_primanota.primanota,origin_party:"
-msgid "Party of Origin"
-msgstr "Party of Origin"
+msgctxt "field:account_primanota.primanota,origin_parties:"
+msgid "Parties of Origin"
+msgstr "Parties of Origin"
 
-msgctxt "help:account_primanota.primanota,origin_party:"
-msgid "Party of the origin data record, if existing"
-msgstr "Party of the origin data record, if existing"
+msgctxt "help:account_primanota.primanota,origin_parties:"
+msgid "Parties of the origin data record, if existing"
+msgstr "Parties of the origin data record, if existing"
 
 msgctxt "field:account_primanota.primanota,move:"
 msgid "Move"
 msgstr "Move"
 
 msgctxt "model:account_primanota.primanota.context,name:"
 msgid "Primanota Context"
```

### Comparing `mds_account_primanota-6.8.6/mds_account_primanota.egg-info/PKG-INFO` & `mds_account_primanota-6.8.7/mds_account_primanota.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mds-account-primanota
-Version: 6.8.6
+Version: 6.8.7
 Summary: Tryton module to add a primanota-view.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-account-primanota
         =====================
@@ -18,14 +18,18 @@
         Requires
         ========
         - Tryton 6.8
         
         Changes
         =======
         
+        *6.8.7 - 27.06.2023*
+        
+        - updt: field 'origin_party' --> 'origin_parties'
+        
         *6.8.6 - 27.06.2023*
         
         - add: fields - move, move_parties, origin_party
         
         *6.8.5 - 19.06.2023*
         
         - init
```

### Comparing `mds_account_primanota-6.8.6/mds_account_primanota.egg-info/SOURCES.txt` & `mds_account_primanota-6.8.7/mds_account_primanota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.6/menu.xml` & `mds_account_primanota-6.8.7/menu.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.6/primanota.py` & `mds_account_primanota-6.8.7/primanota.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,26 +30,31 @@
         string='Period', readonly=True, model_name='account.period')
     journal = fields.Many2One(
         string='Journal', readonly=True, model_name='account.journal')
     date = fields.Date(string='Effective Date', readonly=True)
     post_date = fields.Date(string='Post Date', readonly=True)
     description = fields.Char(string='Description', readonly=True)
     line_description = fields.Char(string='Line Description', readonly=True)
+
+    # origin as function-field because search dont work in
+    # reference in list-view of client
+    # and we need to update the clause
     origin2 = fields.Reference(
         string='Origin', selection='get_move_originsel', readonly=True)
     origin = fields.Function(fields.Reference(
         string='Origin', help='Origin of the Move',
         selection='get_move_originsel', readonly=True),
         'on_change_with_origin', searcher='search_origin')
     line_origin2 = fields.Reference(
         string='Line Origin', selection='get_line_originsel', readonly=True)
     line_origin = fields.Function(fields.Reference(
         string='Line Origin', help='Origin of the Moveline',
         selection='get_line_originsel', readonly=True),
         'on_change_with_line_origin', searcher='search_line_origin')
+
     state = fields.Selection(
         string='State', readonly=True, selection=[
             ('draft', 'Draft'),
             ('posted', 'Posted'),
         ])
     debit = fields.Numeric(
         string='Debit', readonly=True, depends=['currency_digits'],
@@ -91,21 +96,21 @@
     second_currency_digits = fields.Function(fields.Integer(
         string='Second Currency Digits'),
         'on_change_with_second_currency_digits')
 
     move_parties = fields.Function(fields.One2Many(
         string='Parties of account move', field=None,
         help='Contains the parties from the posting record lines.',
-        model_name='party.party'),
+        model_name='party.party', readonly=True),
         'on_change_with_move_parties')
-    origin_party = fields.Function(fields.Many2One(
-        string='Party of Origin', model_name='party.party',
-        readonly=True,
-        help='Party of the origin data record, if existing'),
-        'on_change_with_origin_party')
+    origin_parties = fields.Function(fields.One2Many(
+        string='Parties of Origin', field=None,
+        help='Parties of the origin data record, if existing',
+        model_name='party.party', readonly=True),
+        'on_change_with_origin_parties')
 
     _model_has_field_cache = Cache(
         'account_primanota.primanota.model_has_field')
 
     @classmethod
     def __setup__(cls):
         super(PrimaNota, cls).__setup__()
@@ -238,23 +243,37 @@
 
         if self.move:
             return [
                 x.party.id
                 for x in AccountMoveLine.search([
                         ('move', '=', self.move.id),
                         ('party', '!=', None),
-                    ])]
+                    ], order=[('party.name', 'ASC')])]
         return []
 
     @fields.depends('line_origin2')
-    def on_change_with_origin_party(self, name=None):
+    def on_change_with_origin_parties(self, name=None):
         """ get field 'party' from origin if exists
         """
-        return getattr(getattr(
-            self.line_origin2, 'party', None), 'id', None)
+        result = []
+
+        # party-field at origin
+        party = getattr(getattr(self.line_origin2, 'party', None), 'id', None)
+        if party:
+            result.append(party)
+
+        # 'origin' has lines with party-field
+        lines = getattr(self.line_origin2, 'lines', [])
+        if isinstance(lines, (list, tuple)):
+            for line in lines:
+                party = getattr(line, 'party', None)
+                if party:
+                    if party.id not in result:
+                        result.append(party.id)
+        return result
 
     @classmethod
     def get_move_originsel(cls):
         """ get list of selections
         """
         AccountMove = Pool().get('account.move')
         return AccountMove.get_origin()
```

### Comparing `mds_account_primanota-6.8.6/primanota.xml` & `mds_account_primanota-6.8.7/primanota.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.6/setup.py` & `mds_account_primanota-6.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.6/view/primanota_context_form.xml` & `mds_account_primanota-6.8.7/view/primanota_context_form.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.6/view/primanota_form.xml` & `mds_account_primanota-6.8.7/view/primanota_form.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.6/view/primanota_list.xml` & `mds_account_primanota-6.8.7/view/primanota_list.xml`

 * *Files identical despite different names*

