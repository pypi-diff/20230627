# Comparing `tmp/controlnet_aux-0.0.5.tar.gz` & `tmp/controlnet_aux-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "controlnet_aux-0.0.5.tar", last modified: Fri May 26 09:48:40 2023, max compression
+gzip compressed data, was "controlnet_aux-0.0.6.tar", last modified: Tue Jun 27 19:53:08 2023, max compression
```

## Comparing `controlnet_aux-0.0.5.tar` & `controlnet_aux-0.0.6.tar`

### file list

```diff
@@ -1,181 +1,196 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    11357 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/LICENSE.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3287 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2336 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/README.md
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8777 2023-05-26 09:47:39.000000 controlnet_aux-0.0.5/setup.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.937408 controlnet_aux-0.0.5/src/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      515 2023-05-26 09:47:55.000000 controlnet_aux-0.0.5/src/controlnet_aux/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/canny/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      547 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/canny/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/hed/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7994 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/hed/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/lineart/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5293 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/lineart/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/lineart_anime/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7718 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/lineart_anime/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/mediapipe_face/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      645 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/mediapipe_face/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7118 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2992 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5276 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/api.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/base_model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9242 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/blocks.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3154 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/dpt_depth.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/midas_net.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/midas_net_custom.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/transforms.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    14625 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4582 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/midas/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2314 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9678 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9180 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    24134 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/mlsd/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2662 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      597 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/NNET.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:17.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2980 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/baseline.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:28.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10480 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/decoder.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:38.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2428 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5993 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       89 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3000 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3113 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9187 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4760 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      206 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4170 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2690 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2294 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4549 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3350 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12093 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    26514 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    59925 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2833 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15009 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      707 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       22 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2730 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5821 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2932 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      843 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4905 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1737 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1297 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6632 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1060 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/encoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5703 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/submodules.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/utils/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:29.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/utils/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7570 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/utils/losses.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6725 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/normalbae/utils/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6199 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10837 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/body.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15271 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/face.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6484 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/hand.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8743 2023-04-11 17:22:02.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7934 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/open_pose/util.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/pidi/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2978 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/pidi/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    21794 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/pidi/model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4430 2023-05-26 09:41:40.000000 controlnet_aux-0.0.5/src/controlnet_aux/processor.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2502 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15148 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/automatic_mask_generator.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2941 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/build_sam.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      385 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1479 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/common.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    14420 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/image_encoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6615 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/mask_decoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8594 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7226 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/sam.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8397 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/transformer.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    11664 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/predictor.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      197 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12712 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/amg.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5812 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/onnx.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3972 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/transforms.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/shuffle/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3468 2023-04-14 15:40:08.000000 controlnet_aux-0.0.5/src/controlnet_aux/shuffle/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3890 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/util.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2192 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15248 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    13757 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6909 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3436 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1045 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      333 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      931 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1576 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7284 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6899 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12792 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6099 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8552 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2390 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/builder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7362 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/depth_model.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1153 2023-05-22 19:47:00.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8693 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4838 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6733 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4163 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3438 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/model_io.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1270 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1587 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      556 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12630 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1276 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1968 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    16363 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      624 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    16310 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/config.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.945408 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/easydict/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3426 2023-04-20 08:19:12.000000 controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-26 09:48:40.941408 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3287 2023-05-26 09:48:40.000000 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8383 2023-05-26 09:48:40.000000 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-05-26 09:48:40.000000 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      120 2023-05-26 09:48:40.000000 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       15 2023-05-26 09:48:40.000000 controlnet_aux-0.0.5/src/controlnet_aux.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.315416 controlnet_aux-0.0.6/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11357 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/LICENSE.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4561 2023-06-27 19:53:08.315416 controlnet_aux-0.0.6/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3610 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/README.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-06-27 19:53:08.315416 controlnet_aux-0.0.6/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8777 2023-06-27 19:52:46.000000 controlnet_aux-0.0.6/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      548 2023-06-27 19:51:54.000000 controlnet_aux-0.0.6/src/controlnet_aux/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/canny/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1353 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/canny/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/hed/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5732 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/hed/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/leres/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4371 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/leres/leres/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6241 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/leres/Resnet.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8547 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/leres/Resnext_torch.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/leres/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    22911 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/leres/depthmap.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1122 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/leres/multi_depth_model_woauxi.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2029 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/leres/net_tools.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    16887 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/leres/network_auxi.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3095 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/models/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    10714 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/models/base_model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1660 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/models/base_model_hg.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    28960 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/models/networks.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7404 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/options/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      136 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/options/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9364 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/options/base_options.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1062 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/options/test_options.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/util/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       83 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/util/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3110 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/leres/pix2pix/util/util.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/lineart/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5805 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/lineart/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/lineart_anime/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8204 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/lineart_anime/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/mediapipe_face/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1944 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/mediapipe_face/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7118 2023-05-26 09:41:40.000000 controlnet_aux-0.0.6/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3581 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5276 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/api.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/base_model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9242 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/blocks.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3154 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/dpt_depth.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/midas_net.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/midas_net_custom.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/transforms.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    14625 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4582 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/midas/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/mlsd/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2816 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/mlsd/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/mlsd/models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/mlsd/models/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9678 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9180 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    24189 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/mlsd/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3647 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      597 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/NNET.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:17.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2980 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/baseline.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:28.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    10480 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/decoder.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:38.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2428 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5993 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      206 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4170 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2690 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2294 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4549 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3350 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12093 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    26514 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    59925 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2833 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15009 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      707 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       22 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2730 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5821 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2932 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      843 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4905 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1737 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1297 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6632 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1060 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/encoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5703 2023-04-14 15:40:08.000000 controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/submodules.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/open_pose/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9477 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/open_pose/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12915 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/open_pose/body.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    13491 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/open_pose/face.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3210 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/open_pose/hand.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8743 2023-04-11 17:22:02.000000 controlnet_aux-0.0.6/src/controlnet_aux/open_pose/model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    13737 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/open_pose/util.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/pidi/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3131 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/pidi/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    21813 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/pidi/model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6144 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/processor.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3357 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15148 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/automatic_mask_generator.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2941 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/build_sam.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      385 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1479 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/common.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    14420 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/image_encoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6615 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/mask_decoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8594 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7226 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/sam.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8397 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/transformer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11664 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/predictor.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/utils/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      197 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/utils/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12712 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/utils/amg.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5812 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/utils/onnx.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3972 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/utils/transforms.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/shuffle/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3330 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/shuffle/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5434 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/util.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2648 2023-06-27 19:48:39.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15248 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    13757 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.311416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6909 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3436 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1045 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      333 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      931 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1576 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7284 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6899 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12792 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6099 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8552 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2390 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/builder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7362 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/depth_model.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.315416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1153 2023-05-22 19:47:00.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8693 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4838 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6733 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4163 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3438 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/model_io.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.315416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1270 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1587 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      556 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12630 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.315416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1276 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1968 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    16363 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.315416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/utils/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/utils/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      624 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    16310 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/utils/config.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.315416 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/utils/easydict/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3426 2023-04-20 08:19:12.000000 controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:53:08.307416 controlnet_aux-0.0.6/src/controlnet_aux.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4561 2023-06-27 19:53:08.000000 controlnet_aux-0.0.6/src/controlnet_aux.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8788 2023-06-27 19:53:08.000000 controlnet_aux-0.0.6/src/controlnet_aux.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-06-27 19:53:08.000000 controlnet_aux-0.0.6/src/controlnet_aux.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      120 2023-06-27 19:53:08.000000 controlnet_aux-0.0.6/src/controlnet_aux.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       15 2023-06-27 19:53:08.000000 controlnet_aux-0.0.6/src/controlnet_aux.egg-info/top_level.txt
```

### Comparing `controlnet_aux-0.0.5/LICENSE.txt` & `controlnet_aux-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/PKG-INFO` & `controlnet_aux-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,57 @@
-Metadata-Version: 2.1
-Name: controlnet_aux
-Version: 0.0.5
-Summary: Auxillary models for controlnet
-Home-page: https://github.com/patrickvonplaten/controlnet_aux
-Author: The HuggingFace team
-Author-email: patrick@huggingface.co
-License: Apache
-Keywords: deep learning
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # ControlNet auxiliary models
 
 This is a PyPi installable package of [lllyasviel's ControlNet Annotators](https://github.com/lllyasviel/ControlNet/tree/main/annotator)
 
 The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
 All credit & copyright goes to https://github.com/lllyasviel .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.4
+pip install controlnet-aux==0.0.5
 ```
 
 ## Usage
 
+
+You can use the processor class, which can load each of the auxiliary models with the following code
+```python
+import requests
+from PIL import Image
+from io import BytesIO
+
+from controlnet_aux.processor import Processor
+
+# load image
+url = "https://huggingface.co/lllyasviel/sd-controlnet-openpose/resolve/main/images/pose.png"
+
+response = requests.get(url)
+img = Image.open(BytesIO(response.content)).convert("RGB").resize((512, 512))
+
+# load processor from processor_id
+# options are:
+# ["canny", "depth_leres", "depth_leres++", "depth_midas", "depth_zoe", "lineart_anime",
+#  "lineart_coarse", "lineart_realistic", "mediapipe_face", "mlsd", "normal_bae", "normal_midas",
+#  "openpose", "openpose_face", "openpose_faceonly", "openpose_full", "openpose_hand",
+#  "scribble_hed, "scribble_pidinet", "shuffle", "softedge_hed", "softedge_hedsafe",
+#  "softedge_pidinet", "softedge_pidsafe"]
+processor_id = 'scribble_hed'
+processor = Processor(processor_id)
+
+processed_image = processor(img, to_pil=True)
+```
+
+Each model can be loaded individually by importing and instantiating them as follows
 ```python
 from PIL import Image
 import requests
 from io import BytesIO
-from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector, ZoeDetector, MediapipeFaceDetector, SamDetector
+from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector, ZoeDetector, MediapipeFaceDetector, SamDetector, LeresDetector
 
 # load image
 url = "https://huggingface.co/lllyasviel/sd-controlnet-openpose/resolve/main/images/pose.png"
 
 response = requests.get(url)
 img = Image.open(BytesIO(response.content)).convert("RGB").resize((512, 512))
 
@@ -57,15 +61,16 @@
 mlsd = MLSDdetector.from_pretrained("lllyasviel/Annotators")
 open_pose = OpenposeDetector.from_pretrained("lllyasviel/Annotators")
 pidi = PidiNetDetector.from_pretrained("lllyasviel/Annotators")
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
 zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
-sam = SamDetector.from_pretrained("./weight_path")
+sam = SamDetector.from_pretrained("ybelkada/segment-anything", subfolder="checkpoints")
+leres = LeresDetector.from_pretrained("lllyasviel/Annotators")
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
 face_detector = MediapipeFaceDetector()
 
 
@@ -75,14 +80,14 @@
 processed_image_mlsd = mlsd(img)
 processed_image_open_pose = open_pose(img, hand_and_face=True)
 processed_image_pidi = pidi(img, safe=True)
 processed_image_normal_bae = normal_bae(img)
 processed_image_lineart = lineart(img, coarse=True)
 processed_image_lineart_anime = lineart_anime(img)
 processed_image_zoe = zoe(img)
+processed_image_sam = sam(img)
+processed_image_leres = leres(img)
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
 processed_image_mediapipe_face = face_detector(img)
 ```
-
-
```

### Comparing `controlnet_aux-0.0.5/setup.py` & `controlnet_aux-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     deps["torchvision"],
     deps["timm"],
     deps["scikit-image"],
 ]
 
 setup(
     name="controlnet_aux",
-    version="0.0.5",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    version="0.0.6",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
     description="Auxillary models for controlnet",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="patrick@huggingface.co",
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 from .hed import HEDdetector
+from .leres import LeresDetector
+from .lineart import LineartDetector
+from .lineart_anime import LineartAnimeDetector
 from .midas import MidasDetector
 from .mlsd import MLSDdetector
+from .normalbae import NormalBaeDetector
 from .open_pose import OpenposeDetector
 from .pidi import PidiNetDetector
-from .normalbae import NormalBaeDetector
-from .lineart import LineartDetector
-from .lineart_anime import LineartAnimeDetector
 from .zoe import ZoeDetector
 
 from .canny import CannyDetector
-from .shuffle import ContentShuffleDetector
 from .mediapipe_face import MediapipeFaceDetector
 from .segment_anything import SamDetector
+from .shuffle import ContentShuffleDetector
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/lineart/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/lineart/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
+import warnings
+
 import cv2
-import torch
 import numpy as np
-
-from huggingface_hub import hf_hub_download
+import torch
 import torch.nn as nn
 from einops import rearrange
+from huggingface_hub import hf_hub_download
 from PIL import Image
-from ..open_pose.util import HWC3, resize_image
 
+from ..util import HWC3, resize_image
 
 norm_layer = nn.InstanceNorm2d
 
 
 class ResidualBlock(nn.Module):
     def __init__(self, in_features):
         super(ResidualBlock, self).__init__()
@@ -88,20 +89,16 @@
         out = self.model4(out)
 
         return out
 
 
 class LineartDetector:
     def __init__(self, model, coarse_model):
-        self.model = model.eval()
-        self.model_coarse = coarse_model.eval()
-
-        if torch.cuda.is_available():
-            self.model.cuda()
-            self.model_coarse.cuda()
+        self.model = model
+        self.model_coarse = coarse_model
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, coarse_filename=None, cache_dir=None):
         filename = filename or "sk_model.pth"
         coarse_filename = coarse_filename or "sk_model2.pth"
 
         if os.path.isdir(pretrained_model_or_path):
