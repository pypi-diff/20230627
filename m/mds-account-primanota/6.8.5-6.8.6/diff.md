# Comparing `tmp/mds_account_primanota-6.8.5.tar.gz` & `tmp/mds_account_primanota-6.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_account_primanota-6.8.5.tar", last modified: Mon Jun 19 11:36:10 2023, max compression
+gzip compressed data, was "mds_account_primanota-6.8.6.tar", last modified: Tue Jun 27 08:43:12 2023, max compression
```

## Comparing `mds_account_primanota-6.8.5.tar` & `mds_account_primanota-6.8.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:36:10.642758 mds_account_primanota-6.8.5/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1440 2023-06-19 11:36:10.642758 mds_account_primanota-6.8.5/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      214 2023-06-19 11:35:22.000000 mds_account_primanota-6.8.5/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      614 2023-06-19 11:32:35.000000 mds_account_primanota-6.8.5/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2688 2023-06-19 11:33:26.000000 mds_account_primanota-6.8.5/analytic.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1010 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/analytic.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:36:10.638758 mds_account_primanota-6.8.5/locale/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6793 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/locale/de.po
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6164 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:36:10.642758 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1440 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      728 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      572 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/menu.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    12045 2023-06-19 11:32:03.000000 mds_account_primanota-6.8.5/primanota.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2577 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/primanota.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-19 11:36:10.642758 mds_account_primanota-6.8.5/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3703 2023-06-19 11:35:07.000000 mds_account_primanota-6.8.5/setup.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:36:10.638758 mds_account_primanota-6.8.5/tests/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      144 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11780 2023-06-19 11:32:07.000000 mds_account_primanota-6.8.5/tests/test_primanota.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      133 2023-06-19 11:34:53.000000 mds_account_primanota-6.8.5/tryton.cfg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:36:10.638758 mds_account_primanota-6.8.5/view/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      505 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/analytic_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      377 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/analytic_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      358 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/analyticline_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      700 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/primanota_context_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2449 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/primanota_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1081 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/primanota_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      316 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/taxline_list.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 08:43:12.015759 mds_account_primanota-6.8.6/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1544 2023-06-27 08:43:12.015759 mds_account_primanota-6.8.6/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      286 2023-06-27 08:41:12.000000 mds_account_primanota-6.8.6/README.rst
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      614 2023-06-19 11:32:35.000000 mds_account_primanota-6.8.6/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2688 2023-06-19 11:33:26.000000 mds_account_primanota-6.8.6/analytic.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1010 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/analytic.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 08:43:12.011759 mds_account_primanota-6.8.6/locale/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7464 2023-06-27 08:40:23.000000 mds_account_primanota-6.8.6/locale/de.po
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6818 2023-06-27 08:40:23.000000 mds_account_primanota-6.8.6/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 08:43:12.015759 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1544 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      728 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-27 08:43:11.000000 mds_account_primanota-6.8.6/mds_account_primanota.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      572 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/menu.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    13358 2023-06-27 08:40:23.000000 mds_account_primanota-6.8.6/primanota.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2577 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/primanota.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-27 08:43:12.015759 mds_account_primanota-6.8.6/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3703 2023-06-19 11:35:07.000000 mds_account_primanota-6.8.6/setup.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 08:43:12.011759 mds_account_primanota-6.8.6/tests/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      144 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    12585 2023-06-27 08:40:23.000000 mds_account_primanota-6.8.6/tests/test_primanota.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      134 2023-06-27 08:41:20.000000 mds_account_primanota-6.8.6/tryton.cfg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-27 08:43:12.011759 mds_account_primanota-6.8.6/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      505 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/analytic_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      377 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/analytic_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      358 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/analyticline_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      700 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/primanota_context_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2449 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/primanota_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1081 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/primanota_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      316 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.6/view/taxline_list.xml
```

### Comparing `mds_account_primanota-6.8.5/PKG-INFO` & `mds_account_primanota-6.8.6/mds_account_primanota.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds_account_primanota
-Version: 6.8.5
+Name: mds-account-primanota
+Version: 6.8.6
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
         
