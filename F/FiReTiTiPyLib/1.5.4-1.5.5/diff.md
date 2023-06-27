# Comparing `tmp/FiReTiTiPyLib-1.5.4.tar.gz` & `tmp/FiReTiTiPyLib-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiReTiTiPyLib-1.5.4.tar", last modified: Tue May 16 18:44:13 2023, max compression
+gzip compressed data, was "FiReTiTiPyLib-1.5.5.tar", last modified: Tue Jun 27 18:00:41 2023, max compression
```

## Comparing `FiReTiTiPyLib-1.5.4.tar` & `FiReTiTiPyLib-1.5.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.938201 FiReTiTiPyLib-1.5.4/
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.909472 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.913098 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/
--rw-r--r--   0 firetiti   (501) staff       (20)    17914 2022-08-03 21:19:30.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_JavaInterfacer.py
--rw-r--r--   0 firetiti   (501) staff       (20)     3812 2022-09-27 18:24:16.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_MarkersExclusiveness.py
--rwxrwxrwx   0 firetiti   (501) staff       (20)    18871 2023-05-16 18:40:45.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_Registration.py
--rw-r--r--   0 firetiti   (501) staff       (20)      732 2021-07-08 18:41:36.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_Utils.py
--rw-r--r--   0 firetiti   (501) staff       (20)        1 2021-09-17 15:36:01.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)    14803 2022-08-08 22:26:45.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Evaluations.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.918174 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/
--rw-r--r--   0 firetiti   (501) staff       (20)    10215 2023-03-29 22:50:57.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Datasets.py
--rw-r--r--   0 firetiti   (501) staff       (20)     9876 2022-10-04 22:11:12.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Denoiser.py
--rw-r--r--   0 firetiti   (501) staff       (20)    10045 2023-03-29 22:52:23.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations copie.py
--rw-r--r--   0 firetiti   (501) staff       (20)    11378 2022-08-04 06:45:51.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations.py
--rw-r--r--   0 firetiti   (501) staff       (20)     7372 2022-07-06 23:57:34.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Losses.py
--rw-r--r--   0 firetiti   (501) staff       (20)     1534 2019-11-02 07:53:49.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Schedulers.py
--rw-r--r--   0 firetiti   (501) staff       (20)    33168 2022-07-19 19:11:17.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Segmentator.py
--rw-r--r--   0 firetiti   (501) staff       (20)      358 2022-07-17 08:41:02.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Transformations.py
--rw-r--r--   0 firetiti   (501) staff       (20)    10581 2022-05-06 19:56:26.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/Segmentation_Datasets.py
--rw-r--r--   0 firetiti   (501) staff       (20)      660 2022-08-08 19:41:02.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.919178 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Graphics/
--rw-r--r--   0 firetiti   (501) staff       (20)     7242 2022-10-25 08:02:30.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Graphics/Graphics.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-10-22 06:51:36.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Graphics/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.920026 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/IO/
--rw-r--r--   0 firetiti   (501) staff       (20)      218 2022-07-07 20:25:41.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/IO/IOColors.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-07-07 20:24:41.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/IO/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)    48611 2021-09-19 21:40:03.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/ImageDataGenerator.py
--rw-r--r--   0 firetiti   (501) staff       (20)     1686 2023-03-25 03:02:08.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/ImageTools.py
--rw-r--r--   0 firetiti   (501) staff       (20)    16489 2023-05-15 18:15:00.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/ImagesIO.py
--rw-r--r--   0 firetiti   (501) staff       (20)     3964 2021-09-19 21:40:24.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Metrics.py
--rw-r--r--   0 firetiti   (501) staff       (20)     8885 2022-07-20 07:25:42.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Normalizers.py
--rw-r--r--   0 firetiti   (501) staff       (20)      418 2019-10-10 23:12:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Processing.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.920931 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.922570 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/
--rw-r--r--   0 firetiti   (501) staff       (20)     9202 2021-09-19 21:46:32.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/Attentions.py
--rw-r--r--   0 firetiti   (501) staff       (20)    10798 2020-10-01 00:31:32.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/NonLocalBlock.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.926461 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)    19971 2022-05-06 19:38:51.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/blocks.py
--rw-r--r--   0 firetiti   (501) staff       (20)    16797 2022-05-06 19:38:51.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/ceecnet.py
--rw-r--r--   0 firetiti   (501) staff       (20)     4706 2022-05-06 19:39:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/head.py
--rw-r--r--   0 firetiti   (501) staff       (20)     2434 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/loss.py
--rw-r--r--   0 firetiti   (501) staff       (20)     3000 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/utils.py
--rw-r--r--   0 firetiti   (501) staff       (20)     5900 2023-01-19 23:42:50.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CoCo.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.930020 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)     6671 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/losses.py
--rw-r--r--   0 firetiti   (501) staff       (20)    13047 2022-07-20 18:25:21.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/main.py
--rw-r--r--   0 firetiti   (501) staff       (20)     4802 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/mask_gen.py
--rw-r--r--   0 firetiti   (501) staff       (20)      390 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/metrics.py
--rw-r--r--   0 firetiti   (501) staff       (20)     5006 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/smallunet.py
--rw-r--r--   0 firetiti   (501) staff       (20)      746 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/utils.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.931410 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/
--rw-r--r--   0 firetiti   (501) staff       (20)     3386 2022-07-27 08:46:54.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/Denoising.py
--rw-r--r--   0 firetiti   (501) staff       (20)     4934 2022-07-02 09:22:02.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/NRRN.py
--rw-r--r--   0 firetiti   (501) staff       (20)      715 2022-07-27 08:35:58.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.932998 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/
--rw-r--r--   0 firetiti   (501) staff       (20)    21854 2023-04-14 16:18:56.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN.py
--rw-r--r--   0 firetiti   (501) staff       (20)    10192 2020-08-25 21:18:24.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN_Utils.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.933959 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/ResUnetA/
--rw-r--r--   0 firetiti   (501) staff       (20)    24635 2021-09-19 21:19:22.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/ResUnetA/ResUnetA.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 21:18:29.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/ResUnetA/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.934842 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/SegNet/
--rw-r--r--   0 firetiti   (501) staff       (20)     4974 2019-02-11 00:12:15.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/SegNet/SegNet.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/SegNet/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.935772 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/U-Net/
--rw-r--r--   0 firetiti   (501) staff       (20)    14940 2021-09-19 21:23:45.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/U-Net/UNet.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/U-Net/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)     1032 2022-08-08 19:48:59.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.937044 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/
--rw-r--r--   0 firetiti   (501) staff       (20)    23945 2021-09-20 07:02:02.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/ApiTests.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:55:38.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)     1896 2023-03-25 07:44:55.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/test_ImageTools.py
--rw-r--r--   0 firetiti   (501) staff       (20)     2849 2022-07-09 22:24:02.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tools.py
--rw-r--r--   0 firetiti   (501) staff       (20)    16078 2022-07-17 08:40:20.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Transformations.py
--rw-r--r--   0 firetiti   (501) staff       (20)       49 2023-05-15 20:29:08.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.911065 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/
--rw-r--r--   0 firetiti   (501) staff       (20)     1588 2023-05-16 18:44:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/PKG-INFO
--rw-r--r--   0 firetiti   (501) staff       (20)     3123 2023-05-16 18:44:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/SOURCES.txt
--rw-r--r--   0 firetiti   (501) staff       (20)        1 2023-05-16 18:44:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/dependency_links.txt
--rw-r--r--   0 firetiti   (501) staff       (20)      422 2023-05-16 18:44:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/requires.txt
--rw-r--r--   0 firetiti   (501) staff       (20)       14 2023-05-16 18:44:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/top_level.txt
--rw-r--r--   0 firetiti   (501) staff       (20)     1588 2023-05-16 18:44:13.937734 FiReTiTiPyLib-1.5.4/PKG-INFO
--rw-r--r--   0 firetiti   (501) staff       (20)       38 2023-05-16 18:44:13.938404 FiReTiTiPyLib-1.5.4/setup.cfg
--rw-r--r--   0 firetiti   (501) staff       (20)     2934 2023-05-16 18:41:29.000000 FiReTiTiPyLib-1.5.4/setup.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.583639 FiReTiTiPyLib-1.5.5/
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.539932 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.545442 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/CyclicIF/
+-rw-r--r--   0 firetiti   (501) staff       (20)    17914 2022-08-03 21:19:30.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/CyclicIF/CyclicIF_JavaInterfacer.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     3812 2022-09-27 18:24:16.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/CyclicIF/CyclicIF_MarkersExclusiveness.py
+-rwxrwxrwx   0 firetiti   (501) staff       (20)    19239 2023-06-27 17:56:01.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/CyclicIF/CyclicIF_Registration.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      732 2021-07-08 18:41:36.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/CyclicIF/CyclicIF_Utils.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        1 2021-09-17 15:36:01.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/CyclicIF/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    14803 2022-08-08 22:26:45.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Evaluations.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.553971 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/
+-rw-r--r--   0 firetiti   (501) staff       (20)    10215 2023-03-29 22:50:57.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Datasets.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     9876 2022-10-04 22:11:12.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Denoiser.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    10045 2023-03-29 22:52:23.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations copie.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    11378 2022-08-04 06:45:51.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     7372 2022-07-06 23:57:34.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Losses.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     1534 2019-11-02 07:53:49.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Schedulers.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    33168 2022-07-19 19:11:17.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Segmentator.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      358 2022-07-17 08:41:02.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Transformations.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    10581 2022-05-06 19:56:26.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/Segmentation_Datasets.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      660 2022-08-08 19:41:02.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.555583 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Graphics/
+-rw-r--r--   0 firetiti   (501) staff       (20)     7242 2022-10-25 08:02:30.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Graphics/Graphics.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-10-22 06:51:36.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Graphics/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.556816 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/IO/
+-rw-r--r--   0 firetiti   (501) staff       (20)      218 2022-07-07 20:25:41.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/IO/IOColors.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-07-07 20:24:41.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/IO/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    48611 2021-09-19 21:40:03.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/ImageDataGenerator.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     1686 2023-03-25 03:02:08.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/ImageTools.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    16489 2023-05-15 18:15:00.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/ImagesIO.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     3964 2021-09-19 21:40:24.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Metrics.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     8885 2022-07-20 07:25:42.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Normalizers.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      418 2019-10-10 23:12:13.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Processing.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.557985 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.560531 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Attentions/
+-rw-r--r--   0 firetiti   (501) staff       (20)     9202 2021-09-19 21:46:32.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Attentions/Attentions.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    10798 2020-10-01 00:31:32.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Attentions/NonLocalBlock.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Attentions/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.565471 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    19971 2022-05-06 19:38:51.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/blocks.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    16797 2022-05-06 19:38:51.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/ceecnet.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     4706 2022-05-06 19:39:13.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/head.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     2434 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/loss.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     3000 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/utils.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     5900 2023-01-19 23:42:50.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CoCo.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.571591 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     6671 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/losses.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    13047 2022-07-20 18:25:21.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/main.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     4802 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/mask_gen.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      390 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/metrics.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     5006 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/smallunet.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      746 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/utils.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.574111 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Denoising/
+-rw-r--r--   0 firetiti   (501) staff       (20)     3386 2022-07-27 08:46:54.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Denoising/Denoising.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     4934 2022-07-02 09:22:02.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Denoising/NRRN.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      715 2022-07-27 08:35:58.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Denoising/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.577000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/
+-rw-r--r--   0 firetiti   (501) staff       (20)    21854 2023-04-14 16:18:56.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    10192 2020-08-25 21:18:24.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN_Utils.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.578753 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/ResUnetA/
+-rw-r--r--   0 firetiti   (501) staff       (20)    24635 2021-09-19 21:19:22.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/ResUnetA/ResUnetA.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 21:18:29.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/ResUnetA/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.579773 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/SegNet/
+-rw-r--r--   0 firetiti   (501) staff       (20)     4974 2019-02-11 00:12:15.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/SegNet/SegNet.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/SegNet/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.580791 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/U-Net/
+-rw-r--r--   0 firetiti   (501) staff       (20)    14940 2021-09-19 21:23:45.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/U-Net/UNet.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/U-Net/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     1032 2022-08-08 19:48:59.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.582565 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Tests/
+-rw-r--r--   0 firetiti   (501) staff       (20)    23945 2021-09-20 07:02:02.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Tests/ApiTests.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:55:38.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Tests/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     1896 2023-03-25 07:44:55.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Tests/test_ImageTools.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     2849 2022-07-09 22:24:02.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Tools.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    16078 2022-07-17 08:40:20.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Transformations.py
+-rw-r--r--   0 firetiti   (501) staff       (20)       49 2023-06-27 16:20:03.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-06-27 18:00:41.542390 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib.egg-info/
+-rw-r--r--   0 firetiti   (501) staff       (20)     1588 2023-06-27 18:00:40.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib.egg-info/PKG-INFO
+-rw-r--r--   0 firetiti   (501) staff       (20)     3123 2023-06-27 18:00:41.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib.egg-info/SOURCES.txt
+-rw-r--r--   0 firetiti   (501) staff       (20)        1 2023-06-27 18:00:40.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib.egg-info/dependency_links.txt
+-rw-r--r--   0 firetiti   (501) staff       (20)      422 2023-06-27 18:00:41.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib.egg-info/requires.txt
+-rw-r--r--   0 firetiti   (501) staff       (20)       14 2023-06-27 18:00:41.000000 FiReTiTiPyLib-1.5.5/FiReTiTiPyLib.egg-info/top_level.txt
+-rw-r--r--   0 firetiti   (501) staff       (20)     1588 2023-06-27 18:00:41.583176 FiReTiTiPyLib-1.5.5/PKG-INFO
+-rw-r--r--   0 firetiti   (501) staff       (20)       38 2023-06-27 18:00:41.583793 FiReTiTiPyLib-1.5.5/setup.cfg
+-rw-r--r--   0 firetiti   (501) staff       (20)     2934 2023-05-16 18:41:29.000000 FiReTiTiPyLib-1.5.5/setup.py
```

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_JavaInterfacer.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/CyclicIF/CyclicIF_JavaInterfacer.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_MarkersExclusiveness.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/CyclicIF/CyclicIF_MarkersExclusiveness.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_Registration.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/CyclicIF/CyclicIF_Registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import sys
 import time
 
 import cv2
 import numpy as np
 import psutil
 import scipy
-import skimage
 import skimage.morphology as mm
 import skimage.registration as skReg
 
 from natsort import humansorted
 from skimage.transform import warp
 
 import FiReTiTiPyLib.CyclicIF.CyclicIF_Utils as utils
@@ -22,28 +21,30 @@
 
 class CyclicIF_Registration:
 	""" This class performs the registration for cyclic immunofluoresence images.
 		Code inspired from https://learnopencv.com/feature-based-image-alignment-using-opencv-c-python/
 	"""
 
 	def __init__(self, MaxFeatures: int=2013, Reverse: bool=True, SaveImages: bool=True, Copyright: str=None,
-						Debug: bool=False, MonitorMemory: bool=False):
+						Debug: bool=False, MonitorMemory: bool=False, HistogramCutoff: float=0.95):
 		""" Simple init.
 		:param MaxFeatures: Maximum number of features to extract.
 		:param Reverse: If True the last round is used as reference, otherwise the first.
 		:param SaveImages: Save the images after registration? Useful for debuging.
 		:param Debug: Run using debeging mode?
-		:param SkipTransformation: If True, the transformations are not performed.
+		:param MonitorMemory: If True, the memory information are display between important operations.
+		:param HistogramCutoff: The histogram percentage cutoff value.
 		"""
 		self.MaxFeatures = MaxFeatures
 		self.Reverse = Reverse
 		self.SaveImages = SaveImages
 		self.Copyright = Copyright
 		self.Debug = Debug
 		self.MonitorMemory = MonitorMemory
+		self.HistogramCutoff = HistogramCutoff
 
 		#self.Safety = 32760
 		self.Warning = 46300
 		
 		self.MatrixSafety = 0.017
 		self.MatrixDiagSafety = 0.023
 
@@ -352,29 +353,38 @@
 		sys.stdout.flush()
 		
 		channel, height, width = image.shape
 		#if self.Safety < channel or self.Safety < height or self.Safety < width:
 		#	raise Exception("Image too big. Max accepted = " + str(self.Safety))
 		
 		if self.Warning <= channel or self.Warning <= height or self.Warning <= width:
-			print("WARNING - Not recommended to register such big images as the processing will likely generate an "
-					+ "error with Java if the number of pixels is higher than 2^31. "
-					+ "Max recommended = " + str(self.Warning), file=sys.stderr)
+			print("WARNING - Very big images might generate an error with Java if the number of pixels is bigger than "
+					+ "2^31. Max recommended = " + str(self.Warning) + "x" + str(self.Warning), file=sys.stderr)
 			sys.stderr.flush()
 		
 		if raw:
 			return image
 
-		#print("Image [%d,%d]" % (image.min(), image.max()))
 		if preprocess:
+			hist, _ = np.histogram(image, bins=65535, range=(1, 65536))
+			histsum = hist.sum()
+			
+			MaxIndex = 1
+			cutoff = float(hist[MaxIndex]) / histsum
+			while cutoff < self.HistogramCutoff:
+				MaxIndex += 1
+				if 0 < hist[MaxIndex]:
+					cutoff += float(hist[MaxIndex]) / histsum
+			
 			min = image.min()
-			A = 65535.0 / (image.max() - min)
+			A = 65535.0 / (MaxIndex - min)
 			B = -A * min
 			image = image * A + B
-
+			image[65535 < image] = 65535
+		
 		image /= 65535.0
 		image *= 255.0
 		#return np.uint8(image.squeeze())
 		return mm.white_tophat(np.uint8(image.squeeze()), mm.square(113))
```

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_Utils.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/CyclicIF/CyclicIF_Utils.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Evaluations.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Evaluations.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Datasets.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Datasets.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Denoiser.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Denoiser.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations copie.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations copie.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Losses.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Losses.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Schedulers.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Schedulers.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Segmentator.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Segmentator.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/Segmentation_Datasets.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/Segmentation_Datasets.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/__init__.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/FiReTiTiPyTorchLib/__init__.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Graphics/Graphics.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Graphics/Graphics.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/ImageDataGenerator.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/ImageDataGenerator.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/ImageTools.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/ImageTools.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/ImagesIO.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/ImagesIO.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Metrics.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Metrics.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Normalizers.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Normalizers.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/Attentions.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Attentions/Attentions.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/NonLocalBlock.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Attentions/NonLocalBlock.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/blocks.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/blocks.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/ceecnet.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/ceecnet.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/head.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/head.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/loss.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/loss.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/utils.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CEECNET/utils.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CoCo.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CoCo.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/losses.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/losses.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/main.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/main.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/mask_gen.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/mask_gen.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/smallunet.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/smallunet.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/utils.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/utils.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/Denoising.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Denoising/Denoising.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/NRRN.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Denoising/NRRN.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/__init__.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/Denoising/__init__.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN_Utils.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN_Utils.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/ResUnetA/ResUnetA.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/ResUnetA/ResUnetA.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/SegNet/SegNet.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/SegNet/SegNet.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/U-Net/UNet.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/U-Net/UNet.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/__init__.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/PyTorch_Models/__init__.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/ApiTests.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Tests/ApiTests.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/test_ImageTools.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Tests/test_ImageTools.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tools.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Tools.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Transformations.py` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib/Transformations.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/PKG-INFO` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FiReTiTiPyLib
-Version: 1.5.4
+Version: 1.5.5
 Summary: Python libraries used as support/tools.