@@ -109,21 +106,36 @@
             coarse_model_path = os.path.join(pretrained_model_or_path, coarse_filename)
         else:
             model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
             coarse_model_path = hf_hub_download(pretrained_model_or_path, coarse_filename, cache_dir=cache_dir)
 
         model = Generator(3, 1, 3)
         model.load_state_dict(torch.load(model_path, map_location=torch.device('cpu')))
+        model.eval()
 
         coarse_model = Generator(3, 1, 3)
         coarse_model.load_state_dict(torch.load(coarse_model_path, map_location=torch.device('cpu')))
+        coarse_model.eval()
 
         return cls(model, coarse_model)
+    
+    def to(self, device):
+        self.model.to(device)
+        self.model_coarse.to(device)
+        return self
+    
+    def __call__(self, input_image, coarse=False, detect_resolution=512, image_resolution=512, output_type="pil", **kwargs):
+        if "return_pil" in kwargs:
+            warnings.warn("return_pil is deprecated. Use output_type instead.", DeprecationWarning)
+            output_type = "pil" if kwargs["return_pil"] else "np"
+        if type(output_type) is bool:
+            warnings.warn("Passing `True` or `False` to `output_type` is deprecated and will raise an error in future versions")
+            if output_type:
+                output_type = "pil"
 
-    def __call__(self, input_image, coarse=False, detect_resolution=512, image_resolution=512, return_pil=True):
         device = next(iter(self.model.parameters())).device
         if not isinstance(input_image, np.ndarray):
             input_image = np.array(input_image, dtype=np.uint8)
 
         input_image = HWC3(input_image)
         input_image = resize_image(input_image, detect_resolution)
 
@@ -145,11 +157,11 @@
 
         img = resize_image(input_image, image_resolution)
         H, W, C = img.shape
 
         detected_map = cv2.resize(detected_map, (W, H), interpolation=cv2.INTER_LINEAR)
         detected_map = 255 - detected_map
         
-        if return_pil:
+        if output_type == "pil":
             detected_map = Image.fromarray(detected_map)
 
         return detected_map
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/lineart_anime/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/lineart_anime/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-import numpy as np
-import torch
-import torch.nn as nn
 import functools
-
 import os
+import warnings
+
 import cv2
+import numpy as np
+import torch
+import torch.nn as nn
 from einops import rearrange
-from PIL import Image
-from ..open_pose.util import HWC3, resize_image
 from huggingface_hub import hf_hub_download
