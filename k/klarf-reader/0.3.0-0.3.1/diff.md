# Comparing `tmp/klarf-reader-0.3.0.tar.gz` & `tmp/klarf-reader-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarf-reader-0.3.0.tar", last modified: Wed Apr  5 15:55:19 2023, max compression
+gzip compressed data, was "klarf-reader-0.3.1.tar", last modified: Tue Jun 27 07:47:40 2023, max compression
```

## Comparing `klarf-reader-0.3.0.tar` & `klarf-reader-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 15:55:19.833808 klarf-reader-0.3.0/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      569 2023-04-05 15:55:19.830650 klarf-reader-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 15:55:19.755843 klarf-reader-0.3.0/klarf_reader/
--rw-rw-rw-   0        0        0     1054 2023-04-05 13:54:30.000000 klarf-reader-0.3.0/klarf_reader/klarf.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:55:19.804151 klarf-reader-0.3.0/klarf_reader/models/
--rw-rw-rw-   0        0        0     2084 2023-04-05 14:38:01.000000 klarf-reader-0.3.0/klarf_reader/models/klarf_content.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:55:19.811006 klarf-reader-0.3.0/klarf_reader/readers/
--rw-rw-rw-   0        0        0    12000 2023-04-05 15:51:59.000000 klarf-reader-0.3.0/klarf_reader/readers/klarf_file_reader.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:55:19.818174 klarf-reader-0.3.0/klarf_reader/utils/
--rw-rw-rw-   0        0        0     1377 2023-03-07 12:43:34.000000 klarf-reader-0.3.0/klarf_reader/utils/klarf_convert.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:55:19.796984 klarf-reader-0.3.0/klarf_reader.egg-info/
--rw-rw-rw-   0        0        0      569 2023-04-05 15:55:19.000000 klarf-reader-0.3.0/klarf_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-04-05 15:55:19.000000 klarf-reader-0.3.0/klarf_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 15:55:19.000000 klarf-reader-0.3.0/klarf_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-05 15:55:19.000000 klarf-reader-0.3.0/klarf_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-05 15:55:19.000000 klarf-reader-0.3.0/klarf_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 15:55:19.834875 klarf-reader-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-04-05 15:54:20.000000 klarf-reader-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:55:19.822702 klarf-reader-0.3.0/tests/
--rw-rw-rw-   0        0        0     4280 2023-04-05 15:47:48.000000 klarf-reader-0.3.0/tests/test_klarf.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:47:40.508157 klarf-reader-0.3.1/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      569 2023-06-27 07:47:40.502554 klarf-reader-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 07:47:40.415577 klarf-reader-0.3.1/klarf_reader/
+-rw-rw-rw-   0        0        0     1060 2023-06-27 07:08:50.000000 klarf-reader-0.3.1/klarf_reader/klarf.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:47:40.468010 klarf-reader-0.3.1/klarf_reader/models/
+-rw-rw-rw-   0        0        0     2365 2023-06-27 07:10:16.000000 klarf-reader-0.3.1/klarf_reader/models/klarf_content.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:47:40.479372 klarf-reader-0.3.1/klarf_reader/readers/
+-rw-rw-rw-   0        0        0    13286 2023-06-27 07:10:48.000000 klarf-reader-0.3.1/klarf_reader/readers/klarf_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:47:40.486815 klarf-reader-0.3.1/klarf_reader/utils/
+-rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.1/klarf_reader/utils/klarf_convert.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:47:40.459657 klarf-reader-0.3.1/klarf_reader.egg-info/
+-rw-rw-rw-   0        0        0      569 2023-06-27 07:47:40.000000 klarf-reader-0.3.1/klarf_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-06-27 07:47:40.000000 klarf-reader-0.3.1/klarf_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 07:47:40.000000 klarf-reader-0.3.1/klarf_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-27 07:47:40.000000 klarf-reader-0.3.1/klarf_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 07:47:40.000000 klarf-reader-0.3.1/klarf_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 07:47:40.509164 klarf-reader-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-06-27 07:45:36.000000 klarf-reader-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:47:40.497136 klarf-reader-0.3.1/tests/
+-rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.1/tests/test_klarf.py
```

### Comparing `klarf-reader-0.3.0/LICENSE.txt` & `klarf-reader-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.0/PKG-INFO` & `klarf-reader-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.0
+Version: 0.3.1
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.0.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.0/README.md` & `klarf-reader-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.0/klarf_reader/klarf.py` & `klarf-reader-0.3.1/klarf_reader/klarf.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from .readers import klarf_file_reader
 
 
 class Klarf:
     @staticmethod
     def load_from_file(
         filepath: Path,
-        custom_columns_lot: List[str] = None,
-        custom_columns_defects: List[str] = None,
+        custom_columns_wafer: List[str] = None,
+        custom_columns_defect: List[str] = None,
     ) -> KlarfContent:
         return Klarf.load_from_file_with_raw_content(
             filepath=filepath,
-            custom_columns_lot=custom_columns_lot,
-            custom_columns_defects=custom_columns_defects,
+            custom_columns_wafer=custom_columns_wafer,
+            custom_columns_defect=custom_columns_defect,
         )[0]
 
     @staticmethod
     def load_from_file_with_raw_content(
         filepath: Path,
-        custom_columns_lot: List[str] = None,
-        custom_columns_defects: List[str] = None,
+        custom_columns_wafer: List[str] = None,
+        custom_columns_defect: List[str] = None,
     ) -> Tuple[KlarfContent, List[str]]:
         return klarf_file_reader.readKlarf(
             klarf=filepath,
-            custom_columns_lot=custom_columns_lot,
-            custom_columns_defects=custom_columns_defects,
+            custom_columns_wafer=custom_columns_wafer,
+            custom_columns_defect=custom_columns_defect,
         )
 
     def __repr__(self):
         print(self.__dict__)