-Download-URL: https://www.thibault.biz/Doc/FiReTiTiPyLib/FiReTiTiPyLib-1.5.4.tar.gz
+Download-URL: https://www.thibault.biz/Doc/FiReTiTiPyLib/FiReTiTiPyLib-1.5.5.tar.gz
 Author: Guillaume THIBAULT
 Author-email: thibaulg@ohsu.org
 Maintainer: Guillaume THIBAULT
 Maintainer-email: thibaulg@ohsu.edu
 License: MIT
 Keywords: cyclic Immunofluorescence,cycif,immunofluorescence,registration,segmentation,features,features extraction,nuclei,nucleus,cells,cell,cell analysis
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/SOURCES.txt` & `FiReTiTiPyLib-1.5.5/FiReTiTiPyLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.4/PKG-INFO` & `FiReTiTiPyLib-1.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FiReTiTiPyLib
-Version: 1.5.4
+Version: 1.5.5
 Summary: Python libraries used as support/tools.
-Download-URL: https://www.thibault.biz/Doc/FiReTiTiPyLib/FiReTiTiPyLib-1.5.4.tar.gz
+Download-URL: https://www.thibault.biz/Doc/FiReTiTiPyLib/FiReTiTiPyLib-1.5.5.tar.gz
 Author: Guillaume THIBAULT
 Author-email: thibaulg@ohsu.org
 Maintainer: Guillaume THIBAULT
 Maintainer-email: thibaulg@ohsu.edu
 License: MIT
 Keywords: cyclic Immunofluorescence,cycif,immunofluorescence,registration,segmentation,features,features extraction,nuclei,nucleus,cells,cell,cell analysis
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FiReTiTiPyLib-1.5.4/setup.py` & `FiReTiTiPyLib-1.5.5/setup.py`

 * *Files identical despite different names*