+from PIL import Image
+
+from ..util import HWC3, resize_image
 
 
 class UnetGenerator(nn.Module):
     """Create a Unet-based generator"""
 
     def __init__(self, input_nc, output_nc, num_downs, ngf=64, norm_layer=nn.BatchNorm2d, use_dropout=False):
         """Construct a Unet generator
@@ -109,18 +111,15 @@
             return self.model(x)
         else:   # add skip connections
             return torch.cat([x, self.model(x)], 1)
 
 
 class LineartAnimeDetector:
     def __init__(self, model):
-        self.model = model.eval()
-
-        if torch.cuda.is_available():
-            self.model.cuda()
+        self.model = model
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         filename = filename or "netG.pth"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
@@ -131,18 +130,31 @@
         net = UnetGenerator(3, 1, 8, 64, norm_layer=norm_layer, use_dropout=False)
         ckpt = torch.load(model_path)
         for key in list(ckpt.keys()):
             if 'module.' in key:
                 ckpt[key.replace('module.', '')] = ckpt[key]
                 del ckpt[key]
         net.load_state_dict(ckpt)
+        net.eval()
 
         return cls(net)
 
-    def __call__(self, input_image, detect_resolution=512, image_resolution=512, return_pil=True):
+    def to(self, device):
+        self.model.to(device)
+        return self
+    
+    def __call__(self, input_image, detect_resolution=512, image_resolution=512, output_type="pil", **kwargs):
+        if "return_pil" in kwargs:
+            warnings.warn("return_pil is deprecated. Use output_type instead.", DeprecationWarning)
+            output_type = "pil" if kwargs["return_pil"] else "np"
+        if type(output_type) is bool:
+            warnings.warn("Passing `True` or `False` to `output_type` is deprecated and will raise an error in future versions")
+            if output_type:
+                output_type = "pil"
+
         device = next(iter(self.model.parameters())).device
         if not isinstance(input_image, np.ndarray):
             input_image = np.array(input_image, dtype=np.uint8)
 
         input_image = HWC3(input_image)
         input_image = resize_image(input_image, detect_resolution)
 
@@ -167,11 +179,11 @@
 
         img = resize_image(input_image, image_resolution)
         H, W, C = img.shape
 
         detected_map = cv2.resize(detected_map, (W, H), interpolation=cv2.INTER_LINEAR)
         detected_map = 255 - detected_map
         
-        if return_pil:
+        if output_type == "pil":
             detected_map = Image.fromarray(detected_map)
 
         return detected_map
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py` & `controlnet_aux-0.0.6/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/midas/api.py` & `controlnet_aux-0.0.6/src/controlnet_aux/midas/api.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/blocks.py` & `controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/dpt_depth.py` & `controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/midas_net.py` & `controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/midas_net_custom.py` & `controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/transforms.py` & `controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/midas/midas/vit.py` & `controlnet_aux-0.0.6/src/controlnet_aux/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/midas/utils.py` & `controlnet_aux-0.0.6/src/controlnet_aux/midas/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/mlsd/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/mlsd/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+import os
+import warnings
+
 import cv2
 import numpy as np
 import torch
-import os
-
 from huggingface_hub import hf_hub_download
-from .models.mbv2_mlsd_tiny import MobileV2_MLSD_Tiny
+from PIL import Image
+
+from ..util import HWC3, resize_image
 from .models.mbv2_mlsd_large import MobileV2_MLSD_Large
 from .utils import pred_lines
-from PIL import Image
-from ..open_pose.util import HWC3, resize_image
 
 
 class MLSDdetector:
     def __init__(self, model):
-        self.model = model.eval()
+        self.model = model
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         if pretrained_model_or_path == "lllyasviel/ControlNet":
             filename = filename or "annotator/ckpts/mlsd_large_512_fp32.pth"
         else:
             filename = filename or "mlsd_large_512_fp32.pth"
@@ -25,18 +26,31 @@
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
             model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         model = MobileV2_MLSD_Large()
         model.load_state_dict(torch.load(model_path), strict=True)
+        model.eval()
 
         return cls(model)
 
-    def __call__(self, input_image, thr_v=0.1, thr_d=0.1, detect_resolution=512, image_resolution=512, return_pil=True):
+    def to(self, device):
+        self.model.to(device)
+        return self
+    
+    def __call__(self, input_image, thr_v=0.1, thr_d=0.1, detect_resolution=512, image_resolution=512, output_type="pil", **kwargs):
+        if "return_pil" in kwargs:
+            warnings.warn("return_pil is deprecated. Use output_type instead.", DeprecationWarning)
+            output_type = "pil" if kwargs["return_pil"] else "np"
+        if type(output_type) is bool:
+            warnings.warn("Passing `True` or `False` to `output_type` is deprecated and will raise an error in future versions")
+            if output_type:
+                output_type = "pil"
+
         if not isinstance(input_image, np.ndarray):
             input_image = np.array(input_image, dtype=np.uint8)
 
         input_image = HWC3(input_image)
         input_image = resize_image(input_image, detect_resolution)
 
         assert input_image.ndim == 3
@@ -48,18 +62,18 @@
                 for line in lines:
                     x_start, y_start, x_end, y_end = [int(val) for val in line]
                     cv2.line(img_output, (x_start, y_start), (x_end, y_end), [255, 255, 255], 1)
         except Exception as e:
             pass
 
         detected_map = img_output[:, :, 0]
-
         detected_map = HWC3(detected_map)
+
         img = resize_image(input_image, image_resolution)
         H, W, C = img.shape
 
-        detected_map = cv2.resize(detected_map, (W, H), interpolation=cv2.INTER_NEAREST)
+        detected_map = cv2.resize(detected_map, (W, H), interpolation=cv2.INTER_LINEAR)
 
-        if return_pil:
+        if output_type == "pil":
             detected_map = Image.fromarray(detected_map)
 
         return detected_map
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py` & `controlnet_aux-0.0.6/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py` & `controlnet_aux-0.0.6/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/mlsd/utils.py` & `controlnet_aux-0.0.6/src/controlnet_aux/mlsd/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,22 +101,23 @@
                          'w_area': 1.86,
                          'w_center': 0.14}):
     '''
     shape = [height, width]
     '''
     h, w, _ = image.shape
     original_shape = [h, w]
+    device = next(iter(model.parameters())).device
 
     resized_image = np.concatenate([cv2.resize(image, (input_shape[0], input_shape[1]), interpolation=cv2.INTER_AREA),
                                     np.ones([input_shape[0], input_shape[1], 1])], axis=-1)
     resized_image = resized_image.transpose((2, 0, 1))
     batch_image = np.expand_dims(resized_image, axis=0).astype('float32')
     batch_image = (batch_image / 127.5) - 1.0
 
-    batch_image = torch.from_numpy(batch_image).float().cuda()
+    batch_image = torch.from_numpy(batch_image).float().to(device)
     outputs = model(batch_image)
 
     pts, pts_score, vmap = deccode_output_score_and_ptss(outputs, 200, 3)
     start = vmap[:, :, :2]  # (x, y)
     end = vmap[:, :, 2:]  # (x, y)
     dist_map = np.sqrt(np.sum((start - end) ** 2, axis=-1))
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/NNET.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/NNET.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/baseline.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/baseline.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/decoder.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/encoder.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/normalbae/nets/submodules/submodules.py` & `controlnet_aux-0.0.6/src/controlnet_aux/normalbae/nets/submodules/submodules.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/open_pose/body.py` & `controlnet_aux-0.0.6/src/controlnet_aux/open_pose/body.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,89 @@
+import math
+from typing import List, NamedTuple, Union
+
 import cv2
+import matplotlib.pyplot as plt
 import numpy as np
-import math
-import time
-from scipy.ndimage.filters import gaussian_filter
 import torch
+from scipy.ndimage.filters import gaussian_filter
 
 from . import util
 from .model import bodypose_model
 
+
+class Keypoint(NamedTuple):
+    x: float
+    y: float
+    score: float = 1.0
+    id: int = -1
+
+
+class BodyResult(NamedTuple):
+    # Note: Using `Union` instead of `|` operator as the ladder is a Python
+    # 3.10 feature.
+    # Annotator code should be Python 3.8 Compatible, as controlnet repo uses
+    # Python 3.8 environment.
+    # https://github.com/lllyasviel/ControlNet/blob/d3284fcd0972c510635a4f5abe2eeb71dc0de524/environment.yaml#L6
+    keypoints: List[Union[Keypoint, None]]
+    total_score: float
+    total_parts: int
+
+
 class Body(object):
-    def __init__(self, model_path, device):
-        self.device = device
+    def __init__(self, model_path):
         self.model = bodypose_model()
         model_dict = util.transfer(self.model, torch.load(model_path))
         self.model.load_state_dict(model_dict)
-        self.model.to(self.device)
         self.model.eval()
 
+    def to(self, device):
+        self.model.to(device)
+        return self
+
     def __call__(self, oriImg):
+        device = next(iter(self.model.parameters())).device
         # scale_search = [0.5, 1.0, 1.5, 2.0]
         scale_search = [0.5]
         boxsize = 368
         stride = 8
         padValue = 128
         thre1 = 0.1
         thre2 = 0.05
         multiplier = [x * boxsize / oriImg.shape[0] for x in scale_search]
         heatmap_avg = np.zeros((oriImg.shape[0], oriImg.shape[1], 19))
         paf_avg = np.zeros((oriImg.shape[0], oriImg.shape[1], 38))
 
         for m in range(len(multiplier)):
             scale = multiplier[m]
-            imageToTest = cv2.resize(oriImg, (0, 0), fx=scale, fy=scale, interpolation=cv2.INTER_CUBIC)
+            imageToTest = util.smart_resize_k(oriImg, fx=scale, fy=scale)
             imageToTest_padded, pad = util.padRightDownCorner(imageToTest, stride, padValue)
             im = np.transpose(np.float32(imageToTest_padded[:, :, :, np.newaxis]), (3, 2, 0, 1)) / 256 - 0.5
             im = np.ascontiguousarray(im)
 
             data = torch.from_numpy(im).float()
-            data = data.to(self.device)
+            data = data.to(device)
             # data = data.permute([2, 0, 1]).unsqueeze(0).float()
             with torch.no_grad():
                 Mconv7_stage6_L1, Mconv7_stage6_L2 = self.model(data)
             Mconv7_stage6_L1 = Mconv7_stage6_L1.cpu().numpy()
             Mconv7_stage6_L2 = Mconv7_stage6_L2.cpu().numpy()
 
             # extract outputs, resize, and remove padding
             # heatmap = np.transpose(np.squeeze(net.blobs[output_blobs.keys()[1]].data), (1, 2, 0))  # output 1 is heatmaps
             heatmap = np.transpose(np.squeeze(Mconv7_stage6_L2), (1, 2, 0))  # output 1 is heatmaps
-            heatmap = cv2.resize(heatmap, (0, 0), fx=stride, fy=stride, interpolation=cv2.INTER_CUBIC)
+            heatmap = util.smart_resize_k(heatmap, fx=stride, fy=stride)
             heatmap = heatmap[:imageToTest_padded.shape[0] - pad[2], :imageToTest_padded.shape[1] - pad[3], :]
-            heatmap = cv2.resize(heatmap, (oriImg.shape[1], oriImg.shape[0]), interpolation=cv2.INTER_CUBIC)
+            heatmap = util.smart_resize(heatmap, (oriImg.shape[0], oriImg.shape[1]))
 
             # paf = np.transpose(np.squeeze(net.blobs[output_blobs.keys()[0]].data), (1, 2, 0))  # output 0 is PAFs
             paf = np.transpose(np.squeeze(Mconv7_stage6_L1), (1, 2, 0))  # output 0 is PAFs
-            paf = cv2.resize(paf, (0, 0), fx=stride, fy=stride, interpolation=cv2.INTER_CUBIC)
+            paf = util.smart_resize_k(paf, fx=stride, fy=stride)
             paf = paf[:imageToTest_padded.shape[0] - pad[2], :imageToTest_padded.shape[1] - pad[3], :]
-            paf = cv2.resize(paf, (oriImg.shape[1], oriImg.shape[0]), interpolation=cv2.INTER_CUBIC)
+            paf = util.smart_resize(paf, (oriImg.shape[0], oriImg.shape[1]))
 
             heatmap_avg += heatmap_avg + heatmap / len(multiplier)
             paf_avg += + paf / len(multiplier)
 
         all_peaks = []
         peak_counter = 0
 
@@ -198,17 +222,56 @@
             if subset[i][-1] < 4 or subset[i][-2] / subset[i][-1] < 0.4:
                 deleteIdx.append(i)
         subset = np.delete(subset, deleteIdx, axis=0)
 
         # subset: n*20 array, 0-17 is the index in candidate, 18 is the total score, 19 is the total parts
         # candidate: x, y, score, id
         return candidate, subset
+    
+    @staticmethod
+    def format_body_result(candidate: np.ndarray, subset: np.ndarray) -> List[BodyResult]:
+        """
+        Format the body results from the candidate and subset arrays into a list of BodyResult objects.
+        
+        Args:
+            candidate (np.ndarray): An array of candidates containing the x, y coordinates, score, and id
+                for each body part.
+            subset (np.ndarray): An array of subsets containing indices to the candidate array for each
+                person detected. The last two columns of each row hold the total score and total parts
+                of the person.
+
+        Returns:
+            List[BodyResult]: A list of BodyResult objects, where each object represents a person with
+                detected keypoints, total score, and total parts.
+        """
+        return [
+            BodyResult(
+                keypoints=[
+                    Keypoint(
+                        x=candidate[candidate_index][0],
+                        y=candidate[candidate_index][1],
+                        score=candidate[candidate_index][2],
+                        id=candidate[candidate_index][3]
+                    ) if candidate_index != -1 else None
+                    for candidate_index in person[:18].astype(int)
+                ],
+                total_score=person[18],
+                total_parts=person[19]
+            )
+            for person in subset
+        ]
+    
 
 if __name__ == "__main__":
     body_estimation = Body('../model/body_pose_model.pth')
 
     test_image = '../images/ski.jpg'
     oriImg = cv2.imread(test_image)  # B,G,R order
     candidate, subset = body_estimation(oriImg)
-    canvas = util.draw_bodypose(oriImg, candidate, subset)
+    bodies = body_estimation.format_body_result(candidate, subset)
+
+    canvas = oriImg
+    for body in bodies:
+        canvas = util.draw_bodypose(canvas, body)
+        
     plt.imshow(canvas[:, :, [2, 1, 0]])
     plt.show()
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/open_pose/face.py` & `controlnet_aux-0.0.6/src/controlnet_aux/open_pose/face.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
+
 import numpy as np
-from torchvision.transforms import ToTensor, ToPILImage
 import torch
 import torch.nn.functional as F
-import cv2
+from torch.nn import Conv2d, MaxPool2d, Module, ReLU, init
+from torchvision.transforms import ToPILImage, ToTensor
 
 from . import util
-from torch.nn import Conv2d, Module, ReLU, MaxPool2d, init
 
 
 class FaceNet(Module):
     """Model the cascading heatmaps. """
     def __init__(self):
         super(FaceNet, self).__init__()
         # cnn to make feature map
@@ -310,33 +310,37 @@
     Args:
         inference_size: set the size of the inference image size, suggested:
             368, 736, 1312, default 736
         gaussian_sigma: blur the heatmaps, default 2.5
         heatmap_peak_thresh: return landmark if over threshold, default 0.1
 
     """
