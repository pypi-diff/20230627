# Comparing `tmp/owl2yams-1.3.0.tar.gz` & `tmp/owl2yams-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/owl2yams-1.3.0.tar", last modified: Mon Apr 24 12:25:14 2023, max compression
+gzip compressed data, was "owl2yams-1.4.0.tar", last modified: Tue Jun 27 08:13:47 2023, max compression
```

## Comparing `owl2yams-1.3.0.tar` & `owl2yams-1.4.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/
--rw-r--r--   0 murloc    (1000) murloc    (1000)      267 2022-11-17 15:54:54.000000 owl2yams-1.3.0/MANIFEST.in
--rw-r--r--   0 murloc    (1000) murloc    (1000)     2876 2023-04-24 12:25:14.000000 owl2yams-1.3.0/PKG-INFO
--rw-r--r--   0 murloc    (1000) murloc    (1000)     2577 2022-07-04 12:53:24.000000 owl2yams-1.3.0/README.md
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams/
--rw-r--r--   0 murloc    (1000) murloc    (1000)    18404 2023-04-24 12:20:23.000000 owl2yams-1.3.0/owl2yams/__init__.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)     5342 2023-04-24 12:17:06.000000 owl2yams-1.3.0/owl2yams/ccplugin.py
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams/cw_react_admin/
--rw-r--r--   0 murloc    (1000) murloc    (1000)  1474880 2022-11-17 14:01:32.000000 owl2yams-1.3.0/owl2yams/cw_react_admin/main.js
--rw-r--r--   0 murloc    (1000) murloc    (1000)      480 2022-11-17 14:40:11.000000 owl2yams-1.3.0/owl2yams/generate_appjstemplate.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)     4213 2021-11-26 14:03:57.000000 owl2yams-1.3.0/owl2yams/generate_entities.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)      267 2022-11-17 13:50:43.000000 owl2yams-1.3.0/owl2yams/generate_init.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)     1052 2023-04-24 12:17:06.000000 owl2yams-1.3.0/owl2yams/generate_postcreate.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)     1069 2022-11-17 15:11:21.000000 owl2yams-1.3.0/owl2yams/generate_schema.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)     1550 2022-11-17 14:06:49.000000 owl2yams-1.3.0/owl2yams/generate_views.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)   136241 2021-11-25 15:02:23.000000 owl2yams-1.3.0/owl2yams/prefixes.json
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/
--rw-r--r--   0 murloc    (1000) murloc    (1000)     2876 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/PKG-INFO
--rw-r--r--   0 murloc    (1000) murloc    (1000)     1240 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/SOURCES.txt
--rw-r--r--   0 murloc    (1000) murloc    (1000)        1 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/dependency_links.txt
--rw-r--r--   0 murloc    (1000) murloc    (1000)       44 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/entry_points.txt
--rw-r--r--   0 murloc    (1000) murloc    (1000)        1 2021-10-12 13:30:58.000000 owl2yams-1.3.0/owl2yams.egg-info/not-zip-safe
--rw-r--r--   0 murloc    (1000) murloc    (1000)       60 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/requires.txt
--rw-r--r--   0 murloc    (1000) murloc    (1000)        9 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/top_level.txt
--rw-r--r--   0 murloc    (1000) murloc    (1000)       38 2023-04-24 12:25:14.000000 owl2yams-1.3.0/setup.cfg
--rw-r--r--   0 murloc    (1000) murloc    (1000)     1287 2023-04-24 12:22:32.000000 owl2yams-1.3.0/setup.py
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/test/
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/test/data/
--rw-r--r--   0 murloc    (1000) murloc    (1000)      293 2021-10-26 13:13:22.000000 owl2yams-1.3.0/test/data/test_attribute.owl
--rw-r--r--   0 murloc    (1000) murloc    (1000)       96 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_attribute.yams
--rw-r--r--   0 murloc    (1000) murloc    (1000)      293 2021-10-26 15:46:23.000000 owl2yams-1.3.0/test/data/test_attribute_owl_thing.owl
--rw-r--r--   0 murloc    (1000) murloc    (1000)      169 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_attribute_owl_thing.yams
--rw-r--r--   0 murloc    (1000) murloc    (1000)      104 2021-10-26 12:52:43.000000 owl2yams-1.3.0/test/data/test_class.owl
--rw-r--r--   0 murloc    (1000) murloc    (1000)       78 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_class.yams
--rw-r--r--   0 murloc    (1000) murloc    (1000)      216 2021-10-26 13:24:20.000000 owl2yams-1.3.0/test/data/test_hierarchy.owl
--rw-r--r--   0 murloc    (1000) murloc    (1000)      132 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_hierarchy.yams
--rw-r--r--   0 murloc    (1000) murloc    (1000)      197 2021-10-26 14:02:16.000000 owl2yams-1.3.0/test/data/test_multi_attribute.owl
--rw-r--r--   0 murloc    (1000) murloc    (1000)       30 2021-11-24 14:30:28.000000 owl2yams-1.3.0/test/data/test_multi_attribute.yams
--rw-r--r--   0 murloc    (1000) murloc    (1000)      179 2021-10-26 13:41:53.000000 owl2yams-1.3.0/test/data/test_multi_class.owl
--rw-r--r--   0 murloc    (1000) murloc    (1000)      119 2021-11-24 14:32:57.000000 owl2yams-1.3.0/test/data/test_multi_class.yams
--rw-r--r--   0 murloc    (1000) murloc    (1000)      193 2021-10-26 14:14:35.000000 owl2yams-1.3.0/test/data/test_multi_relation.owl
--rw-r--r--   0 murloc    (1000) murloc    (1000)       30 2021-11-24 14:34:53.000000 owl2yams-1.3.0/test/data/test_multi_relation.yams
--rw-r--r--   0 murloc    (1000) murloc    (1000)      295 2021-10-26 13:15:12.000000 owl2yams-1.3.0/test/data/test_relation.owl
--rw-r--r--   0 murloc    (1000) murloc    (1000)      196 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_relation.yams
--rw-r--r--   0 murloc    (1000) murloc    (1000)      306 2021-10-26 15:51:01.000000 owl2yams-1.3.0/test/data/test_relation_multi_range.owl
--rw-r--r--   0 murloc    (1000) murloc    (1000)      291 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_relation_multi_range.yams
--rw-r--r--   0 murloc    (1000) murloc    (1000)      264 2021-10-26 15:43:32.000000 owl2yams-1.3.0/test/data/test_relation_without_domain_range.owl
--rw-r--r--   0 murloc    (1000) murloc    (1000)      291 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_relation_without_domain_range.yams
--rw-r--r--   0 murloc    (1000) murloc    (1000)     4025 2021-11-24 14:33:52.000000 owl2yams-1.3.0/test/test_owl2yams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:13:47.903775 owl2yams-1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-06-27 08:13:35.000000 owl2yams-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2856 2023-06-27 08:13:47.903775 owl2yams-1.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2023-06-27 08:13:35.000000 owl2yams-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:13:47.887775 owl2yams-1.4.0/owl2yams/
+-rw-rw-rw-   0 root         (0) root         (0)    18444 2023-06-27 08:13:35.000000 owl2yams-1.4.0/owl2yams/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5342 2023-06-27 08:13:35.000000 owl2yams-1.4.0/owl2yams/ccplugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:13:47.891775 owl2yams-1.4.0/owl2yams/cw_react_admin/
+-rw-rw-rw-   0 root         (0) root         (0)  1474880 2023-06-27 08:13:35.000000 owl2yams-1.4.0/owl2yams/cw_react_admin/main.js
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-06-27 08:13:35.000000 owl2yams-1.4.0/owl2yams/generate_appjstemplate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4213 2023-06-27 08:13:35.000000 owl2yams-1.4.0/owl2yams/generate_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-06-27 08:13:35.000000 owl2yams-1.4.0/owl2yams/generate_init.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-06-27 08:13:35.000000 owl2yams-1.4.0/owl2yams/generate_postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-27 08:13:35.000000 owl2yams-1.4.0/owl2yams/generate_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1550 2023-06-27 08:13:35.000000 owl2yams-1.4.0/owl2yams/generate_views.py
+-rw-rw-rw-   0 root         (0) root         (0)   136241 2023-06-27 08:13:35.000000 owl2yams-1.4.0/owl2yams/prefixes.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:13:47.891775 owl2yams-1.4.0/owl2yams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2856 2023-06-27 08:13:47.000000 owl2yams-1.4.0/owl2yams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-06-27 08:13:47.000000 owl2yams-1.4.0/owl2yams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:13:47.000000 owl2yams-1.4.0/owl2yams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-27 08:13:47.000000 owl2yams-1.4.0/owl2yams.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:13:47.000000 owl2yams-1.4.0/owl2yams.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-27 08:13:47.000000 owl2yams-1.4.0/owl2yams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-27 08:13:47.000000 owl2yams-1.4.0/owl2yams.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 08:13:47.903775 owl2yams-1.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-06-27 08:13:35.000000 owl2yams-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:13:47.895775 owl2yams-1.4.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:13:47.899775 owl2yams-1.4.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_attribute.owl
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_attribute.yams
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_attribute_owl_thing.owl
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_attribute_owl_thing.yams
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_class.owl
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_class.yams
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_hierarchy.owl
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_hierarchy.yams
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_multi_attribute.owl
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_multi_attribute.yams
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_multi_class.owl
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_multi_class.yams
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_multi_relation.owl
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_multi_relation.yams
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_relation.owl
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_relation.yams
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_relation_multi_range.owl
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_relation_multi_range.yams
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_relation_without_domain_range.owl
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/data/test_relation_without_domain_range.yams
+-rw-rw-rw-   0 root         (0) root         (0)     4025 2023-06-27 08:13:35.000000 owl2yams-1.4.0/test/test_owl2yams.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `owl2yams-1.3.0/PKG-INFO` & `owl2yams-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: owl2yams
-Version: 1.3.0
+Version: 1.4.0
 Summary: A tools to transforms owl into yams schema
 Home-page: https://forge.extranet.logilab.fr/cubicweb/owl2yams
 Author: Fabien Amarger
 Author-email: famarger@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # OWL2YAMS
 
 A script to create a new CubicWeb instance from OWL ontology and RDF data
 
 ## Installing the project
@@ -92,9 +91,7 @@
 installed by default when using OWL2YAMS. You can find the
 [`open-api`](https://www.openapis.org) spec using the route `/api/v1/openapi`.
 
 This cube is mandatory to use the
 (`cubicweb-react-admin`)[https://forge.extranet.logilab.fr/cubicweb/react-admin-cubicweb]
 tool.  This tool lets you navigate and administrate your data using a modern
 and dynamic interface.
-
-
```

