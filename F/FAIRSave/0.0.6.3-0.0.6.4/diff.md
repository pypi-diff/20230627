# Comparing `tmp/FAIRSave-0.0.6.3.tar.gz` & `tmp/FAIRSave-0.0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FAIRSave-0.0.6.3.tar", last modified: Tue Jun 27 08:16:26 2023, max compression
+gzip compressed data, was "FAIRSave-0.0.6.4.tar", last modified: Tue Jun 27 08:27:38 2023, max compression
```

## Comparing `FAIRSave-0.0.6.3.tar` & `FAIRSave-0.0.6.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:16:26.455692 FAIRSave-0.0.6.3/
-drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:16:26.445150 FAIRSave-0.0.6.3/FAIRSave/
--rw-r--r--   0 ilia       (502) staff       (20)        0 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/__init__.py
--rw-r--r--   0 ilia       (502) staff       (20)     9069 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/configuration.py
--rw-r--r--   0 ilia       (502) staff       (20)     2780 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/eln_manager.py
--rw-r--r--   0 ilia       (502) staff       (20)     4351 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/kadi_download.py
--rw-r--r--   0 ilia       (502) staff       (20)    18108 2023-06-27 08:05:47.000000 FAIRSave-0.0.6.3/FAIRSave/kadi_identifier.py
--rw-r--r--   0 ilia       (502) staff       (20)     3512 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/kadi_instances.py
--rw-r--r--   0 ilia       (502) staff       (20)     8304 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/kadi_json_writer.py
--rw-r--r--   0 ilia       (502) staff       (20)    14148 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/kadi_record.py
--rw-r--r--   0 ilia       (502) staff       (20)    11780 2023-06-27 08:05:47.000000 FAIRSave-0.0.6.3/FAIRSave/kadi_search.py
--rw-r--r--   0 ilia       (502) staff       (20)     1315 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/kadi_template.py
-drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:16:26.454341 FAIRSave-0.0.6.3/FAIRSave/tools/
--rw-r--r--   0 ilia       (502) staff       (20)        0 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/tools/__init__.py
--rw-r--r--   0 ilia       (502) staff       (20)     9224 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/tools/comparison.py
--rw-r--r--   0 ilia       (502) staff       (20)    16384 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/tools/difference.py
--rw-r--r--   0 ilia       (502) staff       (20)     6812 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/tools/json_reader.py
--rw-r--r--   0 ilia       (502) staff       (20)    10455 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/tools/key.py
--rw-r--r--   0 ilia       (502) staff       (20)     9660 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/tools/metadata.py
--rw-r--r--   0 ilia       (502) staff       (20)     2460 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/tools/surftheowl_json.py
--rw-r--r--   0 ilia       (502) staff       (20)     4386 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/FAIRSave/tools/validation.py
-drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:16:26.448448 FAIRSave-0.0.6.3/FAIRSave.egg-info/
--rw-r--r--   0 ilia       (502) staff       (20)     3443 2023-06-27 08:16:26.000000 FAIRSave-0.0.6.3/FAIRSave.egg-info/PKG-INFO
--rw-r--r--   0 ilia       (502) staff       (20)      667 2023-06-27 08:16:26.000000 FAIRSave-0.0.6.3/FAIRSave.egg-info/SOURCES.txt
--rw-r--r--   0 ilia       (502) staff       (20)        1 2023-06-27 08:16:26.000000 FAIRSave-0.0.6.3/FAIRSave.egg-info/dependency_links.txt
--rw-r--r--   0 ilia       (502) staff       (20)       57 2023-06-27 08:16:26.000000 FAIRSave-0.0.6.3/FAIRSave.egg-info/requires.txt
--rw-r--r--   0 ilia       (502) staff       (20)        9 2023-06-27 08:16:26.000000 FAIRSave-0.0.6.3/FAIRSave.egg-info/top_level.txt
--rw-r--r--   0 ilia       (502) staff       (20)    11533 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/LICENSE
--rw-r--r--   0 ilia       (502) staff       (20)     3443 2023-06-27 08:16:26.455199 FAIRSave-0.0.6.3/PKG-INFO
--rw-r--r--   0 ilia       (502) staff       (20)     2858 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.3/README.md
--rw-r--r--   0 ilia       (502) staff       (20)       38 2023-06-27 08:16:26.455819 FAIRSave-0.0.6.3/setup.cfg
--rw-r--r--   0 ilia       (502) staff       (20)     1187 2023-06-27 08:06:42.000000 FAIRSave-0.0.6.3/setup.py
+drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:27:38.013455 FAIRSave-0.0.6.4/
+drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:27:38.000734 FAIRSave-0.0.6.4/FAIRSave/
+-rw-r--r--   0 ilia       (502) staff       (20)        0 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/__init__.py
+-rw-r--r--   0 ilia       (502) staff       (20)     9069 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/configuration.py
+-rw-r--r--   0 ilia       (502) staff       (20)     2780 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/eln_manager.py
+-rw-r--r--   0 ilia       (502) staff       (20)     4351 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/kadi_download.py
+-rw-r--r--   0 ilia       (502) staff       (20)    18129 2023-06-27 08:27:06.000000 FAIRSave-0.0.6.4/FAIRSave/kadi_identifier.py
+-rw-r--r--   0 ilia       (502) staff       (20)     3512 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/kadi_instances.py
+-rw-r--r--   0 ilia       (502) staff       (20)     8304 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/kadi_json_writer.py
+-rw-r--r--   0 ilia       (502) staff       (20)    14148 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/kadi_record.py
+-rw-r--r--   0 ilia       (502) staff       (20)    11801 2023-06-27 08:27:06.000000 FAIRSave-0.0.6.4/FAIRSave/kadi_search.py
+-rw-r--r--   0 ilia       (502) staff       (20)     1315 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/kadi_template.py
+drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:27:38.011562 FAIRSave-0.0.6.4/FAIRSave/tools/
+-rw-r--r--   0 ilia       (502) staff       (20)        0 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/tools/__init__.py
+-rw-r--r--   0 ilia       (502) staff       (20)     9224 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/tools/comparison.py
+-rw-r--r--   0 ilia       (502) staff       (20)    16384 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/tools/difference.py
+-rw-r--r--   0 ilia       (502) staff       (20)     6812 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/tools/json_reader.py
+-rw-r--r--   0 ilia       (502) staff       (20)    10455 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/tools/key.py
+-rw-r--r--   0 ilia       (502) staff       (20)     9660 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/tools/metadata.py
+-rw-r--r--   0 ilia       (502) staff       (20)     2460 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/tools/surftheowl_json.py
+-rw-r--r--   0 ilia       (502) staff       (20)     4386 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/FAIRSave/tools/validation.py
+drwxr-xr-x   0 ilia       (502) staff       (20)        0 2023-06-27 08:27:38.004205 FAIRSave-0.0.6.4/FAIRSave.egg-info/
+-rw-r--r--   0 ilia       (502) staff       (20)     3443 2023-06-27 08:27:37.000000 FAIRSave-0.0.6.4/FAIRSave.egg-info/PKG-INFO
+-rw-r--r--   0 ilia       (502) staff       (20)      667 2023-06-27 08:27:37.000000 FAIRSave-0.0.6.4/FAIRSave.egg-info/SOURCES.txt
+-rw-r--r--   0 ilia       (502) staff       (20)        1 2023-06-27 08:27:37.000000 FAIRSave-0.0.6.4/FAIRSave.egg-info/dependency_links.txt
+-rw-r--r--   0 ilia       (502) staff       (20)       57 2023-06-27 08:27:37.000000 FAIRSave-0.0.6.4/FAIRSave.egg-info/requires.txt
+-rw-r--r--   0 ilia       (502) staff       (20)        9 2023-06-27 08:27:37.000000 FAIRSave-0.0.6.4/FAIRSave.egg-info/top_level.txt
+-rw-r--r--   0 ilia       (502) staff       (20)    11533 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/LICENSE
+-rw-r--r--   0 ilia       (502) staff       (20)     3443 2023-06-27 08:27:38.012706 FAIRSave-0.0.6.4/PKG-INFO
+-rw-r--r--   0 ilia       (502) staff       (20)     2858 2023-06-27 08:04:52.000000 FAIRSave-0.0.6.4/README.md
+-rw-r--r--   0 ilia       (502) staff       (20)       38 2023-06-27 08:27:38.013615 FAIRSave-0.0.6.4/setup.cfg
+-rw-r--r--   0 ilia       (502) staff       (20)     1187 2023-06-27 08:23:33.000000 FAIRSave-0.0.6.4/setup.py
```

### Comparing `FAIRSave-0.0.6.3/FAIRSave/configuration.py` & `FAIRSave-0.0.6.4/FAIRSave/configuration.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/eln_manager.py` & `FAIRSave-0.0.6.4/FAIRSave/eln_manager.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/kadi_download.py` & `FAIRSave-0.0.6.4/FAIRSave/kadi_download.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/kadi_identifier.py` & `FAIRSave-0.0.6.4/FAIRSave/kadi_identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     """
     
     if collection is not None:
         collection_id = search_item_id_kadi(instance,
                                             title=collection,
                                             item='collection')
         
-    sr = KadiManager(instance).search_resources()
+    sr = KadiManager(instance).search.search_resources()
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
+    sr = KadiManager(instance).search.search_resources()
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
+    searchresource = KadiManager(instance=instance).search.search_resources()
     search_results = (searchresource.search_items(item='record',collection=collection_id,child_collections=True,visibility="private",per_page =100))
     total_items = search_results.json()['_pagination'].get('total_items')
     per_page = search_results.json()['_pagination'].get('per_page')
     
     tuples = []
     for n in range(math.ceil(total_items / per_page)):
         var = searchresource.search_items(item='record',collection=collection_id,per_page =100,child_collections=True,visibility="private", page=n+1).json().get('items')
```

### Comparing `FAIRSave-0.0.6.3/FAIRSave/kadi_instances.py` & `FAIRSave-0.0.6.4/FAIRSave/kadi_instances.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/kadi_json_writer.py` & `FAIRSave-0.0.6.4/FAIRSave/kadi_json_writer.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/kadi_record.py` & `FAIRSave-0.0.6.4/FAIRSave/kadi_record.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/kadi_search.py` & `FAIRSave-0.0.6.4/FAIRSave/kadi_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         description = None
 
     if collection is not None:
         collection_id = search_item_id_kadi(instance,
                                             title=collection,
                                             item='collection')
 
-    sr = KadiManager(instance=instance).search_resources()
+    sr = KadiManager(instance=instance).search.search_resources()
 
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
+    sr = KadiManager(instance=instance).search.search_resources()
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
+    sr = KadiManager(instance=instance).search.search_resources()
     search_results = (sr.search_items(item=item,
                                       collection=collection_id,
                                       type=record_type,
                                       title=title,
                                       per_page=100,
                                       visibility=visibility))
     pages = search_results.json()['_pagination'].get('total_pages')
```

### Comparing `FAIRSave-0.0.6.3/FAIRSave/kadi_template.py` & `FAIRSave-0.0.6.4/FAIRSave/kadi_template.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/tools/comparison.py` & `FAIRSave-0.0.6.4/FAIRSave/tools/comparison.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/tools/difference.py` & `FAIRSave-0.0.6.4/FAIRSave/tools/difference.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/tools/json_reader.py` & `FAIRSave-0.0.6.4/FAIRSave/tools/json_reader.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/tools/key.py` & `FAIRSave-0.0.6.4/FAIRSave/tools/key.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/tools/metadata.py` & `FAIRSave-0.0.6.4/FAIRSave/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/tools/surftheowl_json.py` & `FAIRSave-0.0.6.4/FAIRSave/tools/surftheowl_json.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave/tools/validation.py` & `FAIRSave-0.0.6.4/FAIRSave/tools/validation.py`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/FAIRSave.egg-info/PKG-INFO` & `FAIRSave-0.0.6.4/FAIRSave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FAIRSave
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: Package to run the FAIR-Save toolbox
 Author: Malte Flachmann, Floriane Bresser, Ilia Bagov (Karlsruhe Institute of Technology)
 Author-email: malte.flachmann@student.kit.edu
 License: Apache-2.0
 Project-URL: GitLab, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save_Utilities
 Project-URL: Changelog, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save-Utilities/-/blob/main/Changelog.md
 Keywords: Kadi4Mat,FAIR
```

### Comparing `FAIRSave-0.0.6.3/FAIRSave.egg-info/SOURCES.txt` & `FAIRSave-0.0.6.4/FAIRSave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/LICENSE` & `FAIRSave-0.0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/PKG-INFO` & `FAIRSave-0.0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FAIRSave
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: Package to run the FAIR-Save toolbox
 Author: Malte Flachmann, Floriane Bresser, Ilia Bagov (Karlsruhe Institute of Technology)
 Author-email: malte.flachmann@student.kit.edu
 License: Apache-2.0
 Project-URL: GitLab, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save_Utilities
 Project-URL: Changelog, https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save-Utilities/-/blob/main/Changelog.md
 Keywords: Kadi4Mat,FAIR
```

### Comparing `FAIRSave-0.0.6.3/README.md` & `FAIRSave-0.0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `FAIRSave-0.0.6.3/setup.py` & `FAIRSave-0.0.6.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="FAIRSave",
-    version="0.0.6.3",
+    version="0.0.6.4",
     project_urls={"GitLab": "https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save_Utilities",
                   "Changelog": "https://gitlab.com/linked-tribological-data/fair-save/FAIR-Save-Utilities/-/blob/main/Changelog.md"},
     author="Malte Flachmann, Floriane Bresser, Ilia Bagov (Karlsruhe Institute of Technology)",
     author_email="malte.flachmann@student.kit.edu",
     license="Apache-2.0",
     description="Package to run the FAIR-Save toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     keywords="Kadi4Mat, FAIR",
     python_requires='>=3.10',
-    install_requires=['kadi-apy>=0.25.0',
+    install_requires=['kadi-apy>=0.30.0',
                       'xmltodict>=0.13.0',
                       'nested_lookup>=0.2.25']
     )
```