-    def __init__(self, face_model_path, device,
+    def __init__(self, face_model_path,
                  inference_size=None,
                  gaussian_sigma=None,
                  heatmap_peak_thresh=None):
-        self.device = device
         self.inference_size = inference_size or params["inference_img_size"]
         self.sigma = gaussian_sigma or params['gaussian_sigma']
         self.threshold = heatmap_peak_thresh or params["heatmap_peak_thresh"]
         self.model = FaceNet()
         self.model.load_state_dict(torch.load(face_model_path))
-        self.model.to(self.device)
         self.model.eval()
 
+    def to(self, device):
+        self.model.to(device)
+        return self
+
     def __call__(self, face_img):
+        device = next(iter(self.model.parameters())).device
         H, W, C = face_img.shape
 
         w_size = 384
         x_data = torch.from_numpy(util.smart_resize(face_img, (w_size, w_size))).permute([2, 0, 1]) / 256.0 - 0.5
-        x_data = x_data.to(self.device)
+
+        x_data = x_data.to(device)
 
         with torch.no_grad():
             hs = self.model(x_data[None, ...])
             heatmaps = F.interpolate(
                 hs[-1],
                 (H, W),
                 mode='bilinear', align_corners=True).cpu().numpy()[0]
@@ -353,79 +357,8 @@
 
             positions = np.where(binary > 0.5)
             intensities = map_ori[positions]
             mi = np.argmax(intensities)
             y, x = positions[0][mi], positions[1][mi]
             all_peaks.append([x, y])
 
-        return np.array(all_peaks)
-
-
-# Written by Lvmin
-def faceDetect(candidate, subset, oriImg):
-    # left right eye ear 14 15 16 17
-    detect_result = []
-    image_height, image_width = oriImg.shape[0:2]
-    for person in subset.astype(int):
-        has_head = person[0] > -1
-        if not has_head:
-            continue
-
-        has_left_eye = person[14] > -1
-        has_right_eye = person[15] > -1
-        has_left_ear = person[16] > -1
-        has_right_ear = person[17] > -1
-
-        if not (has_left_eye or has_right_eye or has_left_ear or has_right_ear):
-            continue
-
-        head, left_eye, right_eye, left_ear, right_ear = person[[0, 14, 15, 16, 17]]
-
-        width = 0.0
-        x0, y0 = candidate[head][:2]
-
-        if has_left_eye:
-            x1, y1 = candidate[left_eye][:2]
-            d = max(abs(x0 - x1), abs(y0 - y1))
-            width = max(width, d * 3.0)
-
-        if has_right_eye:
-            x1, y1 = candidate[right_eye][:2]
-            d = max(abs(x0 - x1), abs(y0 - y1))
-            width = max(width, d * 3.0)
-
-        if has_left_ear:
-            x1, y1 = candidate[left_ear][:2]
-            d = max(abs(x0 - x1), abs(y0 - y1))
-            width = max(width, d * 1.5)
-
-        if has_right_ear:
-            x1, y1 = candidate[right_ear][:2]
-            d = max(abs(x0 - x1), abs(y0 - y1))
-            width = max(width, d * 1.5)
-
-        x, y = x0, y0
-
-        x -= width
-        y -= width
-
-        if x < 0:
-            x = 0
-
-        if y < 0:
-            y = 0
-
-        width1 = width * 2
-        width2 = width * 2
-
-        if x + width > image_width:
-            width1 = image_width - x
-
-        if y + width > image_height:
-            width2 = image_height - y
-
-        width = min(width1, width2)
-
-        if width >= 20:
-            detect_result.append([int(x), int(y), int(width)])
-
-    return detect_result
+        return np.array(all_peaks)
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/open_pose/model.py` & `controlnet_aux-0.0.6/src/controlnet_aux/open_pose/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/pidi/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/pidi/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
-import torch
+import warnings
+
+import cv2
 import numpy as np
+import torch
 from einops import rearrange
-import cv2
 from huggingface_hub import hf_hub_download
-from .model import pidinet
-from ..open_pose.util import HWC3, resize_image
-from ..util import safe_step
 from PIL import Image
 
+from ..util import HWC3, nms, resize_image, safe_step
+from .model import pidinet
+
 
 class PidiNetDetector:
     def __init__(self, netNetwork):
         self.netNetwork = netNetwork
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
@@ -25,62 +27,58 @@
 
         netNetwork = pidinet()
         netNetwork.load_state_dict({k.replace('module.', ''): v for k, v in torch.load(model_path)['state_dict'].items()})
         netNetwork.eval()
 
         return cls(netNetwork)
 
-    def __call__(self, input_image, detect_resolution=512, image_resolution=512, safe=False, return_pil=True, scribble=False):
+    def to(self, device):
+        self.netNetwork.to(device)
+        return self
+    
+    def __call__(self, input_image, detect_resolution=512, image_resolution=512, safe=False, output_type="pil", scribble=False, apply_filter=False, **kwargs):
+        if "return_pil" in kwargs:
+            warnings.warn("return_pil is deprecated. Use output_type instead.", DeprecationWarning)
+            output_type = "pil" if kwargs["return_pil"] else "np"
+        if type(output_type) is bool:
+            warnings.warn("Passing `True` or `False` to `output_type` is deprecated and will raise an error in future versions")
+            if output_type:
+                output_type = "pil"
+
+        device = next(iter(self.netNetwork.parameters())).device
         if not isinstance(input_image, np.ndarray):
             input_image = np.array(input_image, dtype=np.uint8)
 
         input_image = HWC3(input_image)
         input_image = resize_image(input_image, detect_resolution)
         assert input_image.ndim == 3
         input_image = input_image[:, :, ::-1].copy()
         with torch.no_grad():
-            image_pidi = torch.from_numpy(input_image).float()
+            image_pidi = torch.from_numpy(input_image).float().to(device)
             image_pidi = image_pidi / 255.0
             image_pidi = rearrange(image_pidi, 'h w c -> 1 c h w')
             edge = self.netNetwork(image_pidi)[-1]
             edge = edge.cpu().numpy()
+            if apply_filter:
+                edge = edge > 0.5 
             if safe:
                 edge = safe_step(edge)
             edge = (edge * 255.0).clip(0, 255).astype(np.uint8)
 
         detected_map = edge[0, 0]
-
         detected_map = HWC3(detected_map)
 
         img = resize_image(input_image, image_resolution)
         H, W, C = img.shape
 
         detected_map = cv2.resize(detected_map, (W, H), interpolation=cv2.INTER_LINEAR)
         
         if scribble:
             detected_map = nms(detected_map, 127, 3.0)
             detected_map = cv2.GaussianBlur(detected_map, (0, 0), 3.0)
             detected_map[detected_map > 4] = 255
             detected_map[detected_map < 255] = 0
 
-        if return_pil:
+        if output_type == "pil":
             detected_map = Image.fromarray(detected_map)
 
         return detected_map
-
-
-def nms(x, t, s):
-    x = cv2.GaussianBlur(x.astype(np.float32), (0, 0), s)
-
-    f1 = np.array([[0, 0, 0], [1, 1, 1], [0, 0, 0]], dtype=np.uint8)
-    f2 = np.array([[0, 1, 0], [0, 1, 0], [0, 1, 0]], dtype=np.uint8)
-    f3 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]], dtype=np.uint8)
-    f4 = np.array([[0, 0, 1], [0, 1, 0], [1, 0, 0]], dtype=np.uint8)
-
-    y = np.zeros_like(x)
-
-    for f in [f1, f2, f3, f4]:
-        np.putmask(y, cv2.dilate(x, kernel=f) == x, x)
-
-    z = np.zeros_like(y, dtype=np.uint8)
-    z[y > t] = 255
-    return z
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/pidi/model.py` & `controlnet_aux-0.0.6/src/controlnet_aux/pidi/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,15 @@
             assert weights.size(2) == 3 and weights.size(3) == 3, 'kernel size for rd_conv should be 3x3'
             padding = 2 * dilation
 
             shape = weights.shape
             if weights.is_cuda:
                 buffer = torch.cuda.FloatTensor(shape[0], shape[1], 5 * 5).fill_(0)
             else:
-                buffer = torch.zeros(shape[0], shape[1], 5 * 5)
+                buffer = torch.zeros(shape[0], shape[1], 5 * 5).to(weights.device)
             weights = weights.view(shape[0], shape[1], -1)
             buffer[:, :, [0, 2, 4, 10, 14, 20, 22, 24]] = weights[:, :, 1:]
             buffer[:, :, [6, 7, 8, 11, 13, 16, 17, 18]] = -weights[:, :, 1:]
             buffer[:, :, 12] = 0
             buffer = buffer.view(shape[0], shape[1], 5, 5)
             y = F.conv2d(x, buffer, bias, stride=stride, padding=padding, dilation=dilation, groups=groups)
             return y
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/processor.py` & `controlnet_aux-0.0.6/src/controlnet_aux/processor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,145 @@
 """
 This file contains a Processor that can be used to process images with controlnet aux processors
 """
 import io
-from typing import Union
+import logging
+from typing import Dict, Optional, Union
 
 from PIL import Image
-import numpy as np
-import torch
-from controlnet_aux import (HEDdetector,
-                            MidasDetector,
-                            MLSDdetector,
-                            OpenposeDetector,
-                            PidiNetDetector,
-                            NormalBaeDetector,
-                            LineartDetector,
-                            LineartAnimeDetector,
-                            CannyDetector,
-                            ContentShuffleDetector,
-                            ZoeDetector,
-                            MediapipeFaceDetector)
+
+from controlnet_aux import (CannyDetector, ContentShuffleDetector, HEDdetector,
+                            LeresDetector, LineartAnimeDetector,
+                            LineartDetector, MediapipeFaceDetector,
+                            MidasDetector, MLSDdetector, NormalBaeDetector,
+                            OpenposeDetector, PidiNetDetector, ZoeDetector)
+
+LOGGER = logging.getLogger(__name__)
 
 
 MODELS = {
     # checkpoint models
-    'hed': {'class': HEDdetector, 'checkpoint': True},
-    'midas': {'class': MidasDetector, 'checkpoint': True},
+    'scribble_hed': {'class': HEDdetector, 'checkpoint': True},
+    'softedge_hed': {'class': HEDdetector, 'checkpoint': True},
+    'scribble_hedsafe': {'class': HEDdetector, 'checkpoint': True},
+    'softedge_hedsafe': {'class': HEDdetector, 'checkpoint': True},
+    'depth_midas': {'class': MidasDetector, 'checkpoint': True},
     'mlsd': {'class': MLSDdetector, 'checkpoint': True},
     'openpose': {'class': OpenposeDetector, 'checkpoint': True},
-    'pidinet': {'class': PidiNetDetector, 'checkpoint': True},
-    'normalbae': {'class': NormalBaeDetector, 'checkpoint': True},
-    'lineart': {'class': LineartDetector, 'checkpoint': True},
+    'openpose_face': {'class': OpenposeDetector, 'checkpoint': True},
+    'openpose_faceonly': {'class': OpenposeDetector, 'checkpoint': True},
+    'openpose_full': {'class': OpenposeDetector, 'checkpoint': True},
+    'openpose_hand': {'class': OpenposeDetector, 'checkpoint': True},
+    'scribble_pidinet': {'class': PidiNetDetector, 'checkpoint': True},
+    'softedge_pidinet': {'class': PidiNetDetector, 'checkpoint': True},
+    'scribble_pidsafe': {'class': PidiNetDetector, 'checkpoint': True},
+    'softedge_pidsafe': {'class': PidiNetDetector, 'checkpoint': True},
+    'normal_bae': {'class': NormalBaeDetector, 'checkpoint': True},
     'lineart_coarse': {'class': LineartDetector, 'checkpoint': True},
+    'lineart_realistic': {'class': LineartDetector, 'checkpoint': True},
     'lineart_anime': {'class': LineartAnimeDetector, 'checkpoint': True},
-    'zoe': {'class': ZoeDetector, 'checkpoint': True}, 
+    'depth_zoe': {'class': ZoeDetector, 'checkpoint': True}, 
+    'depth_leres': {'class': LeresDetector, 'checkpoint': True}, 
+    'depth_leres++': {'class': LeresDetector, 'checkpoint': True}, 
     # instantiate
-    'content_shuffle': {'class': ContentShuffleDetector, 'checkpoint': False},
+    'shuffle': {'class': ContentShuffleDetector, 'checkpoint': False},
     'mediapipe_face': {'class': MediapipeFaceDetector, 'checkpoint': False},
     'canny': {'class': CannyDetector, 'checkpoint': False},
 }
 