### Comparing `owl2yams-1.3.0/README.md` & `owl2yams-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `owl2yams-1.3.0/owl2yams/__init__.py` & `owl2yams-1.4.0/owl2yams/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,14 +394,15 @@
     # add dependencies
     pkginfo_path = Path(
         os.path.join(cube_master_folder, cube_subfolder, "__pkginfo__.py")
     )
     red = RedBaron(pkginfo_path.read_text())
     dependencies_node = red.find("assign", target=lambda x: x.value == "__depends__")
     dependencies = dependencies_node.value.to_python()
+    dependencies["cubicweb"] = "<4.0.0"
     dependencies["cubicweb-api"] = None
     dependencies["pyramid-jinja2"] = None
     dependencies_node.value = str(dependencies)
     pkginfo_path.write_text(red.dumps())
 
     if only_cube:
         print("Cube correctly initialized")
```

### Comparing `owl2yams-1.3.0/owl2yams/ccplugin.py` & `owl2yams-1.4.0/owl2yams/ccplugin.py`

 * *Files identical despite different names*

### Comparing `owl2yams-1.3.0/owl2yams/cw_react_admin/main.js` & `owl2yams-1.4.0/owl2yams/cw_react_admin/main.js`

 * *Files identical despite different names*

### Comparing `owl2yams-1.3.0/owl2yams/generate_entities.py` & `owl2yams-1.4.0/owl2yams/generate_entities.py`

 * *Files identical despite different names*

### Comparing `owl2yams-1.3.0/owl2yams/generate_postcreate.py` & `owl2yams-1.4.0/owl2yams/generate_postcreate.py`

 * *Files identical despite different names*

### Comparing `owl2yams-1.3.0/owl2yams/generate_schema.py` & `owl2yams-1.4.0/owl2yams/generate_schema.py`

 * *Files identical despite different names*

### Comparing `owl2yams-1.3.0/owl2yams/generate_views.py` & `owl2yams-1.4.0/owl2yams/generate_views.py`

 * *Files identical despite different names*

### Comparing `owl2yams-1.3.0/owl2yams/prefixes.json` & `owl2yams-1.4.0/owl2yams/prefixes.json`

 * *Files identical despite different names*

### Comparing `owl2yams-1.3.0/owl2yams.egg-info/PKG-INFO` & `owl2yams-1.4.0/owl2yams.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: owl2yams
-Version: 1.3.0
+Version: 1.4.0
 Summary: A tools to transforms owl into yams schema
 Home-page: https://forge.extranet.logilab.fr/cubicweb/owl2yams
 Author: Fabien Amarger
 Author-email: famarger@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # OWL2YAMS
 
 A script to create a new CubicWeb instance from OWL ontology and RDF data
 
 ## Installing the project
