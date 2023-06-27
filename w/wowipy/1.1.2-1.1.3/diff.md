# Comparing `tmp/wowipy-1.1.2.tar.gz` & `tmp/wowipy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wowipy-1.1.2.tar", last modified: Tue Jun 27 13:20:39 2023, max compression
+gzip compressed data, was "wowipy-1.1.3.tar", last modified: Tue Jun 27 14:19:54 2023, max compression
```

## Comparing `wowipy-1.1.2.tar` & `wowipy-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 13:20:39.389423 wowipy-1.1.2/
--rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.2/COPYING
--rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-06-27 13:20:39.388411 wowipy-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-27 13:20:39.389423 wowipy-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1277 2023-06-27 13:19:57.000000 wowipy-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:20:39.372455 wowipy-1.1.2/wowipy/
--rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.2/wowipy/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.2/wowipy/exceptions.py
--rw-rw-rw-   0        0        0    38772 2023-06-27 12:49:00.000000 wowipy-1.1.2/wowipy/models.py
--rw-rw-rw-   0        0        0     4550 2023-06-27 13:11:28.000000 wowipy-1.1.2/wowipy/rest_adapter.py
--rw-rw-rw-   0        0        0    40022 2023-06-27 13:11:28.000000 wowipy-1.1.2/wowipy/wowipy.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:20:39.387414 wowipy-1.1.2/wowipy.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-06-27 13:20:39.000000 wowipy-1.1.2/wowipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-27 13:20:39.000000 wowipy-1.1.2/wowipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 13:20:39.000000 wowipy-1.1.2/wowipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-27 13:20:39.000000 wowipy-1.1.2/wowipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 13:20:39.000000 wowipy-1.1.2/wowipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 14:19:54.879138 wowipy-1.1.3/
+-rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.3/COPYING
+-rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-06-27 14:19:54.879138 wowipy-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-27 14:19:54.879138 wowipy-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-06-27 13:46:21.000000 wowipy-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:19:54.859192 wowipy-1.1.3/wowipy/
+-rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.3/wowipy/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.3/wowipy/exceptions.py
+-rw-rw-rw-   0        0        0    38772 2023-06-27 12:49:00.000000 wowipy-1.1.3/wowipy/models.py
+-rw-rw-rw-   0        0        0     4550 2023-06-27 13:11:28.000000 wowipy-1.1.3/wowipy/rest_adapter.py
+-rw-rw-rw-   0        0        0    41565 2023-06-27 14:00:21.000000 wowipy-1.1.3/wowipy/wowipy.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:19:54.878143 wowipy-1.1.3/wowipy.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-06-27 14:19:54.000000 wowipy-1.1.3/wowipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-27 14:19:54.000000 wowipy-1.1.3/wowipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 14:19:54.000000 wowipy-1.1.3/wowipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 14:19:54.000000 wowipy-1.1.3/wowipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 14:19:54.000000 wowipy-1.1.3/wowipy.egg-info/top_level.txt
```

### Comparing `wowipy-1.1.2/COPYING` & `wowipy-1.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.2/LICENSE` & `wowipy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.2/PKG-INFO` & `wowipy-1.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.2
+Version: 1.1.3
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `wowipy-1.1.2/setup.py` & `wowipy-1.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup
 
 setup(
     name='wowipy',
-    version='1.1.2',
+    version='1.1.3',
     description='OPENWOWI Wowiport API wrapper for python',
     url='https://github.com/seb-bau/WowiPy',
     author='Sebastian Bauhaus',
     author_email='sebastian@bytewish.de',
     license='GPL-3.0',
     packages=['wowipy'],
     install_requires=['requests>=2.0',
                       'pyhumps>=3.0',
+                      'jsonmerge>=1.9'
                       ],
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Other Audience',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```

### Comparing `wowipy-1.1.2/wowipy/models.py` & `wowipy-1.1.3/wowipy/models.py`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.2/wowipy/rest_adapter.py` & `wowipy-1.1.3/wowipy/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.2/wowipy/wowipy.py` & `wowipy-1.1.3/wowipy/wowipy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 import logging
 import humps
 import pickle
+from jsonmerge import Merger
 from wowipy.rest_adapter import RestAdapter
 from wowipy.exceptions import WowiPyException
 from wowipy.models import *
 
 
 class WowiPy:
     CACHE_LICENSE_AGREEMENTS = "license_agreements"