-# @patrickvonplaten, I can change this so people can pass their own parameters
-# but for my use case I'm using this Dictionary
+
 MODEL_PARAMS = {
-    'hed': {'resize': False},
-    'midas': {'resize': 512},
-    'mlsd': {'resize': False},
-    'openpose': {'resize': False, 'hand_and_face': True},
-    'pidinet': {'resize': False, 'safe': True},
-    'normalbae': {'resize': False},
-    'lineart': {'resize': False, 'coarse': True},
-    'lineart_coarse': {'resize': False, 'coarse': True},
-    'lineart_anime': {'resize': False},
-    'canny': {'resize': False},
-    'content_shuffle': {'resize': False},
-    'zoe': {'resize': False},
-    'mediapipe_face': {'resize': False},
+    'scribble_hed': {'scribble': True},
+    'softedge_hed': {'scribble': False},
+    'scribble_hedsafe': {'scribble': True, 'safe': True},
+    'softedge_hedsafe': {'scribble': False, 'safe': True},
+    'depth_midas': {},
+    'mlsd': {},
+    'openpose': {'include_body': True, 'include_hand': False, 'include_face': False},
+    'openpose_face': {'include_body': True, 'include_hand': False, 'include_face': True},
+    'openpose_faceonly': {'include_body': False, 'include_hand': False, 'include_face': True},
+    'openpose_full': {'include_body': True, 'include_hand': True, 'include_face': True},
+    'openpose_hand': {'include_body': False, 'include_hand': True, 'include_face': False},
+    'scribble_pidinet': {'safe': False, 'scribble': True},
+    'softedge_pidinet': {'safe': False, 'scribble': False},
+    'scribble_pidsafe': {'safe': True, 'scribble': True},
+    'softedge_pidsafe': {'safe': True, 'scribble': False},
+    'normal_bae': {},
+    'lineart_realistic': {'coarse': False},
+    'lineart_coarse': {'coarse': True},
+    'lineart_anime': {},
+    'canny': {},
+    'shuffle': {},
+    'depth_zoe': {},
+    'depth_leres': {'boost': False},
+    'depth_leres++': {'boost': True},
+    'mediapipe_face': {},
 }
 
+CHOICES = f"Choices for the processor are {list(MODELS.keys())}"
+
 
 class Processor:
-    def __init__(self, processor_id: str) -> 'Processor':
+    def __init__(self, processor_id: str, params: Optional[Dict] = None) -> None:
         """Processor that can be used to process images with controlnet aux processors
 
         Args:
-            processor_id (str): processor name
-
-        Returns:
-            Processor: Processor object
+            processor_id (str): processor name, options are 'hed, midas, mlsd, openpose,
+                                pidinet, normalbae, lineart, lineart_coarse, lineart_anime,
+                                canny, content_shuffle, zoe, mediapipe_face
+            params (Optional[Dict]): parameters for the processor
         """
-        print(f"Loading {processor_id} processor")
+        LOGGER.info("Loading %s".format(processor_id))
+
+        if processor_id not in MODELS:
+            raise ValueError(f"{processor_id} is not a valid processor id. Please make sure to choose one of {', '.join(MODELS.keys())}")
+
         self.processor_id = processor_id
         self.processor = self.load_processor(self.processor_id)
+
+        # load default params
         self.params = MODEL_PARAMS[self.processor_id]
-        self.resize = self.params.pop('resize', False)
-        if self.resize:
-            # print warning: image will be resized
-            print(f"Warning: {self.processor_id} will resize image to {self.resize}x{self.resize}")
+        # update with user params
+        if params:
+            self.params.update(params)
 
-    def load_processor(self, processor_id: str):
+    def load_processor(self, processor_id: str) -> 'Processor':
         """Load controlnet aux processors
 
         Args:
             processor_id (str): processor name
+
+        Returns:
+            Processor: controlnet aux processor
         """
         processor = MODELS[processor_id]['class']
 
+        # check if the proecssor is a checkpoint model
         if MODELS[processor_id]['checkpoint']:
             processor = processor.from_pretrained("lllyasviel/Annotators")
         else:
             processor = processor()
         return processor
 
     def __call__(self, image: Union[Image.Image, bytes],
-                 to_bytes: bool = True) -> Union[Image.Image, bytes]:
+                 to_pil: bool = True) -> Union[Image.Image, bytes]:
         """processes an image with a controlnet aux processor
 
         Args:
             image (Union[Image.Image, bytes]): input image in bytes or PIL Image
-            to_bytes (bool): whether to return bytes or PIL Image
+            to_pil (bool): whether to return bytes or PIL Image
 
         Returns:
             Union[Image.Image, bytes]: processed image in bytes or PIL Image
         """
         # check if bytes or PIL Image
         if isinstance(image, bytes):
             image = Image.open(io.BytesIO(image)).convert("RGB")
 
-        if self.resize:
-            image = image.resize((self.resize, self.resize))
-
         processed_image = self.processor(image, **self.params)
 
-        if to_bytes:
+        if to_pil:
+            return processed_image
+        else:
             output_bytes = io.BytesIO()
             processed_image.save(output_bytes, format='JPEG')
             return output_bytes.getvalue()
-        else:
-            return processed_image
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
+
 import os
-from PIL import Image
+import warnings
+from typing import Union
+
+import cv2
 import numpy as np
 import torch
-import gc
-
 from huggingface_hub import hf_hub_download
+from PIL import Image
 
