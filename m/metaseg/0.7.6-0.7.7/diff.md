# Comparing `tmp/metaseg-0.7.6.tar.gz` & `tmp/metaseg-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.7.6.tar", max compression
+gzip compressed data, was "metaseg-0.7.7.tar", max compression
```

## Comparing `metaseg-0.7.6.tar` & `metaseg-0.7.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-06-27 15:04:03.040725 metaseg-0.7.6/LICENSE
--rw-r--r--   0        0        0     4231 2023-06-27 15:04:03.040725 metaseg-0.7.6/README.md
--rw-r--r--   0        0        0      771 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/falai_demo.py
--rw-r--r--   0        0        0      438 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/generator/__init__.py
--rw-r--r--   0        0        0    15292 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0        0        0     3094 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/generator/build_sam.py
--rw-r--r--   0        0        0    11890 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/generator/predictor.py
--rw-r--r--   0        0        0     8395 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/mask_predictor.py
--rw-r--r--   0        0        0      749 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/__init__.py
--rw-r--r--   0        0        0     1479 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/common.py
--rw-r--r--   0        0        0    14851 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/image_encoder.py
--rw-r--r--   0        0        0     6800 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/mask_decoder.py
--rw-r--r--   0        0        0     8733 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0        0        0     7363 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/sam.py
--rw-r--r--   0        0        0     8436 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/transformer.py
--rw-r--r--   0        0        0     3548 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/sahi_predict.py
--rw-r--r--   0        0        0      924 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/__init__.py
--rw-r--r--   0        0        0    12711 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/amg.py
--rw-r--r--   0        0        0     2835 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/data_utils.py
--rw-r--r--   0        0        0     1295 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/file_utils.py
--rw-r--r--   0        0        0     5932 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/onnx.py
--rw-r--r--   0        0        0     4054 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/transforms.py
--rw-r--r--   0        0        0       44 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/webapp/__init__.py
--rw-r--r--   0        0        0     8595 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/webapp/app.py
--rw-r--r--   0        0        0     2541 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/webapp/demo.py
--rw-r--r--   0        0        0     3949 2023-06-27 15:04:03.048726 metaseg-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     6599 1970-01-01 00:00:00.000000 metaseg-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-27 15:33:14.661577 metaseg-0.7.7/LICENSE
+-rw-r--r--   0        0        0     4804 2023-06-27 15:33:14.661577 metaseg-0.7.7/README.md
+-rw-r--r--   0        0        0      771 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/falai_demo.py
+-rw-r--r--   0        0        0      438 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/generator/__init__.py
+-rw-r--r--   0        0        0    15292 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0        0        0     3094 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/generator/build_sam.py
+-rw-r--r--   0        0        0    11890 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/generator/predictor.py
+-rw-r--r--   0        0        0     8395 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/mask_predictor.py
+-rw-r--r--   0        0        0      749 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/__init__.py
+-rw-r--r--   0        0        0     1479 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/common.py
+-rw-r--r--   0        0        0    14851 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/image_encoder.py
+-rw-r--r--   0        0        0     6800 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0        0        0     8733 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0        0        0     7363 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/sam.py
+-rw-r--r--   0        0        0     8436 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/transformer.py
+-rw-r--r--   0        0        0     3548 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/sahi_predict.py
+-rw-r--r--   0        0        0      924 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/__init__.py
+-rw-r--r--   0        0        0    12711 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/amg.py
+-rw-r--r--   0        0        0     2835 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/data_utils.py
+-rw-r--r--   0        0        0     1295 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/file_utils.py
+-rw-r--r--   0        0        0     5932 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/onnx.py
+-rw-r--r--   0        0        0     4054 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/transforms.py
+-rw-r--r--   0        0        0       44 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/webapp/__init__.py
+-rw-r--r--   0        0        0     8595 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/webapp/app.py
+-rw-r--r--   0        0        0     2541 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/webapp/demo.py
+-rw-r--r--   0        0        0     4112 2023-06-27 15:33:14.665577 metaseg-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     7406 1970-01-01 00:00:00.000000 metaseg-0.7.7/PKG-INFO
```

### Comparing `metaseg-0.7.6/LICENSE` & `metaseg-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/README.md` & `metaseg-0.7.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,33 @@
 <h2>
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
     <a href="https://pepy.tech/project/metaseg"><img src="https://pepy.tech/badge/metaseg" alt="downloads"></a>
-    <a href="https://badge.fury.io/py/metaseg"><img src="https://badge.fury.io/py/metaseg.svg" alt="pypi version"></a>
     <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
-
 </div>
 
