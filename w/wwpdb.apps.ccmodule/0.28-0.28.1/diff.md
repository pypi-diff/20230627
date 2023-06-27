# Comparing `tmp/wwpdb.apps.ccmodule-0.28.tar.gz` & `tmp/wwpdb.apps.ccmodule-0.28.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.ccmodule-0.28.tar", last modified: Thu Jun 22 04:42:23 2023, max compression
+gzip compressed data, was "wwpdb.apps.ccmodule-0.28.1.tar", last modified: Tue Jun 27 12:26:33 2023, max compression
```

## Comparing `wwpdb.apps.ccmodule-0.28.tar` & `wwpdb.apps.ccmodule-0.28.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.025129 wwpdb.apps.ccmodule-0.28/
--rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-06-22 04:42:23.025129 wwpdb.apps.ccmodule-0.28/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       80 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-22 04:42:23.025129 wwpdb.apps.ccmodule-0.28/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2595 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.013129 wwpdb.apps.ccmodule-0.28/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/
--rw-r--r--   0 vsts      (1001) docker     (123)      151 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/
--rw-r--r--   0 vsts      (1001) docker     (123)     5950 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
--rw-r--r--   0 vsts      (1001) docker     (123)   122825 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssign.py
--rw-r--r--   0 vsts      (1001) docker     (123)   105108 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    73659 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12269 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)    11302 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/depict/ChemCompDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/extract/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/extract/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2951 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/extract/ccOps.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    94861 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7123 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompDataExport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7305 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12540 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompEditStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13230 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.021129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/
--rw-r--r--   0 vsts      (1001) docker     (123)     4801 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     4885 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2842 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3367 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15516 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompReports.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8576 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.021129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/
--rw-r--r--   0 vsts      (1001) docker     (123)    10865 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13150 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6259 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8708 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/DbSession.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.021129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/
--rw-r--r--   0 vsts      (1001) docker     (123)     9350 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6407 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.021129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)     7201 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompConfig.py
--rw-r--r--   0 vsts      (1001) docker     (123)    28664 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1136 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      586 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/Exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7942 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.021129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/
--rw-r--r--   0 vsts      (1001) docker     (123)     7378 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/ChemCompView.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5748 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.025129 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)   138698 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    96593 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     4642 2023-06-22 04:41:04.000000 wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/wsgi.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-22 04:42:23.017129 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-06-22 04:42:22.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2370 2023-06-22 04:42:22.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-22 04:42:22.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-22 04:42:07.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      250 2023-06-22 04:42:22.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-22 04:42:22.000000 wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.792517 wwpdb.apps.ccmodule-0.28.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      781 2023-06-27 12:26:33.792517 wwpdb.apps.ccmodule-0.28.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       80 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-27 12:26:33.792517 wwpdb.apps.ccmodule-0.28.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2595 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.784517 wwpdb.apps.ccmodule-0.28.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.784517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.784517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/
+-rw-r--r--   0 vsts      (1001) docker     (123)      153 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.784517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5950 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   122957 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/ChemCompAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   105109 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    73659 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12269 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.784517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11302 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/depict/ChemCompDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.784517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/extract/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/extract/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2951 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/extract/ccOps.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.788517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)    94879 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7123 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/ChemCompDataExport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7305 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/ChemCompDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12540 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/ChemCompEditStore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13230 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/ChemCompIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.788517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4801 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     4885 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2842 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3367 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15516 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/ChemCompReports.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8568 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.788517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10865 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/ChemCompSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13150 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6259 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8708 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/DbSession.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.788517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/sketch/
+-rw-r--r--   0 vsts      (1001) docker     (123)     9350 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6407 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/sketch/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.788517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7201 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/ChemCompConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    28701 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1136 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      586 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/Exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7942 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.788517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/view/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7378 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/view/ChemCompView.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5748 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/view/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.792517 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)   138698 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    96593 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/webapp/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     4642 2023-06-27 12:25:17.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/webapp/wsgi.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:26:33.784517 wwpdb.apps.ccmodule-0.28.1/wwpdb.apps.ccmodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      781 2023-06-27 12:26:33.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb.apps.ccmodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2370 2023-06-27 12:26:33.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb.apps.ccmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 12:26:33.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb.apps.ccmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 12:26:21.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb.apps.ccmodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      250 2023-06-27 12:26:33.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb.apps.ccmodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-27 12:26:33.000000 wwpdb.apps.ccmodule-0.28.1/wwpdb.apps.ccmodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.ccmodule-0.28/PKG-INFO` & `wwpdb.apps.ccmodule-0.28.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ccmodule
-Version: 0.28
+Version: 0.28.1
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ccmodule-0.28/setup.py` & `wwpdb.apps.ccmodule-0.28.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssign.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/ChemCompAssign.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 import traceback
 import inspect
 
 #
 from rcsb.utils.multiproc.MultiProcUtil import MultiProcUtil
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
-from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxCategoryDefinition,PdbxChemCompAssignReader
+from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxCategoryDefinition, PdbxChemCompAssignReader
 from wwpdb.apps.ccmodule.io.ChemCompDataImport import ChemCompDataImport
 from wwpdb.apps.ccmodule.io.ChemCompDataExport import ChemCompDataExport
 from wwpdb.apps.ccmodule.io.ChemCompIo import ChemCompReader
 from wwpdb.apps.ccmodule.io.ChemCompAssignDataStore import ChemCompAssignDataStore
 from mmcif.io.PdbxReader import PdbxReader
 from pathlib import Path
 from wwpdb.io.locator.PathInfo import PathInfo
