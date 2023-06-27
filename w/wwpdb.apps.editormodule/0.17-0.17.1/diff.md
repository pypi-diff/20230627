# Comparing `tmp/wwpdb.apps.editormodule-0.17.tar.gz` & `tmp/wwpdb.apps.editormodule-0.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.editormodule-0.17.tar", last modified: Sun Apr 30 13:30:17 2023, max compression
+gzip compressed data, was "wwpdb.apps.editormodule-0.17.1.tar", last modified: Tue Jun 27 12:59:41 2023, max compression
```

## Comparing `wwpdb.apps.editormodule-0.17.tar` & `wwpdb.apps.editormodule-0.17.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.218037 wwpdb.apps.editormodule-0.17/
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/LICENSE
--rwxr-xr-x   0 vsts      (1001) docker     (123)      110 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      757 2023-04-30 13:30:17.218037 wwpdb.apps.editormodule-0.17/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       51 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-30 13:30:17.218037 wwpdb.apps.editormodule-0.17/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2209 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.210037 wwpdb.apps.editormodule-0.17/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.210037 wwpdb.apps.editormodule-0.17/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.210037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.214037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      290 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
--rw-r--r--   0 vsts      (1001) docker     (123)      170 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7680 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/EditorConfig.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)   144958 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
--rw-r--r--   0 vsts      (1001) docker     (123)   209858 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.214037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/depict/
--rwxr-xr-x   0 vsts      (1001) docker     (123)    52449 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/depict/EditorDepict.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.214037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/
--rw-r--r--   0 vsts      (1001) docker     (123)     4873 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/EditorDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (123)   163711 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxDataIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8061 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1616 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.218037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/
--rw-r--r--   0 vsts      (1001) docker     (123)     6211 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
--rw-r--r--   0 vsts      (1001) docker     (123)      641 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (123)    13947 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (123)    17945 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
--rw-r--r--   0 vsts      (1001) docker     (123)    15904 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
--rw-r--r--   0 vsts      (1001) docker     (123)     3502 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_prototyping.html
--rw-r--r--   0 vsts      (1001) docker     (123)     2470 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.218037 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)    79034 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/EditorWebApp.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)    10750 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/WebRequest.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:29:05.000000 wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:30:17.210037 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      757 2023-04-30 13:30:17.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1637 2023-04-30 13:30:17.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:30:17.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:30:03.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-04-30 13:30:17.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-30 13:30:17.000000 wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.219041 wwpdb.apps.editormodule-0.17.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/LICENSE
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      110 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-06-27 12:59:41.219041 wwpdb.apps.editormodule-0.17.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       51 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-27 12:59:41.219041 wwpdb.apps.editormodule-0.17.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2209 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.211041 wwpdb.apps.editormodule-0.17.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.211041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.211041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/
+-rw-r--r--   0 vsts      (1001) docker     (123)      152 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.215041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      290 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      170 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7792 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/EditorConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   144958 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
+-rw-r--r--   0 vsts      (1001) docker     (123)   212034 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.215041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/depict/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    52449 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/depict/EditorDepict.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.215041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4873 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/EditorDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   163711 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxDataIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8061 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1616 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.219041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6211 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      641 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (123)    13947 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (123)    17945 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
+-rw-r--r--   0 vsts      (1001) docker     (123)    15904 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3502 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_prototyping.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     2470 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.219041 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)    79034 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/EditorWebApp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    10750 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/WebRequest.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:58:31.000000 wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:59:41.211041 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-06-27 12:59:41.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1637 2023-06-27 12:59:41.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 12:59:41.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 12:59:28.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-06-27 12:59:41.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-27 12:59:41.000000 wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.editormodule-0.17/LICENSE` & `wwpdb.apps.editormodule-0.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/PKG-INFO` & `wwpdb.apps.editormodule-0.17.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.17
+Version: 0.17.1
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.editormodule-0.17/setup.py` & `wwpdb.apps.editormodule-0.17.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/EditorConfig.py` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/EditorConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         "pdbx_database_related",
         "pdbx_distant_solvent_atoms",
         "pdbx_entity_src_syn",
         "pdbx_refine_tls_group",
         "pdbx_related_exp_data_set",
         "pdbx_struct_assembly_auth_evidence",
         "pdbx_struct_assembly_prop",
+        "pdbx_struct_assembly_auth_evidence_depositor_info",
+        "pdbx_struct_assembly_gen_depositor_info",
         "pdbx_serial_crystallography_measurement",
         "pdbx_serial_crystallography_sample_delivery",
         "pdbx_serial_crystallography_sample_delivery_injection",
         "pdbx_serial_crystallography_sample_delivery_fixed_target",
         "pdbx_serial_crystallography_data_reduction",
         "refine_ls_restr_ncs",
         "refine_ls_restr",
```

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif`

 * *Files 1% similar despite different names*

```diff
@@ -1130,14 +1130,17 @@
 Derived                      struct_conf_type                    Helices                      struct_conf_type                      multi
 Derived                      pdbx_struct_assembly_depositor_info 'Biological Assembly'        'Depositor Assembly details'          multi
 Derived                      pdbx_struct_assembly                'Biological Assembly'        pdbx_struct_assembly                  multi
 Derived                      pdbx_struct_assembly_auth_evidence  'Biological Assembly'        'Depositor Assembly evidence'         multi
 Derived                      pdbx_struct_assembly_gen            'Biological Assembly'        pdbx_struct_assembly_gen              multi
 Derived                      pdbx_struct_assembly_prop           'Biological Assembly'        pdbx_struct_assembly_prop             multi
 Derived                      struct_biol                         'Biological Assembly'        'Assembly details'                    multi
