# Comparing `tmp/metaseg-0.7.5.tar.gz` & `tmp/metaseg-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.7.5.tar", last modified: Sat May  6 11:09:44 2023, max compression
+gzip compressed data, was "metaseg-0.7.6.tar", max compression
```

## Comparing `metaseg-0.7.5.tar` & `metaseg-0.7.6.tar`

### file list

```diff
@@ -1,44 +1,28 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.526430 metaseg-0.7.5/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-05-06 11:05:04.000000 metaseg-0.7.5/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-05-06 11:05:04.000000 metaseg-0.7.5/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4491 2023-05-06 11:09:44.526430 metaseg-0.7.5/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4217 2023-05-06 11:06:51.000000 metaseg-0.7.5/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.523097 metaseg-0.7.5/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-05-06 11:09:28.000000 metaseg-0.7.5/metaseg/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2848 2023-05-06 11:09:38.000000 metaseg-0.7.5/metaseg/falai_demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.523097 metaseg-0.7.5/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8161 2023-05-06 11:09:38.000000 metaseg-0.7.5/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.526430 metaseg-0.7.5/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.526430 metaseg-0.7.5/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2807 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.526430 metaseg-0.7.5/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8416 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/webapp/app.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2470 2023-05-06 11:05:04.000000 metaseg-0.7.5/metaseg/webapp/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-05-06 11:09:44.523097 metaseg-0.7.5/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4491 2023-05-06 11:09:44.000000 metaseg-0.7.5/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      903 2023-05-06 11:09:44.000000 metaseg-0.7.5/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-05-06 11:09:44.000000 metaseg-0.7.5/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      183 2023-05-06 11:09:44.000000 metaseg-0.7.5/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-05-06 11:09:44.000000 metaseg-0.7.5/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-05-06 11:05:04.000000 metaseg-0.7.5/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      158 2023-05-06 11:09:17.000000 metaseg-0.7.5/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-05-06 11:09:44.529764 metaseg-0.7.5/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-05-06 11:05:04.000000 metaseg-0.7.5/setup.py
+-rw-r--r--   0        0        0    11357 2023-06-27 15:04:03.040725 metaseg-0.7.6/LICENSE
+-rw-r--r--   0        0        0     4231 2023-06-27 15:04:03.040725 metaseg-0.7.6/README.md
+-rw-r--r--   0        0        0      771 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/falai_demo.py
+-rw-r--r--   0        0        0      438 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/generator/__init__.py
+-rw-r--r--   0        0        0    15292 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0        0        0     3094 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/generator/build_sam.py
+-rw-r--r--   0        0        0    11890 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/generator/predictor.py
+-rw-r--r--   0        0        0     8395 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/mask_predictor.py
+-rw-r--r--   0        0        0      749 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/__init__.py
+-rw-r--r--   0        0        0     1479 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/common.py
+-rw-r--r--   0        0        0    14851 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/image_encoder.py
+-rw-r--r--   0        0        0     6800 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0        0        0     8733 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0        0        0     7363 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/sam.py
+-rw-r--r--   0        0        0     8436 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/modeling/transformer.py
+-rw-r--r--   0        0        0     3548 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/sahi_predict.py
+-rw-r--r--   0        0        0      924 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/__init__.py
+-rw-r--r--   0        0        0    12711 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/amg.py
+-rw-r--r--   0        0        0     2835 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/data_utils.py
+-rw-r--r--   0        0        0     1295 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/file_utils.py
+-rw-r--r--   0        0        0     5932 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/onnx.py
+-rw-r--r--   0        0        0     4054 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/utils/transforms.py
+-rw-r--r--   0        0        0       44 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/webapp/__init__.py
+-rw-r--r--   0        0        0     8595 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/webapp/app.py
+-rw-r--r--   0        0        0     2541 2023-06-27 15:04:03.044726 metaseg-0.7.6/metaseg/webapp/demo.py
+-rw-r--r--   0        0        0     3949 2023-06-27 15:04:03.048726 metaseg-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     6599 1970-01-01 00:00:00.000000 metaseg-0.7.6/PKG-INFO
```

### Comparing `metaseg-0.7.5/LICENSE` & `metaseg-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.5/PKG-INFO` & `metaseg-0.7.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: metaseg
-Version: 0.7.5
-Home-page: https://github.com/kadirnar/segment-anything-pip
-Author: kadirnar
-License: Apache-2.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
 <h2>
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
@@ -36,27 +24,27 @@
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 results = SegAutoMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
-    points_per_side=16, 
+    points_per_side=16,
     points_per_batch=64,
     min_area=0,
     output_path="output.jpg",
     show=True,
     save=False,
 )
 
 # For video
 results = SegAutoMaskPredictor().video_predict(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
-    points_per_side=16, 
+    points_per_side=16,
     points_per_batch=64,
     min_area=1000,
     output_path="output.mp4",
 )
 
 # For manuel box and point selection
 
@@ -72,31 +60,35 @@
     show=True,
     save=False,
 )
 
 # For video
 
 results = SegManualMaskPredictor().video_predict(
-    source="test.mp4",
+    source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
-    input_point=[0, 0, 100, 100]
+    input_point=[0, 0, 100, 100],
     input_label=[0, 1],
     input_box=None,
     multimask_output=False,
     random_color=False,
     output_path="output.mp4",
 )
 ```
 
 ### [SAHI](https://github.com/obss/sahi) + Segment Anything
 
+```bash
+pip install sahi metaseg
+```
+
 ```python
 from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
-image_path = "test.jpg"
+image_path = "image.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
     detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
     detection_model_path="yolov5l6.pt",
     conf_th=0.25,
     image_size=1280,
     slice_height=256,
@@ -115,41 +107,41 @@
     save=False,
 )
 ```
 <img width="700" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.5.0/sahi_autoseg.png">
 
 ### [FalAI(Cloud GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything
 ```bash
-pip install fal_serverless
+pip install metaseg fal_serverless
 fal-serverless auth login
 ```
 
 ```python
 # For Auto Mask
 from metaseg import falai_automask_image
 
 image = falai_automask_image(
-    image_path="data.jpg",
+    image_path="image.jpg",
     model_type="vit_b",
     points_per_side=16,
     points_per_batch=32,
     min_area=0,
-)   
+)
 image.show() # Show image
 image.save("output.jpg") # Save image
 
 # For Manual Mask
-from metaseg.falai_demo import falai_automask_image, falai_manuelmask_image
+from metaseg import falai_manuelmask_image
 
 image = falai_manualmask_image(
-    image_path="data.jpg",
+    image_path="image.jpg",
     model_type="vit_b",
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
-    input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
+    input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]],
     multimask_output=False,
     random_color=False,
 )
 image.show() # Show image
 image.save("output.jpg") # Save image
 ```
 # Extra Features
```

#### html2text {}

```diff
@@ -1,11 +1,7 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.7.5 Home-page: https://
-github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
@@ -17,34 +13,34 @@
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=1000,
 output_path="output.mp4", ) # For manuel box and point selection # For image
 results = SegManualMaskPredictor().image_predict( source="image.jpg",
 model_type="vit_l", # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]],
 input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200],
 [100, 100, 200, 200]] multimask_output=False, random_color=False, show=True,
 save=False, ) # For video results = SegManualMaskPredictor().video_predict
-( source="test.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
-0, 100, 100] input_label=[0, 1], input_box=None, multimask_output=False,
+( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
+0, 100, 100], input_label=[0, 1], input_box=None, multimask_output=False,
 random_color=False, output_path="output.mp4", ) ``` ### [SAHI](https://
-github.com/obss/sahi) + Segment Anything ```python from metaseg.sahi_predict
-import SahiAutoSegmentation, sahi_sliced_predict image_path = "test.jpg" boxes
-= sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
-#yolov8, detectron2, mmdetection, torchvision
-detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
-slice_height=256, slice_width=256, overlap_height_ratio=0.2,
+github.com/obss/sahi) + Segment Anything ```bash pip install sahi metaseg ```
+```python from metaseg.sahi_predict import SahiAutoSegmentation,
+sahi_sliced_predict image_path = "image.jpg" boxes = sahi_sliced_predict
+( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
+mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
+image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
 overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
 model_type="vit_b", input_box=boxes, multimask_output=False,
 random_color=False, show=True, save=False, ) ``` [teaser] ### [FalAI(Cloud
 GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything ```bash
-pip install fal_serverless fal-serverless auth login ``` ```python # For Auto
-Mask from metaseg import falai_automask_image image = falai_automask_image
-( image_path="data.jpg", model_type="vit_b", points_per_side=16,
-points_per_batch=32, min_area=0, ) image.show() # Show image image.save
-("output.jpg") # Save image # For Manual Mask from metaseg.falai_demo import
-falai_automask_image, falai_manuelmask_image image = falai_manualmask_image
-( image_path="data.jpg", model_type="vit_b", input_point=[[100, 100], [200,
+pip install metaseg fal_serverless fal-serverless auth login ``` ```python #
+For Auto Mask from metaseg import falai_automask_image image =
+falai_automask_image( image_path="image.jpg", model_type="vit_b",
+points_per_side=16, points_per_batch=32, min_area=0, ) image.show() # Show
+image image.save("output.jpg") # Save image # For Manual Mask from metaseg
+import falai_manuelmask_image image = falai_manualmask_image
+( image_path="image.jpg", model_type="vit_b", input_point=[[100, 100], [200,
 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100,
-200, 200], [100, 100, 200, 200]] multimask_output=False, random_color=False, )
+200, 200], [100, 100, 200, 200]], multimask_output=False, random_color=False, )
 image.show() # Show image image.save("output.jpg") # Save image ``` # Extra
 Features - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision
 models - [x] Support for video and web application(Huggingface Spaces) - [x]
 Support for manual single multi box and point selection - [x] Support for pip
 installation - [x] Support for SAHI library - [x] Support for FalAI
