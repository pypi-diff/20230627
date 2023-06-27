# Comparing `tmp/mds_account_primanota-6.6.5.tar.gz` & `tmp/mds_account_primanota-6.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_account_primanota-6.6.5.tar", last modified: Mon Jun 19 11:43:43 2023, max compression
+gzip compressed data, was "mds_account_primanota-6.8.5.tar", last modified: Mon Jun 19 11:36:10 2023, max compression
```

## Comparing `mds_account_primanota-6.6.5.tar` & `mds_account_primanota-6.8.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:43:43.973666 mds_account_primanota-6.6.5/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1621 2023-06-19 11:43:43.973666 mds_account_primanota-6.6.5/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      381 2023-06-19 11:42:06.000000 mds_account_primanota-6.6.5/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      614 2023-06-19 11:39:52.000000 mds_account_primanota-6.6.5/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2688 2023-06-19 11:39:52.000000 mds_account_primanota-6.6.5/analytic.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1010 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.5/analytic.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:43:43.949666 mds_account_primanota-6.6.5/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6793 2023-06-14 14:40:56.000000 mds_account_primanota-6.6.5/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6164 2023-06-14 14:40:56.000000 mds_account_primanota-6.6.5/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:43:43.973666 mds_account_primanota-6.6.5/mds_account_primanota.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1621 2023-06-19 11:43:43.000000 mds_account_primanota-6.6.5/mds_account_primanota.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      728 2023-06-19 11:43:43.000000 mds_account_primanota-6.6.5/mds_account_primanota.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:43:43.000000 mds_account_primanota-6.6.5/mds_account_primanota.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-06-19 11:43:43.000000 mds_account_primanota-6.6.5/mds_account_primanota.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:43:43.000000 mds_account_primanota-6.6.5/mds_account_primanota.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-19 11:43:43.000000 mds_account_primanota-6.6.5/mds_account_primanota.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-19 11:43:43.000000 mds_account_primanota-6.6.5/mds_account_primanota.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      572 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.5/menu.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    12045 2023-06-19 11:39:52.000000 mds_account_primanota-6.6.5/primanota.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2577 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.5/primanota.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-19 11:43:43.973666 mds_account_primanota-6.6.5/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3654 2023-06-19 11:40:24.000000 mds_account_primanota-6.6.5/setup.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:43:43.961666 mds_account_primanota-6.6.5/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      144 2023-06-14 14:41:09.000000 mds_account_primanota-6.6.5/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11788 2023-06-19 11:39:52.000000 mds_account_primanota-6.6.5/tests/test_primanota.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      133 2023-06-19 11:41:47.000000 mds_account_primanota-6.6.5/tryton.cfg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.5/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:43:43.969666 mds_account_primanota-6.6.5/view/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      505 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.5/view/analytic_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      377 2023-06-14 14:55:22.000000 mds_account_primanota-6.6.5/view/analytic_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      358 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.5/view/analyticline_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      700 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.5/view/primanota_context_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2449 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.5/view/primanota_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1081 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.5/view/primanota_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      316 2023-04-06 08:58:35.000000 mds_account_primanota-6.6.5/view/taxline_list.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:36:10.642758 mds_account_primanota-6.8.5/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1440 2023-06-19 11:36:10.642758 mds_account_primanota-6.8.5/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      214 2023-06-19 11:35:22.000000 mds_account_primanota-6.8.5/README.rst
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      614 2023-06-19 11:32:35.000000 mds_account_primanota-6.8.5/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2688 2023-06-19 11:33:26.000000 mds_account_primanota-6.8.5/analytic.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1010 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/analytic.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:36:10.638758 mds_account_primanota-6.8.5/locale/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6793 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/locale/de.po
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6164 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:36:10.642758 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1440 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      728 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-19 11:36:10.000000 mds_account_primanota-6.8.5/mds_account_primanota.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      572 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/menu.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    12045 2023-06-19 11:32:03.000000 mds_account_primanota-6.8.5/primanota.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2577 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/primanota.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-19 11:36:10.642758 mds_account_primanota-6.8.5/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3703 2023-06-19 11:35:07.000000 mds_account_primanota-6.8.5/setup.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:36:10.638758 mds_account_primanota-6.8.5/tests/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      144 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    11780 2023-06-19 11:32:07.000000 mds_account_primanota-6.8.5/tests/test_primanota.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      133 2023-06-19 11:34:53.000000 mds_account_primanota-6.8.5/tryton.cfg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-19 11:36:10.638758 mds_account_primanota-6.8.5/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      505 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/analytic_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      377 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/analytic_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      358 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/analyticline_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      700 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/primanota_context_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2449 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/primanota_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1081 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/primanota_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      316 2023-06-19 11:01:40.000000 mds_account_primanota-6.8.5/view/taxline_list.xml
```

### Comparing `mds_account_primanota-6.6.5/PKG-INFO` & `mds_account_primanota-6.8.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mds_account_primanota
-Version: 6.6.5
+Version: 6.8.5
 Summary: Tryton module to add a primanota-view.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-account-primanota
         =====================