+        *6.8.6 - 27.06.2023*
+        
+        - add: fields - move, move_parties, origin_party
+        
         *6.8.5 - 19.06.2023*
         
         - init
         
 Keywords: tryton account primanota
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mds_account_primanota-6.8.5/__init__.py` & `mds_account_primanota-6.8.6/__init__.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.5/analytic.py` & `mds_account_primanota-6.8.6/analytic.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.5/analytic.xml` & `mds_account_primanota-6.8.6/analytic.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.5/locale/de.po` & `mds_account_primanota-6.8.6/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,34 @@
 msgid "Analytic Lines"
 msgstr "Kostenstellen"
 
 msgctxt "help:account_primanota.primanota,has_analytic_lines:"
 msgid "Account move line has analytic lines."
 msgstr "Buchungszeile hat Kostenstellenzeilen."
 
+msgctxt "field:account_primanota.primanota,move_parties:"
+msgid "Parties of account move"
+msgstr "Parteien des Buchungssatzes"
+
+msgctxt "help:account_primanota.primanota,move_parties:"
+msgid "Contains the parties from the posting record lines."
+msgstr "enthält die Parteien aus den Buchungssatzzeilen."
+
+msgctxt "field:account_primanota.primanota,origin_party:"
+msgid "Party of Origin"
+msgstr "Partei der Herkunft"
+
+msgctxt "help:account_primanota.primanota,origin_party:"
+msgid "Party of the origin data record, if existing"
+msgstr "Partei des Herkunftdatensatzes, sofern existent"
+
+msgctxt "field:account_primanota.primanota,move:"
+msgid "Move"
+msgstr "Buchungssatz"
+
 
 #######################################
 # account_primanota.primanota.context #
 #######################################
 msgctxt "model:account_primanota.primanota.context,name:"
 msgid "Primanota Context"
 msgstr "Primanota Kontext"
```

### Comparing `mds_account_primanota-6.8.5/locale/en.po` & `mds_account_primanota-6.8.6/locale/en.po`

 * *Files 3% similar despite different names*

```diff
@@ -194,14 +194,34 @@
 msgid "Analytic Lines"
 msgstr "Analytic Lines"
 
 msgctxt "help:account_primanota.primanota,has_analytic_lines:"
 msgid "Account move line has analytic lines."
 msgstr "Account move line has analytic lines."
 
+msgctxt "field:account_primanota.primanota,move_parties:"
+msgid "Parties of account move"
+msgstr "Parties of account move"
+
+msgctxt "help:account_primanota.primanota,move_parties:"
+msgid "Contains the parties from the posting record lines."
+msgstr "Contains the parties from the posting record lines."
+
+msgctxt "field:account_primanota.primanota,origin_party:"
+msgid "Party of Origin"
+msgstr "Party of Origin"
+
+msgctxt "help:account_primanota.primanota,origin_party:"
+msgid "Party of the origin data record, if existing"
+msgstr "Party of the origin data record, if existing"
+
+msgctxt "field:account_primanota.primanota,move:"
+msgid "Move"
+msgstr "Move"
+
 msgctxt "model:account_primanota.primanota.context,name:"
 msgid "Primanota Context"
 msgstr "Primanota Context"
 
 msgctxt "field:account_primanota.primanota.context,company:"
 msgid "Company"
 msgstr "Company"
```

### Comparing `mds_account_primanota-6.8.5/mds_account_primanota.egg-info/PKG-INFO` & `mds_account_primanota-6.8.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds-account-primanota
-Version: 6.8.5
+Name: mds_account_primanota
+Version: 6.8.6
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
         
+        *6.8.6 - 27.06.2023*
+        
+        - add: fields - move, move_parties, origin_party
+        
         *6.8.5 - 19.06.2023*
         
         - init
         
 Keywords: tryton account primanota
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mds_account_primanota-6.8.5/mds_account_primanota.egg-info/SOURCES.txt` & `mds_account_primanota-6.8.6/mds_account_primanota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.5/menu.xml` & `mds_account_primanota-6.8.6/menu.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.5/primanota.py` & `mds_account_primanota-6.8.6/primanota.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 class PrimaNota(ModelSQL, ModelView):
     'Primanota'
     __name__ = 'account_primanota.primanota'
 
     movenumber = fields.Char(
         string='Number', readonly=True, help='Number of Move')