```

### Comparing `metaseg-0.7.5/metaseg/falai_demo.py` & `metaseg-0.7.6/metaseg/falai_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 from metaseg.utils.data_utils import load_server_image
 
 try:
     from fal_serverless import isolated
 except ImportError:
-    raise ImportError("Please install FalAI library using 'pip install fal_serverless'.")
+    raise ImportError(
+        "Please install FalAI library using 'pip install fal_serverless'."
+    )
 
 
 @isolated(requirements=["metaseg"], keep_alive=1800, machine_type="GPU-T4")
-def automask_image(data, model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0):
+def automask_image(
+    data, model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0
+):
     image_path, output_path = load_server_image(data)
     SegAutoMaskPredictor().image_predict(
         source=image_path,
         model_type=model_type,
         points_per_side=points_per_side,
         points_per_batch=points_per_batch,
         min_area=min_area,
@@ -57,15 +61,17 @@
     )
     with open(output_path, "rb") as f:
         result = f.read()
 
     return result
 
 
-def falai_automask_image(image_path, model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0):
+def falai_automask_image(
+    image_path, model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0
+):
     with open(image_path, "rb") as f:
         data = f.read()
 
     image = automask_image(
         data=data,
         model_type=model_type,
         points_per_side=points_per_side,
```

### Comparing `metaseg-0.7.5/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.7.6/metaseg/generator/automatic_mask_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,15 +168,17 @@
                 mask_data,
                 self.min_mask_region_area,
                 max(self.box_nms_thresh, self.crop_nms_thresh),
             )
 
         # Encode masks
         if self.output_mode == "coco_rle":
-            mask_data["segmentations"] = [coco_encode_rle(rle) for rle in mask_data["rles"]]
+            mask_data["segmentations"] = [
+                coco_encode_rle(rle) for rle in mask_data["rles"]
+            ]
         elif self.output_mode == "binary_mask":
             mask_data["segmentations"] = [rle_to_mask(rle) for rle in mask_data["rles"]]
         else:
             mask_data["segmentations"] = mask_data["rles"]
 
         # Write mask records
         curr_anns = []
@@ -192,15 +194,17 @@
             }
             curr_anns.append(ann)
 
         return curr_anns
 
     def _generate_masks(self, image: np.ndarray) -> MaskData:
         orig_size = image.shape[:2]
-        crop_boxes, layer_idxs = generate_crop_boxes(orig_size, self.crop_n_layers, self.crop_overlap_ratio)
+        crop_boxes, layer_idxs = generate_crop_boxes(
+            orig_size, self.crop_n_layers, self.crop_overlap_ratio
+        )
 
         # Iterate over image crops
         data = MaskData()
         for crop_box, layer_idx in zip(crop_boxes, layer_idxs):
             crop_data = self._process_crop(image, crop_box, layer_idx, orig_size)
             data.cat(crop_data)
 
@@ -236,15 +240,17 @@
         # Get points for this crop
         points_scale = np.array(cropped_im_size)[None, ::-1]
         points_for_image = self.point_grids[crop_layer_idx] * points_scale
 
         # Generate masks for this crop in batches
         data = MaskData()
         for (points,) in batch_iterator(self.points_per_batch, points_for_image):
-            batch_data = self._process_batch(points, cropped_im_size, crop_box, orig_size)
+            batch_data = self._process_batch(
+                points, cropped_im_size, crop_box, orig_size
+            )
             data.cat(batch_data)
             del batch_data
         self.predictor.reset_image()
 
         # Remove duplicates within this crop.
         keep_by_nms = batched_nms(
             data["boxes"].float(),
@@ -269,15 +275,17 @@
         orig_size: Tuple[int, ...],
     ) -> MaskData:
         orig_h, orig_w = orig_size
 
         # Run model on this batch
         transformed_points = self.predictor.transform.apply_coords(points, im_size)
         in_points = torch.as_tensor(transformed_points, device=self.predictor.device)
-        in_labels = torch.ones(in_points.shape[0], dtype=torch.int, device=in_points.device)
+        in_labels = torch.ones(
+            in_points.shape[0], dtype=torch.int, device=in_points.device
+        )
         masks, iou_preds, _ = self.predictor.predict_torch(
             in_points[:, None, :],
             in_labels[:, None],
             multimask_output=True,
             return_logits=True,
         )
 
@@ -292,38 +300,44 @@
         # Filter by predicted IoU
         if self.pred_iou_thresh > 0.0:
             keep_mask = data["iou_preds"] > self.pred_iou_thresh
             data.filter(keep_mask)
 
         # Calculate stability score
         data["stability_score"] = calculate_stability_score(
-            data["masks"], self.predictor.model.mask_threshold, self.stability_score_offset
+            data["masks"],
+            self.predictor.model.mask_threshold,
+            self.stability_score_offset,
         )
         if self.stability_score_thresh > 0.0:
             keep_mask = data["stability_score"] >= self.stability_score_thresh
             data.filter(keep_mask)
 
         # Threshold masks and calculate boxes
         data["masks"] = data["masks"] > self.predictor.model.mask_threshold
         data["boxes"] = batched_mask_to_box(data["masks"])
 
         # Filter boxes that touch crop boundaries
-        keep_mask = ~is_box_near_crop_edge(data["boxes"], crop_box, [0, 0, orig_w, orig_h])
+        keep_mask = ~is_box_near_crop_edge(
+            data["boxes"], crop_box, [0, 0, orig_w, orig_h]
+        )
         if not torch.all(keep_mask):
             data.filter(keep_mask)
 
         # Compress to RLE
         data["masks"] = uncrop_masks(data["masks"], crop_box, orig_h, orig_w)
         data["rles"] = mask_to_rle_pytorch(data["masks"])
         del data["masks"]
 
         return data
 
     @staticmethod
-    def postprocess_small_regions(mask_data: MaskData, min_area: int, nms_thresh: float) -> MaskData:
+    def postprocess_small_regions(
+        mask_data: MaskData, min_area: int, nms_thresh: float
+    ) -> MaskData:
         """
         Removes small disconnected regions and holes in masks, then reruns
         box NMS to remove any new duplicates.
 
         Edits mask_data in place.
 
         Requires open-cv as a dependency.
```

### Comparing `metaseg-0.7.5/metaseg/generator/build_sam.py` & `metaseg-0.7.6/metaseg/generator/build_sam.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 from functools import partial
 
 import torch
 
-from metaseg.modeling import ImageEncoderViT, MaskDecoder, PromptEncoder, Sam, TwoWayTransformer
+from metaseg.modeling import (
+    ImageEncoderViT,
+    MaskDecoder,
+    PromptEncoder,
+    Sam,
+    TwoWayTransformer,
+)
 
 
 def build_sam_vit_h(checkpoint=None):
     return _build_sam(
         encoder_embed_dim=1280,
         encoder_depth=32,
         encoder_num_heads=16,
@@ -40,14 +46,21 @@
         encoder_depth=12,
         encoder_num_heads=12,
         encoder_global_attn_indexes=[2, 5, 8, 11],
         checkpoint=checkpoint,
     )
 
 
+build_sam_vit_h = {
+    "default": build_sam,
+    "vit_h": build_sam,
+    "vit_l": build_sam_vit_l,
+    "vit_b": build_sam_vit_b,
+}
+
 sam_model_registry = {
     "default": build_sam,
     "vit_h": build_sam,
     "vit_l": build_sam_vit_l,
     "vit_b": build_sam_vit_b,
 }
```

### Comparing `metaseg-0.7.5/metaseg/generator/predictor.py` & `metaseg-0.7.6/metaseg/generator/predictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,17 @@
         ], f"image_format must be in ['RGB', 'BGR'], is {image_format}."
         if image_format != self.model.image_format:
             image = image[..., ::-1]
 
         # Transform the image to the form expected by the model
         input_image = self.transform.apply_image(image)
         input_image_torch = torch.as_tensor(input_image, device=self.device)
-        input_image_torch = input_image_torch.permute(2, 0, 1).contiguous()[None, :, :, :]
+        input_image_torch = input_image_torch.permute(2, 0, 1).contiguous()[
+            None, :, :, :
+        ]
 
         self.set_torch_image(input_image_torch, image.shape[:2])
 
     @torch.no_grad()
     def set_torch_image(
         self,
         transformed_image: torch.Tensor,
@@ -75,15 +77,18 @@
           original_image_size (tuple(int, int)): The size of the image
             before transformation, in (H, W) format.
         """
         assert (
             len(transformed_image.shape) == 4
             and transformed_image.shape[1] == 3
             and max(*transformed_image.shape[2:]) == self.model.image_encoder.img_size
-        ), f"set_torch_image input must be BCHW with long side {self.model.image_encoder.img_size}."
+        ), (
+            f"set_torch_image input must be BCHW with long side "
+            f"{self.model.image_encoder.img_size}."
+        )
         self.reset_image()
 
         self.original_size = original_image_size
         self.input_size = tuple(transformed_image.shape[-2:])
         input_image = self.model.preprocess(transformed_image)
         self.features = self.model.image_encoder(input_image)
         self.is_image_set = True
