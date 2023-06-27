# Comparing `tmp/velour-client-0.5.0.tar.gz` & `tmp/velour-client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velour-client-0.5.0.tar", last modified: Mon Jun 26 11:29:17 2023, max compression
+gzip compressed data, was "velour-client-0.6.0.tar", last modified: Tue Jun 27 17:50:28 2023, max compression
```

## Comparing `velour-client-0.5.0.tar` & `velour-client-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:29:17.770211 velour-client-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 11:29:08.000000 velour-client-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-26 11:29:17.770211 velour-client-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 11:29:08.000000 velour-client-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 11:29:08.000000 velour-client-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 11:29:17.770211 velour-client-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-26 11:29:08.000000 velour-client-0.5.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:29:17.770211 velour-client-0.5.0/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_yolo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:29:17.770211 velour-client-0.5.0/velour/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:29:17.770211 velour-client-0.5.0/velour/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/integrations/chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/integrations/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/integrations/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:29:17.770211 velour-client-0.5.0/velour_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-26 11:29:17.000000 velour-client-0.5.0/velour_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-26 11:29:17.000000 velour-client-0.5.0/velour_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:29:17.000000 velour-client-0.5.0/velour_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 11:29:17.000000 velour-client-0.5.0/velour_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 11:29:17.000000 velour-client-0.5.0/velour_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:50:28.913708 velour-client-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-27 17:50:19.000000 velour-client-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-27 17:50:28.913708 velour-client-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 17:50:19.000000 velour-client-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-27 17:50:19.000000 velour-client-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:50:28.913708 velour-client-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-27 17:50:19.000000 velour-client-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:50:28.909708 velour-client-0.6.0/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-27 17:50:19.000000 velour-client-0.6.0/unit-tests/test_chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-27 17:50:19.000000 velour-client-0.6.0/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-27 17:50:19.000000 velour-client-0.6.0/unit-tests/test_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-27 17:50:19.000000 velour-client-0.6.0/unit-tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-27 17:50:19.000000 velour-client-0.6.0/unit-tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-27 17:50:19.000000 velour-client-0.6.0/unit-tests/test_yolo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:50:28.909708 velour-client-0.6.0/velour/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-27 17:50:19.000000 velour-client-0.6.0/velour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31576 2023-06-27 17:50:19.000000 velour-client-0.6.0/velour/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-27 17:50:19.000000 velour-client-0.6.0/velour/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:50:28.913708 velour-client-0.6.0/velour/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-06-27 17:50:19.000000 velour-client-0.6.0/velour/integrations/chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-27 17:50:19.000000 velour-client-0.6.0/velour/integrations/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-27 17:50:19.000000 velour-client-0.6.0/velour/integrations/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 17:50:19.000000 velour-client-0.6.0/velour/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-27 17:50:19.000000 velour-client-0.6.0/velour/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:50:28.913708 velour-client-0.6.0/velour_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-27 17:50:28.000000 velour-client-0.6.0/velour_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-27 17:50:28.000000 velour-client-0.6.0/velour_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:50:28.000000 velour-client-0.6.0/velour_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 17:50:28.000000 velour-client-0.6.0/velour_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 17:50:28.000000 velour-client-0.6.0/velour_client.egg-info/top_level.txt
```

### Comparing `velour-client-0.5.0/LICENSE` & `velour-client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/PKG-INFO` & `velour-client-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `velour-client-0.5.0/pyproject.toml` & `velour-client-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/unit-tests/test_chariot.py` & `velour-client-0.6.0/unit-tests/test_chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/unit-tests/test_client.py` & `velour-client-0.6.0/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/unit-tests/test_coco.py` & `velour-client-0.6.0/unit-tests/test_coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/unit-tests/test_data_types.py` & `velour-client-0.6.0/unit-tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/unit-tests/test_viz.py` & `velour-client-0.6.0/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/unit-tests/test_yolo.py` & `velour-client-0.6.0/unit-tests/test_yolo.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/velour/client.py` & `velour-client-0.6.0/velour/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     BoundingBox,
     BoundingPolygon,
     GroundTruthDetection,
     GroundTruthImageClassification,
     GroundTruthInstanceSegmentation,
     GroundTruthSemanticSegmentation,
     Image,
+    Info,
     Label,
     Metadatum,
     Point,
     PolygonWithHole,
     PredictedDetection,
     PredictedImageClassification,
     ScoredLabel,
@@ -109,27 +110,62 @@
 
 
 class ClientException(Exception):
     pass
 
 
 class DatasetBase:
-    def __init__(self, client: "Client", name: str):
+    def __init__(
+        self,
+        client: "Client",
+        name: str,
+        href: Optional[str] = None,
+        description: Optional[str] = None,
+    ):
         self.client = client
         self.name = name
+        self.href = href
+        self.description = description
 
     def get_labels(self) -> List[Label]:
         labels = self.client._requests_get_rel_host(
             f"datasets/{self.name}/labels"
         ).json()
 
         return [
             Label(key=label["key"], value=label["value"]) for label in labels
         ]
 
+    def get_label_distribution(self) -> Dict[Label, int]:
+        distribution = self.client._requests_get_rel_host(
+            f"datasets/{self.name}/labels/distribution"
+        ).json()
+
+        return {
+            Label(
+                key=label["label"]["key"], value=label["label"]["value"]
+            ): label["count"]
+            for label in distribution
+        }
+
+    def get_info(self) -> Info:
+        resp = self.client._requests_get_rel_host(
+            f"datasets/{self.name}/info"
+        ).json()
+
+        return Info(
+            annotation_type=resp["annotation_type"],
+            number_of_classifications=resp["number_of_classifications"],
+            number_of_bounding_boxes=resp["number_of_bounding_boxes"],
+            number_of_bounding_polygons=resp["number_of_bounding_polygons"],
+            number_of_segmentations=resp["number_of_segmentation_rasters"],
+            associated_datasets=None,
+            associated_models=resp["associated"],
+        )
+
     def finalize(self):
         return self.client._requests_put_rel_host(
             f"datasets/{self.name}/finalize"
         )
 
     def delete(self):
         return self.client.delete_dataset(self.name)
@@ -375,17 +411,25 @@
 
 
 def _remove_none_from_dict(d: dict) -> dict:
     return {k: v for k, v in d.items() if v is not None}
 
 
 class ModelBase:
-    def __init__(self, client: "Client", name: str):
+    def __init__(
+        self,
+        client: "Client",
+        name: str,
+        href: Optional[str] = None,
+        description: Optional[str] = None,
+    ):
         self.client = client
         self.name = name
+        self.href = href
+        self.description = description
 
     def finalize_inferences(self, dataset: DatasetBase) -> None:
         return self.client._requests_put_rel_host(
             f"models/{self.name}/inferences/{dataset.name}/finalize"
         ).json()
 
     def evaluate_classification(
@@ -504,14 +548,51 @@
             df = df.pivot(
                 index=["type", "parameters", "label"], columns=["dataset"]
             )
             ret.append({"settings": grp["settings"], "df": df})
 
         return ret
 
+    def get_labels(self) -> List[Label]:
+        labels = self.client._requests_get_rel_host(
+            f"models/{self.name}/labels"
+        ).json()
+
+        return [
+            Label(key=label["key"], value=label["value"]) for label in labels
+        ]
+
+    def get_label_distribution(self) -> Dict[Label, int]:
+        distribution = self.client._requests_get_rel_host(
+            f"models/{self.name}/labels/distribution"
+        ).json()
+
+        return {
+            Label(key=label["label"]["key"], value=label["label"]["value"]): {
+                "count": label["count"],
+                "scores": label["scores"],
+            }
+            for label in distribution
+        }
+
+    def get_info(self) -> Info:
+        resp = self.client._requests_get_rel_host(
+            f"models/{self.name}/info"
+        ).json()
+
+        return Info(
+            annotation_type=resp["annotation_type"],
+            number_of_classifications=resp["number_of_classifications"],
+            number_of_bounding_boxes=resp["number_of_bounding_boxes"],
+            number_of_bounding_polygons=resp["number_of_bounding_polygons"],
+            number_of_segmentations=resp["number_of_segmentation_rasters"],
+            associated_datasets=resp["associated"],
+            associated_models=None,
+        )
+
 
 class ImageModel(ModelBase):
     def add_predictions(
         self,
         dataset: ImageDataset,
         predictions: list,
         chunk_size: int = 1000,
@@ -792,15 +873,17 @@
                 "name": name,
                 "href": href,
                 "description": description,
                 "type": datum_type.value,
             },
         )
 
-        return class_(client=self, name=name)
+        return class_(
+            client=self, name=name, href=href, description=description
+        )
 
     def create_image_dataset(
         self, name: str, href: str = None, description: str = None
     ) -> ImageDataset:
         return self._create_model_or_dataset(
             entity_type="datasets",
             datum_type=DatumTypes.IMAGE,
@@ -834,15 +917,20 @@
             raise ValueError(f"Expected `entity_type` to be in {entity_types}")
 
         resp = self._requests_get_rel_host(f"{entity_type}/{name}").json()
 
         datum_type = DatumTypes.invert(resp["type"])
         class_ = self.datum_type_and_entity_to_class[entity_type][datum_type]
 
-        return class_(client=self, name=resp["name"])
+        return class_(
+            client=self,
+            name=resp["name"],
+            href=resp["href"],
+            description=resp["description"],
+        )
 
     def get_model(self, name: str) -> ModelBase:
         return self._get_model_or_dataset(entity_type="models", name=name)
 
     def get_dataset(self, name: str) -> DatasetBase:
         return self._get_model_or_dataset(entity_type="datasets", name=name)
```