@@ -13,30 +13,22 @@
         Install
         =======
         
         pip install mds-account-primanota
         
         Requires
         ========
-        - Tryton 6.6
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.6.5 - 19.06.2023*
+        *6.8.5 - 19.06.2023*
         
-        - copde optmimized
-        
-        *6.6.4 - 14.06.2023*
-        
-        - add: column 'analytic lines' - to search for existing/missing analytic-lines
-        
-        *6.6.3 - 06.04.2023*
-        
-        - compatibility to Tryton 6.6
+        - init
         
 Keywords: tryton account primanota
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,7 +39,8 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Natural Language :: German
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mds_account_primanota-6.6.5/__init__.py` & `mds_account_primanota-6.8.5/__init__.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/analytic.py` & `mds_account_primanota-6.8.5/analytic.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/analytic.xml` & `mds_account_primanota-6.8.5/analytic.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/locale/de.po` & `mds_account_primanota-6.8.5/locale/de.po`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/locale/en.po` & `mds_account_primanota-6.8.5/locale/en.po`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/mds_account_primanota.egg-info/PKG-INFO` & `mds_account_primanota-6.8.5/mds_account_primanota.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mds-account-primanota
-Version: 6.6.5
+Version: 6.8.5
 Summary: Tryton module to add a primanota-view.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-account-primanota
         =====================
@@ -13,30 +13,22 @@
         Install
         =======
         
         pip install mds-account-primanota
         
         Requires
         ========
-        - Tryton 6.6
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.6.5 - 19.06.2023*
+        *6.8.5 - 19.06.2023*
         
-        - copde optmimized
-        
-        *6.6.4 - 14.06.2023*
-        
-        - add: column 'analytic lines' - to search for existing/missing analytic-lines
-        
-        *6.6.3 - 06.04.2023*
-        
-        - compatibility to Tryton 6.6
+        - init
         
 Keywords: tryton account primanota
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,7 +39,8 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Natural Language :: German
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mds_account_primanota-6.6.5/mds_account_primanota.egg-info/SOURCES.txt` & `mds_account_primanota-6.8.5/mds_account_primanota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/menu.xml` & `mds_account_primanota-6.8.5/menu.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/primanota.py` & `mds_account_primanota-6.8.5/primanota.py`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/primanota.xml` & `mds_account_primanota-6.8.5/primanota.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/setup.py` & `mds_account_primanota-6.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
         modversion[l2[0]] = {'min': l2[1], 'max': l2[2], 'prefix': l2[3]}
 
 # tryton-version
 major_version = 6
-minor_version = 6
+minor_version = 8
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res|webdav)(\W|$)', dep):
         if dep in modversion.keys():
             prefix = 'mds'
             if len(modversion[dep]['prefix']) > 0:
@@ -85,14 +85,15 @@
         'Topic :: Office/Business :: Financial :: Accounting',
         'Natural Language :: German',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: GNU General Public License (GPL)',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
 
     keywords='tryton account primanota',
     package_dir={'trytond.modules.%s' % MODULE: '.'},
     packages=[
         'trytond.modules.%s' % MODULE,
         ],
```

### Comparing `mds_account_primanota-6.6.5/tests/test_primanota.py` & `mds_account_primanota-6.8.5/tests/test_primanota.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is part of the prima-nota-module for Tryton from m-ds.de.
 # The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from trytond.tests.test_tryton import (
-    ModuleTestCase, with_transaction, activate_module, drop_db)
+    ModuleTestCase, with_transaction, activate_module)
 from trytond.pool import Pool
 from trytond.transaction import Transaction
 from trytond.modules.company.tests import create_company, set_company
 from trytond.modules.account.tests import create_chart, get_fiscalyear
 from datetime import date
 from decimal import Decimal
 from unittest.mock import MagicMock
@@ -16,15 +16,15 @@
 
 class PMTestCase(ModuleTestCase):
     'Test pm module'
     module = 'account_primanota'
 
     @classmethod
     def setUpClass(cls):
-        """ add modules
+        """ add modelues
         """
         super(PMTestCase, cls).setUpClass()
         activate_module(['analytic_account'])
 
     def prep_fiscalyear(self, company1):
         """ prepare fiscal year, sequences...
         """
```

### Comparing `mds_account_primanota-6.6.5/view/primanota_context_form.xml` & `mds_account_primanota-6.8.5/view/primanota_context_form.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/view/primanota_form.xml` & `mds_account_primanota-6.8.5/view/primanota_form.xml`

 * *Files identical despite different names*

### Comparing `mds_account_primanota-6.6.5/view/primanota_list.xml` & `mds_account_primanota-6.8.5/view/primanota_list.xml`

 * *Files identical despite different names*