@@ -371,15 +371,15 @@
 
         #########################################################################################################
         # interrogate resulting assign results file for desired match data
         #########################################################################################################
         pR = PdbxChemCompAssignReader(self.__verbose, self.__lfh)
         pR.setFilePath(filePath=pathToAssignFile)
         pR.getBlock()
-        for cN in list(PdbxCategoryDefinition._cDict.keys()):
+        for cN in list(PdbxCategoryDefinition._cDict.keys()):  # pylint: disable=protected-access
             if pR.categoryExists(cN):
                 dataDict[cN] = pR.getCategory(catName=cN)
 
         return dataDict
 
     def saveState(self, pathDict, context="annot", mode=None):
         """ Method for capturing current state of chem component assignments.
@@ -867,15 +867,15 @@
             origCcidDict = self.__getDpstrOrigCcids()
         #
         for retResult in retLists[0]:
             pR = PdbxChemCompAssignReader(self.__verbose, self.__lfh)
             pR.setFilePath(filePath=retResult[1])
             pR.getBlock()
             dd = {}
-            for cN in list(PdbxCategoryDefinition._cDict.keys()):
+            for cN in list(PdbxCategoryDefinition._cDict.keys()):  # pylint: disable=protected-access
                 if pR.categoryExists(cN):
                     dd[cN] = pR.getCategory(catName=cN)
                 #
             #
             ccADS = self.updateDataStoreForInstnc(retResult[0], dd, preFlag=flag, preCcidDict=origCcidDict)
             ccADS.serialize()
         #
@@ -990,15 +990,15 @@
             else:
                 self.__lfh.write("+ChemCompAssign.doAssignInstance() - NO assignment file created.\n")
                 ccAssignFilePath = None
 
             pR = PdbxChemCompAssignReader(self.__verbose, self.__lfh)
             pR.setFilePath(filePath=ccAssignFilePath)
             pR.getBlock()
-            for cN in list(PdbxCategoryDefinition._cDict.keys()):
+            for cN in list(PdbxCategoryDefinition._cDict.keys()):  # pylint: disable=protected-access
                 if pR.categoryExists(cN):
                     dd[cN] = pR.getCategory(catName=cN)
 
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 self.__lfh.write("+ChemCompAssign.doAssignInstance() - pre-processing failed for:  %s\n" % mdlfilePath)
                 traceback.print_exc(file=self.__lfh)
@@ -1066,15 +1066,15 @@
             else:
                 self.__lfh.write("+ChemCompAssign.doAssignInstanceComp() - NO assignment file created.\n")
                 ccAssignFilePath = None
 
             pR = PdbxChemCompAssignReader(self.__verbose, self.__lfh)
             pR.setFilePath(filePath=ccAssignFilePath)
             pR.getBlock()
-            for cN in list(PdbxCategoryDefinition._cDict.keys()):
+            for cN in list(PdbxCategoryDefinition._cDict.keys()):  # pylint: disable=protected-access
                 if pR.categoryExists(cN):
                     dd[cN] = pR.getCategory(catName=cN)
 
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 self.__lfh.write("+ChemCompAssign.doAssignInstanceComp() - pre-processing failed for:  %s\n" % mdlfilePath)
                 traceback.print_exc(file=self.__lfh)
@@ -1573,31 +1573,31 @@
         if ("pdbx_metadata_info" in p_dataDict) and (len(p_dataDict["pdbx_metadata_info"]) > 0):
             for row in p_dataDict["pdbx_metadata_info"]:
                 if ("_pdbx_metadata_info.id" not in row) or (not row["_pdbx_metadata_info.id"]):
                     continue
                 #
                 p_ccAssgnDataStore.setAuthorProvidedRestraintFlag(row["_pdbx_metadata_info.id"])
                 #
-                for keyTupL in ( ( "name", "_pdbx_metadata_info.name" ), ( "formula", "_pdbx_metadata_info.formula" ), \
-                                 ( "natoms", "_pdbx_metadata_info.natoms" ) ):
+                for keyTupL in (("name", "_pdbx_metadata_info.name"), ("formula", "_pdbx_metadata_info.formula"),
+                                ("natoms", "_pdbx_metadata_info.natoms")):
                     if (keyTupL[1] not in row) or (not row[keyTupL[1]]):
                         continue
                     #
                     p_ccAssgnDataStore.addAuthorProvidedMetaData(row["_pdbx_metadata_info.id"], keyTupL[0], row[keyTupL[1]])
                 #
             #
         #
         if ("pdbx_descriptor_info" in p_dataDict) and (len(p_dataDict["pdbx_descriptor_info"]) > 0):
             for row in p_dataDict["pdbx_descriptor_info"]:
                 if ("_pdbx_descriptor_info.id" not in row) or (not row["_pdbx_descriptor_info.id"]) or \
                    ("_pdbx_descriptor_info.type" not in row) or (not row["_pdbx_descriptor_info.type"]) or \
                    ("_pdbx_descriptor_info.descriptor" not in row) or (not row["_pdbx_descriptor_info.descriptor"]):
                     continue
                 #
-                p_ccAssgnDataStore.addAuthorProvidedDescriptor(row["_pdbx_descriptor_info.id"], row["_pdbx_descriptor_info.type"], \
+                p_ccAssgnDataStore.addAuthorProvidedDescriptor(row["_pdbx_descriptor_info.id"], row["_pdbx_descriptor_info.type"],
                                                                row["_pdbx_descriptor_info.descriptor"])
             #
         #
 
     def __ccLiteUploadFileHndling(self, p_ccADS, p_ligId=None):
         """ Method for processing any files that were uploaded by the depositor to supplement
         the data collection for the deposition. Files will be copied to workflow storage