@@ -263,23 +264,23 @@
         :return: Liste mit Nutzungsverträgen (auch bei nur einem Ergebnis!)
         :rtype: Liste[LicenseAgreement]
         """
         limit = 100
         offset = 0
         ret_list = self.get_building_lands(management_idnum=management_idnum,
                                            owner_number=owner_number,
-                                           economic_idnum=economic_idnum,
+                                           economic_unit_idnum=economic_idnum,
                                            add_args=add_args, limit=limit, offset=offset)
         response_len = len(ret_list)
 
         while response_len == limit:
             offset += limit
             t_resp = self.get_building_lands(management_idnum=management_idnum,
                                              owner_number=owner_number,
-                                             economic_idnum=economic_idnum,
+                                             economic_unit_idnum=economic_idnum,
                                              add_args=add_args, limit=limit, offset=offset)
             response_len = len(t_resp)
             ret_list = ret_list + t_resp
             print(f"Building lands {len(ret_list)}")
 
         self._cache[self.CACHE_BUILDING_LANDS] = ret_list
 
@@ -543,29 +544,35 @@
             ret_la = EconomicUnit(**data)
             retlist.append(ret_la)
         return retlist
 
     def get_building_lands(self,
                            management_idnum: str = None,
                            owner_number: str = None,
-                           economic_idnum: str = None,
+                           economic_unit_idnum: str = None,
                            building_land_idnum: str = None,
                            limit: int = None,
                            offset: int = 0,
-                           add_args: Dict = None) -> List[BuildingLand]:
+                           add_args: Dict = None,
+                           fetch_all: bool = False,
+                           use_cache: bool = False) -> List[BuildingLand]:
         """
         Gibt ein oder mehrere Gebäude als Liste zurück.
+        :param fetch_all:
+        :type fetch_all:
+        :param use_cache:
+        :type use_cache:
         :param offset: Verschiebung der Abfrage. Default: 0
         :type offset: int
         :param management_idnum: (Optional) Nur Gebäude dieses Managements zurückgeben
         :type management_idnum: str
         :param owner_number: (Optional) Nur Gebäude dieses Eigentümers zurückgeben
         :type owner_number: str
-        :param economic_idnum: (Optional) Nur Gebäude dieser Wirtschaftseinheit zurückgeben
-        :type economic_idnum: str
+        :param economic_unit_idnum: (Optional) Nur Gebäude dieser Wirtschaftseinheit zurückgeben
+        :type economic_unit_idnum: str
         :param building_land_idnum: (Optional) Nur das Gebäude mit dieser IdNum zurückgeben
         :type building_land_idnum: str
         :param limit: Maxmiale Anzahl an Einträgen, die zurückgegeben werden sollen (max = default = 100)
         :type limit: 100
         :param add_args: Zusätzlich GET-Parameter als DICT, die an die URL angehängt werden.
         :type add_args: Dict
         :return: Liste mit Gebäuden (auch bei nur einem Ergebnis!)
@@ -573,36 +580,59 @@
         """
 
         filter_params = {}
         if management_idnum is not None:
             filter_params['managementIdNum'] = management_idnum
         if owner_number is not None:
             filter_params['ownerNumber'] = owner_number
-        if economic_idnum is not None:
-            filter_params['economicIdNum'] = economic_idnum
+        if economic_unit_idnum is not None:
+            filter_params['economicIdNum'] = economic_unit_idnum
         if building_land_idnum is not None:
             filter_params['buildingLandIdNum'] = building_land_idnum
         if limit is not None:
             filter_params['limit'] = limit
         filter_params['offset'] = offset
 
         # Ein paar Standardwerte, können aber durch add_args überschrieben werden
         filter_params['includeCompanyCode'] = 'true'
 
         if add_args is not None:
             filter_params.update(add_args)
-
-        result = self._rest_adapter.get(endpoint='CommercialInventory/BuildingLands', ep_params=filter_params)
         retlist = []
-        for entry in result.data:
-            data = dict(humps.decamelize(entry))
-            data['id_'] = data.pop('id')
-            data.get('estate_address')['zip_'] = data.get('estate_address').pop('zip')
-            ret_la = BuildingLand(**data)
-            retlist.append(ret_la)
+        if use_cache:
+            cache_entry: BuildingLand
+            for cache_entry in self._cache[self.CACHE_BUILDING_LANDS]:
+                if (economic_unit_idnum is not None and
+                    cache_entry.economic_unit.id_num == economic_unit_idnum) or \
+                        economic_unit_idnum is None:
+                    retlist.append(copy.deepcopy(cache_entry))
+        else:
+            if not fetch_all:
+                result = self._rest_adapter.get(endpoint='CommercialInventory/BuildingLands', ep_params=filter_params)
+            else:
+                result = Result(0, "", [])
+                merge_schema = {"mergeStrategy": "append"}
+                merger = Merger(schema=merge_schema)
+                filter_params['offset'] = 0
+                filter_params['limit'] = 100
+                response_count = 100
+                while response_count == 100:
+                    part_result = self._rest_adapter.get(endpoint='CommercialInventory/BuildingLands',
+                                                         ep_params=filter_params)
+                    result.data = merger.merge(result.data, part_result.data)
+                    filter_params['offset'] += 100
+                    response_count = len(part_result.data)
+                    print(f"Building-Count: {len(result.data)}")
+
+            for entry in result.data:
+                data = dict(humps.decamelize(entry))
+                data['id_'] = data.pop('id')
+                data.get('estate_address')['zip_'] = data.get('estate_address').pop('zip')
+                ret_la = BuildingLand(**data)
+                retlist.append(ret_la)
         return retlist
 
     def get_owners(self,
                    owner_number: str = None,
                    limit: int = None,
                    offset: int = 0,
                    add_args: Dict = None) -> List[Owner]:
```

### Comparing `wowipy-1.1.2/wowipy.egg-info/PKG-INFO` & `wowipy-1.1.3/wowipy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.2
+Version: 1.1.3
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