```

### Comparing `klarf-reader-0.3.0/klarf_reader/models/klarf_content.py` & `klarf-reader-0.3.1/klarf_reader/models/klarf_content.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     y_index: int
     x_size: float
     y_size: float
     area: float
     roughbin: int
     finebin: int
     point: Tuple[float, float] = field(default_factory=lambda: [])
-    custom_attribute:  Dict[str, any] = None
+    custom_attribute: Dict[str, any] = None
 
 
 @dataclass
 class Summary:
     defect_density: float = None
     number_of_defects: int = None
     number_of_dies: int = None
@@ -58,39 +58,55 @@
     percent_of_def_die: float = None
 
     def __post_init__(self):
         self.percent_of_def_die = float(self.number_of_def_dies / self.number_of_dies)
 
 
 @dataclass
+class Test:
+    id: int
+    area: float
+
+
+@dataclass
 class Wafer:
     id: str
     slot: int
     die_origin: DieOrigin
     sample_center_location: SampleCenterLocation
     defects: List[Defect] = field(default_factory=lambda: [])
+    tests: List[Test] = field(default_factory=lambda: [])
+    custom_attribute: Dict[str, any] = None
     summary: Summary = None
 
 
 @dataclass
+class InspectionStationId:
+    mfg: str
+    model: str
+    id: str
+
+
+@dataclass
 class BasicKlarfContent:
     file_version: float
     file_timestamp: str
-    inspection_station_id: str
+    sample_type: str
+    inspection_station_id: InspectionStationId
     result_timestamp: str
     lot_id: str
     device_id: str
     sample_size: int
     setup_id: SetupId
     step_id: str
+    sample_orientation_mark_type: str
     orientation_mark_location: str
     die_pitch: DiePitch
     has_sample_test_plan: bool
     sample_plan_test: SamplePlanTest
-    custom_attribute: Dict[str, any] = None
 
 
 @dataclass
 class KlarfContent(BasicKlarfContent):
     wafers: List[Wafer] = field(default_factory=lambda: [])
 
     @property