```

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1381,15 +1381,15 @@
             if formula:
                 chemCompFrmla = formula
             #
         #
         chemCompDescriptor = p_dataStore.getDpstrCcDscrptrStr(p_grpId)
         chemCompDescriptorType = p_dataStore.getDpstrCcDscrptrType(p_grpId)
         if (chemCompDescriptor is None) or (chemCompDescriptor == "?") or (chemCompDescriptorType is None) or (chemCompDescriptorType == "?"):
-            desType,desStr = p_dataStore.getAuthorProvidedDescriptorInfo(p_grpId)
+            desType, desStr = p_dataStore.getAuthorProvidedDescriptorInfo(p_grpId)
             if desType and desStr:
                 chemCompDescriptor = desStr
                 chemCompDescriptorType = desType
             #
         #
         chemCompDetails = p_dataStore.getDpstrComments(p_grpId)
         p_strReplDict['display_dpstr_info'] = ""
```

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/depict/ChemCompDepict.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/depict/ChemCompDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/extract/ccOps.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/extract/ccOps.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,16 +173,16 @@
         #                                 # so that authoritative precedence given to most recent uploads
         self.__rsrchAcqurdGrpLst = []     # admin/convenience list for keeping track of entity groups for which data was captured for "focus of research" needs.
         self.__dpstrCcRsrchInfo = {}  # dictionary mapping ligand code to research data provied by depositor
         self.__rsrchSlctdGrpLst = []     # admin/convenience list for keeping track of entity groups which were indicated as "focus of research".
         self.__dpstrOrigCcIdMaster = {}  # Authoritative copy of CCID which depositor had originally used to identify the ligand
         # ###################Chem Comp Lite attributes END   ###############################
 