+Derived                      pdbx_struct_assembly_auth_evidence_depositor_info  'Biological Assembly'  'Author Evidence depui'      multi
+Derived                      pdbx_struct_assembly_gen_depositor_info 'Biological Assembly'   'Author assem gen depui'              multi
+
 Derived                      pdbx_distant_solvent_atoms          'Solvent Re-position'        'distant solvent'                     multi
 Derived                      pdbx_solvent_atom_site_mapping      'Solvent Re-position'        'solvent atom mapping'                multi
 
 
 loop_
 _pdbx_display_view_item_info.category_display_name
 _pdbx_display_view_item_info.item_name
@@ -1289,14 +1292,29 @@
 'Assembly details'                    '_struct_biol.id'                                             id                                          N
 'Assembly details'                    '_struct_biol.details'                                        details                                     N
 'Depositor Assembly details'          '_pdbx_struct_assembly_depositor_info.id'                     id                                          Y
 'Depositor Assembly details'          '_pdbx_struct_assembly_depositor_info.details'                'depositor assembly info'                   N
 'Depositor Assembly details'          '_pdbx_struct_assembly_depositor_info.method_details'         'depositor assembly method'                 N
 'Depositor Assembly details'          '_pdbx_struct_assembly_depositor_info.oligomeric_details'     'depositor assembly details'                N
 'Depositor Assembly details'          '_pdbx_struct_assembly_depositor_info.oligomeric_count'       'depositor assembly count'                  N
+
+'Author Evidence depui'               '_pdbx_struct_assembly_auth_evidence_depositor_info.id'       id                                          N
+'Author Evidence depui'               '_pdbx_struct_assembly_auth_evidence_depositor_info.assembly_id'   'assembly id'                          N
+'Author Evidence depui'               '_pdbx_struct_assembly_auth_evidence_depositor_info.experimental_support'   'exptl supp'                  N
+'Author Evidence depui'               '_pdbx_struct_assembly_auth_evidence_depositor_info.details'   'details'                                  N
+'Author assem gen depui'              '_pdbx_struct_assembly_gen_depositor_info.id'                 id                                          N
+'Author assem gen depui'              '_pdbx_struct_assembly_gen_depositor_info.all_chains'         'all chains'                                N
+'Author assem gen depui'              '_pdbx_struct_assembly_gen_depositor_info.assembly_id'        'assembly id'                               N
+'Author assem gen depui'              '_pdbx_struct_assembly_gen_depositor_info.at_unit_matrix'     at_unit_matric                              N
+'Author assem gen depui'              '_pdbx_struct_assembly_gen_depositor_info.oper_expression'    operator                                    N
+'Author assem gen depui'              '_pdbx_struct_assembly_gen_depositor_info.symmetry_operation' symm                                        N
+'Author assem gen depui'              '_pdbx_struct_assembly_gen_depositor_info.chain_id_list'      chains                                      N
+'Author assem gen depui'              '_pdbx_struct_assembly_gen_depositor_info.asym_id_list'       asym_id_list                                N
+'Author assem gen depui'              '_pdbx_struct_assembly_gen_depositor_info.full_matrices'      matrices                                    N
+
 'distant solvent'                     '_pdbx_distant_solvent_atoms.id'                              id                                          Y
 'distant solvent'                     '_pdbx_distant_solvent_atoms.auth_comp_id'                    auth_comp_id                                Y
 'distant solvent'                     '_pdbx_distant_solvent_atoms.auth_asym_id'                    auth_asym_id                                Y
 'distant solvent'                     '_pdbx_distant_solvent_atoms.auth_seq_id'                     auth_seq_id                                 Y
 'distant solvent'                     '_pdbx_distant_solvent_atoms.auth_atom_id'                    auth_atom_id                                Y
 'distant solvent'                     '_pdbx_distant_solvent_atoms.label_comp_id'                   label_comp_id                               Y
 'distant solvent'                     '_pdbx_distant_solvent_atoms.label_asym_id'                   label_asym_id                               Y
```

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/depict/EditorDepict.py` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/depict/EditorDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/EditorDataImport.py` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/EditorDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxDataIo.py` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxDataIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_prototyping.html` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_prototyping.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/EditorWebApp.py` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/EditorWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb/apps/editormodule/webapp/WebRequest.py` & `wwpdb.apps.editormodule-0.17.1/wwpdb/apps/editormodule/webapp/WebRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/PKG-INFO` & `wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.17
+Version: 0.17.1
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.editormodule-0.17/wwpdb.apps.editormodule.egg-info/SOURCES.txt` & `wwpdb.apps.editormodule-0.17.1/wwpdb.apps.editormodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