@@ -126,30 +131,40 @@
           (np.ndarray): An array of length C containing the model's
             predictions for the quality of each mask.
           (np.ndarray): An array of shape CxHxW, where C is the number
             of masks and H=W=256. These low resolution logits can be passed to
             a subsequent iteration as mask input.
         """
         if not self.is_image_set:
-            raise RuntimeError("An image must be set with .set_image(...) before mask prediction.")
+            raise RuntimeError(
+                "An image must be set with .set_image(...) before mask prediction."
+            )
 
         # Transform input prompts
         coords_torch, labels_torch, box_torch, mask_input_torch = None, None, None, None
         if point_coords is not None:
-            assert point_labels is not None, "point_labels must be supplied if point_coords is supplied."
+            assert (
+                point_labels is not None
+            ), "point_labels must be supplied if point_coords is supplied."
             point_coords = self.transform.apply_coords(point_coords, self.original_size)
-            coords_torch = torch.as_tensor(point_coords, dtype=torch.float, device=self.device)
-            labels_torch = torch.as_tensor(point_labels, dtype=torch.int, device=self.device)
+            coords_torch = torch.as_tensor(
+                point_coords, dtype=torch.float, device=self.device
+            )
+            labels_torch = torch.as_tensor(
+                point_labels, dtype=torch.int, device=self.device
+            )
             coords_torch, labels_torch = coords_torch[None, :, :], labels_torch[None, :]
         if box is not None:
             box = self.transform.apply_boxes(box, self.original_size)
             box_torch = torch.as_tensor(box, dtype=torch.float, device=self.device)
             box_torch = box_torch[None, :]
         if mask_input is not None:
-            mask_input_torch = torch.as_tensor(mask_input, dtype=torch.float, device=self.device)
+            mask_input_torch = torch.as_tensor(
+                mask_input, dtype=torch.float, device=self.device
+            )
             mask_input_torch = mask_input_torch[None, :, :, :]
 
         masks, iou_predictions, low_res_masks = self.predict_torch(
             coords_torch,
             labels_torch,
             box_torch,
             mask_input_torch,
@@ -204,15 +219,17 @@
           (torch.Tensor): An array of shape BxC containing the model's
             predictions for the quality of each mask.
           (torch.Tensor): An array of shape BxCxHxW, where C is the number
             of masks and H=W=256. These low res logits can be passed to
             a subsequent iteration as mask input.
         """
         if not self.is_image_set:
-            raise RuntimeError("An image must be set with .set_image(...) before mask prediction.")
+            raise RuntimeError(
+                "An image must be set with .set_image(...) before mask prediction."
+            )
 
         if point_coords is not None:
             points = (point_coords, point_labels)
         else:
             points = None
 
         # Embed prompts
@@ -228,30 +245,36 @@
             image_pe=self.model.prompt_encoder.get_dense_pe(),
             sparse_prompt_embeddings=sparse_embeddings,
             dense_prompt_embeddings=dense_embeddings,
             multimask_output=multimask_output,
         )
 
         # Upscale the masks to the original image resolution
-        masks = self.model.postprocess_masks(low_res_masks, self.input_size, self.original_size)
+        masks = self.model.postprocess_masks(
+            low_res_masks, self.input_size, self.original_size
+        )
 
         if not return_logits:
             masks = masks > self.model.mask_threshold
 
         return masks, iou_predictions, low_res_masks
 
     def get_image_embedding(self) -> torch.Tensor:
         """
         Returns the image embeddings for the currently set image, with
         shape 1xCxHxW, where C is the embedding dimension and (H,W) are
         the embedding spatial dimension of SAM (typically C=256, H=W=64).
         """
         if not self.is_image_set:
-            raise RuntimeError("An image must be set with .set_image(...) to generate an embedding.")
-        assert self.features is not None, "Features must exist if an image has been set."
+            raise RuntimeError(
+                "An image must be set with .set_image(...) to generate an embedding."
+            )
+        assert (
+            self.features is not None
+        ), "Features must exist if an image has been set."
         return self.features
 
     @property
     def device(self) -> torch.device:
         return self.model.device
 
     def reset_image(self) -> None:
```

### Comparing `metaseg-0.7.5/metaseg/mask_predictor.py` & `metaseg-0.7.6/metaseg/mask_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Any, Dict, List, Optional
-
 import cv2
 import numpy as np
 import torch
 from tqdm import tqdm
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import sam_model_registry
@@ -43,21 +41,27 @@
         output_path="output.png",
         show=False,
         save=False,
     ):
         read_image = load_image(source)
         model = self.load_model(model_type)
         mask_generator = SamAutomaticMaskGenerator(
-            model, points_per_side=points_per_side, points_per_batch=points_per_batch, min_mask_region_area=min_area
+            model,
+            points_per_side=points_per_side,
+            points_per_batch=points_per_batch,
+            min_mask_region_area=min_area,
         )
 
         masks = mask_generator.generate(read_image)
 
         sorted_anns = sorted(masks, key=(lambda x: x["area"]), reverse=True)
-        mask_image = np.zeros((masks[0]["segmentation"].shape[0], masks[0]["segmentation"].shape[1], 3), dtype=np.uint8)
+        mask_image = np.zeros(
+            (masks[0]["segmentation"].shape[0], masks[0]["segmentation"].shape[1], 3),
+            dtype=np.uint8,
+        )
         colors = np.random.randint(0, 255, size=(256, 3), dtype=np.uint8)
         for i, ann in enumerate(sorted_anns):
             m = ann["segmentation"]
             img = np.ones((m.shape[0], m.shape[1], 3), dtype=np.uint8)
             color = colors[i % 256]
             for i in range(3):
                 img[:, :, 0] = color[0]
@@ -73,36 +77,52 @@
             show_image(combined_mask)
 
         if save:
             save_image(output_path=output_path, output_image=combined_mask)
 
         return masks
 
-    def video_predict(self, source, model_type, points_per_side, points_per_batch, min_area, output_path="output.mp4"):
+    def video_predict(
+        self,
+        source,
+        model_type,
+        points_per_side,
+        points_per_batch,
+        min_area,
+        output_path="output.mp4",
+    ):
         cap, out = load_video(source, output_path)
         length = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
         colors = np.random.randint(0, 255, size=(256, 3), dtype=np.uint8)
 
         for _ in tqdm(range(length)):
             ret, frame = cap.read()
             if not ret:
                 break
 
             model = self.load_model(model_type)
             mask_generator = SamAutomaticMaskGenerator(
-                model, points_per_side=points_per_side, points_per_batch=points_per_batch, min_mask_region_area=min_area
+                model,
+                points_per_side=points_per_side,
+                points_per_batch=points_per_batch,
+                min_mask_region_area=min_area,
             )
             masks = mask_generator.generate(frame)
 
             if len(masks) == 0:
                 continue
 
             sorted_anns = sorted(masks, key=(lambda x: x["area"]), reverse=True)
             mask_image = np.zeros(
-                (masks[0]["segmentation"].shape[0], masks[0]["segmentation"].shape[1], 3), dtype=np.uint8
+                (
+                    masks[0]["segmentation"].shape[0],
+                    masks[0]["segmentation"].shape[1],
+                    3,
+                ),
+                dtype=np.uint8,
             )
 
             for i, ann in enumerate(sorted_anns):
                 m = ann["segmentation"]
                 color = colors[i % 256]
                 img = np.zeros((m.shape[0], m.shape[1], 3), dtype=np.uint8)
                 img[:, :, 0] = color[0]
```

### Comparing `metaseg-0.7.5/metaseg/modeling/common.py` & `metaseg-0.7.6/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.5/metaseg/modeling/image_encoder.py` & `metaseg-0.7.6/metaseg/modeling/image_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from metaseg.modeling.common import LayerNorm2d, MLPBlock
 
 
-# This class and its supporting functions below lightly adapted from the ViTDet backbone available at: https://github.com/facebookresearch/detectron2/blob/main/detectron2/modeling/backbone/vit.py # noqa
+# This class and its supporting functions below lightly adapted from the
+# ViTDet backbone available at:
+# https://github.com/facebookresearch/detectron2/blob/main/detectron2/modeling/backbone/vit.py
 class ImageEncoderViT(nn.Module):
     def __init__(
         self,
         img_size: int = 1024,
         patch_size: int = 16,
         in_chans: int = 3,
         embed_dim: int = 768,
@@ -42,34 +44,43 @@
             embed_dim (int): Patch embedding dimension.
             depth (int): Depth of ViT.
             num_heads (int): Number of attention heads in each ViT block.
             mlp_ratio (float): Ratio of mlp hidden dim to embedding dim.
             qkv_bias (bool): If True, add a learnable bias to query, key, value.
             norm_layer (nn.Module): Normalization layer.
             act_layer (nn.Module): Activation layer.
-            use_abs_pos (bool): If True, use absolute positional embeddings.
-            use_rel_pos (bool): If True, add relative positional embeddings to the attention map.
-            rel_pos_zero_init (bool): If True, zero initialize relative positional parameters.
-            window_size (int): Window size for window attention blocks.
-            global_attn_indexes (list): Indexes for blocks using global attention.
+            use_abs_pos (bool): If True, use absolute
+                positional embeddings.
+            use_rel_pos (bool): If True, add relative
+                positional embeddings to the attention map.
+            rel_pos_zero_init (bool): If True, zero initialize
+                relative positional parameters.
+            window_size (int): Window size for window
+                attention blocks.
+            global_attn_indexes (list): Indexes for
+                blocks using global attention.
         """
         super().__init__()
         self.img_size = img_size
 
         self.patch_embed = PatchEmbed(
             kernel_size=(patch_size, patch_size),
             stride=(patch_size, patch_size),
             in_chans=in_chans,
             embed_dim=embed_dim,
         )
 
         self.pos_embed: Optional[nn.Parameter] = None
         if use_abs_pos:
             # Initialize absolute positional embedding with pretrain image size.
-            self.pos_embed = nn.Parameter(torch.zeros(1, img_size // patch_size, img_size // patch_size, embed_dim))
+            self.pos_embed = nn.Parameter(
+                torch.zeros(
+                    1, img_size // patch_size, img_size // patch_size, embed_dim
+                )
+            )
 
         self.blocks = nn.ModuleList()
         for i in range(depth):
             block = Block(
                 dim=embed_dim,
                 num_heads=num_heads,
                 mlp_ratio=mlp_ratio,
@@ -111,15 +122,16 @@
 
         x = self.neck(x.permute(0, 3, 1, 2))
 
         return x
 
 
 class Block(nn.Module):
-    """Transformer blocks with support of window attention and residual propagation blocks"""
+    """Transformer blocks with support of window
+    attention and residual propagation blocks"""
 
     def __init__(
         self,
         dim: int,
         num_heads: int,
         mlp_ratio: float = 4.0,
         qkv_bias: bool = True,
@@ -134,34 +146,39 @@
         Args:
             dim (int): Number of input channels.
             num_heads (int): Number of attention heads in each ViT block.
             mlp_ratio (float): Ratio of mlp hidden dim to embedding dim.
             qkv_bias (bool): If True, add a learnable bias to query, key, value.
             norm_layer (nn.Module): Normalization layer.
             act_layer (nn.Module): Activation layer.
-            use_rel_pos (bool): If True, add relative positional embeddings to the attention map.
-            rel_pos_zero_init (bool): If True, zero initialize relative positional parameters.
-            window_size (int): Window size for window attention blocks. If it equals 0, then
-                use global attention.
-            input_size (int or None): Input resolution for calculating the relative positional
-                parameter size.
+            use_rel_pos (bool): If True, add relative
+            positional embeddings to the attention map.
+            rel_pos_zero_init (bool): If True, zero
+            initialize relative positional parameters.
+            window_size (int): Window size for
+            window attention blocks. If it equals 0, then
+            use global attention.
+            input_size (int or None): Input resolution for
+            calculating the relative positional parameter size.
         """
         super().__init__()
         self.norm1 = norm_layer(dim)
         self.attn = Attention(
             dim,
             num_heads=num_heads,
             qkv_bias=qkv_bias,
             use_rel_pos=use_rel_pos,
             rel_pos_zero_init=rel_pos_zero_init,
             input_size=input_size if window_size == 0 else (window_size, window_size),
         )
 
         self.norm2 = norm_layer(dim)
-        self.mlp = MLPBlock(embedding_dim=dim, mlp_dim=int(dim * mlp_ratio), act=act_layer)
+        self.mlp = MLPBlock(
+            embedding_dim=dim, mlp_dim=int(dim * mlp_ratio), act=act_layer
+        )
 
         self.window_size = window_size
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         shortcut = x
         x = self.norm1(x)
         # Window partition
@@ -190,82 +207,105 @@
         qkv_bias: bool = True,
         use_rel_pos: bool = False,
         rel_pos_zero_init: bool = True,
         input_size: Optional[Tuple[int, int]] = None,
     ) -> None:
         """
         Args:
-            dim (int): Number of input channels.
-            num_heads (int): Number of attention heads.
-            qkv_bias (bool:  If True, add a learnable bias to query, key, value.
-            rel_pos (bool): If True, add relative positional embeddings to the attention map.
-            rel_pos_zero_init (bool): If True, zero initialize relative positional parameters.
-            input_size (int or None): Input resolution for calculating the relative positional
+            dim(int): Number of input channels.
+            num_heads(int): Number of attention heads.
+            qkv_bias(bool): If True, add a learnable
+                bias to query, key, value.
+            rel_pos(bool): If True, add relative
+                positional embeddings to the attention map.
+            rel_pos_zero_init(bool): If True, zero initialize
+                relative positional parameters.
+            input_size(int or None): Input resolution for
+                calculating the relative positional
                 parameter size.
         """
         super().__init__()
         self.num_heads = num_heads
         head_dim = dim // num_heads