### Comparing `velour-client-0.5.0/velour/data_types.py` & `velour-client-0.6.0/velour/data_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,20 +35,44 @@
 class Label:
     key: str
     value: str
 
     def tuple(self) -> Tuple[str, str]:
         return (self.key, self.value)
 
+    def __eq__(self, other):
+        if hasattr(other, "key") and hasattr(other, "value"):
+            return self.key == other.key and self.value == other.value
+        return False
+
+    def __hash__(self) -> int:
+        return hash(f"key:{self.key},value:{self.value}")
+
 
 @dataclass
 class ScoredLabel:
     label: Label
     score: float
 
+    @property
+    def key(self):
+        return self.label.key
+
+    @property
+    def value(self):
+        return self.label.value
+
+    def __eq__(self, other):
+        if hasattr(other, "label") and hasattr(other, "score"):
+            return self.score == other.score and self.label == other.label
+        return False
+
+    def __hash__(self) -> int:
+        return hash(f"key:{self.key},value:{self.value},score:{self.score}")
+
 
 @dataclass
 class Point:
     x: float
     y: float
 
     def resize(
@@ -232,7 +256,18 @@
 
         for k, total_score in label_keys_to_sum.items():
             if abs(total_score - 1) > 1e-5:
                 raise ValueError(
                     "For each label key, prediction scores must sum to 1, but"
                     f" for label key {k} got scores summing to {total_score}."
                 )
+
+
+@dataclass
+class Info:
+    annotation_type: List[str]
+    number_of_classifications: int
+    number_of_bounding_boxes: int
+    number_of_bounding_polygons: int
+    number_of_segmentations: int
+    associated_datasets: List[str]
+    associated_models: List[str]
```

### Comparing `velour-client-0.5.0/velour/integrations/chariot.py` & `velour-client-0.6.0/velour/integrations/chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/velour/integrations/coco.py` & `velour-client-0.6.0/velour/integrations/coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/velour/integrations/yolo.py` & `velour-client-0.6.0/velour/integrations/yolo.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/velour/viz.py` & `velour-client-0.6.0/velour/viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.5.0/velour_client.egg-info/PKG-INFO` & `velour-client-0.6.0/velour_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `velour-client-0.5.0/velour_client.egg-info/SOURCES.txt` & `velour-client-0.6.0/velour_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

