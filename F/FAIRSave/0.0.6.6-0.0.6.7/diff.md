# Comparing `tmp/FAIRSave-0.0.6.6.tar.gz` & `tmp/FAIRSave-0.0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FAIRSave-0.0.6.6.tar", last modified: Tue Jun 27 08:53:46 2023, max compression
+gzip compressed data, was "FAIRSave-0.0.6.7.tar", last modified: Tue Jun 27 08:56:15 2023, max compression
```

## Comparing `FAIRSave-0.0.6.6.tar` & `FAIRSave-0.0.6.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:53:46.208918 FAIRSave-0.0.6.6/
-drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:53:46.194983 FAIRSave-0.0.6.6/FAIRSave/
--rw-r--r--   0 ilia       (502) staff       (20)        0 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/__init__.py
--rw-r--r--   0 ilia       (502) staff       (20)     9069 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/configuration.py
--rw-r--r--   0 ilia       (502) staff       (20)     2780 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/eln_manager.py
--rw-r--r--   0 ilia       (502) staff       (20)     4351 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/kadi_download.py
--rw-r--r--   0 ilia       (502) staff       (20)    18108 2023-06-27 08:33:30.000000 FAIRSave-0.0.6.6/FAIRSave/kadi_identifier.py
--rw-r--r--   0 ilia       (502) staff       (20)     3512 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/kadi_instances.py
--rw-r--r--   0 ilia       (502) staff       (20)     8304 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/kadi_json_writer.py
--rw-r--r--   0 ilia       (502) staff       (20)    14148 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/kadi_record.py
--rw-r--r--   0 ilia       (502) staff       (20)    11780 2023-06-27 08:33:30.000000 FAIRSave-0.0.6.6/FAIRSave/kadi_search.py
--rw-r--r--   0 ilia       (502) staff       (20)     1315 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/kadi_template.py
-drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:53:46.206098 FAIRSave-0.0.6.6/FAIRSave/tools/
--rw-r--r--   0 ilia       (502) staff       (20)        0 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/tools/__init__.py
--rw-r--r--   0 ilia       (502) staff       (20)     9224 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/tools/comparison.py
--rw-r--r--   0 ilia       (502) staff       (20)    16384 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/tools/difference.py
--rw-r--r--   0 ilia       (502) staff       (20)     6812 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/tools/json_reader.py
--rw-r--r--   0 ilia       (502) staff       (20)    10455 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/tools/key.py
--rw-r--r--   0 ilia       (502) staff       (20)     9660 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/tools/metadata.py
--rw-r--r--   0 ilia       (502) staff       (20)     2460 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/tools/surftheowl_json.py
--rw-r--r--   0 ilia       (502) staff       (20)     4386 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/FAIRSave/tools/validation.py
-drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:53:46.199094 FAIRSave-0.0.6.6/FAIRSave.egg-info/
--rw-r--r--   0 ilia       (502) staff       (20)     3443 2023-06-27 08:53:46.000000 FAIRSave-0.0.6.6/FAIRSave.egg-info/PKG-INFO
--rw-r--r--   0 ilia       (502) staff       (20)      667 2023-06-27 08:53:46.000000 FAIRSave-0.0.6.6/FAIRSave.egg-info/SOURCES.txt
--rw-r--r--   0 ilia       (502) staff       (20)        1 2023-06-27 08:53:46.000000 FAIRSave-0.0.6.6/FAIRSave.egg-info/dependency_links.txt
--rw-r--r--   0 ilia       (502) staff       (20)       57 2023-06-27 08:53:46.000000 FAIRSave-0.0.6.6/FAIRSave.egg-info/requires.txt
--rw-r--r--   0 ilia       (502) staff       (20)        9 2023-06-27 08:53:46.000000 FAIRSave-0.0.6.6/FAIRSave.egg-info/top_level.txt
--rw-r--r--   0 ilia       (502) staff       (20)    11533 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/LICENSE
--rw-r--r--   0 ilia       (502) staff       (20)     3443 2023-06-27 08:53:46.208125 FAIRSave-0.0.6.6/PKG-INFO
--rw-r--r--   0 ilia       (502) staff       (20)     2858 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.6/README.md
--rw-r--r--   0 ilia       (502) staff       (20)       38 2023-06-27 08:53:46.209131 FAIRSave-0.0.6.6/setup.cfg
--rw-r--r--   0 ilia       (502) staff       (20)     1187 2023-06-27 08:53:26.000000 FAIRSave-0.0.6.6/setup.py
+drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:56:15.117796 FAIRSave-0.0.6.7/
+drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:56:15.106003 FAIRSave-0.0.6.7/FAIRSave/
+-rw-r--r--   0 ilia       (502) staff       (20)        0 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/__init__.py
+-rw-r--r--   0 ilia       (502) staff       (20)     9069 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/configuration.py
+-rw-r--r--   0 ilia       (502) staff       (20)     2780 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/eln_manager.py
+-rw-r--r--   0 ilia       (502) staff       (20)     4351 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/kadi_download.py
+-rw-r--r--   0 ilia       (502) staff       (20)    18105 2023-06-27 08:55:47.000000 FAIRSave-0.0.6.7/FAIRSave/kadi_identifier.py
+-rw-r--r--   0 ilia       (502) staff       (20)     3512 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/kadi_instances.py
+-rw-r--r--   0 ilia       (502) staff       (20)     8304 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/kadi_json_writer.py
+-rw-r--r--   0 ilia       (502) staff       (20)    14148 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/kadi_record.py
+-rw-r--r--   0 ilia       (502) staff       (20)    11777 2023-06-27 08:55:47.000000 FAIRSave-0.0.6.7/FAIRSave/kadi_search.py
+-rw-r--r--   0 ilia       (502) staff       (20)     1315 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/kadi_template.py
+drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:56:15.115873 FAIRSave-0.0.6.7/FAIRSave/tools/
+-rw-r--r--   0 ilia       (502) staff       (20)        0 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/tools/__init__.py
+-rw-r--r--   0 ilia       (502) staff       (20)     9224 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/tools/comparison.py
+-rw-r--r--   0 ilia       (502) staff       (20)    16384 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/tools/difference.py
+-rw-r--r--   0 ilia       (502) staff       (20)     6812 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/tools/json_reader.py
+-rw-r--r--   0 ilia       (502) staff       (20)    10455 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/tools/key.py
+-rw-r--r--   0 ilia       (502) staff       (20)     9660 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/tools/metadata.py
+-rw-r--r--   0 ilia       (502) staff       (20)     2460 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/tools/surftheowl_json.py
+-rw-r--r--   0 ilia       (502) staff       (20)     4386 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/FAIRSave/tools/validation.py
+drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:56:15.109083 FAIRSave-0.0.6.7/FAIRSave.egg-info/
+-rw-r--r--   0 ilia       (502) staff       (20)     3443 2023-06-27 08:56:15.000000 FAIRSave-0.0.6.7/FAIRSave.egg-info/PKG-INFO
+-rw-r--r--   0 ilia       (502) staff       (20)      667 2023-06-27 08:56:15.000000 FAIRSave-0.0.6.7/FAIRSave.egg-info/SOURCES.txt
+-rw-r--r--   0 ilia       (502) staff       (20)        1 2023-06-27 08:56:15.000000 FAIRSave-0.0.6.7/FAIRSave.egg-info/dependency_links.txt
+-rw-r--r--   0 ilia       (502) staff       (20)       57 2023-06-27 08:56:15.000000 FAIRSave-0.0.6.7/FAIRSave.egg-info/requires.txt
+-rw-r--r--   0 ilia       (502) staff       (20)        9 2023-06-27 08:56:15.000000 FAIRSave-0.0.6.7/FAIRSave.egg-info/top_level.txt
+-rw-r--r--   0 ilia       (502) staff       (20)    11533 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/LICENSE
+-rw-r--r--   0 ilia       (502) staff       (20)     3443 2023-06-27 08:56:15.117116 FAIRSave-0.0.6.7/PKG-INFO
+-rw-r--r--   0 ilia       (502) staff       (20)     2858 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.7/README.md
+-rw-r--r--   0 ilia       (502) staff       (20)       38 2023-06-27 08:56:15.117976 FAIRSave-0.0.6.7/setup.cfg
+-rw-r--r--   0 ilia       (502) staff       (20)     1187 2023-06-27 08:55:55.000000 FAIRSave-0.0.6.7/setup.py
```

### Comparing `FAIRSave-0.0.6.6/FAIRSave/configuration.py` & `FAIRSave-0.0.6.7/FAIRSave/configuration.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/eln_manager.py` & `FAIRSave-0.0.6.7/FAIRSave/eln_manager.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/kadi_download.py` & `FAIRSave-0.0.6.7/FAIRSave/kadi_download.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/kadi_identifier.py` & `FAIRSave-0.0.6.7/FAIRSave/kadi_identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     """
     
     if collection is not None:
         collection_id = search_item_id_kadi(instance,
                                             title=collection,
                                             item='collection')
         
-    sr = KadiManager(instance).search_resources()
+    sr = KadiManager(instance).search_resource()
     search_results = (sr.search_items(  item=item,
                                         visibility=visibility,
                                         collection=collection_id,
                                         child_collections=child_collections,
                                         per_page=100))
     pages = search_results.json()['_pagination'].get('total_pages')
 
@@ -189,15 +189,15 @@
     
     # list_of_tuples = []
     # # Store string of tuples as list of tuples
     # list_of_strings = string_of_tuples.split('\n')
     # for string in list_of_strings:
     #     list_of_tuples.append(tuple(map(str, string.split('\t'))))
     
-    sr = KadiManager(instance).search_resources()
+    sr = KadiManager(instance).search_resource()
     search_results = (sr.search_items(  item='record',
                                         visibility='private',
                                         collection=1141,
                                         child_collections=True,
                                         per_page=100))
     pages = search_results.json()['_pagination'].get('total_pages')
 
@@ -296,15 +296,15 @@
     Returns:
         List: List of tuples with titles, invalid identifiers and ids.
     """
 
     if collection != None:
         collection_id = search_item_id_kadi(instance, collection, 'collection')
 