-        self.scale = head_dim ** -0.5
+        self.scale = head_dim**-0.5
 
         self.qkv = nn.Linear(dim, dim * 3, bias=qkv_bias)
         self.proj = nn.Linear(dim, dim)
 
         self.use_rel_pos = use_rel_pos
         if self.use_rel_pos:
-            assert input_size is not None, "Input size must be provided if using relative positional encoding."
+            assert (
+                input_size is not None
+            ), "Input size must be provided if using relative positional encoding."
             # initialize relative positional embeddings
             self.rel_pos_h = nn.Parameter(torch.zeros(2 * input_size[0] - 1, head_dim))
             self.rel_pos_w = nn.Parameter(torch.zeros(2 * input_size[1] - 1, head_dim))
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         B, H, W, _ = x.shape
         # qkv with shape (3, B, nHead, H * W, C)
-        qkv = self.qkv(x).reshape(B, H * W, 3, self.num_heads, -1).permute(2, 0, 3, 1, 4)
+        qkv = (
+            self.qkv(x).reshape(B, H * W, 3, self.num_heads, -1).permute(2, 0, 3, 1, 4)
+        )
         # q, k, v with shape (B * nHead, H * W, C)
         q, k, v = qkv.reshape(3, B * self.num_heads, H * W, -1).unbind(0)
 
         attn = (q * self.scale) @ k.transpose(-2, -1)
 
         if self.use_rel_pos:
-            attn = add_decomposed_rel_pos(attn, q, self.rel_pos_h, self.rel_pos_w, (H, W), (H, W))
+            attn = add_decomposed_rel_pos(
+                attn, q, self.rel_pos_h, self.rel_pos_w, (H, W), (H, W)
+            )
 
         attn = attn.softmax(dim=-1)
-        x = (attn @ v).view(B, self.num_heads, H, W, -1).permute(0, 2, 3, 1, 4).reshape(B, H, W, -1)
+        x = (
+            (attn @ v)
+            .view(B, self.num_heads, H, W, -1)
+            .permute(0, 2, 3, 1, 4)
+            .reshape(B, H, W, -1)
+        )
         x = self.proj(x)
 
         return x
 
 