-from .build_sam import (
-    build_sam,
-    build_sam_vit_h,
-    build_sam_vit_l,
-    build_sam_vit_b,
-    sam_model_registry,
-)
-from .predictor import SamPredictor
+from ..util import HWC3, resize_image
 from .automatic_mask_generator import SamAutomaticMaskGenerator
+from .build_sam import sam_model_registry
 
 
 class SamDetector:
     def __init__(self, mask_generator: SamAutomaticMaskGenerator):
         self.mask_generator = mask_generator
     
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, model_type="vit_h", filename="sam_vit_h_4b8939.pth", cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, model_type="vit_h", filename="sam_vit_h_4b8939.pth", subfolder=None, cache_dir=None):
         """
         Possible model_type : vit_h, vit_l, vit_b
         download weights from https://github.com/facebookresearch/segment-anything
         """
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)  
+            model_path = hf_hub_download(pretrained_model_or_path, filename, subfolder=subfolder, cache_dir=cache_dir)  
         
         sam = sam_model_registry[model_type](checkpoint=model_path)
         
         if torch.cuda.is_available():
             sam.to("cuda")
         
         mask_generator = SamAutomaticMaskGenerator(sam)
@@ -56,21 +53,40 @@
         for ann in sorted_anns:
             m = ann['segmentation']
             img = np.empty((m.shape[0], m.shape[1], 3), dtype=np.uint8)
             for i in range(3):
                 img[:,:,i] = np.random.randint(255, dtype=np.uint8)
             final_img.paste(Image.fromarray(img, mode="RGB"), (0, 0), Image.fromarray(np.uint8(m*255)))
         
-        return final_img
+        return np.array(final_img, dtype=np.uint8)
 
-    def __call__(self, image: Image.Image) -> Image.Image:
-        # Generate Masks
-        if isinstance(image, Image.Image):
-            image = np.array(image)
+    def __call__(self, input_image: Union[np.ndarray, Image.Image]=None, detect_resolution=512, image_resolution=512, output_type="pil", **kwargs) -> Image.Image:
+        if "image" in kwargs:
+            warnings.warn("image is deprecated, please use `input_image=...` instead.", DeprecationWarning)
+            input_image = kwargs.pop("image")
+        
+        if input_image is None:
+            raise ValueError("input_image must be defined.")
 
-        masks = self.mask_generator.generate(image)
-        torch.cuda.empty_cache()
+        if not isinstance(input_image, np.ndarray):
+            input_image = np.array(input_image, dtype=np.uint8)
+        
+        input_image = HWC3(input_image)
+        input_image = resize_image(input_image, detect_resolution)
+
+        # Generate Masks
+        masks = self.mask_generator.generate(input_image)
         # Create map
         map = self.show_anns(masks)
-        del masks
-        gc.collect()
-        return map
+
+        detected_map = map
+        detected_map = HWC3(detected_map)
+
+        img = resize_image(input_image, image_resolution)
+        H, W, C = img.shape
+
+        detected_map = cv2.resize(detected_map, (W, H), interpolation=cv2.INTER_LINEAR)
+        
+        if output_type == "pil":
+            detected_map = Image.fromarray(detected_map)
+
+        return detected_map
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/automatic_mask_generator.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/build_sam.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/common.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/image_encoder.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/mask_decoder.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/sam.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/modeling/transformer.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/predictor.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/amg.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/onnx.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/segment_anything/utils/transforms.py` & `controlnet_aux-0.0.6/src/controlnet_aux/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/shuffle/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/shuffle/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-import random
+import warnings
 
 import cv2
 import numpy as np
 from PIL import Image
-from ..open_pose.util import HWC3, resize_image
+
+from ..util import HWC3, img2mask, make_noise_disk, resize_image
 
 
 class ContentShuffleDetector:
-    def __call__(self, input_image, h=None, w=None, f=None, detect_resolution=512, image_resolution=512, return_pil=True):
+    def __call__(self, input_image, h=None, w=None, f=None, detect_resolution=512, image_resolution=512, output_type="pil", **kwargs):
+        if "return_pil" in kwargs:
+            warnings.warn("return_pil is deprecated. Use output_type instead.", DeprecationWarning)
+            output_type = "pil" if kwargs["return_pil"] else "np"
+        if type(output_type) is bool:
+            warnings.warn("Passing `True` or `False` to `output_type` is deprecated and will raise an error in future versions")
+            if output_type:
+                output_type = "pil"
 
         if not isinstance(input_image, np.ndarray):
             input_image = np.array(input_image, dtype=np.uint8)
 
         input_image = HWC3(input_image)
         input_image = resize_image(input_image, detect_resolution)
 
@@ -21,28 +29,31 @@
         if w is None:
             w = W
         if f is None:
             f = 256
         x = make_noise_disk(h, w, 1, f) * float(W - 1)
         y = make_noise_disk(h, w, 1, f) * float(H - 1)
         flow = np.concatenate([x, y], axis=2).astype(np.float32)
-        image = cv2.remap(input_image, flow, None, cv2.INTER_LINEAR)
+        detected_map = cv2.remap(input_image, flow, None, cv2.INTER_LINEAR)
+
+        img = resize_image(input_image, image_resolution)
+        H, W, C = img.shape
 
-        img = resize_image(image, image_resolution)
+        detected_map = cv2.resize(detected_map, (W, H), interpolation=cv2.INTER_LINEAR)
 
-        if return_pil:
-            image = Image.fromarray(image)
+        if output_type == "pil":
+            detected_map = Image.fromarray(detected_map)
 
-        return image
+        return detected_map
 
 
 class ColorShuffleDetector:
     def __call__(self, img):
         H, W, C = img.shape
-        F = random.randint(64, 384)
+        F = np.random.randint(64, 384)
         A = make_noise_disk(H, W, 3, F)
         B = make_noise_disk(H, W, 3, F)
         C = (A + B) / 2.0
         A = (C + (A - C) * 3.0).clip(0, 1)
         B = (C + (B - C) * 3.0).clip(0, 1)
         L = img.astype(np.float32) / 255.0
         Y = A * L + B * (1 - L)
@@ -83,35 +94,7 @@
     def __init__(self, resolution=(640, 512)):
         self.H, self.W = resolution
 
     def __call__(self, img):
         m = img2mask(img, self.H, self.W)
         m *= 255.0
         return m.clip(0, 255).astype(np.uint8)