-        self.__authorProvidedInfo = {} # Metadata and chemical descriptor(s) information provided by depositor from extra data block(s) 
-                                       # where new chemical information are stored.
+        self.__authorProvidedInfo = {}  # Metadata and chemical descriptor(s) information provided by depositor from extra data block(s)
+                                        # where new chemical information are stored.  # noqa: E116
 
         self.__setup()
 
     def __setup(self):
         """ Setup of a given ChemCompAssignDataStore object involves checking for an existing
             serialized pickle file for the current deposition dataset being processed.
             If such a pickle file exists, we use it to populate the object with the last recorded
@@ -1425,27 +1425,27 @@
         except:  # noqa: E722 pylint: disable=bare-except
             return False
         #
 
     def hasAuthorProvidedRestraintFlag(self, grpId):
         try:
             if (grpId in self.__authorProvidedInfo) and ("restraint" in self.__authorProvidedInfo[grpId]):
-               if self.__authorProvidedInfo[grpId]["restraint"] == "YES":
-                   return True
+                if self.__authorProvidedInfo[grpId]["restraint"] == "YES":
+                    return True
                 #
             #
             return False
         except:  # noqa: E722 pylint: disable=bare-except
             return False
         #
 
     def getAuthorProvidedRestraintGrpIds(self):
         try:
             grpIdList = []
-            for grpId,valD in self.__authorProvidedInfo.items():
+            for grpId, valD in self.__authorProvidedInfo.items():
                 if ("restraint" in valD) and (valD["restraint"] == "YES"):
                     grpIdList.append(grpId)
                 #
             #
             return grpIdList
         except:  # noqa: E722 pylint: disable=bare-except
             return []
@@ -1483,34 +1483,34 @@
             self.__authorProvidedInfo[grpId]["descriptor"][descriptorType] = descriptorVal
             return True
         except:  # noqa: E722 pylint: disable=bare-except
             return False
         #
 
     def getAuthorProvidedDescriptor(self, grpId, descriptorType):
-        try: 
+        try:
             if (grpId in self.__authorProvidedInfo) and ("descriptor" in self.__authorProvidedInfo[grpId]) and \
                (descriptorType in self.__authorProvidedInfo[grpId]["descriptor"]):
                 return self.__authorProvidedInfo[grpId]["descriptor"][descriptorType]
             #
             return None
         except:  # noqa: E722 pylint: disable=bare-except
             return None
         #
 
     def getAuthorProvidedDescriptorInfo(self, grpId):
-        try: 
+        try:
             if (grpId in self.__authorProvidedInfo) and ("descriptor" in self.__authorProvidedInfo[grpId]) and \
                (len(self.__authorProvidedInfo[grpId]["descriptor"]) > 0):
                 itemList = sorted(self.__authorProvidedInfo[grpId]["descriptor"].items())
                 return itemList[-1]
             #
-            return None,None
+            return None, None
         except:  # noqa: E722 pylint: disable=bare-except
-            return None,None
+            return None, None
         #
 
     def setDpstrAltCcId(self, grpId, altId):
         try:
             if altId is None:
                 del self.__dpstrCcAltId[grpId]
             else:
```

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompDataExport.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/ChemCompDataExport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompDataImport.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/ChemCompDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompEditStore.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/ChemCompEditStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/io/ChemCompIo.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/io/ChemCompIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/ChemCompReports.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/ChemCompReports.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,26 +170,26 @@
         #
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         self.__cI = ConfigInfo(self.__siteId)
 
     def runReportGenerator(self, dataList=None, processLabel=None):  # pylint: disable=unused-argument
         for authId in dataList:
             chemCompFilePathAbs = os.path.join(self.__sessionPath, 'assign', authId, authId + '.cif')
-            if (not os.access(chemCompFilePathAbs, os.R_OK)):  
+            if (not os.access(chemCompFilePathAbs, os.R_OK)):
                 continue
             #
             imagePath = os.path.join(self.__sessionPath, 'assign', authId, 'image')
             if not os.access(imagePath, os.F_OK):
                 try:
                     os.makedirs(imagePath)
                 except:  # noqa: E722 pylint: disable=bare-except
                     continue
                 #
             #
-            for paraTupL in ( ( 300, '', False ), ( 1000, '_Big', True ) ):
+            for paraTupL in ((300, '', False), (1000, '_Big', True)):
                 dp = RcsbDpUtility(tmpPath=imagePath, siteId=self.__cI.get('SITE_PREFIX'), verbose=self.__verbose, log=self.__lfh)
                 dp.addInput(name="title", value=authId)
                 dp.addInput(name="path", value=chemCompFilePathAbs)
                 dp.addInput(name="image_path", value=os.path.join(imagePath, authId + paraTupL[1] + '.svg'))
                 dp.addInput(name="size", value=paraTupL[0])
                 dp.addInput(name="label", value=paraTupL[2])
                 dp.op("chem-comp-gen-images")
```

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearch.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/ChemCompSearch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/search/DbSession.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/search/DbSession.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompConfig.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/ChemCompConfig.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import shutil
 from logging import getLogger, StreamHandler, Formatter, DEBUG, INFO
 from wwpdb.apps.ccmodule.chem.ChemCompAssign import ChemCompAssign
 from wwpdb.apps.ccmodule.utils.ChemCompConfig import ChemCompConfig
 from wwpdb.apps.ccmodule.utils.LigandAnalysisState import LigandAnalysisState
 from wwpdb.apps.ccmodule.io.ChemCompDataExport import ChemCompDataExport
-from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxCategoryDefinition,PdbxChemCompAssignReader
+from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxCategoryDefinition, PdbxChemCompAssignReader
 from wwpdb.apps.ccmodule.chem.ChemCompAssignDepictLite import ChemCompAssignDepictLite
 from wwpdb.utils.session.WebRequest import InputRequest
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
 from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
 from pathlib import Path
 from wwpdb.io.locator.PathInfo import PathInfo
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
@@ -182,15 +182,15 @@
         if self._verbose:
             self._logger.debug('Reading assign results for desired match data.')
 
         pR = PdbxChemCompAssignReader(self._verbose, self._lfh)
         pR.setFilePath(filePath=fPath)
         pR.getBlock()
 
-        for cN in list(PdbxCategoryDefinition._cDict.keys()):
+        for cN in list(PdbxCategoryDefinition._cDict.keys()):  # pylint: disable=protected-access
             if pR.categoryExists(cN):
                 dataDict[cN] = pR.getCategory(catName=cN)
 
         return dataDict
 
     def _genLigandReportData(self, instId, instanceCcAbsFilePath=None, rtype='ref'):
         """Generate the actual report file. The file path is based on
```

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/Exceptions.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/ChemCompView.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/view/ChemCompView.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb/apps/ccmodule/webapp/wsgi.py` & `wwpdb.apps.ccmodule-0.28.1/wwpdb/apps/ccmodule/webapp/wsgi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/PKG-INFO` & `wwpdb.apps.ccmodule-0.28.1/wwpdb.apps.ccmodule.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ccmodule
-Version: 0.28
+Version: 0.28.1
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ccmodule-0.28/wwpdb.apps.ccmodule.egg-info/SOURCES.txt` & `wwpdb.apps.ccmodule-0.28.1/wwpdb.apps.ccmodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