-def window_partition(x: torch.Tensor, window_size: int) -> Tuple[torch.Tensor, Tuple[int, int]]:
+def window_partition(
+    x: torch.Tensor, window_size: int
+) -> Tuple[torch.Tensor, Tuple[int, int]]:
     """
     Partition into non-overlapping windows with padding if needed.
     Args:
         x (tensor): input tokens with [B, H, W, C].
         window_size (int): window size.
 
     Returns:
-        windows: windows after partition with [B * num_windows, window_size, window_size, C].
+        windows: windows after partition with
+            [B * num_windows, window_size, window_size, C].
         (Hp, Wp): padded height and width before partition
     """
     B, H, W, C = x.shape
 
     pad_h = (window_size - H % window_size) % window_size
     pad_w = (window_size - W % window_size) % window_size
     if pad_h > 0 or pad_w > 0:
         x = F.pad(x, (0, 0, 0, pad_w, 0, pad_h))
     Hp, Wp = H + pad_h, W + pad_w
 
     x = x.view(B, Hp // window_size, window_size, Wp // window_size, window_size, C)
-    windows = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(-1, window_size, window_size, C)
+    windows = (
+        x.permute(0, 1, 3, 2, 4, 5).contiguous().view(-1, window_size, window_size, C)
+    )
     return windows, (Hp, Wp)
 
 
 def window_unpartition(
-    windows: torch.Tensor, window_size: int, pad_hw: Tuple[int, int], hw: Tuple[int, int]
+    windows: torch.Tensor,
+    window_size: int,
+    pad_hw: Tuple[int, int],
+    hw: Tuple[int, int],
 ) -> torch.Tensor:
     """
     Window unpartition into original sequences and removing padding.
     Args:
         x (tensor): input tokens with [B * num_windows, window_size, window_size, C].
         window_size (int): window size.
         pad_hw (Tuple): padded height and width (Hp, Wp).
@@ -273,15 +313,17 @@
 
     Returns:
         x: unpartitioned sequences with [B, H, W, C].
     """
     Hp, Wp = pad_hw
     H, W = hw
     B = windows.shape[0] // (Hp * Wp // window_size // window_size)
-    x = windows.view(B, Hp // window_size, Wp // window_size, window_size, window_size, -1)
+    x = windows.view(
+        B, Hp // window_size, Wp // window_size, window_size, window_size, -1
+    )
     x = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(B, Hp, Wp, -1)
 
     if Hp > H or Wp > W:
         x = x[:, :H, :W, :].contiguous()
     return x
 
 
@@ -324,15 +366,16 @@
     rel_pos_h: torch.Tensor,
     rel_pos_w: torch.Tensor,
     q_size: Tuple[int, int],
     k_size: Tuple[int, int],
 ) -> torch.Tensor:
     """
     Calculate decomposed Relative Positional Embeddings from :paper:`mvitv2`.
-    https://github.com/facebookresearch/mvit/blob/19786631e330df9f3622e5402b4a419a263a2c80/mvit/models/attention.py   # noqa B950
+    commit_sha: 19786631e330df9f3622e5402b4a419a263a2c80
+    https://github.com/facebookresearch/mvit/blob/main/mvit/models/attention.py
     Args:
         attn (Tensor): attention map.
         q (Tensor): query q in the attention layer with shape (B, q_h * q_w, C).
         rel_pos_h (Tensor): relative position embeddings (Lh, C) for height axis.
         rel_pos_w (Tensor): relative position embeddings (Lw, C) for width axis.
         q_size (Tuple): spatial sequence size of query q with (q_h, q_w).
         k_size (Tuple): spatial sequence size of key k with (k_h, k_w).
@@ -346,17 +389,19 @@
     Rw = get_rel_pos(q_w, k_w, rel_pos_w)
 
     B, _, dim = q.shape
     r_q = q.reshape(B, q_h, q_w, dim)
     rel_h = torch.einsum("bhwc,hkc->bhwk", r_q, Rh)
     rel_w = torch.einsum("bhwc,wkc->bhwk", r_q, Rw)
 
-    attn = (attn.view(B, q_h, q_w, k_h, k_w) + rel_h[:, :, :, :, None] + rel_w[:, :, :, None, :]).view(
-        B, q_h * q_w, k_h * k_w
-    )
+    attn = (
+        attn.view(B, q_h, q_w, k_h, k_w)
+        + rel_h[:, :, :, :, None]
+        + rel_w[:, :, :, None, :]
+    ).view(B, q_h * q_w, k_h * k_w)
 
     return attn
 
 
 class PatchEmbed(nn.Module):
     """
     Image to Patch Embedding.
@@ -376,14 +421,16 @@
             stride (Tuple): stride of the projection layer.
             padding (Tuple): padding size of the projection layer.
             in_chans (int): Number of input image channels.
             embed_dim (int):  embed_dim (int): Patch embedding dimension.
         """
         super().__init__()
 
-        self.proj = nn.Conv2d(in_chans, embed_dim, kernel_size=kernel_size, stride=stride, padding=padding)
+        self.proj = nn.Conv2d(
+            in_chans, embed_dim, kernel_size=kernel_size, stride=stride, padding=padding
+        )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         x = self.proj(x)
         # B C H W -> B H W C
         x = x.permute(0, 2, 3, 1)
         return x
```

### Comparing `metaseg-0.7.5/metaseg/modeling/mask_decoder.py` & `metaseg-0.7.6/metaseg/modeling/mask_decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,44 +47,56 @@
         self.num_multimask_outputs = num_multimask_outputs
 
         self.iou_token = nn.Embedding(1, transformer_dim)
         self.num_mask_tokens = num_multimask_outputs + 1
         self.mask_tokens = nn.Embedding(self.num_mask_tokens, transformer_dim)
 
         self.output_upscaling = nn.Sequential(
-            nn.ConvTranspose2d(transformer_dim, transformer_dim // 4, kernel_size=2, stride=2),
+            nn.ConvTranspose2d(
+                transformer_dim, transformer_dim // 4, kernel_size=2, stride=2
+            ),
             LayerNorm2d(transformer_dim // 4),
             activation(),
-            nn.ConvTranspose2d(transformer_dim // 4, transformer_dim // 8, kernel_size=2, stride=2),
+            nn.ConvTranspose2d(
+                transformer_dim // 4, transformer_dim // 8, kernel_size=2, stride=2
+            ),
             activation(),
         )
         self.output_hypernetworks_mlps = nn.ModuleList(
-            [MLP(transformer_dim, transformer_dim, transformer_dim // 8, 3) for i in range(self.num_mask_tokens)]
+            [
+                MLP(transformer_dim, transformer_dim, transformer_dim // 8, 3)
+                for i in range(self.num_mask_tokens)
+            ]
         )
 
-        self.iou_prediction_head = MLP(transformer_dim, iou_head_hidden_dim, self.num_mask_tokens, iou_head_depth)
+        self.iou_prediction_head = MLP(
+            transformer_dim, iou_head_hidden_dim, self.num_mask_tokens, iou_head_depth
+        )
 
     def forward(
         self,
         image_embeddings: torch.Tensor,
         image_pe: torch.Tensor,
         sparse_prompt_embeddings: torch.Tensor,
         dense_prompt_embeddings: torch.Tensor,
         multimask_output: bool,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """
         Predict masks given image and prompt embeddings.
 
         Arguments:
           image_embeddings (torch.Tensor): the embeddings from the image encoder
-          image_pe (torch.Tensor): positional encoding with the shape of image_embeddings
-          sparse_prompt_embeddings (torch.Tensor): the embeddings of the points and boxes
-          dense_prompt_embeddings (torch.Tensor): the embeddings of the mask inputs
-          multimask_output (bool): Whether to return multiple masks or a single
-            mask.
+          image_pe (torch.Tensor): positional encoding
+            with the shape of image_embeddings
+          sparse_prompt_embeddings (torch.Tensor): the embeddings
+            of the points and boxes
+          dense_prompt_embeddings (torch.Tensor): the embeddings
+            of the mask inputs
+          multimask_output (bool): Whether to return
+            multiple masks or a single mask.
 
         Returns:
           torch.Tensor: batched predicted masks
           torch.Tensor: batched predictions of mask quality
         """
         masks, iou_pred = self.predict_masks(
             image_embeddings=image_embeddings,
@@ -109,16 +121,20 @@
         image_embeddings: torch.Tensor,
         image_pe: torch.Tensor,
         sparse_prompt_embeddings: torch.Tensor,
         dense_prompt_embeddings: torch.Tensor,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Predicts masks. See 'forward' for more details."""
         # Concatenate output tokens
-        output_tokens = torch.cat([self.iou_token.weight, self.mask_tokens.weight], dim=0)
-        output_tokens = output_tokens.unsqueeze(0).expand(sparse_prompt_embeddings.size(0), -1, -1)
+        output_tokens = torch.cat(
+            [self.iou_token.weight, self.mask_tokens.weight], dim=0
+        )
+        output_tokens = output_tokens.unsqueeze(0).expand(
+            sparse_prompt_embeddings.size(0), -1, -1
+        )
         tokens = torch.cat((output_tokens, sparse_prompt_embeddings), dim=1)
 
         # Expand per-image data in batch direction to be per-mask
         src = torch.repeat_interleave(image_embeddings, tokens.shape[0], dim=0)
         src = src + dense_prompt_embeddings
         pos_src = torch.repeat_interleave(image_pe, tokens.shape[0], dim=0)
         b, c, h, w = src.shape
@@ -129,15 +145,17 @@
         mask_tokens_out = hs[:, 1 : (1 + self.num_mask_tokens), :]
 
         # Upscale mask embeddings and predict masks using the mask tokens
         src = src.transpose(1, 2).view(b, c, h, w)
         upscaled_embedding = self.output_upscaling(src)
         hyper_in_list: List[torch.Tensor] = []
         for i in range(self.num_mask_tokens):
-            hyper_in_list.append(self.output_hypernetworks_mlps[i](mask_tokens_out[:, i, :]))
+            hyper_in_list.append(
+                self.output_hypernetworks_mlps[i](mask_tokens_out[:, i, :])
+            )
         hyper_in = torch.stack(hyper_in_list, dim=1)
         b, c, h, w = upscaled_embedding.shape
         masks = (hyper_in @ upscaled_embedding.view(b, c, h * w)).view(b, -1, h, w)
 
         # Generate mask quality predictions
         iou_pred = self.iou_prediction_head(iou_token_out)
 
@@ -154,15 +172,17 @@
         output_dim: int,
         num_layers: int,
         sigmoid_output: bool = False,
     ) -> None:
         super().__init__()
         self.num_layers = num_layers
         h = [hidden_dim] * (num_layers - 1)
-        self.layers = nn.ModuleList(nn.Linear(n, k) for n, k in zip([input_dim] + h, h + [output_dim]))
+        self.layers = nn.ModuleList(
+            nn.Linear(n, k) for n, k in zip([input_dim] + h, h + [output_dim])
+        )
         self.sigmoid_output = sigmoid_output
 
     def forward(self, x):
         for i, layer in enumerate(self.layers):
             x = F.relu(layer(x)) if i < self.num_layers - 1 else layer(x)
         if self.sigmoid_output:
             x = F.sigmoid(x)