@@ -92,9 +91,7 @@
 installed by default when using OWL2YAMS. You can find the
 [`open-api`](https://www.openapis.org) spec using the route `/api/v1/openapi`.
 
 This cube is mandatory to use the
 (`cubicweb-react-admin`)[https://forge.extranet.logilab.fr/cubicweb/react-admin-cubicweb]
 tool.  This tool lets you navigate and administrate your data using a modern
 and dynamic interface.
-
-
```

### Comparing `owl2yams-1.3.0/owl2yams.egg-info/SOURCES.txt` & `owl2yams-1.4.0/owl2yams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owl2yams-1.3.0/setup.py` & `owl2yams-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 here = osp.abspath(osp.dirname(__file__))
 # Get the long description from the relevant file
 with open(osp.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 distname = "owl2yams"
-version = "1.3.0"
+version = "1.4.0"
 license = "LGPL"
 description = "A tools to transforms owl into yams schema"
 author = "Fabien Amarger"
 author_email = "famarger@logilab.fr"
 requires = {
-    "cubicweb": None,
+    "cubicweb": "<4.0.0",
     "yams": ">=0.45.5",
     "rdflib": None,
     "Jinja2": None,
     "black": None,
     "requests": None,
     "redbaron": None,
 }
```

### Comparing `owl2yams-1.3.0/test/test_owl2yams.py` & `owl2yams-1.4.0/test/test_owl2yams.py`

 * *Files identical despite different names*