+    move = fields.Many2One(
+        string='Move', readonly=True, model_name='account.move')
     post_number = fields.Char(
         string='Post Number', readonly=True,
         help='Also known as Folio Number.')
     period = fields.Many2One(
         string='Period', readonly=True, model_name='account.period')
     journal = fields.Many2One(
         string='Journal', readonly=True, model_name='account.journal')
@@ -86,14 +88,25 @@
     currency_digits = fields.Function(fields.Integer(
         string='Currency Digits'),
         'on_change_with_currency_digits')
     second_currency_digits = fields.Function(fields.Integer(
         string='Second Currency Digits'),
         'on_change_with_second_currency_digits')
 
+    move_parties = fields.Function(fields.One2Many(
+        string='Parties of account move', field=None,
+        help='Contains the parties from the posting record lines.',
+        model_name='party.party'),
+        'on_change_with_move_parties')
+    origin_party = fields.Function(fields.Many2One(
+        string='Party of Origin', model_name='party.party',
+        readonly=True,
+        help='Party of the origin data record, if existing'),
+        'on_change_with_origin_party')
+
     _model_has_field_cache = Cache(
         'account_primanota.primanota.model_has_field')
 
     @classmethod
     def __setup__(cls):
         super(PrimaNota, cls).__setup__()
         cls._order.insert(0, ('date', 'DESC'))
@@ -213,14 +226,36 @@
     @fields.depends('second_currency')
     def on_change_with_second_currency_digits(self, name=None):
         if self.second_currency:
             return self.second_currency.digits
         else:
             return 2
 
+    @fields.depends('move')
+    def on_change_with_move_parties(self, name=None):
+        """ get parties of move
+        """
+        AccountMoveLine = Pool().get('account.move.line')
+
+        if self.move:
+            return [
+                x.party.id
+                for x in AccountMoveLine.search([
+                        ('move', '=', self.move.id),
+                        ('party', '!=', None),
+                    ])]
+        return []
+
+    @fields.depends('line_origin2')
+    def on_change_with_origin_party(self, name=None):
+        """ get field 'party' from origin if exists
+        """
+        return getattr(getattr(
+            self.line_origin2, 'party', None), 'id', None)
+
     @classmethod
     def get_move_originsel(cls):
         """ get list of selections
         """
         AccountMove = Pool().get('account.move')
         return AccountMove.get_origin()
 
@@ -283,14 +318,15 @@
             ).select(
                 tab_mvline.id,
                 tab_mvline.create_uid,
                 tab_mvline.create_date,
                 tab_mvline.write_uid,
                 tab_mvline.write_date,
                 tab_move.number.as_('movenumber'),
+                tab_move.id.as_('move'),
                 tab_move.post_number,
                 tab_move.period,
                 tab_move.journal,
                 tab_move.date,
                 tab_move.post_date,
                 tab_move.description,
                 tab_move.origin.as_('origin2'),
```

### Comparing `mds_account_primanota-6.8.5/primanota.xml` & `mds_account_primanota-6.8.6/primanota.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.5/setup.py` & `mds_account_primanota-6.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.5/tests/test_primanota.py` & `mds_account_primanota-6.8.6/tests/test_primanota.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,31 +130,38 @@
                         'credit': Decimal('10.0'),
                         'account': account_lst[1].id,
                         'description': 'Line 2',
                         'party': company1.party.id,
                         }])],
                     }])
                 self.assertEqual(len(am_rec), 1)
+
+                # origin with itself
                 am_rec[0].origin = am_rec[0]
                 am_rec[0].save()
                 am_rec[0].lines[0].origin = am_rec[0].lines[1]
                 am_rec[0].lines[0].save()
+                am_rec[0].lines[1].origin = am_rec[0].lines[0]
+                am_rec[0].lines[1].save()
+
                 AccountMove.post(am_rec)
 
                 pm_lst = PrimaNota.search([])
                 self.assertEqual(len(pm_lst), 2)
 
                 # 2