-    searchresource = KadiManager(instance=instance).search_resources()
+    searchresource = KadiManager(instance=instance).search_resource()
     search_results = (searchresource.search_items(item='record',collection=collection_id,child_collections=True,visibility="private",per_page =100))
     total_items = search_results.json()['_pagination'].get('total_items')
     per_page = search_results.json()['_pagination'].get('per_page')
     
     tuples = []
     for n in range(math.ceil(total_items / per_page)):
         var = searchresource.search_items(item='record',collection=collection_id,per_page =100,child_collections=True,visibility="private", page=n+1).json().get('items')
```

### Comparing `FAIRSave-0.0.6.6/FAIRSave/kadi_instances.py` & `FAIRSave-0.0.6.7/FAIRSave/kadi_instances.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/kadi_json_writer.py` & `FAIRSave-0.0.6.7/FAIRSave/kadi_json_writer.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/kadi_record.py` & `FAIRSave-0.0.6.7/FAIRSave/kadi_record.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/kadi_search.py` & `FAIRSave-0.0.6.7/FAIRSave/kadi_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         description = None
 
     if collection is not None:
         collection_id = search_item_id_kadi(instance,
                                             title=collection,
                                             item='collection')
 
-    sr = KadiManager(instance=instance).search_resources()
+    sr = KadiManager(instance=instance).search_resource()
 
     search_results = (sr.search_items(item=item,
                                       type=record_type,
                                       collection=collection_id,
                                       per_page=100,
                                       visibility=visibility))
     pages = search_results.json()['_pagination'].get('total_pages')