```

### Comparing `klarf-reader-0.3.0/klarf_reader/readers/klarf_file_reader.py` & `klarf-reader-0.3.1/klarf_reader/readers/klarf_file_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 from typing import List, Tuple
 
 # MODELS
 from ..models.klarf_content import (
     Defect,
     DieOrigin,
     DiePitch,
+    InspectionStationId,
     KlarfContent,
     SampleCenterLocation,
     SamplePlanTest,
     SetupId,
     Summary,
+    Test,
     Wafer,
 )
 
 ACCEPTED_KLARF_VERSIONS = [1.2]
 
 
 def readKlarf(
     klarf: Path,
-    custom_columns_lot: List[str] = None,
-    custom_columns_defects: List[str] = None,
+    custom_columns_wafer: List[str] = None,
+    custom_columns_defect: List[str] = None,
 ) -> Tuple[KlarfContent, List[str]]:
     """this function open, read and parse a klarf file
 
     Args:
         klarf (Path): the path of the klarf file
 
     Returns:
@@ -38,23 +40,23 @@
         raise Exception(f"{klarf=} does not exists")
 
     with open(klarf, "r") as f:
         raw_content = f.readlines()
 
     return convert_raw_to_klarf_content(
         raw_content=raw_content,
-        custom_columns_lot=custom_columns_lot,
-        custom_columns_defects=custom_columns_defects,
+        custom_columns_wafer=custom_columns_wafer,
+        custom_columns_defect=custom_columns_defect,
     )
 
 
 def convert_raw_to_klarf_content(
     raw_content: List[str],
-    custom_columns_lot: List[str] = None,
-    custom_columns_defects: List[str] = None,
+    custom_columns_wafer: List[str] = None,
+    custom_columns_defect: List[str] = None,
 ) -> Tuple[KlarfContent, List[str]]:
 
     RAW_DEFECT_COLUMNS = [
         "DEFECTID",
         "XREL",
         "YREL",
         "XINDEX",
@@ -65,37 +67,36 @@
     ]
 
     setup_id = "no_setup"
     next_line_has_coords, next_line_has_numb = False, False
     has_sample_test_plan, next_line_has_sample_test_plan = False, False
     sample_plan_test_x, sample_plan_test_y = [], []
     wafers: List[Wafer] = []
+    tests: List[Test] = []
 
-    column_custom_atribute_defect = []
+    if custom_columns_wafer is None:
+        custom_columns_wafer = []
 
-    if custom_columns_lot is None:
-        custom_columns_lot = []
-
-    if custom_columns_defects is None:
-        custom_columns_defects = []
+    if custom_columns_defect is None:
+        custom_columns_defect = []
 
     index = 0
     custom_columns_found = False
-    custom_columns_lot_dict = {}
+    custom_columns_wafer_dict = {}
     for line in raw_content:
         index += 1
         line: str = line.rstrip("\n")
 
         if index == 1 and not line.lstrip().lower().startswith("fileversion"):
             raise Exception(f"Unable to read this format from klarf")
 
-        for item in custom_columns_lot:
+        for item in custom_columns_wafer:
             if line.lstrip().lower().startswith(item.lower()):
                 attribute_values = line.rstrip(";").split()
-                custom_columns_lot_dict[item] = attribute_values[1]
+                custom_columns_wafer_dict[item] = attribute_values[1]
                 custom_columns_found = True
 
                 break
 
         if custom_columns_found:
             custom_columns_found = False
             continue
@@ -110,15 +111,23 @@
             continue
 
         if line.lstrip().lower().startswith("filetimestamp"):
             file_timestamp = line[14:33].rstrip(";")
             continue
 
         if line.lstrip().lower().startswith("inspectionstationid"):
-            inspection_station_id = line.split('"')[-2]
+            inspection_station_id = line.split(";")[0].split(" ")
+            inspection_station_id = [id.strip('"') for id in inspection_station_id]
+            inspection_station_id = inspection_station_id[1:4]
+
+            inspection_station_id = InspectionStationId(*inspection_station_id)
+            continue
+
+        if line.lstrip().lower().startswith("sampletype"):
+            sample_type = line.rstrip(";").split()[1]
             continue
 
         if line.lstrip().lower().startswith("resulttimestamp"):
             result_timestamp = line[16:35].rstrip(";")
             continue
 
         if line.lstrip().lower().startswith("lotid"):
@@ -141,14 +150,18 @@
             )
             continue
 
         if line.lstrip().lower().startswith("stepid"):
             step_id = line.split('"')[1]
             continue
 
+        if line.lstrip().lower().startswith("sampleorientationmarktype"):
+            sample_orientation_mark_type = line.rstrip(";").split()[1]
+            continue
+
         if line.lstrip().lower().startswith("orientationmarklocation"):
             orientation_mark_location = line.rstrip(";").split()[1]
             continue
 
         if line.lstrip().lower().startswith("diepitch"):
             die_pitch_value = line.rstrip(";").split()
             die_pitch = DiePitch(
@@ -176,26 +189,40 @@
             continue
 
         if line.lstrip().lower().startswith("slot"):
             slot_values = line.rstrip(";").split()
             slot = int(slot_values[1])
             continue
 
+        if line.lstrip().lower().startswith("inspectiontest"):
+            inspection_test = line.rstrip(";").split()
+            inspection_test = int(inspection_test[1])
+            continue
+
+        if line.lstrip().lower().startswith("areapertest"):
+            area_per_test = line.rstrip(";").split()
+            area_per_test = float(area_per_test[1])
+
+            tests.append(
+                Test(id=inspection_test, area=area_per_test),
+            )
+            continue
+
         if line.lstrip().lower().startswith("defectrecordspec"):
             line_without_space = re.sub("\s+", " ", line).strip()
             parameters = line_without_space.strip().split(" ")
 
             defect_columns = {
                 column: parameters.index(column) - 1
                 for column in RAW_DEFECT_COLUMNS
                 if column in parameters
             }
             defect_columns_custom = {
                 column: parameters.index(column) - 1
-                for column in custom_columns_defects
+                for column in custom_columns_defect
                 if column in parameters
             }
 
             continue
 
         if line.lstrip().lower().startswith("defectlist") and not (
             line.rstrip().endswith(";")
@@ -256,17 +283,21 @@
                 wafers.append(
                     Wafer(
                         id=wafer_id,
                         slot=slot,
                         die_origin=die_origin,
                         sample_center_location=sample_center_location,
                         defects=defects,
+                        tests=tests.copy(),
+                        custom_attribute=custom_columns_wafer_dict,
                     )
                 )
 
+                tests.clear()
+
         if line.lstrip().lower().startswith("summarylist") and not (
             line.rstrip().endswith(";")
         ):
             next_line_has_numb = True
             continue
 
         if next_line_has_numb and line.startswith(" "):
@@ -300,26 +331,27 @@
             continue
 
     return (
         KlarfContent(
             file_version=file_version,
             file_timestamp=file_timestamp,
             inspection_station_id=inspection_station_id,
+            sample_type=sample_type,
             result_timestamp=result_timestamp,
             lot_id=lot_id,
             device_id=device_id,
             sample_size=sample_size,
             step_id=step_id,
+            sample_orientation_mark_type=sample_orientation_mark_type,
             orientation_mark_location=orientation_mark_location,
             die_pitch=die_pitch,
             setup_id=setup_id,
             has_sample_test_plan=has_sample_test_plan,
             sample_plan_test=SamplePlanTest(x=sample_plan_test_x, y=sample_plan_test_y),
             wafers=wafers,
-            custom_attribute=custom_columns_lot_dict,
         ),
         raw_content,
     )
 
 
 def convert_coordinates(
     die_pitch: DiePitch,
```

### Comparing `klarf-reader-0.3.0/klarf_reader/utils/klarf_convert.py` & `klarf-reader-0.3.1/klarf_reader/utils/klarf_convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,21 @@
     if wafer_index > klarf_content.number_of_wafers - 1:
         raise ValueError(f"{wafer_index=} does not exist in {KlarfContent.__name__}")
 
     return SingleKlarfContent(
         file_version=klarf_content.file_version,
         file_timestamp=klarf_content.file_timestamp,
         inspection_station_id=klarf_content.inspection_station_id,
+        sample_type=klarf_content.sample_type,
         result_timestamp=klarf_content.result_timestamp,
         lot_id=klarf_content.lot_id,
         device_id=klarf_content.device_id,
         sample_size=klarf_content.sample_size,
         setup_id=klarf_content.setup_id,
         step_id=klarf_content.step_id,
+        sample_orientation_mark_type=klarf_content.sample_orientation_mark_type,
         orientation_mark_location=klarf_content.orientation_mark_location,
         die_pitch=klarf_content.die_pitch,
         has_sample_test_plan=klarf_content.has_sample_test_plan,
         sample_plan_test=klarf_content.sample_plan_test,
         wafer=klarf_content.wafers[wafer_index],
     )
```

### Comparing `klarf-reader-0.3.0/klarf_reader.egg-info/PKG-INFO` & `klarf-reader-0.3.1/klarf_reader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.0
+Version: 0.3.1
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.0.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.0/setup.py` & `klarf-reader-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.0"
+version = "0.3.1"
 
 setup(
     name="klarf-reader",
     version=version,
     packages=[
         "klarf_reader",
         "klarf_reader.models",
```

### Comparing `klarf-reader-0.3.0/tests/test_klarf.py` & `klarf-reader-0.3.1/tests/test_klarf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,16 @@
 # MODULES
 from dataclasses import asdict
-import inspect
 from pathlib import Path
-import dictdiffer
 
 # UNITTEST
 import unittest
 
 # KLARF_READER
 from klarf_reader.klarf import Klarf
-from klarf_reader.models.klarf_content import (
-    DieOrigin,
-    DiePitch,
-    KlarfContent,
-    SampleCenterLocation,
-    SamplePlanTest,
-    SetupId,
-    Summary,
-    Wafer,
-    SingleKlarfContent,
-)
-
-# UTILS
 from klarf_reader.utils import klarf_convert
 
 # TESTS
 from tests.utils import *
 
 
 ASSETS_PATH: Path = Path(__file__).parent / "assets"
@@ -33,111 +18,110 @@
 
 
 class TestKlarf(unittest.TestCase):
     def setUp(self) -> None:
         self.path_klarf_single_wafer = ASSETS_PATH / "J052SBN_8196_J052SBN-01.000"
         self.path_klarf_multi_wafers = ASSETS_PATH / "J237DTA_3236.000"
 
-    def test_klarf_single_wafer(self) -> None:
-        # Given
-        expected = load_json(
-            filename=ASSETS_SAVED_PATH
-            / f"{self.__class__.__name__}__{inspect.currentframe().f_code.co_name}.json"
-        )
+    def assertListOfDictEqual(self, first: list[dict], second: list[dict]):
+        self.assertEqual(len(first), len(second))
+        for index, item in enumerate(first):
+            if isinstance(item, dict):
+                self.assertNestedDictEqual(item, second[index])
+            else:
+                self.assertEqual(item, second[index])
+
+    def assertNestedDictEqual(self, first: dict, second: dict):
+        self.assertEqual(len(first), len(second))
+
+        first = {key: first[key] for key in sorted(first.keys())}
+        second = {key: second[key] for key in sorted(second.keys())}
+
+        for key, value in first.items():
+            second_value = second.get(key)
+            if isinstance(value, (list, tuple)):
+                self.assertListOfDictEqual(value, second_value)
+            elif isinstance(value, dict):
+                self.assertNestedDictEqual(value, second_value)
+            else:
+                self.assertEqual(value, second_value)
 
+    @load_expected_data(saved_path=ASSETS_SAVED_PATH)
+    def test_klarf_single_wafer(self, expected_data, saved_path) -> None:
         # When
         content = Klarf.load_from_file(filepath=self.path_klarf_single_wafer)
+        content_dict = asdict(content)
 
         save_as_json(
-            ASSETS_SAVED_PATH
-            / f"{self.__class__.__name__}__{inspect.currentframe().f_code.co_name}.json",
-            dict=asdict(content),
+            saved_path,
+            dict=content_dict,
         )
 
         # Then
-        self.assertEqual(asdict(content), expected)
+        self.assertNestedDictEqual(content_dict, expected_data)
 
-    def test_klarf_single_wafer_with_custom_attributes(self) -> None:
+    @load_expected_data(saved_path=ASSETS_SAVED_PATH)
+    def test_klarf_single_wafer_with_custom_attributes(
+        self, expected_data, saved_path
+    ) -> None:
         # Given
-        expected = load_json(
-            filename=ASSETS_SAVED_PATH
-            / f"{self.__class__.__name__}__{inspect.currentframe().f_code.co_name}.json"
-        )
-
         custom_columns_lot = ["TOTO"]
         custom_columns_defects = ["DEFECTAREA"]
 
         # When
         content = Klarf.load_from_file(
             filepath=self.path_klarf_single_wafer,
-            custom_columns_lot=custom_columns_lot,
-            custom_columns_defects=custom_columns_defects,
+            custom_columns_wafer=custom_columns_lot,
+            custom_columns_defect=custom_columns_defects,
         )
+        content_dict = asdict(content)
 
         save_as_json(
-            ASSETS_SAVED_PATH
-            / f"{self.__class__.__name__}__{inspect.currentframe().f_code.co_name}.json",
-            dict=asdict(content),
+            saved_path,
+            dict=content_dict,
         )
 
         # Then
-        self.assertEqual(asdict(content), expected)
+        self.assertNestedDictEqual(content_dict, expected_data)
 
     def test_klarf_single_wafer_with_raw_content(self) -> None:
         # Given
         expected_raw_content_length = 13356
 
         # When
-        content, raw_content = Klarf.load_from_file_with_raw_content(
+        _, raw_content = Klarf.load_from_file_with_raw_content(
             filepath=self.path_klarf_single_wafer
         )
 
         # Then
         self.assertEqual(len(raw_content), expected_raw_content_length)
 
-    def test_klarf_multi_wafers(self) -> None:
-        # Given
-        expected = load_json(
-            filename=ASSETS_SAVED_PATH
-            / f"{self.__class__.__name__}__{inspect.currentframe().f_code.co_name}.json"
-        )
-
+    @load_expected_data(saved_path=ASSETS_SAVED_PATH)
+    def test_klarf_multi_wafers(self, expected_data, saved_path) -> None:
         # When
         content = Klarf.load_from_file(filepath=self.path_klarf_multi_wafers)
         content_dict = asdict(content)
 
         save_as_json(
-            ASSETS_SAVED_PATH
-            / f"{self.__class__.__name__}__{inspect.currentframe().f_code.co_name}.json",
+            saved_path,
             dict=content_dict,
         )
 
         # Then
-        diff = get_diff(item_1=[content_dict], item_2=[expected])
-
-        self.assertEqual(content_dict, expected)
-
-    def test_convert_single_klarf_content(self) -> None:
-        # Given
-        expected = load_json(
-            filename=ASSETS_SAVED_PATH
-            / f"{self.__class__.__name__}__{inspect.currentframe().f_code.co_name}.json"
-        )
+        self.assertNestedDictEqual(content_dict, expected_data)
 
+    @load_expected_data(saved_path=ASSETS_SAVED_PATH)
+    def test_convert_single_klarf_content(self, expected_data, saved_path) -> None:
         # When
         content = Klarf.load_from_file(filepath=self.path_klarf_multi_wafers)
         single_klarf_content = klarf_convert.convert_to_single_klarf_content(
             klarf_content=content, wafer_index=0
         )
-
         single_klarf_content_dict = asdict(single_klarf_content)
 
         save_as_json(
-            ASSETS_SAVED_PATH
-            / f"{self.__class__.__name__}__{inspect.currentframe().f_code.co_name}.json",
+            saved_path,
             dict=single_klarf_content_dict,
         )
 
         # Then
-        diff = get_diff(item_1=[single_klarf_content_dict], item_2=[expected])
-
-        self.assertEqual(single_klarf_content_dict, expected)
+        self.assertNestedDictEqual(single_klarf_content_dict, expected_data)
```