```

### Comparing `metaseg-0.7.5/metaseg/modeling/prompt_encoder.py` & `metaseg-0.7.6/metaseg/modeling/prompt_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,19 +39,24 @@
         super().__init__()
         self.embed_dim = embed_dim
         self.input_image_size = input_image_size
         self.image_embedding_size = image_embedding_size
         self.pe_layer = PositionEmbeddingRandom(embed_dim // 2)
 
         self.num_point_embeddings: int = 4  # pos/neg point + 2 box corners
-        point_embeddings = [nn.Embedding(1, embed_dim) for i in range(self.num_point_embeddings)]
+        point_embeddings = [
+            nn.Embedding(1, embed_dim) for i in range(self.num_point_embeddings)
+        ]
         self.point_embeddings = nn.ModuleList(point_embeddings)
         self.not_a_point_embed = nn.Embedding(1, embed_dim)
 
-        self.mask_input_size = (4 * image_embedding_size[0], 4 * image_embedding_size[1])
+        self.mask_input_size = (
+            4 * image_embedding_size[0],
+            4 * image_embedding_size[1],
+        )
         self.mask_downscaling = nn.Sequential(
             nn.Conv2d(1, mask_in_chans // 4, kernel_size=2, stride=2),
             LayerNorm2d(mask_in_chans // 4),
             activation(),
             nn.Conv2d(mask_in_chans // 4, mask_in_chans, kernel_size=2, stride=2),
             LayerNorm2d(mask_in_chans),
             activation(),
@@ -79,26 +84,30 @@
         """Embeds point prompts."""
         points = points + 0.5  # Shift to center of pixel
         if pad:
             padding_point = torch.zeros((points.shape[0], 1, 2), device=points.device)
             padding_label = -torch.ones((labels.shape[0], 1), device=labels.device)
             points = torch.cat([points, padding_point], dim=1)
             labels = torch.cat([labels, padding_label], dim=1)
-        point_embedding = self.pe_layer.forward_with_coords(points, self.input_image_size)
+        point_embedding = self.pe_layer.forward_with_coords(
+            points, self.input_image_size
+        )
         point_embedding[labels == -1] = 0.0
         point_embedding[labels == -1] += self.not_a_point_embed.weight
         point_embedding[labels == 0] += self.point_embeddings[0].weight
         point_embedding[labels == 1] += self.point_embeddings[1].weight
         return point_embedding
 
     def _embed_boxes(self, boxes: torch.Tensor) -> torch.Tensor:
         """Embeds box prompts."""
         boxes = boxes + 0.5  # Shift to center of pixel
         coords = boxes.reshape(-1, 2, 2)
-        corner_embedding = self.pe_layer.forward_with_coords(coords, self.input_image_size)
+        corner_embedding = self.pe_layer.forward_with_coords(
+            coords, self.input_image_size
+        )
         corner_embedding[:, 0, :] += self.point_embeddings[2].weight
         corner_embedding[:, 1, :] += self.point_embeddings[3].weight
         return corner_embedding
 
     def _embed_masks(self, masks: torch.Tensor) -> torch.Tensor:
         """Embeds mask inputs."""
         mask_embedding = self.mask_downscaling(masks)
@@ -145,15 +154,17 @@
           torch.Tensor: sparse embeddings for the points and boxes, with shape
             BxNx(embed_dim), where N is determined by the number of input points
             and boxes.
           torch.Tensor: dense embeddings for the masks, in the shape
             Bx(embed_dim)x(embed_H)x(embed_W)
         """
         bs = self._get_batch_size(points, boxes, masks)
-        sparse_embeddings = torch.empty((bs, 0, self.embed_dim), device=self._get_device())
+        sparse_embeddings = torch.empty(
+            (bs, 0, self.embed_dim), device=self._get_device()
+        )
         if points is not None:
             coords, labels = points
             point_embeddings = self._embed_points(coords, labels, pad=(boxes is None))
             sparse_embeddings = torch.cat([sparse_embeddings, point_embeddings], dim=1)
         if boxes is not None:
             box_embeddings = self._embed_boxes(boxes)
             sparse_embeddings = torch.cat([sparse_embeddings, box_embeddings], dim=1)
@@ -200,13 +211,15 @@
         x_embed = grid.cumsum(dim=1) - 0.5
         y_embed = y_embed / h
         x_embed = x_embed / w
 
         pe = self._pe_encoding(torch.stack([x_embed, y_embed], dim=-1))
         return pe.permute(2, 0, 1)  # C x H x W
 
-    def forward_with_coords(self, coords_input: torch.Tensor, image_size: Tuple[int, int]) -> torch.Tensor:
+    def forward_with_coords(
+        self, coords_input: torch.Tensor, image_size: Tuple[int, int]
+    ) -> torch.Tensor:
         """Positionally encode points that are not normalized to [0,1]."""
         coords = coords_input.clone()
         coords[:, :, 0] = coords[:, :, 0] / image_size[1]
         coords[:, :, 1] = coords[:, :, 1] / image_size[0]
         return self._pe_encoding(coords.to(torch.float))  # B x N x C
```

### Comparing `metaseg-0.7.5/metaseg/modeling/sam.py` & `metaseg-0.7.6/metaseg/modeling/sam.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,26 @@
 
         Arguments:
           image_encoder (ImageEncoderViT): The backbone used to encode the
             image into image embeddings that allow for efficient mask prediction.
           prompt_encoder (PromptEncoder): Encodes various types of input prompts.
           mask_decoder (MaskDecoder): Predicts masks from the image embeddings
             and encoded prompts.
-          pixel_mean (list(float)): Mean values for normalizing pixels in the input image.
-          pixel_std (list(float)): Std values for normalizing pixels in the input image.
+          pixel_mean (list(float)): Mean values for normalizing
+            pixels in the input image.
+          pixel_std (list(float)): Std values for normalizing
+            pixels in the input image.
         """
         super().__init__()
         self.image_encoder = image_encoder
         self.prompt_encoder = prompt_encoder
         self.mask_decoder = mask_decoder
-        self.register_buffer("pixel_mean", torch.Tensor(pixel_mean).view(-1, 1, 1), False)
+        self.register_buffer(
+            "pixel_mean", torch.Tensor(pixel_mean).view(-1, 1, 1), False
+        )
         self.register_buffer("pixel_std", torch.Tensor(pixel_std).view(-1, 1, 1), False)
 
     @property
     def device(self) -> Any:
         return self.pixel_mean.device
 
     @torch.no_grad()
@@ -90,15 +94,17 @@
                 original size of the image.
               'iou_predictions': (torch.Tensor) The model's predictions
                 of mask quality, in shape BxC.
               'low_res_logits': (torch.Tensor) Low resolution logits with
                 shape BxCxHxW, where H=W=256. Can be passed as mask input
                 to subsequent iterations of prediction.
         """
-        input_images = torch.stack([self.preprocess(x["image"]) for x in batched_input], dim=0)
+        input_images = torch.stack(
+            [self.preprocess(x["image"]) for x in batched_input], dim=0
+        )
         image_embeddings = self.image_encoder(input_images)
 
         outputs = []
         for image_record, curr_embedding in zip(batched_input, image_embeddings):
             if "point_coords" in image_record:
                 points = (image_record["point_coords"], image_record["point_labels"])
             else:
@@ -154,15 +160,17 @@
         masks = F.interpolate(
             masks,
             (self.image_encoder.img_size, self.image_encoder.img_size),
             mode="bilinear",
             align_corners=False,
         )
         masks = masks[..., : input_size[0], : input_size[1]]
-        masks = F.interpolate(masks, original_size, mode="bilinear", align_corners=False)
+        masks = F.interpolate(
+            masks, original_size, mode="bilinear", align_corners=False
+        )
         return masks
 
     def preprocess(self, x: torch.Tensor) -> torch.Tensor:
         """Normalize pixel values and pad to a square input."""
         # Normalize colors
         x = (x - self.pixel_mean) / self.pixel_std
```

### Comparing `metaseg-0.7.5/metaseg/modeling/transformer.py` & `metaseg-0.7.6/metaseg/modeling/transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,17 @@
                     mlp_dim=mlp_dim,
                     activation=activation,
                     attention_downsample_rate=attention_downsample_rate,
                     skip_first_layer_pe=(i == 0),
                 )
             )
 
-        self.final_attn_token_to_image = Attention(embedding_dim, num_heads, downsample_rate=attention_downsample_rate)
+        self.final_attn_token_to_image = Attention(
+            embedding_dim, num_heads, downsample_rate=attention_downsample_rate
+        )
         self.norm_final_attn = nn.LayerNorm(embedding_dim)
 
     def forward(
         self,
         image_embedding: Tensor,
         image_pe: Tensor,
         point_embedding: Tensor,
@@ -127,26 +129,32 @@
           activation (nn.Module): the activation of the mlp block
           skip_first_layer_pe (bool): skip the PE on the first layer
         """
         super().__init__()
         self.self_attn = Attention(embedding_dim, num_heads)
         self.norm1 = nn.LayerNorm(embedding_dim)
 
-        self.cross_attn_token_to_image = Attention(embedding_dim, num_heads, downsample_rate=attention_downsample_rate)
+        self.cross_attn_token_to_image = Attention(
+            embedding_dim, num_heads, downsample_rate=attention_downsample_rate
+        )
         self.norm2 = nn.LayerNorm(embedding_dim)
 
         self.mlp = MLPBlock(embedding_dim, mlp_dim, activation)
         self.norm3 = nn.LayerNorm(embedding_dim)
 
         self.norm4 = nn.LayerNorm(embedding_dim)
-        self.cross_attn_image_to_token = Attention(embedding_dim, num_heads, downsample_rate=attention_downsample_rate)
+        self.cross_attn_image_to_token = Attention(
+            embedding_dim, num_heads, downsample_rate=attention_downsample_rate
+        )
 
         self.skip_first_layer_pe = skip_first_layer_pe
 
-    def forward(self, queries: Tensor, keys: Tensor, query_pe: Tensor, key_pe: Tensor) -> Tuple[Tensor, Tensor]:
+    def forward(
+        self, queries: Tensor, keys: Tensor, query_pe: Tensor, key_pe: Tensor
+    ) -> Tuple[Tensor, Tensor]:
         # Self attention block
         if self.skip_first_layer_pe:
             queries = self.self_attn(q=queries, k=queries, v=queries)
         else:
             q = queries + query_pe
             attn_out = self.self_attn(q=q, k=q, v=queries)
             queries = queries + attn_out
@@ -186,15 +194,17 @@
         num_heads: int,
         downsample_rate: int = 1,
     ) -> None:
         super().__init__()
         self.embedding_dim = embedding_dim
         self.internal_dim = embedding_dim // downsample_rate
         self.num_heads = num_heads
-        assert self.internal_dim % num_heads == 0, "num_heads must divide embedding_dim."
+        assert (
+            self.internal_dim % num_heads == 0
+        ), "num_heads must divide embedding_dim."
 
         self.q_proj = nn.Linear(embedding_dim, self.internal_dim)
         self.k_proj = nn.Linear(embedding_dim, self.internal_dim)
         self.v_proj = nn.Linear(embedding_dim, self.internal_dim)
         self.out_proj = nn.Linear(self.internal_dim, embedding_dim)
 
     def _separate_heads(self, x: Tensor, num_heads: int) -> Tensor:
```

### Comparing `metaseg-0.7.5/metaseg/sahi_predict.py` & `metaseg-0.7.6/metaseg/sahi_predict.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from PIL import Image
 
-from metaseg import SamPredictor, sam_model_registry
-from metaseg.utils import download_model, load_image, multi_boxes, plt_load_box, plt_load_mask
+from metaseg.generator import SamPredictor, sam_model_registry
+from metaseg.utils import (
+    download_model,
+    load_image,
+    multi_boxes,
+    plt_load_box,
+    plt_load_mask,
+)
 
 
 def sahi_sliced_predict(
     image_path,
     detection_model_type,
     detection_model_path,
     conf_th,
     image_size,
     slice_height,
     slice_width,
     overlap_height_ratio,
     overlap_width_ratio,
 ):
-
     try:
         from sahi import AutoDetectionModel
         from sahi.predict import get_prediction, get_sliced_prediction
     except ImportError:
         raise ImportError("Please install SAHI library using 'pip install sahi'.")
 
     device = "cuda" if torch.cuda.is_available() else "cpu"
@@ -74,15 +79,14 @@
         input_point=None,
         input_label=None,
         multimask_output=False,
         random_color=False,
         show=False,
         save=False,
     ):
-
         read_image = load_image(source)
         model = self.load_model(model_type)
         predictor = SamPredictor(model)
         predictor.set_image(read_image)
 
         if type(input_box[0]) == list:
             input_boxes, new_boxes = multi_boxes(input_box, predictor, read_image)
```

### Comparing `metaseg-0.7.5/metaseg/utils/amg.py` & `metaseg-0.7.6/metaseg/utils/amg.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,42 +149,54 @@
     return mask.transpose()  # Put in C order
 
 
 def area_from_rle(rle: Dict[str, Any]) -> int:
     return sum(rle["counts"][1::2])
 
 
-def calculate_stability_score(masks: torch.Tensor, mask_threshold: float, threshold_offset: float) -> torch.Tensor:
+def calculate_stability_score(
+    masks: torch.Tensor, mask_threshold: float, threshold_offset: float
+) -> torch.Tensor:
     """
     Computes the stability score for a batch of masks. The stability
     score is the IoU between the binary masks obtained by thresholding
     the predicted mask logits at high and low values.
     """
     # One mask is always contained inside the other.
     # Save memory by preventing unnecesary cast to torch.int64
-    intersections = (masks > (mask_threshold + threshold_offset)).sum(-1, dtype=torch.int16).sum(-1, dtype=torch.int32)
-    unions = (masks > (mask_threshold - threshold_offset)).sum(-1, dtype=torch.int16).sum(-1, dtype=torch.int32)
+    intersections = (
+        (masks > (mask_threshold + threshold_offset))
+        .sum(-1, dtype=torch.int16)
+        .sum(-1, dtype=torch.int32)
+    )
+    unions = (
+        (masks > (mask_threshold - threshold_offset))
+        .sum(-1, dtype=torch.int16)
+        .sum(-1, dtype=torch.int32)
+    )
     return intersections / unions
 
 
 def build_point_grid(n_per_side: int) -> np.ndarray:
     """Generates a 2D grid of points evenly spaced in [0,1]x[0,1]."""
     offset = 1 / (2 * n_per_side)
     points_one_side = np.linspace(offset, 1 - offset, n_per_side)
     points_x = np.tile(points_one_side[None, :], (n_per_side, 1))
     points_y = np.tile(points_one_side[:, None], (1, n_per_side))
     points = np.stack([points_x, points_y], axis=-1).reshape(-1, 2)
     return points
 
 
-def build_all_layer_point_grids(n_per_side: int, n_layers: int, scale_per_layer: int) -> List[np.ndarray]:
+def build_all_layer_point_grids(
+    n_per_side: int, n_layers: int, scale_per_layer: int
+) -> List[np.ndarray]:
     """Generates point grids for all crop layers."""
     points_by_layer = []
     for i in range(n_layers + 1):
-        n_points = int(n_per_side / (scale_per_layer ** i))
+        n_points = int(n_per_side / (scale_per_layer**i))
         points_by_layer.append(build_point_grid(n_points))
     return points_by_layer
 
 
 def generate_crop_boxes(
     im_size: Tuple[int, ...], n_layers: int, overlap_ratio: float
 ) -> Tuple[List[List[int]], List[int]]:
@@ -236,25 +248,29 @@
     offset = torch.tensor([[x0, y0]], device=points.device)
     # Check if points has a channel dimension
     if len(points.shape) == 3:
         offset = offset.unsqueeze(1)
     return points + offset
 
 
-def uncrop_masks(masks: torch.Tensor, crop_box: List[int], orig_h: int, orig_w: int) -> torch.Tensor:
+def uncrop_masks(
+    masks: torch.Tensor, crop_box: List[int], orig_h: int, orig_w: int
+) -> torch.Tensor:
     x0, y0, x1, y1 = crop_box
     if x0 == 0 and y0 == 0 and x1 == orig_w and y1 == orig_h:
         return masks
     # Coordinate transform masks
     pad_x, pad_y = orig_w - (x1 - x0), orig_h - (y1 - y0)
     pad = (x0, pad_x - x0, y0, pad_y - y0)
     return torch.nn.functional.pad(masks, pad, value=0)
 
 
-def remove_small_regions(mask: np.ndarray, area_thresh: float, mode: str) -> Tuple[np.ndarray, bool]:
+def remove_small_regions(
+    mask: np.ndarray, area_thresh: float, mode: str
+) -> Tuple[np.ndarray, bool]:
     """
     Removes small disconnected regions and holes in a mask. Returns the
     mask and an indicator of if the mask has been modified.
     """
     import cv2  # type: ignore
 
     assert mode in ["holes", "islands"]
```

### Comparing `metaseg-0.7.5/metaseg/utils/data_utils.py` & `metaseg-0.7.6/metaseg/utils/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,22 +81,26 @@
 
 
 def plt_load_box(box, ax):
     import matplotlib.pyplot as plt
 
     x0, y0 = box[0], box[1]
     w, h = box[2] - box[0], box[3] - box[1]
-    ax.add_patch(plt.Rectangle((x0, y0), w, h, edgecolor="green", facecolor=(0, 0, 0, 0), lw=2))
+    ax.add_patch(
+        plt.Rectangle((x0, y0), w, h, edgecolor="green", facecolor=(0, 0, 0, 0), lw=2)
+    )
 
 
 def multi_boxes(boxes, predictor, image):
     import torch
 
     input_boxes = torch.tensor(boxes, device=predictor.device)
-    transformed_boxes = predictor.transform.apply_boxes_torch(input_boxes, image.shape[:2])
+    transformed_boxes = predictor.transform.apply_boxes_torch(
+        input_boxes, image.shape[:2]
+    )
     return input_boxes, transformed_boxes
 
 
 def show_image(output_image):
     import cv2
 
     cv2.imshow("output", output_image)
```

### Comparing `metaseg-0.7.5/metaseg/utils/file_utils.py` & `metaseg-0.7.6/metaseg/utils/file_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import urllib.request
 
 
 def download_model(model_type):
     """
-    model_type: str, A string representing the model type. It can be 'vit_h', 'vit_l', or 'vit_b'.
+    model_type: str, A string representing the model type.
+    It can be 'vit_h', 'vit_l', or 'vit_b'.
     """
 
     # A dictionary containing model types as keys and their respective URLs as values
     model_urls = {
         "vit_h": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
         "vit_l": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
         "vit_b": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
@@ -16,14 +17,19 @@
 
     # Check if the model file already exists and model_type is in model_urls
     filename = f"{model_type}.pth"
     if not os.path.exists(filename) and model_type in model_urls:
         url = model_urls[model_type]
         print(f"Downloading {model_type} model from {url}...")
         urllib.request.urlretrieve(url, filename)
-        print(f"{model_type} model has been successfully downloaded and saved as '{filename}'.")
+        print(
+            f"{model_type} model has been successfully "
+            f"downloaded and saved as '{filename}'."
+        )
     elif os.path.exists(filename):
         print(f"{model_type} model already exists as '{filename}'. Skipping download.")
     else:
-        raise ValueError("Invalid model type. It should be 'vit_h', 'vit_l', or 'vit_b'.")
+        raise ValueError(
+            "Invalid model type. It should be 'vit_h', 'vit_l', or 'vit_b'."
+        )
 
     return filename
```

### Comparing `metaseg-0.7.5/metaseg/utils/onnx.py` & `metaseg-0.7.6/metaseg/utils/onnx.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,45 +35,60 @@
         self.img_size = model.image_encoder.img_size
         self.return_single_mask = return_single_mask
         self.use_stability_score = use_stability_score
         self.stability_score_offset = 1.0
         self.return_extra_metrics = return_extra_metrics
 
     @staticmethod
-    def resize_longest_image_size(input_image_size: torch.Tensor, longest_side: int) -> torch.Tensor:
+    def resize_longest_image_size(
+        input_image_size: torch.Tensor, longest_side: int
+    ) -> torch.Tensor:
         input_image_size = input_image_size.to(torch.float32)
         scale = longest_side / torch.max(input_image_size)
         transformed_size = scale * input_image_size
         transformed_size = torch.floor(transformed_size + 0.5).to(torch.int64)
         return transformed_size
 
-    def _embed_points(self, point_coords: torch.Tensor, point_labels: torch.Tensor) -> torch.Tensor:
+    def _embed_points(
+        self, point_coords: torch.Tensor, point_labels: torch.Tensor
+    ) -> torch.Tensor:
         point_coords = point_coords + 0.5
         point_coords = point_coords / self.img_size
         point_embedding = self.model.prompt_encoder.pe_layer._pe_encoding(point_coords)
         point_labels = point_labels.unsqueeze(-1).expand_as(point_embedding)
 
         point_embedding = point_embedding * (point_labels != -1)
-        point_embedding = point_embedding + self.model.prompt_encoder.not_a_point_embed.weight * (point_labels == -1)
+        point_embedding = (
+            point_embedding
+            + self.model.prompt_encoder.not_a_point_embed.weight * (point_labels == -1)
+        )
 
         for i in range(self.model.prompt_encoder.num_point_embeddings):
-            point_embedding = point_embedding + self.model.prompt_encoder.point_embeddings[i].weight * (
-                point_labels == i
+            point_embedding = (
+                point_embedding
+                + self.model.prompt_encoder.point_embeddings[i].weight
+                * (point_labels == i)
             )
 
         return point_embedding
 
-    def _embed_masks(self, input_mask: torch.Tensor, has_mask_input: torch.Tensor) -> torch.Tensor:
-        mask_embedding = has_mask_input * self.model.prompt_encoder.mask_downscaling(input_mask)
-        mask_embedding = mask_embedding + (1 - has_mask_input) * self.model.prompt_encoder.no_mask_embed.weight.reshape(
-            1, -1, 1, 1
+    def _embed_masks(
+        self, input_mask: torch.Tensor, has_mask_input: torch.Tensor
+    ) -> torch.Tensor:
+        mask_embedding = has_mask_input * self.model.prompt_encoder.mask_downscaling(
+            input_mask
         )
+        mask_embedding = mask_embedding + (
+            1 - has_mask_input
+        ) * self.model.prompt_encoder.no_mask_embed.weight.reshape(1, -1, 1, 1)
         return mask_embedding
 
-    def mask_postprocessing(self, masks: torch.Tensor, orig_im_size: torch.Tensor) -> torch.Tensor:
+    def mask_postprocessing(
+        self, masks: torch.Tensor, orig_im_size: torch.Tensor
+    ) -> torch.Tensor:
         masks = F.interpolate(
             masks,
             size=(self.img_size, self.img_size),
             mode="bilinear",
             align_corners=False,
         )
 
@@ -84,19 +99,20 @@
         h, w = orig_im_size[0], orig_im_size[1]
         masks = F.interpolate(masks, size=(h, w), mode="bilinear", align_corners=False)
         return masks
 
     def select_masks(
         self, masks: torch.Tensor, iou_preds: torch.Tensor, num_points: int
     ) -> Tuple[torch.Tensor, torch.Tensor]:
-        # Determine if we should return the multiclick mask or not from the number of points.
+        # Determine if we should return the multi click
+        # mask or not from the number of points.
         # The reweighting is used to avoid control flow.
-        score_reweight = torch.tensor([[1000] + [0] * (self.model.mask_decoder.num_mask_tokens - 1)]).to(
-            iou_preds.device
-        )
+        score_reweight = torch.tensor(
+            [[1000] + [0] * (self.model.mask_decoder.num_mask_tokens - 1)]
+        ).to(iou_preds.device)
         score = iou_preds + (num_points - 2.5) * score_reweight
         best_idx = torch.argmax(score, dim=1)
         masks = masks[torch.arange(masks.shape[0]), best_idx, :, :].unsqueeze(1)
         iou_preds = iou_preds[torch.arange(masks.shape[0]), best_idx].unsqueeze(1)
 
         return masks, iou_preds
 
@@ -117,15 +133,17 @@
             image_embeddings=image_embeddings,
             image_pe=self.model.prompt_encoder.get_dense_pe(),
             sparse_prompt_embeddings=sparse_embedding,
             dense_prompt_embeddings=dense_embedding,
         )
 
         if self.use_stability_score:
-            scores = calculate_stability_score(masks, self.model.mask_threshold, self.stability_score_offset)
+            scores = calculate_stability_score(
+                masks, self.model.mask_threshold, self.stability_score_offset
+            )
 
         if self.return_single_mask:
             masks, scores = self.select_masks(masks, scores, point_coords.shape[1])
 
         upscaled_masks = self.mask_postprocessing(masks, orig_im_size)
 
         if self.return_extra_metrics:
```

### Comparing `metaseg-0.7.5/metaseg/utils/transforms.py` & `metaseg-0.7.6/metaseg/utils/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,69 +23,89 @@
     def __init__(self, target_length: int) -> None:
         self.target_length = target_length
 
     def apply_image(self, image: np.ndarray) -> np.ndarray:
         """
         Expects a numpy array with shape HxWxC in uint8 format.
         """
-        target_size = self.get_preprocess_shape(image.shape[0], image.shape[1], self.target_length)
+        target_size = self.get_preprocess_shape(
+            image.shape[0], image.shape[1], self.target_length
+        )
         return np.array(resize(to_pil_image(image), target_size))
 
-    def apply_coords(self, coords: np.ndarray, original_size: Tuple[int, ...]) -> np.ndarray:
+    def apply_coords(
+        self, coords: np.ndarray, original_size: Tuple[int, ...]
+    ) -> np.ndarray:
         """
         Expects a numpy array of length 2 in the final dimension. Requires the
         original image size in (H, W) format.
         """
         old_h, old_w = original_size
-        new_h, new_w = self.get_preprocess_shape(original_size[0], original_size[1], self.target_length)
+        new_h, new_w = self.get_preprocess_shape(
+            original_size[0], original_size[1], self.target_length
+        )
         coords = deepcopy(coords).astype(float)
         coords[..., 0] = coords[..., 0] * (new_w / old_w)
         coords[..., 1] = coords[..., 1] * (new_h / old_h)
         return coords
 
-    def apply_boxes(self, boxes: np.ndarray, original_size: Tuple[int, ...]) -> np.ndarray:
+    def apply_boxes(
+        self, boxes: np.ndarray, original_size: Tuple[int, ...]
+    ) -> np.ndarray:
         """
         Expects a numpy array shape Bx4. Requires the original image size
         in (H, W) format.
         """
         boxes = self.apply_coords(boxes.reshape(-1, 2, 2), original_size)
         return boxes.reshape(-1, 4)
 
     def apply_image_torch(self, image: torch.Tensor) -> torch.Tensor:
         """
         Expects batched images with shape BxCxHxW and float format. This
         transformation may not exactly match apply_image. apply_image is
         the transformation expected by the model.
         """
         # Expects an image in BCHW format. May not exactly match apply_image.
-        target_size = self.get_preprocess_shape(image.shape[0], image.shape[1], self.target_length)
-        return F.interpolate(image, target_size, mode="bilinear", align_corners=False, antialias=True)
-
-    def apply_coords_torch(self, coords: torch.Tensor, original_size: Tuple[int, ...]) -> torch.Tensor:
+        target_size = self.get_preprocess_shape(
+            image.shape[0], image.shape[1], self.target_length
+        )
+        return F.interpolate(
+            image, target_size, mode="bilinear", align_corners=False, antialias=True
+        )
+
+    def apply_coords_torch(
+        self, coords: torch.Tensor, original_size: Tuple[int, ...]
+    ) -> torch.Tensor:
         """
         Expects a torch tensor with length 2 in the last dimension. Requires the
         original image size in (H, W) format.
         """
         old_h, old_w = original_size
-        new_h, new_w = self.get_preprocess_shape(original_size[0], original_size[1], self.target_length)
+        new_h, new_w = self.get_preprocess_shape(
+            original_size[0], original_size[1], self.target_length
+        )
         coords = deepcopy(coords).to(torch.float)
         coords[..., 0] = coords[..., 0] * (new_w / old_w)
         coords[..., 1] = coords[..., 1] * (new_h / old_h)
         return coords
 
-    def apply_boxes_torch(self, boxes: torch.Tensor, original_size: Tuple[int, ...]) -> torch.Tensor:
+    def apply_boxes_torch(
+        self, boxes: torch.Tensor, original_size: Tuple[int, ...]
+    ) -> torch.Tensor:
         """
         Expects a torch tensor with shape Bx4. Requires the original image
         size in (H, W) format.
         """
         boxes = self.apply_coords_torch(boxes.reshape(-1, 2, 2), original_size)
         return boxes.reshape(-1, 4)
 
     @staticmethod
-    def get_preprocess_shape(oldh: int, oldw: int, long_side_length: int) -> Tuple[int, int]:
+    def get_preprocess_shape(
+        oldh: int, oldw: int, long_side_length: int
+    ) -> Tuple[int, int]:
         """
         Compute the output size given input size and target long side length.
         """
         scale = long_side_length * 1.0 / max(oldh, oldw)
         newh, neww = oldh * scale, oldw * scale
         neww = int(neww + 0.5)
         newh = int(newh + 0.5)
```

### Comparing `metaseg-0.7.5/metaseg/webapp/app.py` & `metaseg-0.7.6/metaseg/webapp/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,20 @@
                             value=256,
                             label="Slice Width",
                         )
 
                     with gr.Row():
                         with gr.Column():
                             sahi_model_path = gr.Dropdown(
-                                choices=["yolov5l.pt", "yolov5l6.pt", "yolov8l.pt", "yolov8x.pt"],
+                                choices=[
+                                    "yolov5l.pt",
+                                    "yolov5l6.pt",
+                                    "yolov8l.pt",
+                                    "yolov8x.pt",
+                                ],
                                 value="yolov5l6.pt",
                                 label="Detector Model Path",
                             )
 
                             sahi_conf_th = gr.Slider(
                                 minimum=0,
                                 maximum=1,
```

### Comparing `metaseg-0.7.5/metaseg/webapp/demo.py` & `metaseg-0.7.6/metaseg/webapp/demo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-from metaseg import SahiAutoSegmentation, SegAutoMaskPredictor, SegManualMaskPredictor, sahi_sliced_predict
+from metaseg import (
+    SahiAutoSegmentation,
+    SegAutoMaskPredictor,
+    SegManualMaskPredictor,
+    sahi_sliced_predict,
+)
 
 # For image
 
 
-def automask_image_app(image_path, model_type, points_per_side, points_per_batch, min_area):
+def automask_image_app(
+    image_path, model_type, points_per_side, points_per_batch, min_area
+):
     SegAutoMaskPredictor().image_predict(
         source=image_path,
         model_type=model_type,  # vit_l, vit_h, vit_b
         points_per_side=points_per_side,
         points_per_batch=points_per_batch,
         min_area=min_area,
         output_path="output.png",
@@ -16,30 +23,40 @@
     )
     return "output.png"
 
 
 # For video
 
 
-def automask_video_app(video_path, model_type, points_per_side, points_per_batch, min_area):
+def automask_video_app(
+    video_path, model_type, points_per_side, points_per_batch, min_area
+):
     SegAutoMaskPredictor().video_predict(
         source=video_path,
         model_type=model_type,  # vit_l, vit_h, vit_b
         points_per_side=points_per_side,
         points_per_batch=points_per_batch,
         min_area=min_area,
         output_path="output.mp4",
     )
     return "output.mp4"
 
 
 # For manuel box and point selection
 
 
-def manual_app(image_path, model_type, input_point, input_label, input_box, multimask_output, random_color):
+def manual_app(
+    image_path,
+    model_type,
+    input_point,
+    input_label,
+    input_box,
+    multimask_output,
+    random_color,
+):
     SegManualMaskPredictor().image_predict(
         source=image_path,
         model_type=model_type,  # vit_l, vit_h, vit_b
         input_point=input_point,
         input_label=input_label,
         input_box=input_box,
         multimask_output=multimask_output,
@@ -64,15 +81,16 @@
     slice_height,
     slice_width,
     overlap_height_ratio,
     overlap_width_ratio,
 ):
     boxes = sahi_sliced_predict(
         image_path=image_path,
-        detection_model_type=detection_model_type,  # yolov8, detectron2, mmdetection, torchvision
+        # yolov8, detectron2, mmdetection, torchvision
+        detection_model_type=detection_model_type,
         detection_model_path=detection_model_path,
         conf_th=conf_th,
         image_size=image_size,
         slice_height=slice_height,
         slice_width=slice_width,
         overlap_height_ratio=overlap_height_ratio,
         overlap_width_ratio=overlap_width_ratio,
```