+
+<p align="center">
+<a href="https://pypi.org/project/metaseg" target="_blank">
+    <img src="https://img.shields.io/pypi/v/metaseg?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://pypi.org/project/metaseg" target="_blank">
+    <img src="https://img.shields.io/pypi/dm/metaseg?color=red" alt="Download Count">
+</a>
+<a href="https://pypi.org/project/metaseg" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/metaseg.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+<a href="https://pypi.org/project/metaseg" target="_blank">
+    <img src="https://img.shields.io/pypi/status/metaseg?color=orange" alt="Project Status">
+</a>
+</p>
+
 This repo is a packaged version of the [segment-anything](https://github.com/facebookresearch/segment-anything) model.
 
 ### Installation
 ```bash
 pip install metaseg
 ```
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
-                [downloads] [pypi_version] [HuggingFace_Spaces]
+                       [downloads] [HuggingFace_Spaces]
+[Package_version] [Download_Count] [Supported_Python_versions] [Project_Status]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image results =
 SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0,
```

### Comparing `metaseg-0.7.6/metaseg/__init__.py` & `metaseg-0.7.7/metaseg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from .falai_demo import falai_manuelmask_image as falai_manuelmask_image
 from .falai_demo import manuelmask_image as manuelmask_image
 from .mask_predictor import SegAutoMaskPredictor as SegAutoMaskPredictor
 from .mask_predictor import SegManualMaskPredictor as SegManualMaskPredictor
 from .sahi_predict import SahiAutoSegmentation as SahiAutoSegmentation
 from .sahi_predict import sahi_sliced_predict as sahi_sliced_predict
 
-__version__ = "0.7.6"
+__version__ = "0.7.7"
```

### Comparing `metaseg-0.7.6/metaseg/falai_demo.py` & `metaseg-0.7.7/metaseg/falai_demo.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.7.7/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/generator/build_sam.py` & `metaseg-0.7.7/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/generator/predictor.py` & `metaseg-0.7.7/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/mask_predictor.py` & `metaseg-0.7.7/metaseg/mask_predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/modeling/__init__.py` & `metaseg-0.7.7/metaseg/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/modeling/common.py` & `metaseg-0.7.7/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/modeling/image_encoder.py` & `metaseg-0.7.7/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/modeling/mask_decoder.py` & `metaseg-0.7.7/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/modeling/prompt_encoder.py` & `metaseg-0.7.7/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/modeling/sam.py` & `metaseg-0.7.7/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/modeling/transformer.py` & `metaseg-0.7.7/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/sahi_predict.py` & `metaseg-0.7.7/metaseg/sahi_predict.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/utils/__init__.py` & `metaseg-0.7.7/metaseg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/utils/amg.py` & `metaseg-0.7.7/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/utils/data_utils.py` & `metaseg-0.7.7/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/utils/file_utils.py` & `metaseg-0.7.7/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/utils/onnx.py` & `metaseg-0.7.7/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/utils/transforms.py` & `metaseg-0.7.7/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/webapp/app.py` & `metaseg-0.7.7/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/metaseg/webapp/demo.py` & `metaseg-0.7.7/metaseg/webapp/demo.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.6/pyproject.toml` & `metaseg-0.7.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metaseg"
-version = "0.7.6"
+version = "0.7.7"
 description = "MetaSeg: Packaged version of the Segment Anything repository"
 authors = ["Kadir Nar <kadir.nar@hotmail.com>"]
 maintainers = ["Kadir Nar <kadir.nar@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "metaseg"}]
 homepage = "https://github.com/kadirnar/segment-anything-video"
 repository = "https://github.com/kadirnar/segment-anything-video"
@@ -45,21 +45,24 @@
 opencv-python = "^4.7.0.72"
 tqdm = "^4.65.0"
 matplotlib = "^3.7.1"
 pillow = "^9.5.0"
 pycocotools = "^2.0.6"
 fal-serverless = "^0.6.35"
 sahi = "^0.11.14"
+onnx = { version = "^1.14.0", optional = true }
+onnxruntime =  { version ="^1.15.1", optional = true }
+ultralytics = { version = "^8.0.123", optional = true }
+yolov5 = { version ="^7.0.12", optional = true }
 
 
 [tool.poetry.extras]
 full = ["onnxruntime","onnx","yolov5","ultralytics"]
 yolov5 = ["yolov5"]
 yolov8 = ["ultralytics"]
-sahi-full = ["sahi", "yolov5","ultralytics"]
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.0.1"
 bandit = "^1.7.4"
 debugpy = "^1.6.6"
```

### Comparing `metaseg-0.7.6/PKG-INFO` & `metaseg-0.7.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.7.6
+Version: 0.7.7
 Summary: MetaSeg: Packaged version of the Segment Anything repository
 Home-page: https://github.com/kadirnar/segment-anything-video
 License: Apache-2.0
 Keywords: pytorch,segment-anything-video,metaseg
 Author: Kadir Nar
 Author-email: kadir.nar@hotmail.com
 Maintainer: Kadir Nar
@@ -30,43 +30,60 @@
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: full
-Provides-Extra: sahi-full
 Provides-Extra: yolov5
 Provides-Extra: yolov8
 Requires-Dist: fal-serverless (>=0.6.35,<0.7.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: onnx (>=1.14.0,<2.0.0) ; extra == "full"
+Requires-Dist: onnxruntime (>=1.15.1,<2.0.0) ; extra == "full"
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pycocotools (>=2.0.6,<3.0.0)
-Requires-Dist: sahi (>=0.11.14,<0.12.0) ; extra == "sahi-full"
+Requires-Dist: sahi (>=0.11.14,<0.12.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: torchvision (>=0.15.2,<0.16.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: ultralytics (>=8.0.123,<9.0.0) ; extra == "full" or extra == "yolov8"
+Requires-Dist: yolov5 (>=7.0.12,<8.0.0) ; extra == "full" or extra == "yolov5"
 Project-URL: Documentation, https://github.com/kadirnar/segment-anything-video/blob/main/README.md
 Project-URL: Repository, https://github.com/kadirnar/segment-anything-video
 Description-Content-Type: text/markdown
 
 <div align="center">
 <h2>
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
     <a href="https://pepy.tech/project/metaseg"><img src="https://pepy.tech/badge/metaseg" alt="downloads"></a>
-    <a href="https://badge.fury.io/py/metaseg"><img src="https://badge.fury.io/py/metaseg.svg" alt="pypi version"></a>
     <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
-
 </div>
 
+
+<p align="center">
+<a href="https://pypi.org/project/metaseg" target="_blank">
+    <img src="https://img.shields.io/pypi/v/metaseg?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://pypi.org/project/metaseg" target="_blank">
+    <img src="https://img.shields.io/pypi/dm/metaseg?color=red" alt="Download Count">
+</a>
+<a href="https://pypi.org/project/metaseg" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/metaseg.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+<a href="https://pypi.org/project/metaseg" target="_blank">
+    <img src="https://img.shields.io/pypi/status/metaseg?color=orange" alt="Project Status">
+</a>
+</p>
+
 This repo is a packaged version of the [segment-anything](https://github.com/facebookresearch/segment-anything) model.
 
 ### Installation
 ```bash
 pip install metaseg
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.7.6 Summary: MetaSeg: Packaged
+Metadata-Version: 2.1 Name: metaseg Version: 0.7.7 Summary: MetaSeg: Packaged
 version of the Segment Anything repository Home-page: https://github.com/
 kadirnar/segment-anything-video License: Apache-2.0 Keywords: pytorch,segment-
 anything-video,metaseg Author: Kadir Nar Author-email: kadir.nar@hotmail.com
 Maintainer: Kadir Nar Maintainer-email: kadir.nar@hotmail.com Requires-Python:
 >=3.8.1,<3.12.0 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
@@ -15,28 +15,32 @@
 Python :: 3.8 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Image Processing Classifier: Topic :: Scientific/
 Engineering :: Image Recognition Classifier: Topic :: Scientific/Engineering ::
 Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Provides-Extra: full Provides-Extra: sahi-full
-Provides-Extra: yolov5 Provides-Extra: yolov8 Requires-Dist: fal-serverless
-(>=0.6.35,<0.7.0) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist:
-opencv-python (>=4.7.0.72,<5.0.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0)
-Requires-Dist: pycocotools (>=2.0.6,<3.0.0) Requires-Dist: sahi
-(>=0.11.14,<0.12.0) ; extra == "sahi-full" Requires-Dist: torch
-(>=2.0.1,<3.0.0) Requires-Dist: torchvision (>=0.15.2,<0.16.0) Requires-Dist:
-tqdm (>=4.65.0,<5.0.0) Project-URL: Documentation, https://github.com/kadirnar/
-segment-anything-video/blob/main/README.md Project-URL: Repository, https://
-github.com/kadirnar/segment-anything-video Description-Content-Type: text/
-markdown
+:: Libraries :: Python Modules Provides-Extra: full Provides-Extra: yolov5
+Provides-Extra: yolov8 Requires-Dist: fal-serverless (>=0.6.35,<0.7.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: onnx
+(>=1.14.0,<2.0.0) ; extra == "full" Requires-Dist: onnxruntime
+(>=1.15.1,<2.0.0) ; extra == "full" Requires-Dist: opencv-python
+(>=4.7.0.72,<5.0.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist:
+pycocotools (>=2.0.6,<3.0.0) Requires-Dist: sahi (>=0.11.14,<0.12.0) Requires-
+Dist: torch (>=2.0.1,<3.0.0) Requires-Dist: torchvision (>=0.15.2,<0.16.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0) Requires-Dist: ultralytics
+(>=8.0.123,<9.0.0) ; extra == "full" or extra == "yolov8" Requires-Dist: yolov5
+(>=7.0.12,<8.0.0) ; extra == "full" or extra == "yolov5" Project-URL:
+Documentation, https://github.com/kadirnar/segment-anything-video/blob/main/
+README.md Project-URL: Repository, https://github.com/kadirnar/segment-
+anything-video Description-Content-Type: text/markdown
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
-                [downloads] [pypi_version] [HuggingFace_Spaces]
+                       [downloads] [HuggingFace_Spaces]
+[Package_version] [Download_Count] [Supported_Python_versions] [Project_Status]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image results =
 SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0,
```