+                self.assertEqual(pm_lst[0].move.description, 'Test 1')
                 self.assertEqual(pm_lst[0].period.rec_name, '2020-05')
                 self.assertEqual(pm_lst[0].journal.rec_name, 'Revenue')
                 self.assertEqual(pm_lst[0].date, date(2020, 5, 1))
                 self.assertEqual(pm_lst[0].description, 'Test 1')
                 self.assertEqual(pm_lst[0].line_description, 'Line 2')
                 self.assertEqual(pm_lst[0].origin.description, 'Test 1')
                 self.assertEqual(pm_lst[0].line_origin.description, 'Line 1')
+                self.assertEqual(pm_lst[0].origin_party, None)
                 self.assertEqual(pm_lst[0].state, 'posted')
                 self.assertEqual(pm_lst[0].debit, Decimal('0.0'))
                 self.assertEqual(pm_lst[0].credit, Decimal('10.0'))
                 self.assertEqual(
                     pm_lst[0].account.rec_name,
                     '002 - Main Receivable')
                 self.assertEqual(pm_lst[0].account_code, '002')
@@ -172,23 +179,29 @@
                     pm_lst[0].rec_name,
                     '%(mvno)s [%(psno)s] 05/01/2020 002 usd0.00/usd10.00' % {
                         'mvno': pm_lst[0].movenumber,
                         'psno': pm_lst[0].post_number,
                         })
                 self.assertEqual(pm_lst[0].has_analytic_lines, False)
                 self.assertEqual(len(pm_lst[0].analytic_lines), 0)
+                self.assertEqual(len(pm_lst[0].move_parties), 1)
+                self.assertEqual(
+                    pm_lst[0].move_parties[0].rec_name,
+                    'm-ds')
 
                 # 1
+                self.assertEqual(pm_lst[1].move.description, 'Test 1')
                 self.assertEqual(pm_lst[1].period.rec_name, '2020-05')
                 self.assertEqual(pm_lst[1].journal.rec_name, 'Revenue')
                 self.assertEqual(pm_lst[1].date, date(2020, 5, 1))
                 self.assertEqual(pm_lst[1].description, 'Test 1')
                 self.assertEqual(pm_lst[1].line_description, 'Line 1')
                 self.assertEqual(pm_lst[1].origin.description, 'Test 1')
-                self.assertEqual(pm_lst[1].line_origin, None)
+                self.assertEqual(pm_lst[1].line_origin.description, 'Line 2')
+                self.assertEqual(pm_lst[1].origin_party.rec_name, 'm-ds')
                 self.assertEqual(pm_lst[1].state, 'posted')
                 self.assertEqual(pm_lst[1].debit, Decimal('10.0'))
                 self.assertEqual(pm_lst[1].credit, Decimal('0.0'))
                 self.assertEqual(
                     pm_lst[1].account.rec_name,
                     '003 - Main Revenue')
                 self.assertEqual(pm_lst[1].account_code, '003')
@@ -212,14 +225,18 @@
                         'psno': pm_lst[1].post_number,
                         })
                 self.assertEqual(pm_lst[1].has_analytic_lines, True)
                 self.assertEqual(len(pm_lst[1].analytic_lines), 1)
                 self.assertEqual(
                     pm_lst[1].analytic_lines[0].account.code,
                     'K001')
+                self.assertEqual(len(pm_lst[1].move_parties), 1)
+                self.assertEqual(
+                    pm_lst[1].move_parties[0].rec_name,
+                    'm-ds')
 
                 # searcher
                 # search in party
                 self.assertEqual(PrimaNota.search_count([
                     ('rec_name', '=', 'm-ds')]), 1)
                 # post-number/move-number
                 self.assertEqual(PrimaNota.search_count([
```

### Comparing `mds_account_primanota-6.8.5/view/primanota_context_form.xml` & `mds_account_primanota-6.8.6/view/primanota_context_form.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.5/view/primanota_form.xml` & `mds_account_primanota-6.8.6/view/primanota_form.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.8.5/view/primanota_list.xml` & `mds_account_primanota-6.8.6/view/primanota_list.xml`

 * *Files identical despite different names*