@@ -129,15 +129,15 @@
         int: Id of the record.
     """
     if collection is not None:
         collection_id = search_item_id_kadi(instance,
                                             title=collection,
                                             item='collection')
 
-    sr = KadiManager(instance=instance).search_resources()
+    sr = KadiManager(instance=instance).search_resource()
     search_results = (sr.search_items(item=item,
                                       collection=collection_id,
                                       type=record_type,
                                       title=title,
                                       per_page=100,
                                       visibility=visibility))
     pages = search_results.json()['_pagination'].get('total_pages')
@@ -218,15 +218,15 @@
     """
 
     if collection is not None:
         collection_id = search_item_id_kadi(instance,
                                             title=collection,
                                             item='collection')
 
-    sr = KadiManager(instance=instance).search_resources()
+    sr = KadiManager(instance=instance).search_resource()
     search_results = (sr.search_items(item=item,
                                       collection=collection_id,
                                       type=record_type,
                                       title=title,
                                       per_page=100,
                                       visibility=visibility))
     pages = search_results.json()['_pagination'].get('total_pages')
```

### Comparing `FAIRSave-0.0.6.6/FAIRSave/kadi_template.py` & `FAIRSave-0.0.6.7/FAIRSave/kadi_template.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/tools/comparison.py` & `FAIRSave-0.0.6.7/FAIRSave/tools/comparison.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/tools/difference.py` & `FAIRSave-0.0.6.7/FAIRSave/tools/difference.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/tools/json_reader.py` & `FAIRSave-0.0.6.7/FAIRSave/tools/json_reader.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/tools/key.py` & `FAIRSave-0.0.6.7/FAIRSave/tools/key.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/tools/metadata.py` & `FAIRSave-0.0.6.7/FAIRSave/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/tools/surftheowl_json.py` & `FAIRSave-0.0.6.7/FAIRSave/tools/surftheowl_json.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave/tools/validation.py` & `FAIRSave-0.0.6.7/FAIRSave/tools/validation.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/FAIRSave.egg-info/PKG-INFO` & `FAIRSave-0.0.6.7/FAIRSave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FAIRSave
-Version: 0.0.6.6
+Version: 0.0.6.7
 Summary: Package to run the FAIR-Save toolbox
 Author: Malte Flachmann, Floriane Bresser, Ilia Bagov (Karlsruhe Institute of Technology)
 Author-email: malte.flachmann@student.kit.edu
 License: Apache-2.0
 Project-URL: GitLab, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save_Utilities
 Project-URL: Changelog, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save-Utilities/-/blob/main/Changelog.md
 Keywords: Kadi4Mat,FAIR