-
-
-def make_noise_disk(H, W, C, F):
-    noise = np.random.uniform(low=0, high=1, size=((H // F) + 2, (W // F) + 2, C))
-    noise = cv2.resize(noise, (W + 2 * F, H + 2 * F), interpolation=cv2.INTER_CUBIC)
-    noise = noise[F: F + H, F: F + W]
-    noise -= np.min(noise)
-    noise /= np.max(noise)
-    if C == 1:
-        noise = noise[:, :, None]
-    return noise
-
-
-def img2mask(img, H, W, low=10, high=90):
-    assert img.ndim == 3 or img.ndim == 2
-    assert img.dtype == np.uint8
-
-    if img.ndim == 3:
-        y = img[:, :, random.randrange(0, img.shape[2])]
-    else:
-        y = img
-
-    y = cv2.resize(y, (W, H), interpolation=cv2.INTER_CUBIC)
-
-    if random.uniform(0, 1) < 0.5:
-        y = 255 - y
-
-    return y < np.percentile(y, random.randrange(low, high))
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,79 @@
 import os
+
 import cv2
 import numpy as np
-from PIL import Image
 import torch
-
-from huggingface_hub import hf_hub_download
 from einops import rearrange
+from huggingface_hub import hf_hub_download
+from PIL import Image
+
+from ..util import HWC3, resize_image
 from .zoedepth.models.zoedepth.zoedepth_v1 import ZoeDepth
 from .zoedepth.utils.config import get_config
-from ..util import HWC3
+
 
 class ZoeDetector:
     def __init__(self, model):
-        self.model = model.eval()
-        if torch.cuda.is_available():
-            self.model = self.model.cuda()
-            self.model.device = 'cuda'
+        self.model = model
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         filename = filename or "ZoeD_M12_N.pt"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
             model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
             
         conf = get_config("zoedepth", "infer")
         model = ZoeDepth.build_from_config(conf)
         model.load_state_dict(torch.load(model_path, map_location=torch.device('cpu'))['model'])
+        model.eval()
 
         return cls(model)
 
-    def __call__(self, input_image):
-        input_type = "np"
-        if isinstance(input_image, Image.Image):
-            input_image = np.array(input_image)
-            input_type = "pil"
-
+    def to(self, device):
+        self.model.to(device)
+        return self
+    
+    def __call__(self, input_image, detect_resolution=512, image_resolution=512, output_type=None):
+        device = next(iter(self.model.parameters())).device
+        if not isinstance(input_image, np.ndarray):
+            input_image = np.array(input_image, dtype=np.uint8)
+            output_type = output_type or "pil"
+        else:
+            output_type = output_type or "np"
+        
         input_image = HWC3(input_image)
+        input_image = resize_image(input_image, detect_resolution)
+
+        assert input_image.ndim == 3
         image_depth = input_image
         with torch.no_grad():
-            image_depth = torch.from_numpy(image_depth).float()
-            if torch.cuda.is_available():
-                image_depth = image_depth.cuda()
+            image_depth = torch.from_numpy(image_depth).float().to(device)
             image_depth = image_depth / 255.0
             image_depth = rearrange(image_depth, 'h w c -> 1 c h w')
             depth = self.model.infer(image_depth)
 
             depth = depth[0, 0].cpu().numpy()
 
             vmin = np.percentile(depth, 2)
             vmax = np.percentile(depth, 85)
 
             depth -= vmin
             depth /= vmax - vmin
             depth = 1.0 - depth
             depth_image = (depth * 255.0).clip(0, 255).astype(np.uint8)
 
-        if input_type == "pil":
-            depth_image = Image.fromarray(depth_image)
-            depth_image = depth_image.convert("RGB")
-
-        return depth_image
+        detected_map = depth_image
+        detected_map = HWC3(detected_map)      
+         
+        img = resize_image(input_image, image_resolution)
+        H, W, C = img.shape
+
+        detected_map = cv2.resize(detected_map, (W, H), interpolation=cv2.INTER_LINEAR)
+        
+        if output_type == "pil":
+            detected_map = Image.fromarray(detected_map)
+            
+        return detected_map
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/builder.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/depth_model.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/depth_model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/model_io.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/model_io.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/config.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/utils/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py` & `controlnet_aux-0.0.6/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux.egg-info/PKG-INFO` & `controlnet_aux-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: controlnet-aux
-Version: 0.0.5
+Name: controlnet_aux
+Version: 0.0.6
 Summary: Auxillary models for controlnet
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
@@ -30,24 +30,53 @@
 The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
 All credit & copyright goes to https://github.com/lllyasviel .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.4
+pip install controlnet-aux==0.0.5
 ```
 
 ## Usage
 
+
+You can use the processor class, which can load each of the auxiliary models with the following code
+```python
+import requests
+from PIL import Image
+from io import BytesIO
+
+from controlnet_aux.processor import Processor
+
+# load image
+url = "https://huggingface.co/lllyasviel/sd-controlnet-openpose/resolve/main/images/pose.png"
+
+response = requests.get(url)
+img = Image.open(BytesIO(response.content)).convert("RGB").resize((512, 512))
+
+# load processor from processor_id
+# options are:
+# ["canny", "depth_leres", "depth_leres++", "depth_midas", "depth_zoe", "lineart_anime",
+#  "lineart_coarse", "lineart_realistic", "mediapipe_face", "mlsd", "normal_bae", "normal_midas",
+#  "openpose", "openpose_face", "openpose_faceonly", "openpose_full", "openpose_hand",
+#  "scribble_hed, "scribble_pidinet", "shuffle", "softedge_hed", "softedge_hedsafe",
+#  "softedge_pidinet", "softedge_pidsafe"]
+processor_id = 'scribble_hed'
+processor = Processor(processor_id)
+
+processed_image = processor(img, to_pil=True)
+```
+
+Each model can be loaded individually by importing and instantiating them as follows
 ```python
 from PIL import Image
 import requests
 from io import BytesIO
-from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector, ZoeDetector, MediapipeFaceDetector, SamDetector
+from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector, ZoeDetector, MediapipeFaceDetector, SamDetector, LeresDetector
 
 # load image
 url = "https://huggingface.co/lllyasviel/sd-controlnet-openpose/resolve/main/images/pose.png"
 
 response = requests.get(url)
 img = Image.open(BytesIO(response.content)).convert("RGB").resize((512, 512))
 
@@ -57,15 +86,16 @@
 mlsd = MLSDdetector.from_pretrained("lllyasviel/Annotators")
 open_pose = OpenposeDetector.from_pretrained("lllyasviel/Annotators")
 pidi = PidiNetDetector.from_pretrained("lllyasviel/Annotators")
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
 zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
-sam = SamDetector.from_pretrained("./weight_path")
+sam = SamDetector.from_pretrained("ybelkada/segment-anything", subfolder="checkpoints")
+leres = LeresDetector.from_pretrained("lllyasviel/Annotators")
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
 face_detector = MediapipeFaceDetector()
 
 
@@ -75,14 +105,16 @@
 processed_image_mlsd = mlsd(img)
 processed_image_open_pose = open_pose(img, hand_and_face=True)
 processed_image_pidi = pidi(img, safe=True)
 processed_image_normal_bae = normal_bae(img)
 processed_image_lineart = lineart(img, coarse=True)
 processed_image_lineart_anime = lineart_anime(img)
 processed_image_zoe = zoe(img)
+processed_image_sam = sam(img)
+processed_image_leres = leres(img)
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
 processed_image_mediapipe_face = face_detector(img)
 ```
```

### Comparing `controlnet_aux-0.0.5/src/controlnet_aux.egg-info/SOURCES.txt` & `controlnet_aux-0.0.6/src/controlnet_aux.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,33 @@
 src/controlnet_aux.egg-info/PKG-INFO
 src/controlnet_aux.egg-info/SOURCES.txt
 src/controlnet_aux.egg-info/dependency_links.txt
 src/controlnet_aux.egg-info/requires.txt
 src/controlnet_aux.egg-info/top_level.txt
 src/controlnet_aux/canny/__init__.py
 src/controlnet_aux/hed/__init__.py
+src/controlnet_aux/leres/__init__.py
+src/controlnet_aux/leres/leres/Resnet.py
+src/controlnet_aux/leres/leres/Resnext_torch.py
+src/controlnet_aux/leres/leres/__init__.py
+src/controlnet_aux/leres/leres/depthmap.py
+src/controlnet_aux/leres/leres/multi_depth_model_woauxi.py
+src/controlnet_aux/leres/leres/net_tools.py
+src/controlnet_aux/leres/leres/network_auxi.py
+src/controlnet_aux/leres/pix2pix/__init__.py
+src/controlnet_aux/leres/pix2pix/models/__init__.py
+src/controlnet_aux/leres/pix2pix/models/base_model.py
+src/controlnet_aux/leres/pix2pix/models/base_model_hg.py
+src/controlnet_aux/leres/pix2pix/models/networks.py
+src/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py
+src/controlnet_aux/leres/pix2pix/options/__init__.py
+src/controlnet_aux/leres/pix2pix/options/base_options.py
+src/controlnet_aux/leres/pix2pix/options/test_options.py
+src/controlnet_aux/leres/pix2pix/util/__init__.py
+src/controlnet_aux/leres/pix2pix/util/util.py
 src/controlnet_aux/lineart/__init__.py
 src/controlnet_aux/lineart_anime/__init__.py
 src/controlnet_aux/mediapipe_face/__init__.py
 src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
 src/controlnet_aux/midas/__init__.py
 src/controlnet_aux/midas/api.py
 src/controlnet_aux/midas/utils.py
@@ -46,35 +65,27 @@
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
-src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/__init__.py
-src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py
-src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py
-src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py
-src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
 src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
-src/controlnet_aux/normalbae/utils/__init__.py
-src/controlnet_aux/normalbae/utils/losses.py
-src/controlnet_aux/normalbae/utils/utils.py
 src/controlnet_aux/open_pose/__init__.py
 src/controlnet_aux/open_pose/body.py
 src/controlnet_aux/open_pose/face.py
 src/controlnet_aux/open_pose/hand.py
 src/controlnet_aux/open_pose/model.py
 src/controlnet_aux/open_pose/util.py
 src/controlnet_aux/pidi/__init__.py
```