```

### Comparing `FAIRSave-0.0.6.6/FAIRSave.egg-info/SOURCES.txt` & `FAIRSave-0.0.6.7/FAIRSave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/LICENSE` & `FAIRSave-0.0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/PKG-INFO` & `FAIRSave-0.0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FAIRSave
-Version: 0.0.6.6
+Version: 0.0.6.7
 Summary: Package to run the FAIR-Save toolbox
 Author: Malte Flachmann, Floriane Bresser, Ilia Bagov (Karlsruhe Institute of Technology)
 Author-email: malte.flachmann@student.kit.edu
 License: Apache-2.0
 Project-URL: GitLab, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save_Utilities
 Project-URL: Changelog, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save-Utilities/-/blob/main/Changelog.md
 Keywords: Kadi4Mat,FAIR
```

### Comparing `FAIRSave-0.0.6.6/README.md` & `FAIRSave-0.0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.6/setup.py` & `FAIRSave-0.0.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="FAIRSave",
-    version="0.0.6.6",
+    version="0.0.6.7",
     project_urls={"GitLab": "https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save_Utilities",
                   "Changelog": "https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save-Utilities/-/blob/main/Changelog.md"},
     author="Malte Flachmann, Floriane Bresser, Ilia Bagov (Karlsruhe Institute of Technology)",
     author_email="malte.flachmann@student.kit.edu",
     license="Apache-2.0",
     description="Package to run the FAIR-Save toolbox",
     long_description=long_description,
```

